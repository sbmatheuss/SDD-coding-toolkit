# vibe-coding-toolkit

> Project memory for Claude Code. Keep this file short and high-signal.

## Behavioral guidelines
<!-- aia-harness:behavioral — non-negotiable; do not edit, reorder, or remove during enrichment -->

1. **Think before coding** — state assumptions explicitly. If multiple interpretations exist, present them instead of picking silently. Say so when a simpler approach exists. If something is genuinely unclear, stop and ask.
2. **Simplicity first** — minimum code that solves the problem. No speculative features, no abstractions for single-use code, no unrequested configurability, no error handling for impossible scenarios.
3. **Surgical changes** — touch only what the request requires. Match existing style. Don't refactor, reformat, or "improve" adjacent code that wasn't part of the request.
4. **Goal-driven execution** — turn tasks into verifiable goals. For multi-step work, state a brief plan with a verify check per step, then loop until every step is verified.
5. **Orchestrator, not implementer** — the main session plans, decides, and coordinates; it does not implement. Delegable implementation and analysis goes to a specialist subagent, dispatched in parallel when task scopes don't conflict.

## Stack

This repo is documentation-only (Markdown + templates) — no build, lint, test, or run commands apply.

## Canonical commands
Always use these exact commands (do not guess):

- None — this repo has no build, lint, test, or run step (see Stack above). The Engineering-rules bullet "run the lint + test commands above" is a no-op here by design.

## Workflow & Agents

Invoke `superpowers:subagent-driven-development` for **non-trivial** implementation — trigger it when the request meets **≥2** of:

- touches **3+ files** or **2+ domains/layers** (UI + agent, API + DB…)
- is a **new feature / epic / cross-cutting refactor** (not a one-line or single-function change)
- needs a **multi-step plan** or ordered tasks, each with its own verification
- has **unclear scope or root cause** and needs exploration before coding

Skip it — implement inline — for typo/copy fixes, single-function edits, config tweaks, or one-file bugs with an obvious cause.

When dispatching subagents, you MUST use the matching specialist agent from the table below — never the generic agent when a specialist is listed. Cross-reference the task type with the "When to use" column and pass the exact name as `subagent_type`.

Model dispatch: an agent's frontmatter `model` wins; a generic dispatch or a project/user agent with no `model` in frontmatter is force-set to `sonnet` by a PreToolUse hook, so it never silently inherits this session's model — except namespaced plugin agents (`plugin:name`), left unrewritten since their frontmatter isn't reliably hook-resolvable. Pass `model` explicitly yourself for those, or to override for complex work: `haiku` for search/exploration, `sonnet` for implementation, `opus` for architectural judgment — cheapest tier that fits.

| Agent | When to use |
|---|---|
| `orchestrator` | Coordinates multi-agent or cross-domain tasks by subdelegating to specialized agents. Use proactively when a task spans multiple domains or requires parallel subagent execution. MUST BE USED instead of dispatching generic agents directly for complex workflows. |
| `code-reviewer` | Reviews any code change for bugs, security, error handling, and test coverage. Use proactively after editing any source file. MUST BE USED before merging a pull request. |
| `security-reviewer` | Reviews code for OWASP Top 10 vulnerabilities, hardcoded secrets, broken auth, and dependency CVEs. Use proactively before any merge that touches auth, input handling, or secrets. MUST BE USED before shipping security-sensitive changes. |
| `qa-automation-engineer` | Writes and maintains E2E tests (Playwright/Cypress) and CI/CD quality gates. Use proactively after new user flows are implemented or when E2E coverage is missing for a critical path. |
| `test-engineer` | Writes unit and integration tests with TDD discipline, coverage analysis, and edge-case discovery. Use proactively after implementing new logic or when test coverage gaps are identified. |
| `database-architect` | Designs schemas, migrations, indexes, and query strategies for correctness, integrity, and scalability. Use proactively when adding tables, modifying schemas, planning migrations, or diagnosing slow queries. |
| `devops-engineer` | Owns deployment, CI/CD pipelines, infrastructure configuration, and production operations. Use proactively when deploying, configuring servers, setting up CI, or troubleshooting production incidents. |
| `performance-optimizer` | Profiles and fixes performance bottlenecks — slow endpoints, high memory usage, poor Core Web Vitals, and database query inefficiency. Use proactively after profiling reveals a bottleneck or when response times degrade. |
| `product-manager` | Clarifies ambiguous requirements and prioritizes roadmap decisions when requirements are undefined before a story exists. Use when discovery and prioritization need structured analysis. |
| `product-owner` | Translates business objectives into actionable technical specs and defines acceptance criteria for existing stories before implementation begins. Use when a story needs clear acceptance criteria before development starts. |
| `project-planner` | Breaks features and epics into ordered, executable tasks with clear acceptance criteria. Use proactively when starting a new feature, sprint, or significant refactor that needs a structured plan before implementation begins. |
| `code-archaeologist` | Reverse-engineers undocumented or legacy code to uncover intent, trace logic, and map hidden dependencies. Use proactively before refactoring unfamiliar legacy code or when you need to understand why existing behavior exists. |
| `debugger` | Finds the root cause of bugs, crashes, and flaky behavior through systematic, evidence-based investigation. Use proactively when a test fails or a defect is reported, before attempting a fix. |
| `explorer-agent` | Maps an unfamiliar or complex codebase — architecture, patterns, dependencies, and risk areas — to inform planning and integration decisions. Use proactively when onboarding to a new codebase or before planning a cross-cutting change. |
| `documentation-writer` | Produces clear, example-rich technical documentation — READMEs, API docs, runbooks, and guides. Use when documentation is explicitly requested or after a feature ships and needs user-facing docs. |
| `penetration-tester` | Simulates attacker techniques to find exploitable vulnerabilities using PTES and OWASP methodologies. Use proactively before a security release, after adding new auth flows, or when a pentest is required. |
| `security-auditor` | Performs defensive SAST reviews, threat modeling, and hardening recommendations using defense-in-depth principles. Use proactively before a major release or after architectural changes that touch auth, data handling, or trust boundaries. |

