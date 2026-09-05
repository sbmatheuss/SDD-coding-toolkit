# Graph Report - SDD-coding-toolkit  (2026-09-04)

## Corpus Check
- 163 files · ~153,454 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 2009 nodes · 2056 edges · 160 communities (150 shown, 8 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 6 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `e176f487`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Git Workflow Patterns
- Intelligent Agent Routing
- Orchestrator - Native Multi-Agent Coordination
- Code Review Standards
- API Design Patterns
- settings.json
- Playbook de Onboarding
- Project Planner - Smart Project Planning
- allow
- Deployment Procedures
- Red Team Tactics
- Quality Gates de Lint: ESLint + Biome
- Database Architect
- DevOps Engineer
- hook-io.mjs
- Debugger - Root Cause Analysis Expert
- code-reviewer.md
- Performance Optimizer
- Complete Reference — Claude Code Worktrees
- Claude Code — Git Worktrees
- Testing Patterns
- Penetration Tester
- Coordinator Mode — Multi-Agent Orchestration
- PowerShell Windows Patterns
- Tutorial passo a passo — escrevendo um hook seguro do zero
- Bash Linux Patterns
- Server Management
- Uncle Bob Craft — Expanded Reference
- Multi-Agent Orchestration
- large-file-warning.mjs
- Performance Profiling
- Tutorial passo a passo — construindo seu próprio proxy de tokens
- Graphify
- Obsidian como Memória
- Sistema de memória do Claude
- Skills oficiais da Anthropic
- Security Auditor
- Orquestração de subagentes
- Test Engineer
- Available Modes
- Error Handling Patterns
- Superpowers
- Ponytail
- agent-browser
- Product Manager
- Product Owner
- Coding Style
- Documentation Templates
- Caveman
- QA Automation Engineer
- Goal Builder
- Memory System — Persistent Cross-Session Memory
- Context7
- Code Archaeologist
- Explorer Agent - Advanced Discovery & Research
- Security Reviewer
- Clean Code - Pragmatic AI Coding Standards
- Uncle Bob Craft
- Chrome DevTools MCP
- 🎧 Vibe Coding Toolkit
- run_full_scan
- vibe-coding-toolkit
- /test - Test Generation and Execution
- Context Compression — Long Session Management
- Documentation Writer
- worktree-create.mjs
- Parallel Wave Execution (subagent-driven-development)
- Hooks — cross-platform `.mjs` standard
- 02-eslint-warning-burndown.md
- /deploy - Production Deployment
- worktree-seed.mjs
- OWASP Top 10 Audit Checklist
- worktree-write-guard.mjs
- Testing — what deserves a test
- Batch Operation Protocol
- Setup unit testing
- Visão geral
- /preview - Preview Management
- Hooks — cwd resolution standard (event.cwd vs CLAUDE_PROJECT_DIR vs process.cwd())
- uncle-bob-craft/README.md
- Vulnerability Scanner
- /plan - Project Planning Mode
- guard-main-branch.mjs
- memory-stop.mjs
- sql-idempotent-review.mjs
- Lint and Validate Skill
- Test triage — what to test among your changes
- Uncle Bob Craft — Code Review Checklist
- Security Checklists
- Parallel wave dispatch
- Parallel Subagent-Driven Development
- /brainstorm - Structured Idea Exploration
- /debug - Systematic Problem Investigation
- validate-settings-schema.mjs
- Architecture Patterns Reference
- Migration Principles
- Schema Design Principles
- find_schema_files
- detect_project_type
- check_python_coverage
- detect_test_framework
- Clean Architecture — Deep Reference
- Harness strategies
- Sanitização de projeto
- ESLint warning burndown
- Code review multi-agente
- Brainstorm até plano
- Memory bootstrap
- /coordinate — Advanced Multi-Agent Coordination
- /create - Create Application
- /enhance - Update Application
- /remember — Persistent Memory Management
- /verify — Prove Code Works
- check-deps-on-start.mjs
- gh-scope-guard.mjs
- Persistent Memory — Instructions
- Domain-Driven Design
- Design Patterns
- Coding Principles
- Code Quality
- Security
- Common Patterns
- Performance Optimization
- Architecture Decision Framework
- Database Design
- The Clean Coder — Deep Reference
- worktree-prompt-ctx.mjs
- Subagent Dispatch
- Hooks System
- Architecture Examples
- Pattern Selection Guidelines
- Trade-off Analysis & ADR
- Database Selection
- Indexing Principles
- Query Optimization
- get_summary
- Clean Agile — Deep Reference
- Design Patterns — Use vs Misuse
- Context Discovery
- ORM Selection
- Instalação
- install-plugins.mjs
- How It Works
- 11. Reporting Principles
- 1. Security Expert Mindset
- 2. OWASP Top 10:2025
- 3. Supply Chain Security (A03)
- 4. Attack Surface Mapping
- 6. Exceptional Conditions (A10 - New)
- 8. Code Pattern Analysis
- 9. Cloud Security Considerations
- MEMORY.md
- rules/testing.md
- verification.md
- lint-fix/SKILL.md
- pre-commit-verify/SKILL.md
- run-tests/SKILL.md
- .mcp.json

## God Nodes (most connected - your core abstractions)
1. `allow` - 21 edges
2. `readStdinRaw()` - 18 edges
3. `parseHookEvent()` - 18 edges
4. `Orchestrator - Native Multi-Agent Coordination` - 17 edges
5. `Intelligent Agent Routing` - 15 edges
6. `Test Engineer` - 14 edges
7. `Git Workflow Patterns` - 14 edges
8. `Vulnerability Scanner` - 14 edges
9. `Playbook de Onboarding` - 14 edges
10. `DevOps Engineer` - 13 edges

## Surprising Connections (you probably didn't know these)
- `advisory()` --calls--> `sessionScratchDir()`  [EXTRACTED]
  .claude/hooks/large-file-warning.mjs → .claude/hooks/session-scratch.mjs
- `blockOnStop()` --calls--> `sessionScratchDir()`  [EXTRACTED]
  .claude/hooks/large-file-warning.mjs → .claude/hooks/session-scratch.mjs

## Import Cycles
- None detected.

## Communities (160 total, 8 thin omitted)

### Community 0 - "Git Workflow Patterns"
Cohesion: 0.04
Nodes (47): Anti-Patterns, Branch Cleanup, Branch Management, Branching Strategies, Changelog Generation, Code Review Checklist, Commit Message Template, Commit Messages (+39 more)

### Community 1 - "Intelligent Agent Routing"
Cohesion: 0.05
Nodes (43): 1. Request Analysis, 2. Agent Selection Matrix, 3. Automatic Routing Protocol, 4. Response Format, Case 1: Generic Question, Case 2: Extremely Vague Request, Case 3: Contradictory Patterns, COMPLEX (Orchestrator required) (+35 more)

### Community 2 - "Orchestrator - Native Multi-Agent Coordination"
Cohesion: 0.05
Nodes (42): 🔴 AGENT BOUNDARY ENFORCEMENT (CRITICAL), Agent Chaining with Context, Agent States, Available Agents, Best Practices, 🔴 CHECKPOINT 1: Plan Verification (MANDATORY), 🔴 CHECKPOINT 2: Project Type Routing, 🔴 Checkpoint Summary (CRITICAL) (+34 more)

### Community 3 - "Code Review Standards"
Cohesion: 0.05
Nodes (34): Agent Orchestration, Available Agents, Immediate Agent Usage, Multi-Perspective Analysis, Parallel Task Execution, Agent Usage, Approval Criteria, Code Quality (+26 more)

### Community 4 - "API Design Patterns"
Cohesion: 0.05
Nodes (38): API Design Checklist, API Design Patterns, Authentication and Authorization, Authorization Patterns, Collection Response (with Pagination), Common Mistakes, Cursor-Based (Scalable), Error Response (+30 more)

### Community 5 - "settings.json"
Cohesion: 0.06
Nodes (36): autoMemoryEnabled, source, enabledPlugins, aia-harness@leandro-plugins-registry, caveman@caveman, ponytail@ponytail, superpowers@claude-plugins-official, env (+28 more)

### Community 6 - "Playbook de Onboarding"
Cohesion: 0.06
Nodes (34): 1. Brainstorm — destrinchar o pedido ambíguo, 1. Copie e preencha o `CLAUDE.md`, 2. Copie e ajuste o `.claude/settings.json`, 2. Plano — virar a intenção clarificada em passos verificáveis, 3. Implementação — subagent-driven-development em ondas paralelas, 3. (Recomendado) copie a regra de ondas paralelas, 4. Memória — decida agora ou decida depois, 4. Revisão — painel multi-agente antes de fechar (+26 more)

### Community 7 - "Project Planner - Smart Project Planning"
Cohesion: 0.06
Nodes (31): 1. Run All Verifications (RECOMMENDED), 2. Or Run Individually, 3. Build Verification, 📊 4-PHASE WORKFLOW (BMAD-Inspired), 4. Rule Compliance (Manual Check), 4. Runtime Verification, 5. Phase X Completion Marker, 🟢 ANALYTICAL MODE vs. PLANNING MODE (+23 more)

### Community 8 - "allow"
Cohesion: 0.07
Nodes (29): permissions, additionalDirectories, allow, defaultMode, deny, Bash(git add:*), Bash(git branch:*), Bash(git checkout:*) (+21 more)

### Community 9 - "Deployment Procedures"
Cohesion: 0.07
Nodes (27): 10. Best Practices, 1. Platform Selection, 2. Pre-Deployment Principles, 3. Deployment Workflow Principles, 4. Post-Deployment Verification, 5. Rollback Principles, 6. Zero-Downtime Deployment, 7. Emergency Procedures (+19 more)

### Community 10 - "Red Team Tactics"
Cohesion: 0.07
Nodes (27): 10. Anti-Patterns, 1. MITRE ATT&CK Phases, 2. Reconnaissance Principles, 3. Initial Access Vectors, 4. Privilege Escalation Principles, 5. Defense Evasion Principles, 6. Lateral Movement Principles, 7. Active Directory Attacks (+19 more)

### Community 11 - "Quality Gates de Lint: ESLint + Biome"
Cohesion: 0.07
Nodes (28): 10. Escrever sua primeira regra caseira, só quando fizer falta de verdade, 1. Instalar as duas ferramentas, 2. Iniciar e curar a configuração do Biome, 3. Decidir sobre o formatter, 4. Configurar o ESLint com TypeScript e regras conscientes de tipo, 5. Instalar o plugin do seu framework, se tiver um, 6. Separar o script rápido do script consciente de tipo, 7. Conectar o lint rápido a um pre-commit hook (+20 more)

### Community 12 - "Database Architect"
Cohesion: 0.07
Nodes (26): Common Anti-Patterns You Avoid, Database Architect, Database Platform Selection, Decision Frameworks, Design Decision Process, Migrations, Modern Database Platforms, Normalization Decision (+18 more)

### Community 13 - "DevOps Engineer"
Cohesion: 0.07
Nodes (26): Alert Strategy, Anti-Patterns (What NOT to Do), Core Philosophy, Decision Tree, Deployment Platform Selection, Deployment Workflow Principles, DevOps Engineer, Emergency Response Principles (+18 more)

### Community 14 - "hook-io.mjs"
Cohesion: 0.13
Nodes (15): event, ext, parseHookEvent(), readStdinRaw(), event, event, patterns, text (+7 more)

### Community 15 - "Debugger - Root Cause Analysis Expert"
Cohesion: 0.08
Nodes (24): 4-Phase Debugging Process, After Fix, Anti-Patterns (What NOT to Do), Backend Issues, Before Starting, Binary Search Debugging, Browser Issues, Bug Categories & Investigation Strategy (+16 more)

### Community 16 - "code-reviewer.md"
Cohesion: 0.08
Nodes (23): 1. Read Session Context for Plans / PRDs / Specs, 2. Read CLAUDE.md Rules, 3. Read All Project Rules (recursive), Approval Criteria, Best Practices (LOW), Code Quality (HIGH), Common False Positives - Skip These, Compliance Report (append to every review summary) (+15 more)

### Community 17 - "Performance Optimizer"
Cohesion: 0.09
Nodes (22): Anti-Patterns, Bundle Size, Caching, Core Philosophy, Core Web Vitals Targets, CSS, Images, JavaScript (+14 more)

### Community 18 - "Complete Reference — Claude Code Worktrees"
Cohesion: 0.09
Nodes (22): Changing the base branch of an already-created worktree, Checklist: Project setup for worktrees, Comparison: Worktrees vs Subagents vs Agent Teams, Complete lifecycle of a `--worktree` worktree, Complete Reference — Claude Code Worktrees, Complete SVN example, Directory structure created, Expected output (`WorktreeCreate`) (+14 more)

### Community 19 - "Claude Code — Git Worktrees"
Cohesion: 0.09
Nodes (22): Ad-hoc (asking Claude), Additional references, After entering — verify, then keep paths explicit, Claude Code — Git Worktrees, Cleanup and lifecycle, Copying gitignored files to worktrees, Creating or entering a worktree — required path, Desktop App (+14 more)

### Community 20 - "Testing Patterns"
Cohesion: 0.09
Nodes (22): 10. Anti-Patterns, 1. Testing Pyramid, 2. AAA Pattern, 3. Test Type Selection, 4. Unit Test Principles, 5. Integration Test Principles, 6. Mocking Principles, 7. Test Organization (+14 more)

### Community 21 - "Penetration Tester"
Cohesion: 0.09
Nodes (21): Always, Anti-Patterns, Attack Surface Categories, By OWASP Top 10 (2025), By Phase, By Vector, Core Philosophy, Ethical Boundaries (+13 more)

### Community 22 - "Coordinator Mode — Multi-Agent Orchestration"
Cohesion: 0.09
Nodes (21): Anti-Patterns, Best Practices, Concurrency Rules, Continue vs. Spawn Decision, Coordinator Lifecycle, Coordinator Mode — Multi-Agent Orchestration, Fork Rules, Fork Semantics (+13 more)

### Community 23 - "PowerShell Windows Patterns"
Cohesion: 0.09
Nodes (21): 10. Script Template, 1. Operator Syntax Rules, 2. Unicode/Emoji Restriction, 3. Null Check Patterns, 4. String Interpolation, 5. Error Handling, 6. File Paths, 7. Array Operations (+13 more)

### Community 25 - "Tutorial passo a passo — escrevendo um hook seguro do zero"
Cohesion: 0.09
Nodes (22): A correção, A política de fail-open não é hábito, é regra, Boas práticas para hooks, Catálogo de categorias de hooks, Dicas e pegadinhas, Dívida de migração é real — documente, não presuma, Exemplo 1 — reforçar um modo de comportamento persistente, Exemplo 2 — formatar um arquivo automaticamente após a edição (+14 more)

### Community 26 - "Bash Linux Patterns"
Cohesion: 0.10
Nodes (20): 10. Error Handling, 1. Operator Syntax, 2. File Operations, 3. Process Management, 4. Text Processing, 5. Environment Variables, 6. Network, 7. Script Template (+12 more)

### Community 27 - "Server Management"
Cohesion: 0.10
Nodes (20): 1. Process Management Principles, 2. Monitoring Principles, 3. Log Management Principles, 4. Scaling Decisions, 5. Health Check Principles, 6. Security Principles, 7. Troubleshooting Priority, 8. Anti-Patterns (+12 more)

### Community 28 - "Uncle Bob Craft — Expanded Reference"
Cohesion: 0.10
Nodes (21): Clean Agile, Clean Architecture, Component design (summary), Dependency Rule, Design patterns (when and when not), Design smells (from Clean Code / Clean Architecture), Estimation, Heuristics (review checklist style) (+13 more)

### Community 29 - "Multi-Agent Orchestration"
Cohesion: 0.11
Nodes (18): Agent Selection Matrix, Available Agents (20 total), ⏸️ CHECKPOINT: User Approval, 🔴 CRITICAL: Minimum Agent Requirement, 🔴 EXIT GATE, Multi-Agent Orchestration, Orchestration Protocol, Output Format (+10 more)

### Community 30 - "large-file-warning.mjs"
Cohesion: 0.18
Nodes (16): advisory(), blockOnStop(), countLines(), DDD_HINTS, event, IGNORED_DIRS, isSourceFile(), SOURCE_EXTS (+8 more)

### Community 31 - "Performance Profiling"
Cohesion: 0.11
Nodes (18): 1. Core Web Vitals, 2. Profiling Workflow, 3. Bundle Analysis, 4. Runtime Profiling, 5. Common Bottlenecks, 6. Quick Win Priorities, 7. Anti-Patterns, By Symptom (+10 more)

### Community 32 - "Tutorial passo a passo — construindo seu próprio proxy de tokens"
Cohesion: 0.11
Nodes (19): Dicas e pegadinhas, Exemplo 1 — `git status`, Exemplo 2 — `grep` numa árvore grande, Exemplo 3 — quando a reescrita erra: a pegadinha da flag, Exemplos concretos, O que é, Passo 1 — escolha os comandos seguros pra reescrever, Passo 2 — tenha o binário compacto (+11 more)

### Community 33 - "Graphify"
Cohesion: 0.11
Nodes (19): 1. Instale, 2. Rode o pipeline completo, 3. Veja o que foi gerado, 4. Faça uma pergunta ao grafo, 5. Explore um conceito específico, Automação com hooks de git, Comandos principais, Como instalar (+11 more)

### Community 34 - "Obsidian como Memória"
Cohesion: 0.11
Nodes (19): 1. Crie as pastas, 2. Escreva um modelo por pasta, 3. Instale e configure o servidor MCP, 4. Escreva o hook de proteção, 5. Teste os dois caminhos, Automatizando captura e consolidação, Como instalar, Dicas e pegadinhas (+11 more)

### Community 35 - "Sistema de memória do Claude"
Cohesion: 0.11
Nodes (19): A ideia generalizável, Boa — erro corrigido repetidamente na sessão, Boa — onde uma informação externa mora, Boa — padrão de arquitetura descoberto após tentativa falha, Boa — regra de negócio implícita no código, Critério de salvamento, Dicas e pegadinhas, Estrutura (+11 more)

### Community 36 - "Skills oficiais da Anthropic"
Cohesion: 0.11
Nodes (19): 1. Instale o pacote de documentos, 2. Peça o relatório, descrevendo o que ele precisa ter, 3. O que acontece por trás dos panos, 4. Confira o arquivo gerado, Como instalar/ativar, Dicas e pegadinhas, Exemplo 1 — planilha `.xlsx` com fórmulas, a partir de uma lista solta de dados, Exemplo 2 — criar sua própria skill com `skill-creator` (+11 more)

### Community 37 - "Security Auditor"
Cohesion: 0.11
Nodes (17): Anti-Patterns, Before Any Review, Code Patterns (Red Flags), Configuration (A02), Core Philosophy, Decision Framework, How You Approach Security, OWASP Top 10:2025 (+9 more)

### Community 38 - "Orquestração de subagentes"
Cohesion: 0.11
Nodes (18): A solução, Antes das ondas: como decidir a quebra de tarefas, Dicas e pegadinhas, Exemplo 1 — cupom de desconto num app de e-commerce, Exemplo 2 — três chamados de bug num blog, Exemplos, Loop de execução por onda, O problema (+10 more)

### Community 39 - "Test Engineer"
Cohesion: 0.12
Nodes (16): AAA Pattern, Anti-Patterns, Core Philosophy, Coverage Strategy, Deep Audit Approach, Discovery, Framework Selection, Mocking Principles (+8 more)

### Community 40 - "Available Modes"
Cohesion: 0.12
Nodes (16): 1. 🧠 BRAINSTORM Mode, 1. 🔭 EXPLORE Mode, 2. ⚡ IMPLEMENT Mode, 2. 🗺️ PLAN-EXECUTE-CRITIC (PEC), 3. 🔍 DEBUG Mode, 3. 🧠 MENTAL MODEL SYNC, 4. 📋 REVIEW Mode, 5. 📚 TEACH Mode (+8 more)

### Community 41 - "Error Handling Patterns"
Cohesion: 0.12
Nodes (16): API Error Handler (Next.js / Express), Core Principles, Custom Exception Hierarchy, Error Handling Checklist, Error Handling Patterns, FastAPI Global Exception Handler, Go, Python (+8 more)

### Community 42 - "Superpowers"
Cohesion: 0.12
Nodes (17): A regra central, As seis skills essenciais, `brainstorming`, Dicas e boas práticas, `dispatching-parallel-agents`, Do pedido vago ao código: um exemplo encadeado, Instalação, O que é (+9 more)

### Community 43 - "Ponytail"
Cohesion: 0.12
Nodes (17): 1. Entenda o problema antes de subir a escada, 2. Suba a escada, degrau por degrau, e pare no primeiro que resolve, 3. Corrija bugs na causa raiz, não no sintoma, 4. Marque simplificações deliberadas com um comentário `ponytail:`, 5. Feche com uma verificação mínima, quando a lógica não é trivial, 6. Responda direto: código primeiro, explicação em no máximo três linhas, Como instalar/ativar, Dicas e pegadinhas (+9 more)

### Community 44 - "agent-browser"
Cohesion: 0.12
Nodes (17): 1. Instale, 2. Primeiro comando: puxe as instruções reais, 3. Abra uma página, 4. Tire um snapshot — e leia o texto direto dele, agent-browser, Além de páginas web comuns, Como instalar, Dicas e pegadinhas (+9 more)

### Community 45 - "Product Manager"
Cohesion: 0.12
Nodes (15): 1. Product Requirement Document (PRD) Schema, 2. Feature Kickoff, Acceptance Criteria (Gherkin-style preferred), Anti-Patterns (What NOT to do), Core Philosophy, 🤝 Interaction with Other Agents, 📝 Output Formats, Phase 1: Discovery (The "Why") (+7 more)

### Community 46 - "Product Owner"
Cohesion: 0.12
Nodes (15): 1. Product Brief / PRD, 1. Requirements Elicitation, 2. User Story Creation, 2. Visual Roadmap, 3. Scope Management, 4. Backlog Refinement & Prioritization, Anti-Patterns (What NOT to do), Core Philosophy (+7 more)

### Community 47 - "Coding Style"
Cohesion: 0.12
Nodes (15): Code Quality Checklist, Code Smells to Avoid, Coding Style, Core Principles, Deep Nesting, DRY (Don't Repeat Yourself), Error Handling, File Organization (+7 more)

### Community 48 - "Documentation Templates"
Cohesion: 0.12
Nodes (15): 1. README Structure, 2. API Documentation Structure, 3. Code Comment Guidelines, 4. Changelog Template (Keep a Changelog), 5. Architecture Decision Record (ADR), 6. AI-Friendly Documentation, 7. Structure Principles, Documentation Templates (+7 more)

### Community 49 - "Caveman"
Cohesion: 0.12
Nodes (16): 1. O que é cortado, 2. O que nunca é tocado, 3. A sobreposição de clareza automática, 4. Ajustando a intensidade e deixando a regra fixa no repositório, 5. Comandos complementares, Caveman, Como instalar/ativar, Dicas e pegadinhas (+8 more)

### Community 50 - "QA Automation Engineer"
Cohesion: 0.13
Nodes (14): 1. The Smoke Suite (P0), 2. The Regression Suite (P1), 3. Visual Regression, 🤖 Automating the "Unhappy Path", Browser Automation, CI/CD, 📜 Coding Standards for Tests, Core Philosophy (+6 more)

### Community 51 - "Goal Builder"
Cohesion: 0.13
Nodes (14): 1. Collect requirements, 2. Map gaps → AskUserQuestion (max 4 per call), 3. Decide format, 4. Assemble the `/goal`, 5. Deliver, A) Simple task — inline goal, Anatomy of a `/goal` (3 + 1), Anti-patterns (+6 more)

### Community 52 - "Memory System — Persistent Cross-Session Memory"
Cohesion: 0.13
Nodes (14): Architecture, MEMORY.md Index Format, Memory System — Persistent Cross-Session Memory, Memory Taxonomy, Memory vs. Plan vs. Task, Operations, Overview, Prune (Trigger: index exceeds 200 lines) (+6 more)

### Community 53 - "Context7"
Cohesion: 0.13
Nodes (15): 1. Instale, 2. Faça uma pergunta que dependa de doc atual, 3. O agente resolve a biblioteca certa primeiro, 4. O agente busca a doc real daquela versão, 5. A resposta final já vem apoiada na doc real, Como instalar, Context7, Dicas e pegadinhas (+7 more)

### Community 54 - "Code Archaeologist"
Cohesion: 0.14
Nodes (13): 1. Static Analysis, 2. The "Strangler Fig" Pattern, 📝 Archaeologist's Report Format, Code Archaeologist, Core Philosophy, 🕵️ Excavation Toolkit, 🤝 Interaction with Other Agents, Phase 1: Characterization Testing (+5 more)

### Community 55 - "Explorer Agent - Advanced Discovery & Research"
Cohesion: 0.14
Nodes (13): Advanced Exploration Modes, 🔍 Audit Mode, Code Patterns, Discovery Flow, Explorer Agent - Advanced Discovery & Research, 🧪 Feasibility Mode, Interactivity Rules:, 🗺️ Mapping Mode (+5 more)

### Community 56 - "Security Reviewer"
Cohesion: 0.14
Nodes (13): 1. Initial Scan, 2. OWASP Top 10:2025 Check, 3. Code Pattern Review, Analysis Commands, Common False Positives, Core Responsibilities, Emergency Response, Key Principles (+5 more)

### Community 57 - "Clean Code - Pragmatic AI Coding Standards"
Cohesion: 0.14
Nodes (13): Agent → Script Mapping, AI Coding Style, Anti-Patterns (DON'T), 🔴 Before Editing ANY File (THINK FIRST!), Clean Code - Pragmatic AI Coding Standards, Code Structure, Core Principles, Function Rules (+5 more)

### Community 58 - "Uncle Bob Craft"
Cohesion: 0.14
Nodes (14): Aggregators by Source, Best Practices, Common Pitfalls, Design Patterns: Use vs Misuse, Example 1: Code review prompt (copy-pasteable), Example 2: Before/after (extract and name), Examples, Limitations (+6 more)

### Community 59 - "Chrome DevTools MCP"
Cohesion: 0.14
Nodes (14): 1. Instale, 2. Descreva o sintoma, não a causa, 3. O agente abre a página e roda um trace de performance, 4. O agente lê o resultado e aponta a causa raiz, Chrome DevTools MCP, Como instalar, Dicas e pegadinhas, Exemplo 1 — performance trace (+6 more)

### Community 60 - "🎧 Vibe Coding Toolkit"
Cohesion: 0.14
Nodes (14): <a id="comece-por-aqui"></a>🚀 Comece por aqui, <a id="como-usar-este-repositorio"></a>🧑‍💻 Como usar este repositório, <a id="creditos"></a>🙏 Créditos, <a id="documentacao-completa"></a>📚 Documentação completa, <a id="licenca"></a>⚖️ Licença, <a id="o-fluxo-completo"></a>🗺️ O fluxo completo, <a id="sobre-o-projeto"></a>💡 Sobre o projeto, <a id="superpowers-primeiro"></a>⭐ Superpowers primeiro (+6 more)

### Community 61 - "run_full_scan"
Cohesion: 0.27
Nodes (12): Any, main(), Validate no hardcoded secrets (OWASP A04). Checks: API keys, tokens, passwords,…, Validate dangerous code patterns (OWASP A05). Checks: Injection risks, XSS,…, Validate security configuration (OWASP A02). Checks: Security headers, CORS,…, Execute security validation scans., Validate supply chain security (OWASP A03). Checks: npm audit, lock file…, run_full_scan() (+4 more)

### Community 62 - "vibe-coding-toolkit"
Cohesion: 0.15
Nodes (12): Architecture map, Behavioral guidelines, Canonical commands, Conventions, Engineering rules, graphify, Learn more, Parallel wave execution (subagent-driven-development) (+4 more)

### Community 63 - "/test - Test Generation and Execution"
Cohesion: 0.15
Nodes (12): Behavior, Examples, For Test Execution, For Test Generation, Generate Tests, Key Principles, Output Format, Purpose (+4 more)

### Community 64 - "Context Compression — Long Session Management"
Cohesion: 0.15
Nodes (12): Best Practices, Compression Levels, Compression Protocol, Context Compression — Long Session Management, Level 1: Micro-Compact (Tool Output), Level 2: Phase Summary, Level 3: Session Checkpoint, Overview (+4 more)

### Community 65 - "Documentation Writer"
Cohesion: 0.17
Nodes (11): API Documentation Principles, Code Comment Principles, Core Philosophy, Decision Tree, Documentation Principles, Documentation Type Selection, Documentation Writer, Quality Checklist (+3 more)

### Community 66 - "worktree-create.mjs"
Cohesion: 0.23
Nodes (10): claimSeed(), dir, event, git(), gitDirRaw, gitOk(), insideWorktree, isAlivePid() (+2 more)

### Community 67 - "Parallel Wave Execution (subagent-driven-development)"
Cohesion: 0.17
Nodes (11): Fallback: worktree isolation, No numeric concurrency cap, Parallel Wave Execution (subagent-driven-development), Per-wave execution loop, Purpose, Relationship to whole-branch review, Safety rails, Task tagging (+3 more)

### Community 68 - "Hooks — cross-platform `.mjs` standard"
Cohesion: 0.17
Nodes (11): Acceptance criteria, Caveats, Forbidden, Hooks — cross-platform `.mjs` standard, Mandatory rules, Objective, Portability patterns inside the `.mjs`, Runtime decision (+3 more)

### Community 69 - "02-eslint-warning-burndown.md"
Cohesion: 0.18
Nodes (9): Como adaptar os placeholders, Dicas, Exemplo de uso, O prompt, only if React/Next.js:, only if the ORM has one (Drizzle does):, Por que funciona, Quando usar (+1 more)

### Community 70 - "/deploy - Production Deployment"
Cohesion: 0.18
Nodes (10): /deploy - Production Deployment, Deployment Flow, Examples, Failed Deploy, Output Format, Platform Support, Pre-Deployment Checklist, Purpose (+2 more)

### Community 71 - "worktree-seed.mjs"
Cohesion: 0.27
Nodes (8): compilePattern(), copyDereferenced(), copyDereferencedAtomic(), isAlivePid(), readStartedAt(), resolveWorktreeIncludePaths(), walkRelative(), writeStateFinal()

### Community 72 - "OWASP Top 10 Audit Checklist"
Cohesion: 0.18
Nodes (11): A01: Broken Access Control, A02: Security Misconfiguration, A03: Software Supply Chain Failures, A04: Cryptographic Failures, A05: Injection, A06: Insecure Design, A07: Authentication Failures, A08: Software or Data Integrity Failures (+3 more)

### Community 73 - "worktree-write-guard.mjs"
Cohesion: 0.20
Nodes (8): absTarget, event, m, reason, relTarget, relWt, wtDisplay, wtPath

### Community 74 - "Testing — what deserves a test"
Cohesion: 0.20
Nodes (9): Acceptance, Frontend, Graphify — if `graphify-out/` exists, How, Objective, Objective signals — decide + prioritize, Skip it — no logic to break, Test it — real logic + stakes (+1 more)

### Community 75 - "Batch Operation Protocol"
Cohesion: 0.20
Nodes (9): Batch Operation Protocol, Batch Operations — Multi-File Changes, Common Batch Patterns, Safety Rules, Step 1: Define the Pattern, Step 2: Preview Before Executing, Step 3: Execute the Batch, Step 4: Verify the Batch (+1 more)

### Community 76 - "Setup unit testing"
Cohesion: 0.20
Nodes (9): 1. Determine the framework, 2. Install (if needed), 3. Write the config file, 4. Write 1 REAL test, 5. Wire the test script, 6. Run until green, 7. Update CLAUDE.md, 8. Report (+1 more)

### Community 77 - "Visão geral"
Cohesion: 0.20
Nodes (10): 1. Orquestração, não implementação solo, 2. Brainstorm → plano → implementação → revisão, 3. Uma camada de economia de tokens, 4. Duas camadas de personalidade compostas, 5. Gates de qualidade como migração rastreada, 6. Um grafo de conhecimento do código, 7. Um sistema de memória em duas camadas, Leitura complementar oficial (+2 more)

### Community 78 - "/preview - Preview Management"
Cohesion: 0.22
Nodes (8): Commands, Port Conflict, /preview - Preview Management, Start Server, Status Check, Task, Technical, Usage Examples

### Community 79 - "Hooks — cwd resolution standard (event.cwd vs CLAUDE_PROJECT_DIR vs process.cwd())"
Cohesion: 0.22
Nodes (8): Acceptance criteria, Canonical examples in this codebase, Forbidden, Hooks — cwd resolution standard (event.cwd vs CLAUDE_PROJECT_DIR vs process.cwd()), Objective, The three values, and what each actually tracks, Three purposes — resolve them differently, never merge them, Which one do you have? A quick test

### Community 81 - "Vulnerability Scanner"
Cohesion: 0.22
Nodes (9): 10. Anti-Patterns, 5. Risk Prioritization, 7. Scanning Methodology, CVSS + Context, Phase-Based Approach, Prioritization Decision Tree, 📋 Reference Files, 🔧 Runtime Scripts (+1 more)

### Community 82 - "/plan - Project Planning Mode"
Cohesion: 0.25
Nodes (7): After Planning, 🔴 CRITICAL RULES, Expected Output, Naming Examples, /plan - Project Planning Mode, Task, Usage

### Community 83 - "guard-main-branch.mjs"
Cohesion: 0.25
Nodes (6): branch, event, isCommit, isPush, onMain, permissionDecisionReason

### Community 84 - "memory-stop.mjs"
Cohesion: 0.25
Nodes (6): allOps, flag, memoryIndexPath, SKIP_SUFFIXES, SOURCE_EXTS, uniqueSource

### Community 85 - "sql-idempotent-review.mjs"
Cohesion: 0.43
Nodes (7): blockOnStop(), buildIdempotencyRules(), event, markNotified(), NOTIFIED_FLAG, postToolUse(), readNotifiedSet()

### Community 86 - "Lint and Validate Skill"
Cohesion: 0.25
Nodes (7): Error Handling, Lint and Validate Skill, Node.js / TypeScript, Procedures by Ecosystem, Python, Scripts, The Quality Loop

### Community 87 - "Test triage — what to test among your changes"
Cohesion: 0.25
Nodes (7): 1. Collect changed symbols, 2. Score each symbol, 3. Output the triage table, 4. Act, Test triage — what to test among your changes, With graphify (`graphify-out/graph.json` exists), Without graphify

### Community 88 - "Uncle Bob Craft — Code Review Checklist"
Cohesion: 0.25
Nodes (7): 1. Dependency Rule and boundaries, 2. SOLID in context, 3. Smells, 4. Design patterns, 5. Tests and professionalism, Suggested output format for review, Uncle Bob Craft — Code Review Checklist

### Community 89 - "Security Checklists"
Cohesion: 0.25
Nodes (6): API Security Checklist, Authentication Checklist, Data Protection Checklist, Quick Audit Commands, Security Checklists, Security Headers

### Community 90 - "Parallel wave dispatch"
Cohesion: 0.25
Nodes (7): Como adaptar os placeholders, Dicas, Exemplo de uso, O prompt, Parallel wave dispatch, Por que funciona, Quando usar

### Community 91 - "Parallel Subagent-Driven Development"
Cohesion: 0.25
Nodes (8): Escape hatch, Parallel Subagent-Driven Development, Per-wave execution loop, Problem, Task tagging, Wave formation rule, What this does not change, Why this override is safe

### Community 92 - "/brainstorm - Structured Idea Exploration"
Cohesion: 0.29
Nodes (6): Behavior, /brainstorm - Structured Idea Exploration, Examples, Key Principles, Output Format, Purpose

### Community 93 - "/debug - Systematic Problem Investigation"
Cohesion: 0.29
Nodes (6): Behavior, /debug - Systematic Problem Investigation, Examples, Key Principles, Output Format, Purpose

### Community 94 - "validate-settings-schema.mjs"
Cohesion: 0.33
Nodes (5): basename, checkType(), errors, list, validate()

### Community 95 - "Architecture Patterns Reference"
Cohesion: 0.29
Nodes (6): API Patterns, Architecture Patterns Reference, Data Access Patterns, Distributed System Patterns, Domain Logic Patterns, Simplicity Principle

### Community 96 - "Migration Principles"
Cohesion: 0.29
Nodes (6): Migration Philosophy, Migration Principles, Neon (Serverless PostgreSQL), Safe Migration Strategy, Serverless Databases, Turso (Edge SQLite)

### Community 97 - "Schema Design Principles"
Cohesion: 0.29
Nodes (6): Foreign Key ON DELETE, Normalization Decision, Primary Key Selection, Relationship Types, Schema Design Principles, Timestamp Strategy

### Community 98 - "find_schema_files"
Cohesion: 0.48
Nodes (6): find_schema_files(), main(), Path, Find database schema files., Validate Prisma schema file., validate_prisma_schema()

### Community 99 - "detect_project_type"
Cohesion: 0.48
Nodes (6): detect_project_type(), main(), Path, Detect project type and available linters., Run a single linter and return results., run_linter()

### Community 100 - "check_python_coverage"
Cohesion: 0.48
Nodes (6): check_python_coverage(), check_typescript_coverage(), main(), Path, Check TypeScript type coverage., Check Python type hints coverage.

### Community 101 - "detect_test_framework"
Cohesion: 0.48
Nodes (6): detect_test_framework(), main(), Path, Detect test framework and commands., Run tests and return results., run_tests()

### Community 102 - "Clean Architecture — Deep Reference"
Cohesion: 0.29
Nodes (7): Boundaries, Clean Architecture — Deep Reference, Component cohesion and coupling (for larger systems), Dependency Rule, Inversion of dependencies, Layers (from inside out), SOLID in this context

### Community 103 - "Harness strategies"
Cohesion: 0.29
Nodes (6): Canonical command reference, Compilation / typecheck, Harness strategies, Language server, Lint & format, Unit testing

### Community 104 - "Sanitização de projeto"
Cohesion: 0.29
Nodes (7): Como adaptar os placeholders, Dicas, Exemplo de uso, O prompt, Por que funciona, Quando usar, Sanitização de projeto

### Community 105 - "ESLint warning burndown"
Cohesion: 0.29
Nodes (7): Como adaptar os placeholders, Dicas, ESLint warning burndown, Exemplo de uso, O prompt, Por que funciona, Quando usar

### Community 106 - "Code review multi-agente"
Cohesion: 0.29
Nodes (7): Code review multi-agente, Como adaptar os placeholders, Dicas, Exemplo de uso, O prompt, Por que funciona, Quando usar

### Community 107 - "Brainstorm até plano"
Cohesion: 0.29
Nodes (7): Brainstorm até plano, Como adaptar os placeholders, Dicas, Exemplo de uso, O prompt, Por que funciona, Quando usar

### Community 108 - "Memory bootstrap"
Cohesion: 0.29
Nodes (7): Como adaptar os placeholders, Dicas, Exemplo de uso, Memory bootstrap, O prompt, Por que funciona, Quando usar

### Community 109 - "/coordinate — Advanced Multi-Agent Coordination"
Cohesion: 0.33
Nodes (5): After Coordination, /coordinate — Advanced Multi-Agent Coordination, 🔴 CRITICAL RULES, Expected Output, Task

### Community 110 - "/create - Create Application"
Cohesion: 0.33
Nodes (5): Before Starting, /create - Create Application, Steps:, Task, Usage Examples

### Community 111 - "/enhance - Update Application"
Cohesion: 0.33
Nodes (5): Caution, /enhance - Update Application, Steps:, Task, Usage Examples

### Community 112 - "/remember — Persistent Memory Management"
Cohesion: 0.33
Nodes (5): 🔴 CRITICAL RULES, Expected Output, /remember — Persistent Memory Management, Task, Usage Examples

### Community 113 - "/verify — Prove Code Works"
Cohesion: 0.33
Nodes (5): 🔴 CRITICAL RULES, Expected Output, Task, Usage Examples, /verify — Prove Code Works

### Community 114 - "check-deps-on-start.mjs"
Cohesion: 0.33
Nodes (4): event, ghProblem, lines, result

### Community 115 - "gh-scope-guard.mjs"
Cohesion: 0.33
Nodes (4): envTokenOverride, event, GH_SCOPES, refreshCmd

### Community 116 - "Persistent Memory — Instructions"
Cohesion: 0.33
Nodes (5): How to save, Persistent Memory — Instructions, Reading memories, Sanitation (mandatory when index is large), When to save (do not wait to be asked)

### Community 117 - "Domain-Driven Design"
Cohesion: 0.33
Nodes (5): Acceptance criteria, Do, Domain-Driven Design, Don't, Objective

### Community 118 - "Design Patterns"
Cohesion: 0.33
Nodes (5): Acceptance criteria, Design Patterns, Do, Don't, Objective

### Community 119 - "Coding Principles"
Cohesion: 0.33
Nodes (5): Acceptance criteria, Coding Principles, Do, Don't, Objective

### Community 120 - "Code Quality"
Cohesion: 0.33
Nodes (5): Acceptance criteria, Code Quality, Do, Don't, Objective

### Community 121 - "Security"
Cohesion: 0.33
Nodes (5): Acceptance criteria, Do, Don't, Objective, Security

### Community 122 - "Common Patterns"
Cohesion: 0.33
Nodes (5): API Response Format, Common Patterns, Design Patterns, Repository Pattern, Skeleton Projects

### Community 123 - "Performance Optimization"
Cohesion: 0.33
Nodes (5): Build Troubleshooting, Context Window Management, Extended Thinking + Plan Mode, Model Selection Strategy, Performance Optimization

### Community 124 - "Architecture Decision Framework"
Cohesion: 0.33
Nodes (5): Architecture Decision Framework, Core Principle, 🔗 Related Skills, 🎯 Selective Reading Rule, Validation Checklist

### Community 125 - "Database Design"
Cohesion: 0.33
Nodes (5): Anti-Patterns, ⚠️ Core Principle, Database Design, Decision Checklist, 🎯 Selective Reading Rule

### Community 126 - "The Clean Coder — Deep Reference"
Cohesion: 0.33
Nodes (6): Estimation, Mentoring and collaboration, Professionalism, Sustainable pace, Tests as a requirement, The Clean Coder — Deep Reference

### Community 127 - "worktree-prompt-ctx.mjs"
Cohesion: 0.40
Nodes (4): event, hookSpecificOutput, m, RENAMED_FLAG

### Community 128 - "Subagent Dispatch"
Cohesion: 0.40
Nodes (4): Dispatch mechanics, Rule, Subagent Dispatch, Superpowers bridging

### Community 129 - "Hooks System"
Cohesion: 0.40
Nodes (4): Auto-Accept Permissions, Hook Types, Hooks System, TodoWrite Best Practices

### Community 130 - "Architecture Examples"
Cohesion: 0.40
Nodes (4): Architecture Examples, Example 1: MVP E-commerce (Solo Developer), Example 2: SaaS Product (5-10 Developers), Example 3: Enterprise (100K+ Users)

### Community 131 - "Pattern Selection Guidelines"
Cohesion: 0.40
Nodes (4): Main Decision Tree, Pattern Selection Guidelines, Red Flags (Anti-patterns), The 3 Questions (Before ANY Pattern)

### Community 132 - "Trade-off Analysis & ADR"
Cohesion: 0.40
Nodes (4): ADR Storage, ADR Template, Decision Framework, Trade-off Analysis & ADR

### Community 133 - "Database Selection"
Cohesion: 0.40
Nodes (4): Comparison, Database Selection, Decision Tree, Questions to Ask

### Community 134 - "Indexing Principles"
Cohesion: 0.40
Nodes (4): Composite Index Principles, Index Type Selection, Indexing Principles, When to Create Indexes

### Community 135 - "Query Optimization"
Cohesion: 0.40
Nodes (4): N+1 Problem, Optimization Priorities, Query Analysis Mindset, Query Optimization

### Community 136 - "get_summary"
Cohesion: 0.50
Nodes (4): get_summary(), Run Lighthouse audit on URL., Generate summary based on scores., run_lighthouse()

### Community 137 - "Clean Agile — Deep Reference"
Cohesion: 0.40
Nodes (5): Agile values (manifesto), Clean Agile — Deep Reference, Iron Cross (four supporting values), Practices, Relationship to craft

### Community 138 - "Design Patterns — Use vs Misuse"
Cohesion: 0.40
Nodes (5): Cargo cult and misuse, Design Patterns — Use vs Misuse, Good signals, When not to use a pattern, When to use a pattern

### Community 139 - "Context Discovery"
Cohesion: 0.50
Nodes (3): Context Discovery, Project Classification Matrix, Question Hierarchy (Ask User FIRST)

### Community 140 - "ORM Selection"
Cohesion: 0.50
Nodes (3): Comparison, Decision Tree, ORM Selection

### Community 141 - "Instalação"
Cohesion: 0.50
Nodes (4): 1. Claude Code, 2. Plugins e CLIs independentes, Instalação, Quer o passo a passo completo?

### Community 142 - "install-plugins.mjs"
Cohesion: 0.50
Nodes (3): check, marketplaces, plugins

### Community 143 - "How It Works"
Cohesion: 0.67
Nodes (3): How It Works, When reviewing code, When writing or refactoring code

### Community 144 - "11. Reporting Principles"
Cohesion: 0.67
Nodes (3): 11. Reporting Principles, Finding Structure, Severity Classification

### Community 145 - "1. Security Expert Mindset"
Cohesion: 0.67
Nodes (3): 1. Security Expert Mindset, Core Principles, Threat Modeling Questions

### Community 146 - "2. OWASP Top 10:2025"
Cohesion: 0.67
Nodes (3): 2025 Key Changes, 2. OWASP Top 10:2025, Risk Categories

### Community 147 - "3. Supply Chain Security (A03)"
Cohesion: 0.67
Nodes (3): 3. Supply Chain Security (A03), Attack Surface, Defense Principles

### Community 148 - "4. Attack Surface Mapping"
Cohesion: 0.67
Nodes (3): 4. Attack Surface Mapping, Prioritization Matrix, What to Map

### Community 149 - "6. Exceptional Conditions (A10 - New)"
Cohesion: 0.67
Nodes (3): 6. Exceptional Conditions (A10 - New), Fail-Open vs Fail-Closed, What to Check

### Community 150 - "8. Code Pattern Analysis"
Cohesion: 0.67
Nodes (3): 8. Code Pattern Analysis, High-Risk Patterns, Secret Patterns

### Community 151 - "9. Cloud Security Considerations"
Cohesion: 0.67
Nodes (3): 9. Cloud Security Considerations, Cloud-Specific Checks, Shared Responsibility

## Knowledge Gaps
- **1383 isolated node(s):** `event`, `result`, `ghProblem`, `lines`, `event` (+1378 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 1500 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **8 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Playbook de Onboarding` connect `Playbook de Onboarding` to `README.md`?**
  _High betweenness centrality (0.008) - this node is a cross-community bridge._
- **Why does `RTK — proxy de tokens para CLI` connect `Tutorial passo a passo — construindo seu próprio proxy de tokens` to `README.md`?**
  _High betweenness centrality (0.005) - this node is a cross-community bridge._
- **Why does `Quality Gates de Lint: ESLint + Biome` connect `Quality Gates de Lint: ESLint + Biome` to `02-eslint-warning-burndown.md`?**
  _High betweenness centrality (0.004) - this node is a cross-community bridge._
- **What connects `event`, `result`, `ghProblem` to the rest of the system?**
  _1383 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Git Workflow Patterns` be split into smaller, more focused modules?**
  _Cohesion score 0.041666666666666664 - nodes in this community are weakly interconnected._
- **Should `Intelligent Agent Routing` be split into smaller, more focused modules?**
  _Cohesion score 0.045454545454545456 - nodes in this community are weakly interconnected._
- **Should `Orchestrator - Native Multi-Agent Coordination` be split into smaller, more focused modules?**
  _Cohesion score 0.046511627906976744 - nodes in this community are weakly interconnected._