# 🏢 Infraestrutura Essencial para SMBs

> Ferramentas de infra que todo negócio precisa mas paga caro demais: monitoring, segurança, email, SSL, CRM.

---

## 1. henrygd/beszel ⭐ 19.1k

**O que é:** Server monitoring ultra-leve com Docker stats, dados históricos e alertas. Hub (PocketBase) + Agent (3MB).

**Problema real:** Datadog custa $15-23/host/mês. Grafana+Prometheus é complexo demais para PMEs. Beszel é "install and forget" em 2 minutos.

**Eixos de inovação:**
- 🎯 **Problema real:** 90% das PMEs não monitoram servidores por custo/complexidade
- 💸 **Custo:** $0 vs $15-23/host/mês (Datadog) = literalmente infinito x mais barato
- 💎 **Qualidade:** UI limpa, OAuth/OIDC, multi-user, backup automático S3 — features enterprise em pacote indie

**TAM:** Mercado de monitoring infra ~$7B (2025). Segmento SMB+homelab é ~30% = ~$2B.

**Modelo de negócio:**
- Managed cloud (hosted hub) para quem não quer self-host
- Enterprise tier: SAML, audit logs, custom dashboards
- Marketplace de integrações/alertas

**Esforço:** Baixo — já é polished, precisa de managed offering

**Combinações:** Beszel + Pulse (Proxmox) + AllinSSL = **stack de ops completa para SMBs**

---

## 2. octelium/octelium ⭐ 3.1k

**O que é:** Plataforma zero trust unificada: VPN moderna + ZTNA + API gateway + AI/MCP gateway + PaaS — tudo self-hosted sobre Kubernetes.

**Problema real:** Cloudflare Access/Tailscale Teams/Twingate cobram $5-10/user/mês. Para 50 usuários = $500/mês. Octelium é grátis e faz MAIS (API gateway, PaaS, SSH passwordless).

**Eixos de inovação:**
- 🎯 **Problema real:** PMEs precisam de acesso remoto seguro pós-COVID, mas não podem pagar enterprise ZTNA
- 💸 **Custo:** $0 vs $5-10/user/mês (Cloudflare/Twingate) + $0 vs $300-1000/mês (Kong/Apigee API gateway)
- 🚀 **Escala:** De homelab a enterprise — mesmo primitivo escala via K8s
- 💎 **Qualidade:** Secretless access, policy-as-code (CEL+OPA), WireGuard/QUIC, MCP gateway nativo

**TAM:** Mercado ZTNA ~$15B (2025). API Gateway ~$6B. Combinado = ~$21B.

**Modelo de negócio:**
- Enterprise support + SLA
- Managed control plane (como Tailscale model)
- Compliance modules (SOC2, HIPAA, LGPD)

**Esforço:** Médio-Alto — requer K8s, mas docs são excelentes e tem Codespace demo

**Combinações:** Octelium + Beszel (monitoring) + AllinSSL (certs) = **infra enterprise completa self-hosted**

---

## 3. rcourtman/Pulse ⭐ 4.0k

**O que é:** Dashboard unificado para Proxmox VE/PBS/PMG + Docker + Kubernetes com AI chat assistant e patrol automatizado.

**Problema real:** MSPs e homelabs gerenciam múltiplas plataformas em dashboards separados. Pulse é "single pane of glass" com AI que responde perguntas sobre sua infra.

**Eixos de inovação:**
- 🎯 **Problema real:** MSPs com 10-50 clientes gastam horas alternando entre dashboards
- 💎 **Qualidade:** AI Patrol (health checks automáticos), chat natural language, unified metrics — nada no mercado faz isso para Proxmox
- 🚀 **Escala:** De 1 homelab a MSP com centenas de nodes

**TAM:** Proxmox tem ~500k instalações ativas. MSP monitoring = ~$3B. Nicho Proxmox-first = ~$200M.

**Modelo de negócio:**
- **Pulse Pro** (já existe) — features premium
- MSP tier com multi-tenant e white-label
- Per-node pricing para scale

