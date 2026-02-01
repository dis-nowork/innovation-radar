# ☁️ Infra/Cloud

Infraestrutura simplificada — PaaS self-hosted, monitoring, status pages.

| # | Repo | Stars | Encontrado |
|---|------|-------|------------|
| 14 | [coollabsio/coolify](https://github.com/coollabsio/coolify) | 50.1k | 2026-02-01 |
| 15 | [dokploy/dokploy](https://github.com/dokploy/dokploy) | 29.7k | 2026-02-01 |
| 16 | [openstatusHQ/openstatus](https://github.com/openstatusHQ/openstatus) | 8.3k | 2026-02-01 |

---

## 14. coollabsio/coolify ⭐ 50.1k

**Problema:** Deploy de apps no próprio servidor é complexo (Docker, Nginx, SSL, CI/CD). Vercel/Netlify são simples mas caros e vendor-locked. Coolify é a PaaS self-hosted que dá a experiência Vercel/Heroku no seu próprio hardware — deploy com 1-click de apps, databases, e 280+ serviços. SSH connection basta

**Ideia de Produto:** **Self-Hosted PaaS SaaS**: plataforma managed de deployment que compete com Vercel/Heroku/Netlify mas roda na infra do cliente. Já tem cloud pago (app.coolify.io). Monetiza via cloud hosting managed, tiers enterprise (HA, suporte prioritário), marketplace de templates. Self-hosted grátis = funil PLG massivo. Upsell: multi-server management, backups, monitoring avançado, team seats

**Potencial:** 🔥🔥🔥🔥🔥 TAM: PaaS/Cloud Platform $150B+ (Heroku vendido por $0, mas Vercel vale $3.5B+, Netlify $2B+). Apache-2.0. 50.1k stars, 3.5k forks. Criado Jan/2021. Stack: PHP/Laravel + Svelte. Push ativo (última em Jan/2026). O crescimento de 50k stars prova demanda brutal. O timing é perfeito: Heroku matou free tier, devs buscam alternativas. Coolify captura exatamente o "quero Vercel DX mas no meu VPS de $5/mês". Receita já validada com cloud tier

---

## 15. dokploy/dokploy ⭐ 29.7k

**Problema:** Mesmo problema que Coolify mas com abordagem mais moderna e crescimento mais explosivo. Dokploy é PaaS open-source com Docker Compose nativo, multi-node via Docker Swarm, backups automatizados, monitoring real-time, e CLI/API completa. Traefik integrado para routing/load balancing

**Ideia de Produto:** **Cloud Deployment Platform**: PaaS managed que compete diretamente com Coolify mas com stack moderna (TypeScript full). Já tem cloud (app.dokploy.com). Monetiza via cloud tiers, enterprise features (multi-server, SSO, audit logs), suporte premium. Templates marketplace (Plausible, Pocketbase, Cal.com com 1-click)

**Potencial:** 🔥🔥🔥🔥🔥 TAM: PaaS $150B+. Licença custom (source-available). 29.7k stars, 2k forks. Criado **Apr/2024** → 29.7k stars em apenas 21 meses = crescimento mais rápido que Coolify! TypeScript full-stack = melhor DX para contributors. Features diferenciadas: Docker Compose nativo, Docker Swarm multi-node, CLI, monitoring granular por recurso. Sponsors incluem Hostinger (validação de hosting company). O mercado PaaS self-hosted é winner-takes-most e Dokploy está ganhando momentum rápido

---

## 16. openstatusHQ/openstatus ⭐ 8.3k

**Problema:** Status pages e uptime monitoring são caros (Pingdom $15+/mês, Statuspage.io $29+/mês, BetterUptime $20+/mês) e fragmentados. OpenStatus unifica synthetic monitoring global + status pages bonitas + API monitoring num produto open-source moderno. "Monitoring as code"

**Ideia de Produto:** **Synthetic Monitoring + Status Page SaaS**: plataforma que substitui Pingdom + Statuspage.io + UptimeRobot num produto unificado. Monitora globalmente, alerta em tempo real, gera status pages públicas profissionais. Monetiza via cloud (free tier → pro → enterprise), volume de checks, regiões premium, incident management. Enterprise: SSO, SLA reports, custom domains

**Potencial:** 🔥🔥🔥🔥 TAM: Application Performance Monitoring $8B+ (Status Page $2B+, Synthetic Monitoring $3B+). AGPL-3.0. 8.3k stars, 566 forks. Criado Jun/2023. Stack moderna (Next.js, Turso, Tinybird, shadcn/ui). HN front-page + ProductHunt top post = validação da comunidade. Já tem enterprise plan e cal.com booking. O diferencial é "monitoring as code" — config versionável, GitOps-friendly. Todo SaaS precisa de status page + monitoring. Mercado fragmentado e overpriced — oportunidade clara de disrupção open-source
