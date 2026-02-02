# 🏗️ Self-Hosted Infrastructure & Operations

> Ferramentas que substituem SaaS caros com alternativas self-hosted de qualidade enterprise.

---

## 1. henrygd/beszel ⭐ 19.1k

**Link:** https://github.com/henrygd/beszel
**Licença:** MIT | **Linguagem:** Go | **Forks:** 621

### Problema Real
Monitorar servidores requer Datadog ($15-75/host/mês), New Relic, ou montar um stack Prometheus+Grafana complexo. PMEs e homelabbers pagam caro ou ficam no escuro. O gap é enorme entre "zero monitoring" e "enterprise overkill".

### O Que Faz
Plataforma de monitoring ultralight com:
- Docker stats por container (CPU, mem, network)
- Histórico de dados com alertas configuráveis
- Multi-user com compartilhamento de sistemas
- OAuth/OIDC nativo
- Backup automático para disco ou S3
- Backend em PocketBase (single binary)

### Eixos de Inovação
- 🎯 **Problema real:** Milhões de servidores sem monitoring por custo/complexidade
- 💸 **5-10x menor custo:** $0 vs $15-75/host/mês no Datadog
- ⚡ **5-10x mais rápido:** Setup em minutos vs horas/dias de Prometheus+Grafana

### TAM
- Server monitoring market: ~$5.8B (2025)
- Self-hosted/homelab community: 2M+ (estimativa r/selfhosted + r/homelab)
- Target real: PMEs com 2-50 servidores

### Modelo de Negócio
- **Freemium:** Open-source core + enterprise features (SSO avançado, compliance, SLA alerting)
- **Managed:** Beszel Cloud com hosted hub — $5-15/host/mês (vs $15-75 Datadog)
- **Marketplace:** Plugins de integrações (PagerDuty, Slack, custom dashboards)

### Esforço para Produtizar: Baixo
Já é produto maduro com UI polida. Faltam: managed offering, enterprise auth, e white-labeling.