**Esforço:** Baixo — já tem modelo Pro, produto polished

**Combinações:** Pulse (monitoring) + Beszel (server-level) + Octelium (acesso) = **MSP-in-a-box**

---

## 4. maillab/cloud-mail ⭐ 4.2k

**O que é:** Serviço de email completo rodando em Cloudflare Workers — custo quase zero, domínio customizado, RBAC, envio via Resend, storage R2.

**Problema real:** Google Workspace = $6-18/user/mês. FastMail = $5/user/mês. Para uma startup com 10 pessoas = $60-180/mês. Cloud-Mail = custo de Cloudflare Workers (~$5/mês total para uso moderado).

**Eixos de inovação:**
- 🎯 **Problema real:** Email profissional é caro e vendor-locked
- 💸 **Custo:** ~$5/mês (Cloudflare Workers) vs $60-180/mês (Google Workspace para 10 users) = **12-36x mais barato**
- 🚀 **Escala:** Cloudflare edge = disponibilidade global, sem servidor para manter

**TAM:** Business email market ~$30B. Segmento SMB = ~$10B.

**Modelo de negócio:**
- Managed hosting com domínio setup ($3-5/user/mês, ainda mais barato que Google)
- White-label para agencies/MSPs
- Premium features (calendar, contacts sync)

**Esforço:** Médio — funcional mas precisa de calendar/contacts para competir com Google

**Combinações:** Cloud-Mail + BillionMail (marketing email) = **email stack completo zero-cost**

---

## 5. allinssl/allinssl ⭐ 3.3k

**O que é:** Gestão completa do ciclo de vida SSL — aplicação automática, renovação, deploy multi-plataforma (CDN, WAF, cloud panels), monitoramento de expiração.

**Problema real:** Certificados SSL expiram e derrubam sites. Empresas com 50+ domínios gastam horas gerenciando certs manualmente. Ferramentas pagas como DigiCert CertCentral custam $1000+/ano.

**Eixos de inovação:**
- 🎯 **Problema real:** SSL expirado é causa #1 de downtime evitável — afeta milhões de sites
- ⚡ **Velocidade:** Auto-apply + auto-renew + auto-deploy = zero intervenção humana
- 💸 **Custo:** $0 vs $1000+/ano (DigiCert CertCentral) ou $500+/ano (Keyfactor)

**TAM:** Certificate lifecycle management ~$2B (2025). Cresce 15%/ano com regulações.

**Modelo de negócio:**
- Enterprise: multi-org, audit trail, compliance reports
- MSP tier: gerenciar certs de múltiplos clientes
- API/Integration marketplace

**Esforço:** Baixo-Médio — produto funcional, precisa de internacionalização

**Combinações:** AllinSSL + Octelium (zero trust) + Beszel (monitoring) = **security ops stack self-hosted**

---

## 6. Relaticle/relaticle ⭐ 1.1k (Bônus)

**O que é:** CRM next-gen open-source em Laravel 12 + Filament 4 + PHP 8.4. Custom fields no-code, multi-tenant, pipelines visuais.

**Problema real:** HubSpot começa grátis mas escala para $45-3600/mês. Salesforce = $25-300/user/mês. SuiteCRM é poderoso mas UI de 2010.

**Eixos de inovação:**
- 🎯 **Problema real:** PMEs precisam de CRM mas não pagam $50+/user/mês
- 💸 **Custo:** $0 vs $25-300/user/mês (Salesforce) = ∞x mais barato
- 💎 **Qualidade:** UI moderna (Filament 4 é lindo), no-code customization, stack PHP que 80% das agencies já conhecem

**TAM:** CRM market ~$80B (2025). SMB segment ~$25B.

**Modelo de negócio:**
- Cloud hosted (like Twenty.com model)
- Enterprise: SSO, API, audit logs
- Marketplace de plugins/integrações

**Esforço:** Médio — early stage (1.1k stars) mas fundação técnica sólida
