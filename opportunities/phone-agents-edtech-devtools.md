# 📱 Phone Agents, EdTech AI & Developer Productivity Tools
> Atualizado: 2026-02-02 | Rodada: Phone Agents + EdTech + DevTools verticais

---

## 1. zai-org/Open-AutoGLM ⭐23.0k
**Link:** https://github.com/zai-org/Open-AutoGLM
**Categoria:** AI/Phone Agent
**Eixos:** 🎯💎🚀

### Problema Real
Automação de smartphones ainda é território de RPA frágil (Appium, scripts ADB). Usuários querem dizer "abre o app X e faz Y" sem programar. Empresas gastam fortunas em QA mobile manual.

### Por que é 5-10x melhor
- **🎯 Problema:** Controle de smartphone por linguagem natural — nenhum produto open-source faz isso com modelo dedicado
- **💎 Qualidade:** Modelo 9B treinado especificamente para UI de celular (não é um LLM genérico fazendo OCR)
- **🚀 Escala:** De "scripting ADB manual" → comando de voz. Bilhões de smartphones Android/HarmonyOS

### TAM
- Mobile testing: $50B+ (Appium, BrowserStack, etc.)
- RPA mobile / assistentes pessoais: mercado nascente, potencial enorme
- Acessibilidade: idosos e PCDs que não conseguem navegar apps complexos

### Modelo de Negócio
- **Cloud API:** Cobrar por execução de tarefas em dispositivos cloud
- **Enterprise QA:** Testes automatizados de apps mobile via NL
- **White-label:** SDK para fabricantes integrarem em smartphones
- **Acessibilidade as-a-Service:** Governos pagam por acessibilidade digital

### Esforço para Produtizar: Médio-Alto
Modelo já funciona, mas precisa de infra cloud (farm de devices), reliability engineering, e suporte multi-idioma robusto.

### Combinações
- + browser-use → agente full-stack (web + mobile)
- + voice AI (Qwen3-TTS) → assistente de voz que executa tarefas no celular
- + DeepTutor → tutor que demonstra passo-a-passo no celular do aluno

---

## 2. HKUDS/DeepTutor ⭐9.9k
**Link:** https://github.com/HKUDS/DeepTutor
**Categoria:** EdTech/AI Tutor
**Eixos:** 🎯💎⚡💸

### Problema Real
Tutoria personalizada é cara ($50-200/hora). Plataformas como Chegg, Coursera, Khan Academy são genéricas. Estudantes precisam de ajuda adaptada ao SEU material (apostilas, papers, manuais técnicos).

### Por que é 5-10x melhor
- **🎯 Problema:** Upload seus docs → tutor que CONHECE seu material específico
- **💎 Qualidade:** Dual-loop reasoning (RAG + web search + code execution), knowledge graphs visuais, quiz generation
- **⚡ Velocidade:** Respostas instantâneas vs agendar horário com tutor
- **💸 Custo:** $0 self-hosted vs $50-200/hora de tutoria humana

### TAM
- Tutoria global: $100B+
- Corporate training: $370B
- Medical/legal continuing education: $20B+

### Modelo de Negócio
- **SaaS para universidades:** $5-20/aluno/mês
- **Corporate training:** White-label para empresas treinarem funcionários
- **API para EdTechs:** Integrar tutoria AI em plataformas existentes
- **Freemium individual:** Free tier limitado, premium com modelos melhores

### Esforço para Produtizar: Médio
Stack moderna (Next.js 16, React 19, Docker), múltiplos LLM providers já suportados. Precisa de multi-tenancy robusta e compliance educacional.

### Combinações
- + daily_stock_analysis → curso de finanças com análise real-time
- + Docling/RAG-Anything → ingestão superior de PDFs complexos (fórmulas, tabelas)
- + Open-AutoGLM → demonstrações práticas em apps reais

---

## 3. ZhuLinsen/daily_stock_analysis ⭐8.8k
**Link:** https://github.com/ZhuLinsen/daily_stock_analysis
**Categoria:** Fintech/Stock Analysis
**Eixos:** 🎯💸⚡🚀

### Problema Real
Bloomberg Terminal custa $24k/ano. Até ferramentas básicas como TradingView Pro custam $15-60/mês. Investidores retail querem análise inteligente sem pagar fortunas.

### Por que é 5-10x melhor
- **🎯 Problema:** Análise diária automatizada de carteira com AI — de graça
- **💸 Custo:** ZERO (Gemini free + GitHub Actions free) vs $24k/ano Bloomberg
- **⚡ Velocidade:** Análise automática diária push notification vs análise manual
- **🚀 Escala:** De "1 analista para 1 carteira" → 1 sistema para milhões de carteiras

### TAM
- Retail investing tools: $15B+
- Robo-advisory: $2.5T AUM
- Financial data terminals: $35B (Bloomberg, Refinitiv, etc.)

