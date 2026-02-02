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

---

### [ubicloud/ubicloud](https://github.com/ubicloud/ubicloud) ⭐ 11.8k | 🎯💸🚀📈
**Problema:** AWS/Azure/GCP cobram 3-10x mais que o custo real de bare metal. Startups e médias empresas pagam premium por conveniência. Lock-in é brutal — migrar custa meses de trabalho.
**Solução:** Cloud open-source que roda em bare metal (Hetzner, Leaseweb, AWS Bare Metal). Compute elástico, block storage, firewall, load balancer, managed Postgres, K8s, AI inference, IAM. Tudo self-hosted ou managed.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo negócio com infra cloud sofre com custos excessivos — é o pain point #1 de CTOs
- 💸 **Custo:** 3-10x mais barato que AWS. Hetzner bare metal + Ubicloud = cloud completa a preço de VPS
- 🚀 **Escala:** De um servidor a clusters completos, com K8s integrado
- 📈 **Volume:** GitHub Actions integration = CI/CD 10x mais barato. AI inference nativo
**TAM:** $500B+ (cloud infrastructure é um dos maiores mercados de tech)
**Modelo de negócio:** Managed service (console.ubicloud.com) + enterprise features + suporte
**Esforço:** Alto — infra é complexo, mas o projeto está maduro (Ruby, Docker, 11.8k stars)
**Combinações:** Ubicloud + Coolify/Dokploy = PaaS self-hosted completo. Ubicloud + AI inference = GPU cloud 5x mais barato

---

### [tw93/Mole](https://github.com/tw93/Mole) ⭐ 32.8k | 🎯💸💎

**O que faz:** CLI all-in-one para limpeza e otimização de Mac — substitui CleanMyMac ($40/ano), AppCleaner, DaisyDisk ($13), iStat Menus ($12). Limpeza profunda (caches, logs, browser data), desinstalador inteligente (remove remnants ocultos), análise de disco visual, monitor de sistema real-time, purge de build artifacts. Homebrew install, Vim keybinds, dry-run mode.

**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo Mac user acumula dezenas de GB em caches/logs. CleanMyMac é o app mais popular mas custa $40/ano
- 💸 **Grátis e open-source** vs $65+/ano combinado (CleanMyMac+DaisyDisk+iStatMenus)
- 💎 **4 ferramentas em 1** — CLI elegante com UX pensada (Vim bindings, dry-run, whitelists, operation log)

**TAM:** $2B+ (Mac utility software) — 100M+ Mac users ativos

**Modelo de negócio:**
- Freemium: CLI grátis, GUI app pro paga
- Enterprise: fleet management, MDM integration
- Sponsorship/donations (já tem BuyMeACoffee)

**Esforço:** Baixo — já funcional, `brew install mole`. Oportunidade em GUI wrapper e versão Windows

**Combinações:**
- Standalone — já é produto completo
- + Zerobyte (#170): clean + backup = maintenance suite completa p/ self-hosters

---

### [nicotsx/zerobyte](https://github.com/nicotsx/zerobyte) ⭐ 5.2k | 🎯💸💎

**O que faz:** Automação de backup self-hosted com UI web moderna. Built on Restic. Suporta NFS, SMB, WebDAV, SFTP, local. Criptografia E2E, compressão, retention policies, scheduling visual. Docker deploy.

**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Self-hosters precisam de backup confiável. Restic é poderoso mas CLI-only. Synology/QNAP cobram por hardware proprietário
- 💸 **Grátis** vs Veeam ($400+/ano), Acronis ($50+/ano), ou NAS proprietário
- 💎 **UI moderna sobre Restic** — scheduling visual, monitoring, multi-protocolo num clique

**TAM:** $10B+ (backup & recovery market)

**Modelo de negócio:**
- Managed cloud: hosted Zerobyte com storage incluso
- Enterprise: multi-node management, compliance reports, alerting
- Premium features: dedup analytics, disaster recovery testing

**Esforço:** Baixo-Médio — já funcional (v0.25), precisa maturar (v0.x)

**Combinações:**
- + Coolify/Dokploy: self-hosted PaaS + backup = stack completa
- + Mole (#164): cleanup + backup = lifecycle management de dados
