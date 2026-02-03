# AI Agent Orchestration & Research Infrastructure (Fev 3, 2026)

**Ângulo:** Plataformas e frameworks que formam a infraestrutura da próxima onda de AI agents autônomos — desde agents que pesquisam, até agents que controlam computadores, passando pela cola (backends e canvas) que junta tudo.

---

## 72. kortix-ai/suna ⭐ 19.3k
**Link:** https://github.com/kortix-ai/suna
**O que faz:** Plataforma completa para criar, gerenciar e treinar AI agents autônomos. Inclui "Kortix Super Worker" — um agent generalista que faz browser automation, file management, web crawling, API integrations, e system operations.

**Problema real:** Empresas querem AI agents customizados mas não têm infra. Hoje, montar um agent autônomo requer juntar 5-10 libs (browser, files, search, code exec, memory) manualmente. Suna é plug-and-play.

**Eixos de inovação:**
- 🎯 **Problema real:** Empresas gastam semanas montando infra de agents. Suna = dias.
- ⚡ **5-10x mais rápido:** Agent Builder visual + templates prontos vs. código from scratch
- 🚀 **5-10x mais escala:** De "1 developer fazendo 1 agent" pra "equipe inteira criando fleet de agents"
- 💸 **5-10x menor custo:** Self-hostable vs. plataformas pagas ($200-500/mês como OpenAI's platform)

**TAM:** AI agent platforms = $5-15B em 2027. Enterprise agent deployment = growing 80% YoY.

**Modelo de negócio:** Cloud managed (freemium) + Enterprise self-hosted + Marketplace de agents/templates

**Esforço para produtizar:** Médio — já tem UI, Docker deploy, templates. Precisa polir enterprise features (RBAC, audit log, multi-tenant).

**Combinações:** Suna + flowgram.ai (canvas visual) + cua (computer use sandbox) = plataforma enterprise completa de AI agents.

---

## 73. bytedance/deer-flow ⭐ 19.6k
**Link:** https://github.com/bytedance/deer-flow
**O que faz:** Framework de Deep Research que combina LLMs com web search, crawling, e Python code execution para fazer pesquisas autônomas profundas. Gera relatórios completos com imagens e até podcasts.

**Problema real:** Pesquisar temas complexos leva horas/dias de trabalho manual. Consultores, analistas, acadêmicos gastam 60%+ do tempo coletando informação. Deep Research automatiza o loop search→read→synthesize→refine.

**Eixos de inovação:**
- 🎯 **Problema real:** Pesquisa manual é o maior gargalo de knowledge workers
- ⚡ **5-10x mais rápido:** Relatório que levaria 4-8h feito em 10-30min
- 💎 **5-10x mais qualidade:** Multi-source synthesis + iterative refinement > Google search manual

**TAM:** Research & analytics tools = $30B. Consulting services (McKinsey, BCG, etc.) = $300B — AI research agents canibalizam parcela significativa.

**Modelo de negócio:** API usage-based + Enterprise white-label + Vertical solutions (legal research, market intelligence, due diligence)

**Esforço para produtizar:** Médio — bem documentado, MCP integration, Docker ready. Precisa customização por vertical.

**Combinações:** deer-flow + ExtractThinker (#55) = deep research com document intelligence. deer-flow + kreuzberg (#36) = research pipeline que lê 50+ formatos de docs.

---

## 74. MotiaDev/motia ⭐ 14.5k
**Link:** https://github.com/MotiaDev/motia
**O que faz:** Framework backend unificado que consolida APIs, background jobs, filas, workflows, streams, e AI agents num único primitivo: o "Step". Multi-language (JS, TS, Python). Built-in observability e state management.

**Problema real:** Backend dev é fragmentado — Express pra APIs, Bull pra filas, cron pra jobs, LangChain pra agents, cada um com seu runtime. Motia unifica tudo como React unificou frontend com componentes.

**Eixos de inovação:**
- 🎯 **Problema real:** Developer fatigue de gerenciar 5-8 runtimes diferentes
- ⚡ **5-10x mais rápido:** Um primitivo (Step) em vez de aprender 5 frameworks
- 🚀 **5-10x mais escala:** Auto-discovery + event-driven = horizontal scaling natural

**TAM:** Backend framework market = $5B+. Workflow orchestration = $10B+. Motia ataca a interseção.

**Modelo de negócio:** Open core + Cloud hosted (managed Steps) + Enterprise support (SLA, custom integrations)

**Esforço para produtizar:** Médio-Alto — framework precisa de ecosystem (plugins, templates, marketplace). Vercel partnership ajuda (vide Open Source Program).

**Combinações:** Motia + flowgram.ai = visual builder sobre backend unificado. Motia + activepieces = automation platform com backend robusto.

---

## 75. trycua/cua ⭐ 12.2k
**Link:** https://github.com/trycua/cua
**O que faz:** Infraestrutura open-source para Computer-Use Agents. Inclui: sandboxes isolados (Docker, QEMU, Apple Virtualization), SDK para controlar desktops, benchmarks para avaliar agents, e suporte a macOS/Linux/Windows.

**Problema real:** Computer-use agents (tipo Claude Computer Use, OpenAI Operator) precisam de ambientes isolados e seguros para rodar. Hoje, montar isso é complexo e inseguro. CUA resolve com sandboxes + SDK + benchmarking suite.

**Eixos de inovação:**
- 🎯 **Problema real:** Rodar AI agents que controlam computadores sem sandbox = risco de segurança massivo
- ⚡ **5-10x mais rápido:** SDK pronto vs. construir infra de sandbox + screen capture + input injection from scratch
- 🚀 **5-10x mais escala:** De "1 agent no meu laptop" pra "fleet de agents em VMs isoladas"
- 💎 **5-10x mais qualidade:** Benchmarking suite (OSWorld, ScreenSpot, Windows Arena) = medir e melhorar agents sistematicamente

**TAM:** Computer-use agent market nascente mas explodindo. RPA market = $13B (2025). Computer-use agents substituem RPA → $20-30B em 3-5 anos.

**Modelo de negócio:** Cloud sandbox hosting (pay-per-minute) + Enterprise deployment + Benchmark-as-a-service para empresas de AI

**Esforço para produtizar:** Médio — já tem Docker, SDK, CLI. Precisa de cloud hosting layer e billing.

**Combinações:** cua + nanobrowser (#76) = agents que controlam tanto desktop quanto browser. cua + suna (#72) = plataforma completa de agents com sandbox seguro.

---

## 76. nanobrowser/nanobrowser ⭐ 12.1k
**Link:** https://github.com/nanobrowser/nanobrowser
**O que faz:** Chrome extension open-source para AI web automation com multi-agent system (Planner + Navigator). Usa sua própria API key de LLM — alternativa gratuita ao OpenAI Operator ($200/mês).

**Problema real:** OpenAI Operator custa $200/mês. Pessoas querem AI browser automation mas não querem pagar ou ceder dados. Nanobrowser = grátis, roda local, usa qualquer LLM.

**Eixos de inovação:**
- 🎯 **Problema real:** Browser automation com AI é o futuro do trabalho de escritório
- 💸 **5-10x menor custo:** $0/mês + seus API keys vs. $200/mês do Operator
- 🚀 **5-10x mais escala:** Multi-agent system (Planner auto-corrige e redireciona Navigator) = mais confiável

**TAM:** RPA + browser automation = $15B. AI-powered = premium segment growing 100%+ YoY.

**Modelo de negócio:** Freemium extension + Pro features (scheduling, multi-tab, team workflows) + Enterprise managed deployment

**Esforço para produtizar:** Baixo-Médio — já é extension publicada no Chrome Web Store. Monetizar via premium features.

**Combinações:** nanobrowser + postiz (#8) = social media automation inteligente. nanobrowser + chatwoot (#7) = AI customer service que navega por sistemas.

---

## 77. bytedance/flowgram.ai ⭐ 7.6k
**Link:** https://github.com/bytedance/flowgram.ai
**O que faz:** Framework extensível para construir plataformas de AI workflow. Inclui: canvas visual (free layout + fixed layout), forms de configuração, variáveis com scope chain, materiais prontos (LLM, Condition, Code Editor). Não é uma plataforma pronta — é o toolkit para construir a sua.

**Problema real:** Todo mundo quer construir "o Dify/n8n do meu nicho" mas o canvas visual é a parte mais difícil e demorada (6-12 meses de dev). FlowGram = canvas pronto em dias.

**Eixos de inovação:**
- 🎯 **Problema real:** Construir visual workflow builder from scratch = 6-12 meses. Com FlowGram = dias.
- ⚡ **5-10x mais rápido:** Framework pronto com canvas, forms, variáveis, drag-and-drop
- 🚀 **5-10x mais escala:** Um framework, infinitas plataformas verticais

**TAM:** Workflow automation platforms = $15B+. FlowGram é infra-layer — multiplica por cada vertical (healthcare workflows, legal workflows, finance workflows).

**Modelo de negócio:** Open core + Enterprise support + Commercial license para platforms built on FlowGram

**Esforço para produtizar:** Médio — é framework, não produto final. Mas isso é o ponto: quem usa FlowGram para construir vertical platforms tem vantagem massiva.

**Combinações:** FlowGram + motia (#74) = visual workflow builder sobre backend unificado. FlowGram + suna (#72) = agent builder platform com canvas visual profissional. FlowGram + simstudio (#9) = competidor direto do Dify.
