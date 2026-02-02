# ☁️ Infra/Cloud

Deploy, monitoring, PaaS self-hosted.

### [coollabsio/coolify](https://github.com/coollabsio/coolify) ⭐ 50.1k | 🎯💸🚀
**Problema:** Vercel/Netlify ficam caros em produção ($20-100/mês por projeto).
**Solução:** PaaS self-hosted: deploy 1-click no seu VPS de $5/mês. DX de Vercel, preço de VPS.
**Por que é superior:** 💸 $5/mês vs $100+ no Vercel. 🚀 50k stars = maior PaaS open-source. 🎯 Todo dev precisa de deploy.

---

### [dokploy/dokploy](https://github.com/dokploy/dokploy) ⭐ 29.7k | 🎯💸
**Problema:** Mesmo problema do Coolify — deploy caro e lock-in em plataformas cloud.
**Solução:** PaaS open-source com Docker: deploy, databases, certificados, tudo em um painel.
**Por que é superior:** 💸 Grátis vs Heroku/Railway. 🎯 29k stars, UX moderna. Alternativa mais leve ao Coolify.

---

### [openstatusHQ/openstatus](https://github.com/openstatusHQ/openstatus) ⭐ 8.3k | 🎯💸
**Problema:** Pingdom ($15/mês) + Statuspage ($29/mês) = $44/mês só pra monitorar uptime.
**Solução:** Monitoring + status page unificados, open-source.
**Por que é superior:** 💸 2 ferramentas pagas substituídas por 1 grátis. 🎯 Todo SaaS precisa de status page.

---

### [skypilot-org/skypilot](https://github.com/skypilot-org/skypilot) ⭐ 9.4k | 💸⚡
**Problema:** Workloads de AI ficam presos num cloud provider caro (GPU on-demand é proibitivo).
**Solução:** Orquestrador multi-cloud: roda AI workloads no provider mais barato automaticamente.
**Por que é superior:** 💸 Encontra GPU 3-5x mais barata entre providers. ⚡ Setup automático, sem lock-in.

---

### [alibaba/higress](https://github.com/alibaba/higress) ⭐ 7.4k | ⚡📈
**Problema:** API gateways tradicionais não entendem tráfego de LLMs (tokens, rate limiting por modelo).
**Solução:** API gateway AI-native: roteamento inteligente de LLMs, load balancing por custo/latência.
**Por que é superior:** ⚡ Roteamento inteligente reduz latência. 📈 Escala tráfego de AI sem config manual.

---


### [ai-dynamo/dynamo](https://github.com/ai-dynamo/dynamo) ⭐ 6.0k | ⚡📈🚀💸
**Problema:** Servir LLMs em produção requer orquestração complexa de GPUs, especialmente para modelos grandes que excedem capacidade de uma GPU. Tensor parallelism cria gargalos de coordenação. Empresas gastam fortunas em infra subotimizada.
**Solução:** NVIDIA Dynamo — framework open-source de inferência distribuída. Disaggregated prefill & decode, dynamic GPU scheduling, LLM-aware request routing, KV cache offloading. Engine-agnostic (TRT-LLM, vLLM, SGLang). Rust + Python.
**Por que é 5-10x melhor:**
- ⚡ **Velocidade:** Disaggregated serving + NIXL = latência dramaticamente menor
- 📈 **Volume:** Datacenter-scale, multi-node nativo — não é wrapper, é framework fundamental
- 🚀 **Escala:** De single-GPU para clusters com scheduling dinâmico
- 💸 **Custo:** Open-source vs proprietary serving (Anyscale, Modal pricing). GPU utilization otimizada = menos GPUs necessárias
**TAM:** $10B+ (AI inference infrastructure, o mercado mais quente de 2025-2026)
**Modelo de negócio:** Open-core (NVIDIA vende hardware + consulting), mas terceiros podem construir managed platforms em cima
**Esforço:** Alto — requer expertise em GPU infra e distributed systems
**Combinações:** Dynamo + qualquer modelo open-source = serving de produção. Dynamo + deepinfra/together model = competir com OpenAI em custo