### Superpowers → Project Specialists (mandatory bridging)
<!-- aia-harness:agent-routing — superpowers→specialist bridge; do not remove -->

Superpowers skills (`superpowers:dispatching-parallel-agents`, `superpowers:subagent-driven-development`,
`superpowers:executing-plans`, `superpowers:systematic-debugging`) show `general-purpose` as the default
`subagent_type` in their examples. **Never dispatch `general-purpose` (or a generic
implementer) when a specialist below covers the domain** — pass the specialist's exact
name as `subagent_type` instead.

> Basis: superpowers itself states "User's explicit instructions (CLAUDE.md) — highest
> priority." This section applies that priority over the agent types its examples suggest.
> The normal flow is unchanged (`superpowers:brainstorming` → `superpowers:writing-plans` → `superpowers:subagent-driven-development`);
> only the dispatched `subagent_type` changes.

| When superpowers would use `general-purpose` for… | Dispatch instead |
|---|---|
| Multi-domain feature — subdelegates to specialists | `orchestrator` |
| Review / audit changed code | `code-reviewer` / `security-reviewer` |
| E2E / QA automation | `qa-automation-engineer` |
| Unit / integration tests | `test-engineer` |
| Schema / migration / query / data modeling | `database-architect` |
| Deploy / CI/CD / infra | `devops-engineer` |
| Performance profiling / optimization | `performance-optimizer` |
| Understand legacy code before changing it | `code-archaeologist` |
| Bug / crash / root-cause analysis | `debugger` |
| Explore / map an unfamiliar codebase | `explorer-agent` |
| Documentation (only when explicitly requested) | `documentation-writer` |
| Offensive security / pentest | `penetration-tester` |
| Security audit / defensive review | `security-auditor` |

### Parallel wave execution (subagent-driven-development)
<!-- aia-harness:parallel-sdd — parallel wave execution override; do not remove -->

Override `superpowers:subagent-driven-development`'s serial one-implementer-at-a-time default with
parallel waves of independent tasks. Its "never dispatch implementers in parallel" red flag is
superseded here because its two premises are removed: disjoint file ownership per wave, and
controller-serialized commits instead of implementer self-commits. During planning, tag each task
`Files:` / `Depends-on:`; batch tasks with disjoint `Files` and no mutual dependency into one wave,
and dispatch their implementers in a single message using the specialist types from the table above.
Keep the skill's implementer/reviewer prompt contracts intact — the only change is implementers do
NOT self-commit. Untagged or uncertain tasks run serial (no regression). Full protocol:
`.claude/rules/08-parallel-subagent-driven-development.md`.

## Architecture map

Single-tree docs repo — no code, no nested domain `CLAUDE.md` files.

