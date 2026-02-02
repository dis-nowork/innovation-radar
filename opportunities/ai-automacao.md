# 🤖 AI/Automação

Agentes, automação de browser, workflows inteligentes.

### [browser-use/browser-use](https://github.com/browser-use/browser-use) ⭐ 77.5k | 🎯⚡🚀
**Problema:** RPA tradicional quebra quando sites mudam layout. Empresas gastam fortunas mantendo scripts Selenium/Puppeteer.
**Solução:** Automação de browser com LLMs que enxergam a página como humano — não depende de seletores CSS.
**Por que é superior:** ⚡ 10x mais rápido de configurar (sem mapear seletores). 🚀 Escala pra qualquer site sem manutenção. TAM: RPA $13B+.

---

### [mem0ai/mem0](https://github.com/mem0ai/mem0) ⭐ 46.3k | 🎯⚡📈
**Problema:** Chatbots e agentes AI esquecem tudo entre sessões — zero continuidade.
**Solução:** API de memória persistente que qualquer app AI integra em minutos.
**Por que é superior:** ⚡ Integração em horas vs semanas construindo do zero. 📈 Cada interação melhora o retrieval (efeito rede). Infra-play tipo Pinecone.

---

### [simstudioai/sim](https://github.com/simstudioai/sim) ⭐ 26.3k | 🎯⚡🚀
**Problema:** Orquestrar agentes AI exige código complexo — inacessível pra não-devs.
**Solução:** Builder visual drag-and-drop pra criar pipelines de agentes AI sem código.
**Por que é superior:** ⚡ De semanas de código pra horas no visual builder. 🚀 Abre mercado de AI agents pra qualquer empresa. 26k stars em 1 ano.

---

### [Skyvern-AI/skyvern](https://github.com/Skyvern-AI/skyvern) ⭐ 20.2k | 🎯💎⚡
**Problema:** Bots de automação web quebram toda vez que o site atualiza o layout.
**Solução:** RPA com AI vision — entende interfaces visualmente como humano, não depende de DOM.
**Por que é superior:** 💎 Qualidade absurda: bots que não quebram. ⚡ Zero manutenção quando sites mudam. AGPL = moat competitivo.

---

### [comet-ml/opik](https://github.com/comet-ml/opik) ⭐ 17.6k | 🎯⚡
**Problema:** LLMs em produção são caixas pretas — sem visibilidade de erros, custos ou drift.
**Solução:** Observabilidade e debug de LLMs/agentes — tracing, avaliação, monitoramento contínuo.
**Por que é superior:** 🎯 Problema real e urgente: toda empresa com AI em produção precisa. ⚡ Setup em minutos vs construir monitoring from scratch.

---

