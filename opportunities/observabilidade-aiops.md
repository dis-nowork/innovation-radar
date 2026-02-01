# 📊 Observabilidade & AIOps

## openobserve/openobserve ⭐ 17.8k
**Link:** https://github.com/openobserve/openobserve
**Eixos:** 🎯💸⚡📈 (4 eixos!)

### Problema Real
Elasticsearch, Splunk e Datadog são caríssimos. Empresas pagam $50k-500k+/ano em observabilidade. O storage de logs é o maior custo, e cresce exponencialmente com escala.

### Por que é 5-10x melhor
- **🎯 Problema real:** Custos de observabilidade são top 3 em infra para empresas SaaS
- **💸 Custo:** 140x menor custo de storage vs Elasticsearch (Parquet + S3). Literalmente 140x — não 2x, não 10x
- **⚡ Velocidade:** Setup em 2 minutos. Single binary. Queries mais rápidas com 1/4 do hardware
- **📈 Volume:** Escala de terabytes (single node) a petabytes (HA mode)

### TAM
- Observability market: $40B+ (2025), crescendo 15%+ ao ano
- Datadog sozinho fatura $2.7B/ano
- Público: Toda empresa com software em produção

### Modelo de Negócio
- **Open core:** Community edition grátis → Cloud managed com premium features
- **Enterprise:** SSO, RBAC, SLA, compliance = $$$
- **Managed cloud:** Pay-per-ingestion (como Datadog mas 10-50x mais barato)

### Esforço para Produtizar: Baixo
Já tem cloud offering. Produto muito maduro. Escrito em Rust = performance real.

### Combinações
- + Keep (AIOps) = stack completa de observabilidade + incident management
- + SigNoz (complementar em APM)
- + 1Panel (deploy fácil do OpenObserve)

---

## keephq/keep ⭐ 11.3k
**Link:** https://github.com/keephq/keep
**Eixos:** 🎯💸🚀

### Problema Real
Equipes de DevOps/SRE recebem alertas de 10+ ferramentas diferentes (Datadog, PagerDuty, CloudWatch, Grafana...). Alert fatigue é real — 70% dos alertas são duplicados ou irrelevantes. PagerDuty cobra $21-41/user/mês.

### Por que é 5-10x melhor
- **🎯 Problema real:** Alert fatigue causa downtime real. Engenheiros ignoram alertas importantes por excesso de ruído
- **💸 Custo:** Self-hosted grátis vs PagerDuty ($500+/mês para equipes médias)
- **🚀 Escala:** Integra com 80+ tools de monitoring. AI-powered correlation reduz ruído automaticamente

### TAM
- Incident management: $5B+ (2025)
- AIOps: $15B+
- Público: Toda equipe de engineering/DevOps/SRE

### Modelo de Negócio
- **Open core:** Self-hosted grátis → Cloud com features enterprise
- **Enterprise:** SSO, audit logs, SLA guarantees
- **Marketplace:** Integrações premium com ferramentas enterprise

### Esforço para Produtizar: Baixo-Médio
Já tem cloud platform. Precisa crescer base de integrações enterprise.

### Combinações
- + OpenObserve = stack observability + AIOps completa (Datadog killer end-to-end)
- + Automatisch/n8n para workflows de remediação automática

---

## SigNoz/signoz ⭐ 25.5k
**Link:** https://github.com/SigNoz/signoz
**Eixos:** 🎯💸🚀 (3 eixos)

### Problema Real
Datadog cobra $15-31/host/mês por infra, $12.50/milhão de log events, $1.70/span de APM. Startups com 50 servers pagam facilmente $5-20k/mês. NewRelic similar. É o imposto mais odiado do SaaS moderno.

### Por que é 5-10x melhor
- **🎯 Problema real:** O custo de observabilidade cresce linearmente com a infra — quanto mais sucesso, mais caro. Empresas estão desesperadas por alternativas
- **💸 Custo:** Self-hosted gratuito. Cloud managed ~80% mais barato que Datadog. Sem surpresas de billing
- **🚀 Escala:** OpenTelemetry nativo (standard da indústria) = logs + traces + metrics num só lugar, sem vendor lock-in

### TAM
- Observability market: $40B+ (2025), CAGR 15%+
- Datadog: $2.7B revenue, 28k+ clientes
- NewRelic: $900M+ revenue
- Público: Todo time de engenharia em produção

### Modelo de Negócio
- **Open core + SaaS:** Community self-hosted → Enterprise cloud
- **Usage-based pricing:** Transparente, sem "surprise bills" (o oposto do Datadog)
- **Enterprise:** SSO, RBAC, dashboards customizados, alerting avançado

### Esforço para Produtizar: Baixo
Produto muito maduro. Cloud offering ativo. Equipe de 50+ pessoas. VC-funded ($6.5M seed).

### Combinações
- + OpenObserve (complementar: SigNoz mais forte em APM/traces, OpenObserve em log storage barato)
- + Keep (AIOps + incident management) = stack completa anti-Datadog
- + VoltAgent (observability nativa pra AI agents) = nicho emergente de "AI observability"
