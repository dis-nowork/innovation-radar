# 🛠️ DevTools

Extração documental, geração de código, TTS, MCP tooling, coding agents.

### [kreuzberg-dev/kreuzberg](https://github.com/kreuzberg-dev/kreuzberg) ⭐ 5.7k | 🎯⚡💸
**Problema:** Extrair texto de PDFs, imagens, DOCX, etc. exige múltiplas libs e muita gambiarra.
**Solução:** Uma lib Python que extrai texto de 50+ formatos com OCR embutido (Rust = rápido).
**Por que é superior:** ⚡ Rust backend = 5x mais rápido que PyPDF. 💸 Grátis vs APIs pagas de OCR. 🎯 Todo pipeline de dados precisa.

---

### [enoch3712/ExtractThinker](https://github.com/enoch3712/ExtractThinker) ⭐ 1.5k | 🎯⚡
**Problema:** Extrair dados estruturados de contratos/faturas exige regex frágil ou trabalho manual.
**Solução:** ORM para documentos: define schema, LLM extrai os campos. Contratos viram queries.
**Por que é superior:** ⚡ Horas de regex → minutos com schema. 🎯 Toda empresa processa documentos.

---

### [gofireflyio/aiac](https://github.com/gofireflyio/aiac) ⭐ 3.8k | ⚡💸
**Problema:** Escrever Terraform/Pulumi/Docker configs é repetitivo e propenso a erros.
**Solução:** Gera IaC com linguagem natural: descreve o que quer, recebe o código pronto.
**Por que é superior:** ⚡ Minutos vs horas escrevendo YAML. 💸 Menos erros de infra = menos downtime.

---

### [Zyphra/Zonos](https://github.com/Zyphra/Zonos) ⭐ 7.2k | 💸🚀
**Problema:** TTS de qualidade (ElevenLabs) custa $5-99/mês por voz.
**Solução:** TTS open-weight qualidade comercial — 200k+ horas de treino, roda local.
**Por que é superior:** 💸 Grátis vs $99/mês. 🚀 Roda local = sem API, sem limites, privacidade total.

---


### [jlowin/fastmcp](https://github.com/jlowin/fastmcp) ⭐ 22.5k | 🎯⚡🚀
**Problema:** Criar MCP servers é complexo — serialização, validação, error handling, protocol compliance. O SDK oficial é verboso.
**Solução:** Framework Pythonic que abstrai toda complexidade MCP em decorators simples. FastMCP 1.0 foi incorporado ao SDK oficial; hoje powera 70% de todos MCP servers.
**Por que é superior:** ⚡ De dias → horas pra criar um MCP server. 🚀 1M+ downloads/dia, se tornou o padrão de facto. 🎯 Todo dev que quer expor tools pra AI precisa disso.
**TAM:** MCP ecosystem estimado em bilhões. Todo SaaS, API, database eventualmente terá MCP server.
**Modelo de negócio:** Já da Prefect (empresa madura). Upsell: Prefect Cloud pra orquestração. MCP hosting managed.
**Esforço:** Baixo (já produtizado). Oportunidade: managed MCP hosting, marketplace de servers, enterprise support.
**Licença:** Apache-2.0 | 1.7k forks

---

### [oraios/serena](https://github.com/oraios/serena) ⭐ 19.6k | 🎯⚡💎
**Problema:** Coding agents (Claude Code, Codex, Gemini CLI) desperdiçam tokens lendo arquivos inteiros e fazendo grep cego. Em codebases grandes, isso é ineficiente e caro.
**Solução:** Toolkit que dá capacidades de IDE ao LLM via MCP — retrieval semântico por símbolo (find_symbol, find_referencing_symbols, insert_after_symbol). O agent navega como um dev sênior, não como um estagiário com grep.
**Por que é superior:** 💎 Qualidade muito superior: edições precisas por símbolo vs string replacement. ⚡ 5-10x menos tokens = 5-10x menor custo. 🎯 Todo dev usando AI coding agents se beneficia.
**TAM:** AI coding tools market $2B+ e crescendo 100%+ a.a.
**Modelo de negócio:** Freemium (MIT). Plugin JetBrains já lançado. Enterprise: self-hosted com suporte, custom language packs.
**Esforço:** Baixo-Médio. Já funcional com Claude Code, Gemini CLI, Cursor, VSCode.
**Combinação:** Serena + FastMCP = coding agents que são IDE-aware E eficientes em tokens.
**Licença:** MIT | 1.3k forks

