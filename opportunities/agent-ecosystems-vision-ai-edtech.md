# Agent Ecosystems, Vision AI & EdTech Gaming — 2026-02-02

## 1. GetStream/Vision-Agents ⭐ 4.8k
**Open Vision Agents — real-time video AI framework**
- **Problema real:** Construir apps de video AI com latência <30ms é nightmare de infra. Precisa combinar YOLO + LLM + edge network + SDKs nativos. Hoje leva 6+ meses e equipe especializada.
- **O que faz:** Framework completo p/ criar "agents que veem" — combina object detection (YOLO/Roboflow) com LLMs (Gemini/OpenAI) em real-time via edge network da Stream. SDKs p/ React, iOS, Android, Flutter, Unity.
- **Eixos de inovação:** 🎯⚡🚀💸
  - 🎯 Resolve integração complexa video+AI+edge em poucas linhas
  - ⚡ Latência <30ms, join em 500ms — ordem de magnitude melhor que soluções DIY
  - 🚀 De "preciso de equipe de 5 engenheiros" → "1 dev em 1 dia"
  - 💸 Open-source vs custom builds de $200k+
- **TAM:** Video AI market $20B+ (security, sports coaching, healthcare, retail analytics, AR/VR)
- **Modelo de negócio:** Open-source framework + Stream edge network (usage-based), enterprise support
- **Esforço:** Médio — framework funcional, mas precisa edge infra (Stream ou própria)
- **Combinações:** + NVIDIA Personaplex (#330) p/ full-duplex voice over video + OpenCut p/ video editing pipeline
- **Use cases demonstrados:** Golf coaching AI, security camera com theft detection + WANTED poster automático, invisible interview assistant

## 2. langchain-ai/deepagents ⭐ 8.8k
**Batteries-included agent harness by LangChain**
- **Problema real:** Criar AI agents funcionais ainda requer wiring manual de prompts, tools, context management, sub-agents. Cada projeto reinventa a roda.
- **O que faz:** Agent harness opinionado que funciona out-of-box: planning (write_todos/read_todos), filesystem (read/write/edit), shell access, sub-agents, auto-summarization. `pip install deepagents` e pronto.
- **Eixos de inovação:** 🎯⚡🚀
  - 🎯 Elimina ~80% do boilerplate de agent creation
  - ⚡ De "semanas configurando" → "1 comando pip install"
  - 🚀 Provider-agnostic (Claude/OpenAI/Google/qualquer LangChain-compatible)
- **TAM:** AI agent tooling $5-10B, developer tools $30B+
- **Modelo de negócio:** Open-source (MIT) + LangSmith (observability SaaS) + LangChain Cloud (hosting)
- **Esforço:** Baixo — funciona imediatamente, customização é gradual
- **Combinações:** + MCP servers qualquer + LangSmith p/ observability + Modal/Runloop p/ sandboxing
- **Diferencial:** LangChain ecosystem (100k+ devs), native LangGraph (streaming, persistence, checkpointing)

## 3. sapientinc/HRM ⭐ 12.3k
**Hierarchical Reasoning Model — 27M params that beat huge models on reasoning**
- **Problema real:** LLMs de reasoning (o3, DeepSeek-R1) usam CoT que é lento, caro e requer dados massivos. Inference de um problema complexo = minutos e $$$. 
- **O que faz:** Arquitetura recurrent novel com 2 módulos: high-level (planejamento abstrato lento) + low-level (computação rápida detalhada). 27M params, 1000 training samples, sem pre-training ou CoT data.
- **Eixos de inovação:** 🎯💎⚡💸
  - 🎯 Resolve reasoning em single forward pass (sem chain-of-thought iterativo)
  - 💎 Near-perfect em Sudoku complexo, maze pathfinding. Supera modelos 1000x maiores no ARC benchmark
  - ⚡ Single forward pass vs iterações repetidas de CoT
  - 💸 27M params vs bilhões — ordens de magnitude mais barato em inference
- **TAM:** AI reasoning/foundation model market $50B+ (se escalar)
- **Modelo de negócio:** Research → licensing, inference API, embedded reasoning engine
- **Esforço:** Alto — pesquisa frontier, precisa validação em tarefas broader
- **Potencial transformativo:** Se HRM escala pra linguagem natural, pode redefinir custo de inference em 100x
- **Risco:** Ainda é pesquisa. Performance em puzzles ≠ performance em NL tasks

## 4. jd-opensource/joyagent-jdgenie ⭐ 11.3k
**First end-to-end open-source multi-agent product by JD.com**
- **Problema real:** Frameworks de agents (LangChain, Dify, n8n) requerem desenvolvimento adicional. Não são produtos prontos para uso.
- **O que faz:** Produto completo end-to-end: query ou task → resposta/solução direta. Sub-agents especializados (report gen, code, PPT, file, data). Frontend + backend + framework + engine, tudo open-source.
- **Eixos de inovação:** 🎯💎🚀
  - 🎯 Primeiro agent product (não framework) verdadeiramente open-source
  - 💎 GAIA benchmark: 75.15% validation (supera OWL/CAMEL, Smolagent/HuggingFace, xManus)
  - 🚀 De framework customizável → produto usável sem dev
- **TAM:** Enterprise AI assistants $15B+, knowledge worker productivity
- **Modelo de negócio:** Open-source product + enterprise customization + vertical solutions
- **Esforço:** Médio — produto funcional, precisa localização e vertical customization
- **Diferencial vs Manus/Dify:** Não depende de ecossistema externo (vs Alibaba→Bailian, Coze→Volcengine)

## 5. pshenok/server-survival ⭐ 4.5k
**Tower defense game that teaches cloud architecture**
- **Problema real:** Cloud architecture é complexo demais para aprender via docs. Profissionais levam meses para entender scaling, DDoS mitigation, load balancing na prática.
- **O que faz:** Jogo 3D interativo onde você é um Cloud Architect — build infra (firewalls, load balancers, CDN, databases), gerencia budget, reputa e health contra traffic escalante e DDoS attacks.
- **Eixos de inovação:** 🎯💎🚀
  - 🎯 Gamificação de conhecimento técnico complexo — aprende fazendo
  - 💎 Visualização 3D interativa vs slides estáticos de treinamento
  - 🚀 De "preciso estudar 6 meses de docs" → "aprendo jogando em 2 horas"
- **TAM:** Cloud training/certification $5B+ (AWS/GCP/Azure certification market alone)
- **Modelo de negócio:** Freemium game + enterprise training licenses + certification prep
- **Esforço:** Médio — game funcional, precisa conteúdo expandido e branding
- **Combinações:** + real cloud sandboxes (Ubicloud #135) p/ apply skills aprendidos

## 6. aidenybai/react-grab ⭐ 4.7k
**Select context for coding agents directly from your website**
- **Problema real:** Coding agents (Cursor, Claude Code) não sabem qual componente React corresponde a qual elemento visual. Dev precisa encontrar manualmente file+component+code.
- **O que faz:** Hover sobre qualquer elemento + Cmd+C → copia filename, React component name e HTML source. Dá 3x speedup e accuracy pra coding agents.
- **Eixos de inovação:** 🎯⚡💎
  - 🎯 Ponte visual→código que ninguém tinha construído
  - ⚡ 3x mais rápido vs busca manual
  - 💎 Context perfeito (component + file path + source) vs copia-e-cola genérico
- **TAM:** Developer tools $30B+ (especificamente coding agent tooling, crescendo exponencialmente)
- **Modelo de negócio:** Open-source dev tool + premium features (enterprise, team analytics)
- **Esforço:** Baixo — `npx grab init` e funciona
- **Combinações:** + Onlook (#78) p/ visual editing + Figma-Context-MCP (#255)
