# 📈 Marketing/Growth

Social media, email marketing, automação de marketing.

### [gitroomhq/postiz-app](https://github.com/gitroomhq/postiz-app) ⭐ 26.3k | 🎯💸🚀
**Problema:** Buffer/Hootsuite custam $15-100/mês e não têm AI real pra conteúdo.
**Solução:** Scheduling de social media com AI que gera e agenda posts.
**Por que é superior:** 💸 Grátis self-hosted. 🚀 AI content = 5x mais posts com mesmo esforço. 26k stars.

---

### [knadh/listmonk](https://github.com/knadh/listmonk) ⭐ 18.9k | 🎯💸📈
**Problema:** Mailchimp/SendGrid ficam caros com volume (>10k contatos = $100+/mês).
**Solução:** Email marketing self-hosted: 7M emails com 57MB de RAM. Go single-binary.
**Por que é superior:** 💸 Custo próximo de zero vs $100+/mês. 📈 7M emails sem degradar. 🎯 18k stars, battle-tested.

---

### [mautic/mautic](https://github.com/mautic/mautic) ⭐ 9.1k | 🎯💸🚀
**Problema:** HubSpot custa $800+/mês pra marketing automation completo.
**Solução:** Marketing automation open-source: email, landing pages, scoring, workflows.
**Por que é superior:** 💸 HubSpot a fração do custo. 🚀 Extensível com plugins. 🎯 9k stars, comunidade madura.

---

### [formbricks/formbricks](https://github.com/formbricks/formbricks) ⭐ ~9k | 🎯💸
**Problema:** Typeform cobra $25-83/mês pra pesquisas com lógica e branding.
**Solução:** Pesquisas e feedback open-source com targeting, lógica condicional, integrações.
**Por que é superior:** 💸 Grátis self-hosted vs $83/mês. 🎯 In-app surveys = feedback no momento certo.

---


---

### [usesend/useSend](https://github.com/usesend/useSend) ⭐ 3.9k | 🎯💸
**Problema:** Resend cobra $20-100+/mês. Sendgrid/Postmark similar. Email transacional é commodity mas cobrado como premium. Startups pagam caro por dashboard bonito em cima de AWS SES ($0.10/1000 emails).
**Solução:** Dashboard open-source em cima do AWS SES. Transactional + marketing emails, SMTP, REST API, webhooks, contact management, email editor visual. Next.js + Prisma + shadcn/ui.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo SaaS precisa de email transacional — é infraestrutura básica
- 💸 **Custo:** SES pricing ($0.10/1000) vs Resend ($20/mês pra 5000 emails). 10-50x mais barato em volume
**TAM:** $5B+ (email marketing + transactional email market)
**Modelo de negócio:** Managed cloud (freemium), enterprise features, add-ons (SMS, push, WhatsApp na roadmap)
**Esforço:** Médio — beta stage, precisa maturar. Stack moderna (Next.js, tRPC, Prisma)
**Combinações:** useSend + Listmonk (bulk) = email stack completo. useSend + BillionMail = sending + server próprio