- `README.md` — PT-BR project pitch and full doc index; entry point.
- `docs/00-overview.md` — philosophy behind all 7 pillars; read before any tool doc.
- `docs/01-installation.md` — copy-paste install commands, no narrative.
- `docs/02-playbook-onboarding.md` — guided end-to-end onboarding walkthrough (recommended start).
- `docs/tools/01..14-*.md` — one self-contained reference per pillar/tool (Superpowers, subagent waves, RTK, Ponytail, Caveman, ESLint/Biome gates, Graphify, Obsidian, Claude memory, hooks, agent-browser, Context7, Anthropic Skills, Chrome DevTools MCP).
- `docs/prompts/01..07-*.md` — ready-to-paste prompt templates; body block stays English by design, wrapper prose is PT-BR.
- `docs/harness/strategies.md` — generated by `aia-harness`; lint/typecheck/test strategy notes for this repo's own harness.
- `templates/CLAUDE.md.template` — the deliverable end users copy into *their own* project; deliberately opinion-free/minimal, distinct from this repo's own root `CLAUDE.md`.
- `templates/settings.json.example`, `templates/hooks/hook-io.mjs.example`, `templates/rules/parallel-subagent-driven-development.md` — example config artifacts referenced by the templates section of the README.
- `scripts/install-plugins.mjs` — `aia-harness`-generated plugin installer for maintaining *this* repo's own harness, not a product deliverable.
- `.claude/` — this repo's own Claude Code harness (agents, skills, rules, hooks); dogfoods the workflow the toolkit documents.

## Conventions

- README and everything under `docs/` is written in PT-BR.
- Ready-to-paste prompt blocks under `docs/prompts/` stay in English by design.
- Every `docs/prompts/NN-*.md` follows the same shape: `## Quando usar` → `## Por que funciona` → `## Como adaptar os placeholders` → the pasteable English prompt block. Match it for new prompt docs.
- `docs/`, `docs/tools/`, and `docs/prompts/` files use a two-digit numeric prefix marking reading/reference order (`00-` = read first). New docs append the next number in their folder, they don't renumber existing files.
- `templates/CLAUDE.md.template` is the product deliverable (opinion-free, `[PLACEHOLDER]`-driven) — never merge this repo's own richer root `CLAUDE.md` content into it.
- First use of a technical term in README/docs gets an inline parenthetical explanation in the same sentence (e.g. "hook (um gancho, ou seja, um script que roda automaticamente...)") — the audience is devs of any level, not just specialists.

## Engineering rules
<!-- aia-harness:fixed — non-negotiable; do not edit, reorder, or remove during enrichment -->

- Match the style of surrounding code; do not introduce new patterns unprompted.
- Test what can break — business rules, branching logic, money/security/auth, bug regressions; skip trivial getters, wrappers, config, presentational UI (rubric: `.claude/rules/05-testing.md`).
- Run the lint + test commands above before claiming work is complete.
- Never commit secrets; keep them in gitignored env files (`.env`/`.env.local`) — `.claude/settings.local.json` is only for MCP-server credentials referenced by `.mcp.json`.
- Fix every compilation/syntax/lint error found during a session — regardless of whether you edited the file. Never leave the build broken or label errors "pre-existing, not related".
- When performing a code review (user requests it or a workflow triggers it), always use `code-reviewer` and `security-reviewer`, applying the `uncle-bob-craft` skill's criteria (Dependency Rule, SOLID in context, code smells) alongside their findings.

## Learn more

See `docs/00-overview.md` for the philosophy behind this repo's structure.

## graphify

This project has a knowledge graph at graphify-out/ with god nodes, community structure, and cross-file relationships.

Rules:
- For codebase questions, first run `graphify query "<question>"` when graphify-out/graph.json exists. Use `graphify path "<A>" "<B>"` for relationships and `graphify explain "<concept>"` for focused concepts. These return a scoped subgraph, usually much smaller than GRAPH_REPORT.md or raw grep output.
- If graphify-out/wiki/index.md exists, use it for broad navigation instead of raw source browsing.
- Read graphify-out/GRAPH_REPORT.md only for broad architecture review or when query/path/explain do not surface enough context.
- After modifying code, run `graphify update .` to keep the graph current (AST-only, no API cost).

@.claude/memory/INSTRUCTIONS.md
@.claude/memory/MEMORY.md
<!-- Generated by aia-harness. Edit freely; re-run /aia-harness:doctor to audit. -->
