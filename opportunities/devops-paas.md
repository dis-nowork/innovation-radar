# 🚀 DevOps / PaaS Self-Hosted

## hunvreus/devpush ⭐ 4.4k
**Link:** https://github.com/hunvreus/devpush
**Stack:** Go backend, Docker-based runners

### Problema Real
Vercel ($20/dev/mês), Render ($25/mês+), Netlify — custos escalam rápido para times e projetos múltiplos. Desenvolvedores querem git-push-deploy sem vendor lock-in e sem custos mensais crescentes.

### Eixos de Inovação
- 🎯 **Problema real:** Custos de PaaS explodem com escala de times/projetos
- 💸 **5-10x custo:** Self-hosted em VPS barata ($5-20/mês) vs $100+/mês em PaaS
- 🚀 **5-10x escala:** Multi-language (Python, Node, PHP, Go...) vs Vercel (JS-focused)

### TAM
- PaaS market: ~$15B em 2025
- Segmento self-hosted: startups, agências, times indie

### Modelo de Negócio
- **Managed hosting:** DevPush Cloud (como Coolify Cloud faz)
- **Enterprise:** SSO, audit logs, multi-cluster
- **Marketplace:** Buildpacks e templates da comunidade

### Esforço para Produtizar: Médio
Instalador one-liner existe. Falta: UI polish, monitoring integrado, auto-scaling.

### Combinações
- **+ OpenCloud:** File management + deploy = workspace completo
- **+ zerobyte:** Deploy + backup automático

---

## Análise Comparativa: PaaS Open-Source

| Projeto | Stars | Multi-lang | Self-hosted | UI | Maturidade |
|---------|-------|-----------|-------------|-----|-----------|
| Coolify | 35k+ | ✅ | ✅ | ✅ | Alta |
| DevPush | 4.4k | ✅ | ✅ | ✅ | Média |
| Dokku | 29k+ | ✅ | ✅ | CLI | Alta |

DevPush se diferencia pelo foco em **DX moderna** (similar a Vercel) com **multi-language real**. Coolify é mais maduro mas mais complexo.