### Combinações
- **Beszel + Keep (AIOps, #80):** Monitoring + alert correlation inteligente = NOC automático
- **Beszel + 1Panel (#71):** Monitoring + gerenciamento de server = painel ops unificado
- **Beszel + OpenObserve (#79):** Metrics + logs 140x barato = observability stack completo

---

## 2. fosrl/pangolin ⭐ 18.5k

**Link:** https://github.com/fosrl/pangolin
**Licença:** AGPL-3.0 | **Linguagem:** TypeScript | **Forks:** 553

### Problema Real
Acesso remoto seguro a recursos internos requer combinar VPN (WireGuard/OpenVPN) + reverse proxy (Nginx/Traefik) + identity provider (Keycloak) + SSL certs (Let's Encrypt). São 4+ ferramentas que não conversam entre si. Cloudflare Tunnel resolve parte, mas é vendor lock-in e tem limites.

### O Que Faz
Plataforma unificada que combina VPN + reverse proxy + identity:
- Tunnels WireGuard sem IP público necessário
- Reverse proxy com autenticação identity-aware
- NAT traversal inteligente
- Browser-based access a web apps
- Client-based access a SSH, RDP, databases
- SSL automático, health checking, load balancing
- CrowdSec integration (WAF)

### Eixos de Inovação
- 🎯 **Problema real:** Acesso remoto seguro é fragmentado e complexo
- 💸 **5-10x menor custo:** $0 vs Cloudflare Access ($7/user/mês) ou Tailscale Teams ($6/user/mês)
- 🚀 **5-10x mais escala:** De "1 VPN config por site" para "N sites em 1 plataforma com identity management"

### TAM
- Zero Trust Network Access market: ~$2.5B (2025), crescendo 15%+ ao ano
- VPN market: ~$45B
- Target real: empresas remote-first, MSPs, homelabbers

### Modelo de Negócio
- **Community Edition:** AGPL, gratuito
- **Enterprise Edition:** License comercial, gratuito até $100k receita
- **Pangolin Cloud:** Managed service com pay-as-you-go
- **MSP/White-label:** Empresas de TI oferecem para clientes

### Esforço para Produtizar: Baixo
Produto já maduro com managed cloud (app.pangolin.net). Modelo de revenue diversificado.

### Combinações
- **Pangolin + Pocket-ID (#220):** VPN identity-aware + auth passwordless = zero-trust sem senhas
- **Pangolin + Beszel (#215):** Acesso remoto + monitoring = ops remoto completo
- **Pangolin + 1Panel (#71):** Rede segura + painel de gerenciamento = MSP-in-a-box

---

## 3. Zackriya-Solutions/meeting-minutes (Meetily) ⭐ 9.6k

**Link:** https://github.com/Zackriya-Solutions/meeting-minutes
**Licença:** MIT | **Linguagem:** Rust | **Forks:** 831

### Problema Real
Tools de meeting AI (Otter.ai $16.67/mês, Fireflies.ai $19/mês, Grain $19/mês) gravam e processam áudio em nuvem — violação de privacidade para empresas em healthcare, jurídico, finanças. $4.4M custo médio por breach (IBM 2024). €5.88B em multas GDPR.

### O Que Faz
Assistente AI de reuniões 100% local:
- Transcrição real-time com Parakeet (4x mais rápido que Whisper)
- Speaker diarization (identifica quem falou)
- Sumarização com Ollama (zero cloud)
- Suporte Mac e Windows
- Funciona offline
- Rust-based (performance nativa)

### Eixos de Inovação
- 🎯 **Problema real:** Meeting transcription viola privacidade/compliance em setores regulados
- 💸 **5-10x menor custo:** $0 vs $17-19/mês/user em Otter/Fireflies
- ⚡ **5-10x mais rápido:** Parakeet é 4x faster que Whisper, processamento local sem latência de upload

### TAM
- Meeting minutes/transcription market: ~$3.2B (2025)
- Enterprise meeting management: ~$9.5B
- Target real: empresas reguladas (health, legal, finance) + privacy-conscious

### Modelo de Negócio
- **Community:** Free forever (open-source)
- **Meetily PRO:** Templates de summary, exports PDF/DOCX, auto-detection, GDPR compliance built-in
- **Enterprise:** On-prem deployment, custom AI models, integration APIs, audit logs
- **Hardware bundle:** Pre-configured meeting devices com Meetily

### Esforço para Produtizar: Médio
Community edition forte. PRO já existe (meetily.ai). Gap: integrações com calendários, CRMs, e plataformas de videoconferência.

### Combinações
- **Meetily + Twenty CRM (#64):** Transcrição → extrai action items → cria tasks no CRM automaticamente
- **Meetily + Khoj (#77):** Reuniões alimentam o "second brain" pessoal — busca semântica em todas as conversas
- **Meetily + chatterbox (#73):** Transcrição + TTS = robô que lê resumos em voz, envia audio notes

---

## 4. Billionmail/BillionMail ⭐ 13.4k

**Link:** https://github.com/Billionmail/BillionMail
**Licença:** AGPL-3.0 | **Linguagem:** Go | **Forks:** 1,357

### Problema Real
Email marketing é absurdamente caro em escala: Mailchimp cobra $350/mês para 50k contatos, SendGrid $89.95/mês para 50k emails. Listmonk (#14, 18.9k ⭐) resolve parte, mas não inclui mail server. BillionMail é mail server + marketing platform num pacote.

### O Que Faz
Plataforma completa de email self-hosted:
- Mail server full (Postfix + Dovecot + Rspamd)
- Newsletter builder com templates
- Campaign management e segmentação
- Analytics: delivery, open rates, click-through
- Envio ilimitado
- WebMail integrado (Roundcube)
- SSL automático
- Instalação em 8 minutos

### Eixos de Inovação
- 🎯 **Problema real:** Email marketing caro demais para PMEs e criadores em escala
- 💸 **5-10x menor custo:** $0 + custo de servidor ($5-20/mês) vs $100-1000+/mês em Mailchimp/SendGrid
- 📈 **5-10x mais volume:** Envio ilimitado vs limites de plano

### TAM
- Email marketing market: ~$12.6B (2025)
- 4B+ email accounts globalmente
- Target real: PMEs, e-commerce, newsletters, criadores de conteúdo

### Modelo de Negócio
- **Self-hosted:** Gratuito, ilimitado
- **Managed cloud:** BillionMail Cloud com setup gerenciado — $29-99/mês
- **Enterprise:** Dedicated IP pools, deliverability consulting, white-label
- **Marketplace:** Templates premium, integrações

### Esforço para Produtizar: Baixo-Médio
Produto funcional e instalável. Gap: deliverability tooling avançado (IP warming, reputation management), e UI mais polida.

### Combinações
- **BillionMail + Listmonk (#14):** BillionMail como mail server + Listmonk como frontend de marketing = stack imbatível
- **BillionMail + Postiz (#8):** Email + social media scheduling = distribuição omnichannel $0
- **BillionMail + Formbricks (#25):** Feedback → segmentação → email personalizado = loop de growth grátis

---

## 5. crbnos/carbon ⭐ 1.8k

**Link:** https://github.com/crbnos/carbon
**Licença:** Custom (Fossorial) | **Linguagem:** TypeScript | **Forks:** 190

### Problema Real
Manufacturing ERPs são caros ($150-500/user/mês no SAP/Oracle), complexos, e projetados para Fortune 500. Job shops, custom manufacturers, e montadoras pequenas ficam com Excel ou ERPs antigos sem suporte. AureusERP (#69) é genérico; Carbon é especializado em manufatura.

### O Que Faz
ERP + MES + QMS para manufatura:
- Bill of Materials (BOM) management
- Work orders e production scheduling
- Quality management system integrado
- Inventory e purchasing
- API-first architecture (Remix + Supabase)
- Configure-to-order e job shop workflows
- Extensível via apps/plugins

### Eixos de Inovação
- 🎯 **Problema real:** Manufatureiros pequenos sem ERP acessível e moderno
- 💸 **5-10x menor custo:** $0 + hosting vs $150-500/user/mês SAP
- 💎 **5-10x mais qualidade:** API-first, TypeScript moderno vs interfaces legadas de 2005

### TAM
- Manufacturing ERP market: ~$12.6B (2025)
- SMB manufacturers: ~250k só nos EUA
- Target real: job shops, custom assembly, make-to-order (5-200 funcionários)

### Modelo de Negócio
- **Open-source core:** Gratuito para sempre
- **Enterprise:** Features avançados (advanced scheduling, AI demand forecasting)
- **Vertical SaaS:** Carbon Cloud para nichos (metalúrgicas, eletrônica, food manufacturing)
- **Implementation services:** Consulting + customização ($5k-50k por projeto)

### Esforço para Produtizar: Alto
Produto early-stage mas arquitetura sólida. Precisa: mais módulos, onboarding UX, e cases de sucesso.

### Combinações
- **Carbon + InvenTree (#76):** Manufacturing ERP + inventory granular = supply chain completo
- **Carbon + open-edge-platform/anomalib (#39):** ERP + AI quality inspection = zero-defect manufacturing
- **Carbon + Lago (#68):** Manufacturing + billing usage-based = model para contract manufacturers

---

## 6. pocket-id/pocket-id ⭐ 6.4k

**Link:** https://github.com/pocket-id/pocket-id
**Licença:** BSD-2 | **Linguagem:** Go | **Forks:** 196

### Problema Real
Self-hosters que querem SSO para seus serviços precisam de Keycloak (complexo, 1GB+ RAM), Authentik (pesado), ou Authelia (limitado). Pocket-ID é o OIDC provider mais simples e leve, com passkeys nativos — a autenticação do futuro.

### O Que Faz
OIDC provider minimalista com foco em passkeys:
- Autenticação por passkeys (biometria, hardware keys)
- OIDC compliant para qualquer serviço
- Interface simples e clean
- Leve em recursos (Go binary)
- Self-hosted por design

### Eixos de Inovação
- 🎯 **Problema real:** SSO para self-hosted é complexo demais (Keycloak = overkill)
- ⚡ **5-10x mais rápido:** Setup em minutos vs horas de Keycloak
- 💎 **5-10x mais qualidade:** Passkeys nativo = passwordless = mais seguro e melhor UX

### TAM
- Identity and Access Management market: ~$19.1B (2025)
- Self-hosted community: 2M+ users
- Target real: homelabbers, small dev teams, SMBs

### Modelo de Negócio
- **Open-source:** Gratuito, BSD license permissiva
- **Managed cloud:** Pocket-ID hosted — $3-10/mês para teams
- **Enterprise:** SCIM provisioning, audit logs, compliance features
- **Plugin marketplace:** Connectors para serviços específicos

### Esforço para Produtizar: Baixo-Médio
Produto funcional e focado. Gap: enterprise features (SCIM, directory sync, compliance logging).

### Combinações
- **Pocket-ID + Pangolin (#216):** Auth passwordless + VPN identity-aware = zero-trust passwordless completo
- **Pocket-ID + Beszel (#215):** SSO leve para monitoring multi-user
- **Pocket-ID + voidauth (#214):** Pocket-ID como backend + voidauth como camada de management = auth stack completo
