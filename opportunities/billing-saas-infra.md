# 💳 Billing & SaaS Infrastructure

## useautumn/autumn ⭐ 2.3k
**Link:** https://github.com/useautumn/autumn
**YC-backed** | TypeScript | Self-hostable

### Problema Real
Billing em SaaS é deceptivamente complexo. Não é só pagamentos — é metering, limites de uso, upgrades/downgrades, cancelamentos, failed payments, race conditions. Devs gastam semanas construindo isso internamente ou pagam $$$$ por soluções como Stripe Billing ($0.5-0.8% per transaction), Chargebee ($249-549/mês), ou Lago.

### O que faz
Camada open-source entre Stripe e seu app. 3 funções: `attach()` (checkout/upgrade), `check()` (acesso/uso), `report()` (metering). Suporta subscriptions, credits, usage-based, seat-based, pay upfront. Dashboard visual para criar pricing models.

### Eixos de Inovação
- 🎯 **Problema real:** Todo SaaS precisa de billing. É o #1 pain point depois de auth.
- 💸 **5-10x menor custo:** Self-hosted = $0 vs Chargebee $249-549/mês ou Stripe Billing fees
- ⚡ **5-10x mais rápido:** 3 funções vs semanas de integração webhook
- 🚀 **5-10x mais escala:** Iterate pricing sem redeploy, sem DB migrations

### TAM
~$15B (billing/subscription management market). Todo SaaS startup é cliente potencial.

### Modelo de Negócio
Cloud hosted (freemium) + Enterprise self-hosted. Classic open-core.

### Esforço para Produtizar
**Baixo** — já tem cloud offering funcional e self-hosted documentado.

---

## flowglad/flowglad ⭐ 1.7k
**Link:** https://github.com/flowglad/flowglad
**YC-backed** | TypeScript | Full-stack SDK

### Problema Real
O mesmo billing pain, mas com abordagem diferente: **zero webhooks, stateless**. Flowglad é a single source of truth — seu app não precisa de tabela "subscriptions", não precisa mapear price IDs, não precisa consumer_id columns.

### O que faz
Full-stack SDK (React `useBilling()` hook + Node `getBilling()`) que integra em <1 minuto. Usa IDs do seu próprio auth system. Dashboard para rodar pricing models em testmode e push para prod em um clique.

### Eixos de Inovação
- 🎯 **Problema real:** Webhooks são a parte mais frágil de qualquer billing stack
- 💸 **5-10x menor custo:** Open-source core vs soluções proprietárias
- ⚡ **5-10x mais rápido:** Setup <1 minuto vs dias/semanas de integração Stripe

### TAM
Mesmo mercado que Autumn (~$15B), mas posicionamento mais dev-first.

### Modelo de Negócio
Cloud hosted + Enterprise. SDK approach permite monetizar via managed service.

### Combinação Interessante
**Autumn + Flowglad** são competitors, mas representam o nascimento de um novo segmento: **"billing middleware" open-source**. Quem integrar billing + usage analytics + pricing experiments vence.

---

## Análise Comparativa: Autumn vs Flowglad

| Aspecto | Autumn | Flowglad |
|---------|--------|----------|
| Abordagem | Dashboard-first, API second | SDK-first, developer-centric |
| Webhooks | Elimina necessidade | Zero webhooks (stateless) |
| Setup | Self-hosted via Docker | Full-stack SDK install |
| Pricing models | Visual dashboard | Testmode → prod em 1 click |
| SDK | REST API | React hooks + Node client |
| YC | ✅ | ✅ |

**Veredicto:** Ambos validam que billing middleware open-source é uma categoria emergente. Flowglad tem DX superior; Autumn tem flexibilidade maior de pricing models.
