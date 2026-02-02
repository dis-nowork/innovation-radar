# 🧠 RAG & Memory: Novos Paradigmas (Fev 2026)

## LEANN — O Menor Vector Index do Mundo
- **Repo:** [yichuan-w/LEANN](https://github.com/yichuan-w/LEANN)
- **Stars:** 9.8k ⭐ | **Forks:** 834 | **Criado:** Jun 2025
- **Eixos:** 🎯💸⚡💎

### Problema Real
Vector databases tradicionais (Pinecone, Weaviate, Chroma) requerem armazenar TODOS os embeddings — consumindo storage massivo. Para 60M chunks de texto, isso são ~201GB. Inviável para uso pessoal/local.

### Inovação
LEANN usa **graph-based selective recomputation** com high-degree preserving pruning. Em vez de armazenar embeddings, computa on-demand. Resultado: **60M chunks em 6GB** (97% economia de storage) SEM perda de accuracy.

### Por que 5-10x melhor:
- **💸 Custo:** 97% menos storage = rodar RAG enterprise num laptop, zero cloud
- **⚡ Velocidade:** Indexação e busca comparáveis a soluções tradicionais
- **💎 Qualidade:** Mesma accuracy que vector DBs pesados
- **🎯 Problema:** RAG pessoal (emails, browser, chat history, code) antes era impraticável

### Use Cases Únicos
- RAG sobre browser history inteiro
- RAG sobre emails (Apple Mail integration)
- RAG sobre chat history (WeChat, iMessage)  
- RAG sobre agent memory (ChatGPT, Claude conversations)
- Drop-in MCP service para Claude Code (substitui grep keyword search)

### TAM
- Personal AI assistants: $30B+
- Enterprise RAG: $15B+
- Developer tools (code search): $5B+

### Modelo de Negócio
- **Open-source core** (MIT)
- **Managed cloud** para quem não quer self-host
- **Enterprise features** (multi-user, SSO, audit logs)

### Combinações
- LEANN + Khoj (#77) = second brain com RAG ultra-eficiente
- LEANN + Claude Code = semantic code search sem infraestrutura
- LEANN + ScreenPipe (#86) = memória total do desktop em formato compact

---

## Supermemory — Memory API Universal
- **Repo:** [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory)
- **Stars:** 16.1k ⭐ | **Forks:** 1.6k | **Criado:** Fev 2024
- **Eixos:** 🎯⚡🚀

### Problema Real
AI tools (ChatGPT, Claude, Cursor) não compartilham memória. Cada um é um silo. Você tem conhecimento espalhado em 10+ ferramentas e nenhuma conecta com a outra.

### Inovação
API de memória unificada que conecta com qualquer AI tool via MCP. Browser extension captura contexto automaticamente. Integra com Notion, Google Drive, OneDrive. Chat com suas memórias usando qualquer LLM.

### Por que 5-10x melhor:
- **🎯 Problema:** Fragmentação de conhecimento entre ferramentas AI
- **⚡ Velocidade:** Add memory em 1 clique (extension) ou via API
- **🚀 Escala:** De uso pessoal a enterprise teams

### Modelo de Negócio
- Freemium app (app.supermemory.ai)
- API paga para empresas (console.supermemory.ai)
- Self-hosting para enterprise

---

## Microsoft Magentic-UI — Web Agent Human-Centered
- **Repo:** [microsoft/magentic-ui](https://github.com/microsoft/magentic-ui)
- **Stars:** 9.6k ⭐ | **Forks:** 972 | **Criado:** Mai 2025
- **Eixos:** 🎯💎🚀

### Problema Real
Web agents existentes (browser-use, Skyvern) são black-boxes — fazem coisas sem explicar ou pedir permissão. Para tarefas sensíveis (compras, formulários, dados pessoais), isso é inaceitável.

### Inovação
**Human-in-the-loop como feature, não bug:**
- **Co-Planning:** Agente mostra plano antes de executar, humano pode editar
- **Co-Tasking:** Humano pode intervir mid-execution via browser ou chat
- **Action Guards:** Ações sensíveis requerem aprovação explícita
- **Plan Learning:** Aprende de runs anteriores para melhorar

### Por que 5-10x melhor:
- **💎 Qualidade:** 82.2% WebVoyager, 42.52% GAIA — SoTA com human-in-the-loop
- **🎯 Problema:** Confiança em agents para tarefas reais (não demos)
- **🚀 Escala:** "Tell me When" — monitoring tasks que rodam por dias

### Benchmark Results
- GAIA test set: 42.52% (com o4-mini)
- WebVoyager: 82.2%
- AssistantBench: 27.60%
- WebGames: 45.5%

### Modelo de Negócio
- Pesquisa → produto Microsoft (integração com Copilot)
- Oportunidade para forks enterprise
- White-label para vertical agents (e-commerce, travel, finance)

### Combinações
- Magentic-UI + Strix (#177) = security testing com human oversight
- Magentic-UI + TaxHacker (#103) = contabilidade AI supervisionada
- Magentic-UI + nofx (#198) = trading com humano no controle
