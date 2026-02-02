# 🏠 Self-Hosted Digital Sovereignty & Professional Tools

> Ferramentas que devolvem controle total aos indivíduos e PMEs, substituindo SaaS caros.

---

## kurrier-org/kurrier ⭐ 821
**Link:** https://github.com/kurrier-org/kurrier
**Linguagem:** TypeScript | **Licença:** Custom
**Criado:** 2025-09

### Problema Real
Indivíduos e PMEs pagam $6-18/user/mês por Google Workspace ou Microsoft 365 só para ter email+calendário+contatos+storage unificados. Alternativas self-hosted existem (Roundcube, Nextcloud), mas são fragmentadas — cada serviço é uma app separada com UX de 2010.

### O que faz
Workspace self-hosted unificado: email (IMAP/SMTP/SES/SendGrid/Mailgun/Postmark), calendários (CalDAV), contatos (CardDAV), e storage (WebDAV/S3) numa única UI moderna. Sync cross-device nativo (iOS, Android, Thunderbird, macOS).

### Eixos de Inovação: 🎯💸💎
- 🎯 **Problema real:** 3B+ pessoas usam email. PMEs pagam $72-216/user/ano por suites de produtividade
- 💸 **5-10x menor custo:** $0 vs $72-216/user/ano. Para empresa de 50 pessoas = economia de $3.6k-10.8k/ano
- 💎 **Qualidade superior:** UI moderna e unificada vs fragmentação de Roundcube+Radicale+Nextcloud separados

### TAM
- Email hosting market: ~$10B/ano
- Productivity suites: ~$50B/ano
- Self-hosted segment growing 25%+ YoY

### Modelo de Negócio
- **Open-core:** Community free, Enterprise (SSO, multi-tenant, audit logs, SLA)
- **Managed hosting:** Kurrier Cloud com pricing per-user competitivo ($2-5/user/mês)
- **White-label:** ISPs e hosters revendem como webmail premium

### Esforço para Produtizar: Médio
- Core funciona. Precisa: mobile apps nativas, search full-text, encryption E2E, multi-tenant
- Competição: Roundcube (feio), Mailcow (complexo), Zimbra (pesado), Stalwart (backend only)