---

### [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) ⭐ 20.1k | 🎯⚡🚀
**Problema:** Engenheiros usando múltiplos coding agents (Claude Code, Codex, Gemini CLI) não têm forma unificada de orquestrar, monitorar e fazer review do trabalho. Cada agent roda isolado no terminal.
**Solução:** Kanban board que orquestra coding agents — switch entre agents, run em paralelo/sequência, review work, start dev servers, centraliza MCP configs. Suporte SSH remoto.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** A nova realidade: humanos planejam/reviewam, agents codam. Faltava a "IDE humana" pra gerenciar agents
- ⚡ **Velocidade:** Paraleliza múltiplos agents vs rodar um por vez
- 🚀 **Escala:** De 1 agent em 1 terminal para N agents em N projetos com visão unificada
**TAM:** $2B+ (developer productivity tools, mercado crescendo com AI coding)
**Modelo de negócio:** Freemium (individual grátis), Teams/Enterprise (collaboration, analytics, integrations), cloud-hosted
**Esforço:** Médio — produto já funcional, precisa cloud hosting + team features
**Combinações:** Vibe-Kanban + OpenSpec (#X) = spec-driven dev com orchestration visual. Vibe-Kanban + Context7 (#X) = agents com docs atualizados automaticamente

### [lucasgelfond/zerobrew](https://github.com/lucasgelfond/zerobrew) ⭐ 4.8k | ⚡💸
**Problema:** Homebrew é lento. Instalar pacotes leva segundos a minutos. Em CI/CD e setup de novos devs, o tempo se multiplica.
**Solução:** Package manager em Rust, drop-in replacement para Homebrew. Content-addressable store (sha256), APFS clonefile (zero disk overhead), downloads paralelos. 5x cold, 20x warm speedup.
**Por que é 5-10x melhor:**
- ⚡ **Velocidade:** 5-20x comprovado em benchmarks reais (tesseract: 29.5x warm!)
- 💸 **Custo:** Open-source, usa CDN do próprio Homebrew — zero custo extra
**TAM:** $500M+ (dev tooling, package management — nichor porém alto engagement)
**Modelo de negócio:** Enterprise (caching privado, audit trails, compliance), CI/CD integration pricing
**Esforço:** Baixo-Médio — já é funcional, precisa maturar edge cases e enterprise features
**Combinações:** Zerobrew + CI/CD platforms = setup 20x mais rápido em pipelines. Modelo "uv for everything" expandível para outros OS

---

## pranshuparmar/witr ⭐ 12.3k
**Link:** https://github.com/pranshuparmar/witr
**Eixos:** 🎯💎⚡

### Problema Real
Devs e sysadmins gastam horas debugando "por que esse processo está rodando?". Hoje correlacionam manualmente ps, top, lsof, ss, systemctl, docker ps — cada ferramenta mostra estado, mas nenhuma explica causalidade.

### Como Resolve
- Responde "Why is this running?" com uma cadeia de causalidade completa
- Mostra de onde veio (supervisor, container, shell, service), como foi iniciado
- Output human-readable em vez de tabelas crípticas
- Single static binary — Linux, macOS, FreeBSD, Windows
- Homebrew, Conda, instalação via script

### Por que é 5-10x Melhor
- **🎯 Problema real:** Todo dev/sysadmin/SRE debugou processos misteriosos
- **💎 Qualidade:** Causalidade explícita vs inferência manual entre 5+ ferramentas
- **⚡ Velocidade:** 1 comando vs 15min correlacionando outputs de múltiplas tools

### TAM
- 30M+ devs/sysadmins/SREs globalmente
- Mercado de observabilidade/debugging: $20B+
- Pode ser base de produto de debugging/observabilidade mais amplo

### Modelo de Negócio
- CLI open-source como acquisition
- SaaS: versão web/cloud para fleet debugging
- Enterprise: integração com observability stacks (Datadog, Grafana)

### Esforço para Produtizar: Médio
CLI maduro, falta web UI e integração com stacks de observabilidade

### Combinações
- + observabilidade tools: witr como camada de "explicabilidade" sobre Prometheus/Grafana
- + AI: "witr + LLM" = debugging assistant que não só mostra causalidade mas sugere fix

---

## sagekit/magnitude ⭐ 3.9k
**Link:** https://github.com/sagekit/magnitude
**Eixos:** 🎯💎⚡

### Problema Real
Browser automation é frágil — seletores CSS/XPath quebram, manutenção de testes é um pesadelo, e integrar apps sem API requer scraping. Playwright/Selenium resolvem parcialmente mas precisam de código muito específico.

### Como Resolve
- **Vision-first**: usa modelos visuais (Claude Sonnet 4) para "ver" a interface
- **94% no WebVoyager** — state-of-the-art em browser benchmarks
- **API intuitiva**: `agent.act("Create a task", { data: {...} })`
- **Test runner built-in** com visual assertions ("a página parece correta?")
- **Extração estruturada** com schemas Zod

### Por que é 5-10x Melhor
- **🎯 Problema real:** Browser testing/automation é dor universal em eng
- **💎 Qualidade:** 94% accuracy vs ~60-70% de agents baseados em DOM
- **⚡ Velocidade:** Natural language vs CSS selectors = 10x menos código de manutenção

### TAM
- Mercado de test automation: $25B+ em 2025
- RPA (browser automation): $15B+
- Data extraction/scraping: $5B+

### Modelo de Negócio
- Open-core: SDK grátis, cloud execution pago
- Enterprise: CI/CD integration, parallelism, team management
- API: browser automation as a service

### Esforço para Produtizar: Médio
SDK funcional, precisa cloud infra e dashboard de test results

### Combinações
- + browser-use (#1): magnitude como test/verification layer sobre browser-use automations
- + witr (#153): debug de processos + browser agent = full stack observability/automation

---

### [MotiaDev/motia](https://github.com/MotiaDev/motia) ⭐ 14.5k | 🎯⚡🚀

**O que faz:** Framework backend unificado que elimina fragmentação de runtime. APIs, background jobs, queues, workflows, streaming, AI agents e observabilidade — tudo com um único primitivo: o **Step**. Multi-language (TS/JS/Python). Backed by Vercel OSS program.

### Problema Real
Backend moderno exige costurar 6+ ferramentas: Express p/ API, Bull p/ queues, cron p/ schedulers, Temporal p/ workflows, LangChain p/ AI agents. Cada um com sua config, deploy e debugging. Motia unifica tudo com auto-discovery de arquivos.

### Eixos de Inovação
- 🎯 **Problema real:** Todo backend team sofre com fragmentação — Motia é o "React do backend"
- ⚡ **5-10x mais rápido p/ entregar:** Um Step = um arquivo com config + handler, auto-wired
- 🚀 **5-10x mais escala:** De protótipo a produção sem trocar framework — observabilidade built-in

### TAM: $15B+ (backend frameworks + workflow automation)

### Modelo de Negócio
- Motia Cloud (hosted Steps com auto-scaling)
- Enterprise: team management, audit, compliance
- Marketplace de Steps pré-construídos

### Esforço para Produtizar: Baixo-Médio
Framework funcional, `npx motia create` já funciona. Precisa de cloud offering.

### Combinações
- + Supabase (DB) + Motia (backend logic) = full-stack serverless sem vendor lock-in
- + browser-use (automação) como Step = workflows de scraping/automação com observabilidade
