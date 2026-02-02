# 🔥 SaaS Killers Self-Hosted — Open-Source Replacements for Expensive SaaS

## Notifuse/notifuse ⭐1.7k
**Link:** https://github.com/Notifuse/notifuse
**Problema:** Email marketing platforms (Mailchimp, Brevo, Klaviyo) cobram por volume de envio — $100-500+/mês para listas médias. PMEs pagam caro por features que deveriam ser commodity.
**Eixos:** 🎯💸💎🚀

### Por que é 5-10x melhor
- **💸 Custo:** Zero custo de plataforma — usa seus próprios providers (SES = $0.10/1000 emails vs Mailchimp $230/10k contacts)
- **💎 Qualidade:** Drag-drop MJML builder com preview real, A/B testing, analytics completo, notification center embeddable
- **🚀 Escala:** Multi-tenant (agências podem rodar para múltiplos clientes), multi-provider (failover automático)
- **Diferencial vs Listmonk:** Listmonk é funcional mas dated. Notifuse tem UX moderna (React+Ant Design), multi-provider routing, S3 file manager, Liquid templating

### TAM
Email marketing: $12B (2024) → $20B (2028). Self-hosted segment cresce 30%+ YoY.

### Modelo de Negócio
- **Freemium self-hosted** → Enterprise features (SSO, audit logs, dedicated support)
- **Managed hosting** → $29-99/mês (vs Mailchimp $100-500)
- **Agency white-label** → $199/mês per-tenant

### Esforço: Médio
Go+React, clean architecture. Precisa polish na UX e docs. Multi-provider já funciona.

---

## kyantech/Palmr ⭐2.3k
**Link:** https://github.com/kyantech/Palmr
**Problema:** WeTransfer, SendGB cobram $12-23/mês para features básicas. Empresas não querem dados em servidores terceiros. LGPD/GDPR pressionam por data sovereignty.
**Eixos:** 🎯💸🚀

### Por que é 5-10x melhor
- **💸 Custo:** Grátis, sem limites artificiais de upload/download
- **🚀 Escala:** SQLite (simples) ou S3-compatible (enterprise). Self-hosted = controle total
- **Diferencial:** Password protection, custom links, folder organization, dashboard analytics

### TAM
File sharing market: $7B (2024). Enterprise file transfer: $3B.

### Modelo de Negócio
- **Self-hosted grátis** → Managed cloud com SLA ($15-49/mês)
- **Enterprise:** Branding customizado, SSO, audit trail ($99/mês)

### Esforço: Baixo
NextJS+Fastify, SQLite. Stack simples, bem estruturado. Beta mas funcional.

---

## raghavyuva/nixopus ⭐1.3k
**Link:** https://github.com/raghavyuva/nixopus
**Problema:** Vercel ($20+/mês per-seat), Heroku ($25+/app), Netlify ($19+/mês) ficam caros rápido. Devs individuais e startups querem deploy simples sem vendor lock-in.
**Eixos:** 🎯💸💎🚀

### Por que é 5-10x melhor
- **💸 Custo:** VPS $5-20/mês vs Vercel/Heroku $50-500/mês para mesmo workload
- **💎 Qualidade:** Built-in terminal, file manager, monitoring, auto SSL — all-in-one vs cobbled tools
- **🚀 Escala:** GitHub push → auto deploy. Caddy proxy routing. Smart alerts multi-channel
- **vs Coolify/Dokploy:** Mais opinionated e simples. Foco em "it just works" vs flexibility

### TAM
PaaS market: $15B (2024). Self-hosted PaaS: crescimento explosivo (Coolify 35k⭐ prova demanda).

### Modelo de Negócio
- **Open-source core** → Pro features (team management, multi-server, backup)
- **Managed hosting** → Click-to-deploy em cloud ($29-99/mês)

### Esforço: Médio-Alto
Alpha stage. Promissor mas precisa maturar. Go+React.

---

## amicalhq/amical ⭐704
**Link:** https://github.com/amicalhq/amical
**Problema:** Dictation tools (Dragon $15/mês, Otter $17/mês) são cloud-only, caros, e não respeitam privacidade. Profissionais (médicos, advogados, jornalistas) precisam de STT local.
**Eixos:** 🎯💸💎⚡

### Por que é 5-10x melhor
- **💸 Custo:** Grátis, offline, sem subscription
- **💎 Qualidade:** Context-aware — detecta app ativo e formata output adequadamente (email vs chat vs IDE)
- **⚡ Velocidade:** Whisper local = rápido, sem latência de rede
- **Diferencial matador:** Context-awareness é o killer feature. Nenhum concorrente faz isso.

### TAM
Speech-to-text market: $5B (2024) → $12B (2028). Professional dictation: $2B.

### Modelo de Negócio
- **Free core** → Pro (custom vocabularies, team sync, advanced formatting) $9.99/mês
- **Enterprise:** On-prem deployment, custom models, compliance certifications

### Esforço: Médio
Electron+Next.js. macOS first, cross-platform planned. MCP integration no roadmap (huge for agent ecosystem).

---

## 1Panel-dev/CordysCRM ⭐1.7k
**Link:** https://github.com/1Panel-dev/CordysCRM
**Problema:** Salesforce ($25-300/user/mês) é caro e complexo. SMEs na China (e global) querem CRM completo sem custo predatório. Twenty.com existe mas é early-stage.
**Eixos:** 🎯💸🚀💎

