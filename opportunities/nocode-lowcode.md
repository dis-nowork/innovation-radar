# 🔧 Plataformas/No-Code

Stream processing, no-code enterprise, feature stores, event-sourcing.

### [pathwaycom/pathway](https://github.com/pathwaycom/pathway) ⭐ 59.2k | ⚡📈
**Problema:** ETL batch demora horas. Stream processing (Kafka/Flink) é complexo demais pra maioria dos times.
**Solução:** Stream processing + RAG em Python puro. ETL real-time sem Java/Scala.
**Por que é superior:** ⚡ Real-time vs batch de horas. 📈 Python = 10x mais devs conseguem usar vs Flink.

---

### [nocobase/nocobase](https://github.com/nocobase/nocobase) ⭐ 21.4k | 🎯⚡🚀
**Problema:** Apps de negócio (CRM, ERP, gestão) são caros e inflexíveis.
**Solução:** Plataforma no-code pra criar apps de negócio com UI, API e workflows — sem programar.
**Por que é superior:** ⚡ Semanas de dev → dias no no-code. 🚀 Extensível com plugins. 🎯 21k stars, enterprise-ready.

---

### [feast-dev/feast](https://github.com/feast-dev/feast) ⭐ 6.7k | 🎯⚡
**Problema:** Features pra ML em produção: data engineers fazem pipelines ad-hoc, sem reuso, sem versionamento.
**Solução:** Feature store: registra, versiona e serve features pra modelos em tempo real.
**Por que é superior:** 🎯 Infra obrigatória pra ML maduro. ⚡ Features prontas vs rebuild a cada modelo.

---

### [kurrent-io/KurrentDB](https://github.com/kurrent-io/KurrentDB) ⭐ 5.7k | 🎯💎
**Problema:** Bancos tradicionais perdem o histórico de mudanças. Difícil auditar, reverter ou entender decisões passadas.
**Solução:** Event-sourcing DB: armazena cada evento de negócio. Histórico completo, replayable.
**Por que é superior:** 💎 Qualidade de auditoria incomparável — todo estado é derivável. 🎯 Fintech, saúde, compliance precisam.

---

### [ArroyoSystems/arroyo](https://github.com/ArroyoSystems/arroyo) ⭐ 4.8k | ⚡💸
**Problema:** Apache Flink é poderoso mas pesado, caro de operar e exige Java.
**Solução:** Stream processing com SQL em Rust. Flink simplificado, 10x mais leve.
**Por que é superior:** 💸 Fração do custo operacional do Flink. ⚡ Rust = performance nativa, SQL = acessível.

---


---

### [vercel-labs/json-render](https://github.com/vercel-labs/json-render) ⭐ 9.8k | 🎯💎⚡🚀
**Forks:** 529 | **License:** Apache-2.0 | **Criado:** Jan 2026 | **Lang:** TypeScript

**Problema Real:** AI gera texto bem, mas gerar UI é perigoso — output imprevisível, XSS, layouts quebrados. Empresas querem deixar usuários finais criar dashboards/widgets via prompts mas precisam de guardrails. Hoje: ou constroem custom (caro) ou usam no-code builders (limitados, não-AI).

**Eixos de Inovação:**
- 🎯 **Problema real:** O gap entre "AI gera texto" e "AI gera UI segura" é o blocker #1 de AI-powered internal tools.
- 💎 **5-10x qualidade:** Guardrailed — AI só usa componentes do catálogo definido. JSON validado por schema Zod. Zero chance de UI quebrada.
- ⚡ **5-10x velocidade:** Streaming progressivo — renderiza conforme o modelo responde. Prompt → UI em segundos.
- 🚀 **5-10x escala:** Catalog pattern escala infinitamente — defina 10 ou 10,000 componentes. Vercel-backed, React-native.

**TAM:** Low-code/no-code market: $30B+ em 2025, crescendo 25%/ano. Internal tools market: $15B+.

**Modelo de Negócio:**
- OSS framework gratuito + hosted platform premium (ala Vercel)
- Component marketplace: bibliotecas de catálogos pré-prontos por indústria
- Enterprise: catálogos privados, SSO, audit logs
- Embedding fee: empresas embutem json-render em seus produtos

**Esforço:** Baixo — npm install, API clara, Vercel ecosystem. Precisa de catálogos prontos pra diferentes use cases.

**Combinações:**
- json-render + DeepAnalyze (#261) = dados → análise → dashboard AI-generated guardrailed
- json-render + ChartGPU = catálogo com charts WebGPU de alta performance
- json-render + OpenMemory (#262) = dashboards que lembram preferências do usuário