### [getzep/graphiti](https://github.com/getzep/graphiti) ⭐ 22.5k | 🎯💎⚡
**Problema:** Agentes AI operam em ambientes dinâmicos mas dependem de RAG estático (batch processing, embeddings congelados). Quando dados mudam, o contexto fica stale.
**Solução:** Framework para knowledge graphs temporais — integra interações de usuários, dados enterprise e informações externas em grafo queryável em real-time. Modelo bi-temporal (quando aconteceu vs quando foi ingerido). Busca híbrida: semântica + keyword + grafo.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo agente AI precisa de memória estruturada que evolui
- 💎 **Qualidade:** State-of-the-art em agent memory (paper publicado). Não é just outro vector DB
- ⚡ **Velocidade:** Incremental updates em real-time vs recomputar grafo inteiro
**TAM:** $3B+ (AI memory/context infrastructure)
**Modelo de negócio:** Zep (managed platform) é o produto pago. Graphiti é o OSS core
**Esforço:** Médio — requer Neo4j, mas SDK Python/TS bem documentado
**Combinações:** Graphiti + Screenpipe (#86) = knowledge graph do que você vê/ouve. Graphiti + TrendRadar (#90) = intelligence temporal com relações causais

---

### [different-ai/openwork](https://github.com/different-ai/openwork) ⭐ 8.1k | 🎯💸
**Problema:** Claude Cowork é pago e closed-source. Pessoas querem AI workspace colaborativo sem vendor lock-in.
**Solução:** Open-source alternative ao Claude Cowork, powered by opencode. Workspace AI-native para colaboração humano-AI.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Colaboração humano-AI é o futuro do trabalho
- 💸 **Custo:** Grátis self-hosted vs subscription do Claude
**TAM:** $10B+ (AI-assisted productivity tools)
**Modelo de negócio:** Cloud hosting, enterprise features
**Esforço:** Médio — projeto jovem (Jan 2026), crescimento rápido

---

### [bytebot-ai/bytebot](https://github.com/bytebot-ai/bytebot) ⭐ 10.3k | 🎯⚡🚀💎
**Problema:** Browser agents só fazem web. RPA tradicional só faz cliques scripted. Ninguém resolve "dê uma task complexa a um computador virtual e deixe ele resolver".
**Solução:** AI desktop agent self-hosted — Ubuntu Linux completo em container. O AI vê a tela, move mouse, digita, usa qualquer app (browser, IDE, email, terminal), instala software conforme precisa.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Milhões de tarefas manuais que envolvem múltiplos apps desktop
- ⚡ **Velocidade:** Deploy em 2 minutos via Docker
- 🚀 **Escala:** N tasks paralelas, cada uma em container isolado
- 💎 **Qualidade:** Não é limitado a browser — usa QUALQUER app, como um funcionário real
**TAM:** RPA $13B+, AI assistants $25B+
**Modelo de negócio:** Open core → managed cloud → enterprise (multi-agent orchestration)
**Esforço:** Médio — funcional mas early stage

---

### [activepieces/activepieces](https://github.com/activepieces/activepieces) ⭐ 20.6k | 🎯💸🚀⚡
**Problema:** Zapier ($19.99-$799/mês) e Make ($9-$299/mês) são caros. Nenhum tem MCP/AI agents nativos.
**Solução:** Workflow automation open-source com ~400 MCP servers + AI agents nativos.
**Por que é 5-10x melhor:**
- 💸 **Custo:** Self-hosted grátis vs centenas/mês em Zapier
- 🚀 **Escala:** 400+ integrações MCP = AI agent acessa tudo
- ⚡ **Velocidade:** Visual builder + MCP = conectar AI a qualquer serviço em minutos
**TAM:** Workflow automation $15B+
**Modelo de negócio:** Open core → Cloud SaaS → Enterprise
**Esforço:** Baixo — 58k+ commits, equipe ativa, produto maduro

---

### [VoltAgent/voltagent](https://github.com/VoltAgent/voltagent) ⭐ 5.4k | 🎯⚡💎
**Problema:** Construir AI agents em TypeScript/Node.js é fragmentado — sem standard framework, sem observability.
**Solução:** AI Agent Engineering Platform — TypeScript, observability built-in, MCP, multi-agent, console visual.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** TypeScript devs (65%+ dos web devs) precisam de framework sério pra agents
- ⚡ **Velocidade:** Composable architecture — agents como building blocks
- 💎 **Qualidade:** Observability nativa + console visual de debugging
**TAM:** AI framework/tooling $5B+
**Modelo de negócio:** Open core → managed platform → enterprise console
**Esforço:** Médio — crescendo rápido, precisa de mais integrações

---

### [vas3k/TaxHacker](https://github.com/vas3k/TaxHacker) ⭐ 1.1k | 🎯💸⚡
**Problema:** Freelancers gastam 5-20h/mês organizando receipts. QuickBooks/FreshBooks $15-55/mês + input manual.
**Solução:** Contabilidade AI self-hosted. Foto de receipt → AI extrai tudo. Multi-moeda com conversão histórica.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Pain point #1 de freelancers
- 💸 **Custo:** Self-hosted grátis vs $20-55/mês
- ⚡ **Velocidade:** Foto → dados estruturados em segundos vs 5-10 min/receipt manual
**TAM:** 1.57B freelancers. Accounting software $20B+
**Modelo de negócio:** Open core → Cloud → White-label pra contadores
**Esforço:** Médio — early stage, creator com track record (vas3k.club)

---

### [rishikanthc/Scriberr](https://github.com/rishikanthc/Scriberr) ⭐ 2.0k | 🎯💸💎
**Problema:** Otter.ai $16-40/mês, envia dados pra cloud. Profissionais precisam de transcrição local (compliance).
**Solução:** Transcrição AI 100% offline/local. NVIDIA Parakeet + Whisper. Speaker diarization. Word-level timing.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Privacidade de áudio é critical pra legal, saúde, finanças
- 💸 **Custo:** Grátis vs $200-480/ano em SaaS
- 💎 **Qualidade:** NVIDIA Parakeet SoTA em accuracy
**TAM:** Transcription $30B+. Healthcare transcription $5B+
**Modelo de negócio:** Open core → Enterprise (batch, API) → Vertical (legal, medical)
**Esforço:** Médio — funcional, GPU recomendado

---

### [oraios/serena](https://github.com/oraios/serena) ⭐ 19.6k | 🎯💎⚡
**Problema:** LLMs desperdiçam tokens lendo arquivos inteiros pra entender código.
**Solução:** IDE-like tools como MCP — symbol-level retrieval e editing semântico.
**Por que é 5-10x melhor:**
- 💎 **Qualidade:** Symbol-level > text-level. Menos erros, mais precisão
- ⚡ **Velocidade:** 10x menos tokens = 10x mais rápido e barato
**TAM:** AI coding tools $10B+
**Modelo de negócio:** Open core → IDE plugins premium → Enterprise
**Esforço:** Baixo — já funciona com Claude Code, Codex, VSCode, Cursor, IntelliJ

---

### [CapSoftware/Cap](https://github.com/CapSoftware/Cap) ⭐ 16.8k | 🎯💸💎
**Problema:** Loom cobra $12.50-15/user/mês. Times de 20+ pagam $3-4k/ano.
**Solução:** Screen recording open-source com sharing bonito. Tauri/Rust + Next.js. Self-hostável.
**Por que é 5-10x melhor:**
- 💸 **Custo:** Self-hosted grátis vs $150-180/user/ano no Loom
- 💎 **Qualidade:** Tauri (Rust) = performance nativa. Docker deploy em 1 comando
**TAM:** Async video $5B+. Remote work tools $30B+
**Modelo de negócio:** Cloud managed → Enterprise (SSO, branding, analytics)
**Esforço:** Baixo — muito maduro, self-hosting em 1 comando

---

### [rapidaai/voice-ai](https://github.com/rapidaai/voice-ai) ⭐ 559 | 🎯⚡🚀
**Problema:** Vapi.ai ($0.05-0.50/min), Bland.ai ($0.09/min) — voice AI em produção é caro.
**Solução:** Orquestração voice AI open-source em Go/gRPC. LLM-agnostic, production-grade.
**Por que é 5-10x melhor:**
- ⚡ **Velocidade:** Go + gRPC = latência mínima (critical pra conversas)
- 🚀 **Escala:** Enterprise-ready desde day 1
**TAM:** Conversational AI $32B+. Call centers $400B+
**Modelo de negócio:** Open core → managed → enterprise
**Esforço:** Alto — jovem (559 stars), arquitetura sólida, precisa crescer

---

---

## zai-org/Open-AutoGLM ⭐ 23.0k
**Link:** https://github.com/zai-org/Open-AutoGLM
**Eixos:** 🎯⚡🚀💎 (4 eixos!)

### Problema Real
Bilhões de pessoas usam smartphones mas dependem de toque manual para tudo. Automação mobile hoje é caro (Appium é complexo), frágil (coordenadas fixas), e requer dev skills. Assistentes como Siri/Google Assistant fazem muito pouco — abrem apps, não executam tarefas complexas.

### Como Resolve
- **Phone Agent** que controla Android e HarmonyOS via linguagem natural
- Modelo 9B especializado (multilingual: chinês + inglês)
- Usa ADB para controle — screen understanding multimodal
- "Abre Xiaohongshu e busca receitas" → executa automaticamente
- Confirmação de segurança em ações sensíveis
- Suporte remoto via WiFi ADB
- Integração com Midscene.js para iOS/Android automation SDK

### Por que é 5-10x Melhor
- **🎯 Problema real:** 5B+ smartphones, automação mobile é universalmente desejada
- **⚡ Velocidade:** Linguagem natural vs 20 toques manuais por tarefa
- **🚀 Escala:** De "só devs automatizam phones" para "qualquer pessoa automatiza"
- **💎 Qualidade:** Modelo especializado em phone UI > general purpose LLM + prompt

### TAM
- 5B+ smartphones globalmente
- Mercado de RPA mobile: $5B+ e crescendo 30%/ano
- Accessibility market: $10B+ (idosos, PCD)
- Enterprise mobile automation: $8B+

### Modelo de Negócio
- Open-source modelo base, cloud API premium
- Enterprise: fleet management, compliance, auditoria
- Consumer: "AI assistant pro" subscription
- Accessibility: parcerias com governos/ONGs

### Esforço para Produtizar: Alto
Modelo funcional mas focado em ecossistema chinês. Precisa: suporte iOS nativo, UX consumer-friendly, app distribution (Play Store), cloud inference

### Combinações
- + VibeVoice (#76): voice command → phone automation = hands-free phone control
- + browser-use (#1): phone agent + browser agent = automação cross-platform total
- + Hyprnote (#155): durante meeting no phone, agent toma notas e executa follow-ups