### Por que é 5-10x melhor
- **💸 Custo:** Grátis vs Salesforce $25-300/user/mês. Para 50 users = economia de $15K-180K/ano
- **🚀 Escala:** L2C completo (Lead→Opportunity→Contract→Payment), não é CRM parcial
- **💎 Qualidade:** MCP Server integrado, BI (DataEase), AI agents (MaxKB), integração WeChat/DingTalk/Feishu
- **Credibilidade:** FIT2CLOUD (criadores do 1Panel, 25k⭐) substituiu seu próprio Salesforce por CordysCRM

### TAM
CRM market: $80B (2024). Self-hosted CRM: segmento em explosão (~$5B e crescendo).

### Modelo de Negócio
- **Open-source grátis** → Enterprise (SLA, custom integrations, training)
- **Managed cloud** → $29-99/user/mês (still 50-70% cheaper than Salesforce)
- **China-first** com expansão global (enorme vantagem: WeChat/DingTalk ecosystems)

### Esforço: Baixo-Médio
Docker one-click. Production-proven (FIT2CLOUD usa internamente). Java/Vue.

---

## eclaire-labs/eclaire ⭐766
**Link:** https://github.com/eclaire-labs/eclaire
**Problema:** Dados pessoais fragmentados entre 10+ apps (notas, tarefas, fotos, bookmarks, docs). Apple Intelligence/Google AI indexam mas são closed ecosystem. Privacy-conscious users querem AI sobre seus dados SEM enviar para cloud.
**Eixos:** 🎯💸💎🚀

### Por que é 5-10x melhor
- **💸 Custo:** Grátis, self-hosted, local models (Ollama)
- **💎 Qualidade:** Unifica 5 tipos de dados num só lugar com AI (OCR, classification, semantic search)
- **🚀 Escala:** De "app por tipo de dado" para "1 app que entende tudo"
- **Visão:** É o "Apple Intelligence, mas open-source e self-hosted"

### TAM
Personal knowledge management: $2B. Personal AI assistants: $15B (2028).

### Modelo de Negócio
- **Self-hosted grátis** → Cloud sync ($5-15/mês)
- **Pro features:** Advanced AI models, priority support, mobile apps
- **Family/Team plan:** Shared knowledge base ($29/mês)

### Esforço: Médio-Alto
Pre-release. Vite+TanStack Router frontend, Python backend. SQLite+Postgres. Needs maturation.

---

### [HoshinoSuzumi/chronoframe](https://github.com/HoshinoSuzumi/chronoframe) ⭐ 1.6k | 🎯💸💎

**O que é:** Gallery de fotos pessoal self-hosted. Suporta Live/Motion Photos, EXIF parsing, geocoding reverso, explore map. Nuxt 4 + Drizzle ORM + S3.

**Problema real:** Google Photos cobra storage, Apple Photos é Apple-only, Immich é pesado/complexo para quem quer algo leve. Fotógrafos e famílias querem gallery bonita sem vendor lock-in.

**Eixos de inovação:**
- 🎯 **Problema real:** Google Photos storage limits ($2.99-9.99/mês) + privacy concerns
- 💸 **Custo:** Self-hosted + S3 barato = fração do custo de Google/iCloud
- 💎 **Qualidade:** UI moderna (Nuxt 4), Live/Motion Photos nativos, explore map com geocoding

**TAM:** Cloud photo storage = $4.5B by 2028. Self-hosted segment growing 25%+ CAGR.

**Modelo de negócio:**
- Cloud hosted: managed chronoframe = $5-15/mês (competes com Google Photos)
- Enterprise/family: multi-user, shared albums, advanced storage
- Photography: portfolio features, client galleries

**Esforço para produtizar:** Médio — Docker ready, precisa polimento UX e mobile app

---

### [KittenML/KittenTTS](https://github.com/KittenML/KittenTTS) ⭐ 9.6k | ⚡💸💎🚀

**O que é:** TTS state-of-art em menos de 25MB. Ultra-compacto, roda em edge/mobile, qualidade competitiva com modelos 10-100x maiores.

**Problema real:** TTS models (ElevenLabs, Azure, Google) são caros ($0.015-0.030/1k chars) e requerem cloud. Edge devices (IoT, mobile, embedded) precisam de TTS que rode localmente sem GPU.

**Eixos de inovação:**
- ⚡ **Velocidade:** Edge inference sem GPU, latência sub-100ms
- 💸 **Custo:** <25MB model = roda em qualquer device, $0 ongoing cost vs cloud TTS
- 💎 **Qualidade:** SoTA em seu weight class, competitivo com modelos 100x maiores
- 🚀 **Escala:** Habilita TTS em devices que antes não podiam (IoT, wearables, low-end phones)

**TAM:** TTS market = $5.4B by 2030. Edge AI = $14B. Intersection = $2-4B.

**Modelo de negócio:**
- SDK licensing: embed em produtos hardware/software
- Enterprise: custom voices, fine-tuning, support
- API: para quem quer hosted mas barato

**Esforço para produtizar:** Médio — model pronto, precisa SDKs por plataforma (iOS, Android, WASM)

**Combinações:**
- + Dia/Chatterbox → pipeline TTS: KittenTTS para edge, Dia/Chatterbox para cloud quality
- + Open-AutoGLM → phone agent com voz local
- + Amical → dictation+TTS bidirectional em offline