### Combinações
- + BillionMail (#87): Kurrier como UI + BillionMail como MTA = Google Workspace killer completo
- + Pocket-ID (#220): Auth passwordless para o workspace
- + nicotsx/zerobyte (#170): Backup integrado do workspace

---

## tursodatabase/agentfs ⭐ 2,159
**Link:** https://github.com/tursodatabase/agentfs
**Linguagem:** Rust | **Licença:** Custom
**Criado:** 2025-10

### Problema Real
AI agents precisam de persistência de estado, mas hoje usam arquivos soltos, vector DBs complexos, ou soluções ad-hoc. Não existe um "filesystem" pensado para agents — auditável, reproduzível, portátil.

### O que faz
Filesystem baseado em SQLite projetado especificamente para AI agents. Cada operação (file ops, tool calls, state changes) é registrada. Estado inteiro do agent em um único arquivo .db que pode ser copiado, versionado, e restaurado. SDKs em TypeScript, Python, e Rust. CLI com FUSE mount.

### Eixos de Inovação: 🎯💎⚡
- 🎯 **Problema real:** Todo agent builder improvisa persistência. Claude Code usa CLAUDE.md, Codex usa workspace files — tudo ad-hoc
- 💎 **5-10x qualidade:** Auditabilidade SQL completa, snapshot instantâneo, timeline de ações, reprodutibilidade exata
- ⚡ **Velocidade:** SQLite = sub-ms reads, single file = zero infra setup

### TAM
- AI agent infrastructure: projetado em $15-25B até 2028
- Todo agent framework (LangChain, CrewAI, AutoGen, OpenClaw) precisa de storage layer
- By Turso team = credibilidade + distribuição existente

### Modelo de Negócio
- **Open-source SDK** + **Turso Cloud** (managed hosting de AgentFS databases)
- **Enterprise:** Multi-agent sync, access control, compliance logging
- **Platform play:** Se vira padrão, todo agent paga por hosting

### Esforço para Produtizar: Baixo-Médio
- Alpha stage mas funcional. Turso tem infra de produção existente
- Precisa: integrações com frameworks (LangChain, CrewAI), encryption, multi-agent sync

### Combinações
- + memvid (#123): AgentFS como storage layer + memvid como memory retrieval
- + Memori (#191): Knowledge graph on top of AgentFS
- + SimpleMem (#371): Cognitive memory com AgentFS como backend

---

## TNT-Likely/BeeCount ⭐ 1,068
**Link:** https://github.com/TNT-Likely/BeeCount
**Linguagem:** Dart (Flutter) | **Licença:** Other
**Criado:** 2025

### Problema Real
Apps de finanças pessoais (YNAB $99/ano, MoneyLion, Mint) armazenam dados financeiros sensíveis em servidores terceiros, cobram subscriptions, e bombardeiam com anúncios/recomendações de produtos financeiros. Privacidade zero.

### O que faz
App de finanças pessoais open-source com sync self-hosted. Features: OCR de recibos, reconhecimento por foto, entrada por voz, categorização automática, gráficos de análise, import/export. Sync via iCloud (iOS), Supabase, WebDAV, ou S3 (Cloudflare R2/AWS/MinIO). iOS + Android + HarmonyOS.

### Eixos de Inovação: 🎯💸💎
- 🎯 **Problema real:** 2B+ pessoas precisam controlar gastos. Privacy de dados financeiros é crítica
- 💸 **5-10x menor custo:** $0 vs $99/ano (YNAB) ou $48-120/ano (apps premium). AI features grátis vs upsell
- 💎 **Qualidade superior:** AI-powered (OCR, voz, screenshot auto) + 4 opções de sync + offline-first + open-source auditável

### TAM
- Personal finance apps market: ~$1.5B/ano (crescendo 12% YoY)
- 2B+ smartphone users que precisam de controle financeiro
- Mercado chinês + global = enorme

### Modelo de Negócio
- **App gratuita** + **Sync premium** (Supabase managed, $2-5/mês)
- **Enterprise/Family:** Multi-user com dashboards consolidados
- **White-label:** Bancos/fintechs integram como feature

### Esforço para Produtizar: Baixo
- Já tem apps publicadas (App Store + Google Play). Core maduro
- Precisa: mais idiomas, integrações bancárias (Plaid/Open Banking), AI insights mais profundos

### Combinações
- + TaxHacker (#103): BeeCount para tracking + TaxHacker para contabilidade fiscal
- + bigcapital (#139): Finanças pessoais (BeeCount) + business accounting (bigcapital)

---

## Lissy93/networking-toolbox ⭐ 2,273
**Link:** https://github.com/Lissy93/networking-toolbox
**Linguagem:** Svelte | **Licença:** MIT
**Criado:** 2025

### Problema Real
Sysadmins e network engineers usam dezenas de ferramentas online separadas (DNS lookup, WHOIS, port scan, SSL check, IP geo, subnet calc, etc.) — muitas com ads, tracking, ou limitações. Offline não funciona.

### O que faz
100+ ferramentas de networking numa única webapp offline-first. DNS, WHOIS, port scanning, subnet calc, SSL inspection, IP geolocation, header analysis, traceroute, bandwidth test, MAC lookup, encoding tools, e muito mais. Docker deploy, Vercel, GitHub Pages, ou local.

### Eixos de Inovação: 🎯💸💎
- 🎯 **Problema real:** 10M+ sysadmins/devops usam ferramentas de rede diariamente. Ferramentas fragmentadas e online-only
- 💸 **5-10x menor custo:** $0 vs subscriptions de ferramentas premium (SolarWinds $1,500+, PingPlotter $50/ano, etc.)
- 💎 **5-10x qualidade:** 100+ tools em 1 UI, offline-first, zero tracking, by Lissy93 (15+ anos de credibilidade OSS com Dashy)

### TAM
- Network management tools: ~$15B/ano
- 10M+ target users (sysadmins, DevOps, security, MSPs)
- Self-hosted = empresas reguladas (finance, healthcare, gov)

### Modelo de Negócio
- **Open-source** base + **Pro features** (API access, team sharing, custom branding)
- **Enterprise:** On-prem deployment, SSO, audit logs, white-label para MSPs
- **Managed SaaS:** networking-toolbox.as93.net com premium tier

### Esforço para Produtizar: Baixo
- Já funciona e está deployed. By Lissy93 = qualidade comprovada
- Precisa: mobile PWA otimizada, team features, RBAC, export/reporting

### Combinações
- + portracker: networking-toolbox (diagnóstico) + portracker (monitoramento contínuo de portas)
- + scanopy (#201): Discovery automática + diagnóstico manual
- + beszel (#183): Monitoring de servers + networking tools

---

## karanhudia/borg-ui ⭐ 956
**Link:** https://github.com/karanhudia/borg-ui
**Linguagem:** Python | **Licença:** AGPL-3.0
**Criado:** 2025

### Problema Real
BorgBackup é o melhor sistema de backup deduplicado open-source, mas é 100% CLI. Sysadmins que administram backups para múltiplos servers gastam horas em comandos manuais. Não há boa UI para criar, agendar, monitorar e restaurar backups.

### O que faz
Web UI bonita e completa para BorgBackup: dashboard com métricas, criação de repositórios (local/SSH/SFTP), scheduling visual, progresso em tempo real, restore com browse de arquivos, suporte a encryption (repokey/keyfile), compressão (lz4/zstd/zlib/lzma), exclude patterns. Import de repos existentes.

### Eixos de Inovação: 🎯💎
- 🎯 **Problema real:** BorgBackup tem 12k+ stars mas UX é terminal-only. Barreia adoção por não-experts
- 💎 **5-10x qualidade:** De CLI commands complexos para point-and-click com progress bars, browse de arquivos, e scheduling visual

### TAM
- Backup software market: ~$12B/ano
- BorgBackup users: 100k+ (estimativa baseada em stars/downloads)
- Potencial: qualquer sysadmin que prefere UI a CLI para gerenciar backups

### Modelo de Negócio
- **Open-source** + **Pro features** (multi-server management, team RBAC, alertas avançados)
- **Managed service:** Borg-UI Cloud com storage integrado
- **MSP edition:** Multi-tenant backup management dashboard

### Esforço para Produtizar: Médio
- Core funciona bem. Precisa: multi-server, alerting (Slack/email/webhook), API REST, mobile notifications
- Competição: Vorta (desktop only), borgmatic (CLI automation)

### Combinações
- + databasus (#222): Borg-UI para file backups + databasus para database backups = unified backup solution
- + zerobyte (#170): Alternativa com restic engine — ou merge das melhores features de ambos

---

## 0xfurai/peekaping ⭐ 1,018
**Link:** https://github.com/0xfurai/peekaping
**Linguagem:** Go | **Licença:** MIT
**Criado:** 2025

### Problema Real
Uptime Kuma (64k+ stars) é o padrão de monitoring self-hosted, mas tem limitações: Node.js (mais pesado), não é API-first, extensibilidade limitada, status pages básicas.

### O que faz
Sistema de uptime monitoring Go-native: HTTP/TCP/DNS/ICMP monitoring, status pages públicas, alertas multi-canal, API-first architecture, suporte a PostgreSQL/MongoDB/SQLite, Terraform provider comunitário. Leve e rápido por ser Go.

### Eixos de Inovação: 🎯💎⚡
- 🎯 **Problema real:** Uptime monitoring é necessidade universal. Alternativas pagas: Better Uptime ($20-80/mês), Pingdom ($10-450/mês)
- 💎 **Qualidade:** API-first (vs Kuma que é UI-first), extensível, Terraform-ready, arquitetura moderna
- ⚡ **Performance:** Go = menor RAM, startup mais rápido, mais monitors por instância vs Node.js

### TAM
- Website monitoring: ~$3B/ano
- 200M+ websites ativos que precisam de monitoring
- Self-hosted segment: MSPs, empresas reguladas, homelabbers

### Modelo de Negócio
- **Open-source** + **Cloud managed** (peekaping.com)
- **Enterprise:** Multi-org, SSO, SLA reporting, incident management
- **API marketplace:** Integrações premium (PagerDuty, OpsGenie, custom webhooks)

### Esforço para Produtizar: Baixo-Médio
- Já tem cloud offering, docs, Terraform provider. Mais maduro que esperado para 1k stars
- Precisa: incident management workflow, integrations marketplace, mobile app

### Combinações
- + Checkmate (#322): Peekaping para uptime + Checkmate para hardware monitoring
- + openstatus (#28): Comparar abordagens — openstatus é edge-native, peekaping é Go monolith