### Modelo de Negócio
- **Freemium SaaS:** Análise de 5 ações grátis, ilimitado $10/mês
- **White-label para brokers:** Corretoras oferecem AI analysis aos clientes
- **API de análise:** $0.01/análise para fintechs integrarem
- **Premium signals:** Alertas em tempo real com scoring de confiança

### Esforço para Produtizar: Baixo
Já funciona end-to-end com GitHub Actions. Precisa apenas de UI web, multi-tenancy, e compliance financeiro (disclaimers).

### Combinações
- + OpenStock → plataforma completa: dados + análise AI + alertas
- + virattt/dexter → pesquisa profunda + análise diária = hedge fund pessoal
- + push notifications → app mobile com alertas inteligentes

---

## 4. tobi/qmd ⭐5.5k
**Link:** https://github.com/tobi/qmd
**Categoria:** Dev Tools/Local Search
**Eixos:** 🎯💎⚡

### Problema Real
Desenvolvedores e knowledge workers têm docs espalhados (notes, meetings, wikis). Busca do OS é ruim. Grep não entende semântica. Ferramentas como Algolia são cloud-only e caras.

### Por que é 5-10x melhor
- **🎯 Problema:** Busca semântica local em TODOS seus docs — meetings, notes, wikis
- **💎 Qualidade:** Hybrid search (BM25 + vector + LLM reranking) > qualquer busca simples
- **⚡ Velocidade:** CLI instantâneo, 100% local, MCP-ready para agents

### TAM
- Enterprise search: $7B+ (Coveo, Elastic, etc.)
- Personal knowledge management: $2B+
- Developer tools: mercado em expansão com AI agents

### Modelo de Negócio
- **Enterprise:** Team/org search com sync de Confluence, Notion, Slack
- **Desktop app:** Spotlight/Alfred replacement com semantic search
- **MCP marketplace:** Plugin premium para agents (Claude, Copilot)
- **API:** Search-as-a-service local-first

### Esforço para Produtizar: Médio
Core sólido (by Tobi Lütke, CEO do Shopify!), mas precisa de GUI, sync de fontes enterprise, e empacotamento polido.

### Combinações
- + Obsidian/Notion → busca semântica cross-platform
- + meeting transcription → busca em reuniões passadas
- + Claude Code/agents → memória de longo prazo para agents

---

## 5. Maxteabag/sqlit ⭐3.5k
**Link:** https://github.com/Maxteabag/sqlit
**Categoria:** Dev Tools/Database TUI
**Eixos:** 🎯💸💎⚡

### Problema Real
GUIs de database (SSMS, DBeaver, pgAdmin) são pesadas, lentas, e feias. Devs que vivem no terminal querem algo como lazygit mas para databases.

### Por que é 5-10x melhor
- **🎯 Problema:** Query databases do terminal sem sair do flow
- **💸 Custo:** $0 vs DataGrip ($199/ano), TablePlus ($99)
- **💎 Qualidade:** 20+ databases, Docker discovery automática, SSH tunnels, vim keybinds
- **⚡ Velocidade:** Abre instantâneo vs minutos para carregar SSMS/DBeaver

### TAM
- Database management tools: $5B+
- Developer tools subscriptions: mercado em crescimento

### Modelo de Negócio
- **Pro license:** Features avançadas (query optimization, visual explain, diff)
- **Team edition:** Queries compartilhadas, audit log, RBAC
- **Enterprise:** SSO, compliance, suporte

### Esforço para Produtizar: Baixo-Médio
Já é polido e funcional. Precisa de features enterprise e modelo de monetização.

---

## 6. pranshuparmar/witr ⭐12.3k
**Link:** https://github.com/pranshuparmar/witr
**Categoria:** Dev Tools/Observability
**Eixos:** 🎯💎⚡

### Problema Real
Quando algo está rodando no sistema, devs precisam correlacionar ps + top + lsof + systemctl + docker ps manualmente para entender POR QUE está rodando. Nenhuma ferramenta responde essa pergunta diretamente.

### Por que é 5-10x melhor
- **🎯 Problema:** "Why is this running?" — pergunta universal que ninguém respondia
- **💎 Qualidade:** Mostra a CADEIA CAUSAL completa (supervisor → container → service → process)
- **⚡ Velocidade:** Uma pergunta, uma resposta vs correlacionar 5+ ferramentas

### TAM
- DevOps/SRE tools: $10B+
- Incident management: $3B+
- Security forensics: precisa saber "quem/por que iniciou isso?"

### Modelo de Negócio
- **Enterprise CLI:** Licença comercial com integração a SIEM/monitoring
- **SaaS dashboard:** Versão web com histórico e alertas
- **Security product:** "Why is this running?" como feature de EDR/XDR

### Esforço para Produtizar: Baixo
Binário Go estático, cross-platform, já packaged em Homebrew e mais. Core product pronto.

### Combinações
- + observability stacks (SigNoz, OpenObserve) → root cause analysis automática
- + security tools → detecção de processos suspeitos com explicação
