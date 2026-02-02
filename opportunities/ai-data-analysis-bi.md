# 🧠📊 AI Data Analysis & Business Intelligence

Ferramentas que democratizam acesso a dados — qualquer pessoa pergunta em linguagem natural, recebe SQL, gráficos e insights. Substituem Tableau ($70/user/mês), Looker ($5k+/mês), e analistas de dados.

---

### [sinaptik-ai/pandas-ai](https://github.com/sinaptik-ai/pandas-ai) ⭐ 23.1k | 🎯⚡💸🚀
**Problema:** Analistas gastam 60-80% do tempo escrevendo SQL/Python pra responder perguntas simples. Não-técnicos ficam na fila esperando.
**Solução:** Biblioteca Python que permite "conversar" com databases, CSV, parquet. Faz query, gera gráficos, suporta múltiplos DataFrames.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Milhões de PMEs têm dados mas não sabem SQL
- ⚡ **Velocidade:** Pergunta → resposta em segundos vs horas esperando analista
- 💸 **Custo:** Open-source vs Tableau a $70/user/mês
- 🚀 **Escala:** Qualquer pessoa com Python pode usar, não só data analysts
**TAM:** $30B+ (BI + data analytics market)
**Modelo:** Freemium (lib open-source) + cloud hosted + enterprise features
**Esforço:** Médio — precisa UI bonita pra não-técnicos, integração com DBs empresariais
**Combinações:** + WrenAI (semantic layer) + Evidence (reports) = BI stack completa open-source

---

### [vanna-ai/vanna](https://github.com/vanna-ai/vanna) ⭐ 22.5k | 🎯💎⚡🚀
**Problema:** Text-to-SQL genérico erra muito em bancos complexos. Empresas não podem usar sem segurança adequada.
**Solução:** Text-to-SQL com RAG agentic que aprende o schema, web component `<vanna-chat>` embeddable, row-level security, audit logs, streaming.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Cada empresa quer "perguntar ao banco de dados" sem riscos
- 💎 **Qualidade:** Agentic Retrieval + fine-tuning por contexto organizacional = SQL mais preciso
- ⚡ **Velocidade:** Streaming real-time com tabelas + charts + resumo NL
- 🚀 **Escala:** Web component drop-in pra qualquer app (React, Vue, HTML puro)
**TAM:** $15B+ (embedded analytics + enterprise BI)
**Modelo:** Open-source core + Vanna Cloud (hosted) + enterprise licenses
**Esforço:** Baixo — produto já enterprise-ready, 2.0 acabou de lançar
**Combinações:** Embed em CRM (Twenty #5) ou ERP (AureusERP #69) = decision-making integrado

---

### [Canner/WrenAI](https://github.com/Canner/WrenAI) ⭐ 13.6k | 🎯💸⚡🚀
**Problema:** BI tradicional (Tableau, Power BI, Looker) custa $5k-50k/mês e precisa de analistas treinados.
**Solução:** GenBI completo — NL→SQL→Charts→Reports em segundos. Semantic layer (MDL) garante precisão. API pra embeddar em qualquer app.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** 90% das PMEs não usam BI por custo/complexidade
- 💸 **Custo:** Self-hosted grátis vs $70-5000/mês em SaaS BI
- ⚡ **Velocidade:** Setup em 3 min, perguntas respondidas em segundos
- 🚀 **Escala:** Multi-database, embed via API, qualquer idioma
**TAM:** $30B+ (BI market)
**Modelo:** Open-source + WrenAI Cloud + enterprise (segurança, SSO, SLA)
**Esforço:** Médio — precisa mais integrações de dados e templates verticais
**Combinações:** + Bigcapital (#139) = "CFO virtual" pra PMEs que responde perguntas financeiras

---

### [evidence-dev/evidence](https://github.com/evidence-dev/evidence) ⭐ 5.9k | 🎯💸💎
**Problema:** Dashboards drag-and-drop (Tableau, Metabase) são lentos, difíceis de versionar, e impossíveis de review em PR.
**Solução:** BI como código — SQL dentro de Markdown gera sites interativos com charts. Git-versionado, CI/CD compatível, dev-first.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Data teams querem tratar dashboards como código (version, review, deploy)
- 💸 **Custo:** Open-source, deploya em Netlify/Vercel grátis
- 💎 **Qualidade:** Templated pages geram centenas de reports de um template só
**TAM:** $10B+ (BI tools market, segment: dev-first)
**Modelo:** Open-source + Evidence Studio (cloud IDE) + enterprise
**Esforço:** Baixo-Médio — já maduro, precisa mais connectors e AI integration
**Combinações:** + PandasAI (#146) ou Vanna (#147) pra camada conversacional

---

### [Dataherald/dataherald](https://github.com/Dataherald/dataherald) ⭐ 3.6k | 🎯💎⚡
**Problema:** LLMs genéricos (ChatGPT) geram SQL incorreto em schemas empresariais complexos.
**Solução:** NL-to-SQL com fine-tuning contínuo baseado no contexto organizacional. API REST enterprise, golden SQL library, auto-aprendizagem.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Empresas com schemas de 500+ tabelas precisam de contexto
- 💎 **Qualidade:** Fine-tuning contínuo melhora accuracy com uso — quanto mais perguntas, melhor
- ⚡ **Velocidade:** API pronta pra embeddar em minutos
**TAM:** $5B+ (enterprise data querying)
**Modelo:** Open-source + Dataherald AI (cloud hosted) + enterprise
**Esforço:** Médio — precisa simplificar onboarding e adicionar UI pra non-devs

---

### [frappe/books](https://github.com/frappe/books) ⭐ 4.1k | 🎯💸
**Problema:** Software de contabilidade (QuickBooks, Xero) custa $20-100/mês e é complexo demais pra micro-empresas.
**Solução:** App desktop de contabilidade bonito, offline-first, open-source. Invoicing, relatórios, multi-moeda.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Milhões de micro-empresas usam planilhas porque software de contabilidade é caro
- 💸 **Custo:** Grátis vs $20-100/mês (QuickBooks/Xero)
**TAM:** $12B+ (SMB accounting software market)
**Modelo:** Desktop gratuito + cloud sync premium + marketplace de extensões
**Esforço:** Médio — precisa de integrações bancárias regionais (Pix, boleto pra BR)
**Combinações:** + Bigcapital (#139) como backend API + WrenAI (#148) pra perguntas em linguagem natural = "Contabilidade inteligente"

---

### [ruc-datalab/DeepAnalyze](https://github.com/ruc-datalab/DeepAnalyze) ⭐ 3.6k | 🎯💎⚡🚀
**Forks:** 521 | **License:** MIT | **Criado:** Out 2025 | **Lang:** Python

**Problema Real:** Data science é o gargalo de toda empresa data-driven. Cientistas de dados custam $120-200k/ano e o backlog de análises é infinito. PMEs e times de produto querem insights dos seus dados mas não sabem SQL/Python. Ferramentas como Tableau ($70/user/mês) e Looker são caras e exigem modelagem manual.

**Eixos de Inovação:**
- 🎯 **Problema real:** 80% das empresas têm dados mas não conseguem extrair insights. Data science talent gap é 3M+ globalmente.
- 💎 **5-10x qualidade:** Primeiro LLM agêntico treinado especificamente para data science — modelo 8B + 500K dataset de instrução. Não é GPT genérico fazendo pandas.
- ⚡ **5-10x velocidade:** Upload CSV → relatório profissional com visualizações em minutos vs dias/semanas com analista humano.
- 🚀 **5-10x escala:** Modelo open-source (HuggingFace) permite deploy local. Suporta structured, semi-structured e unstructured data.

**TAM:** Business intelligence market: $33B em 2025, crescendo 10%/ano. Data science platforms: $20B+.

**Modelo de Negócio:**
- SaaS cloud: $49-299/mês por volume de análises
- API: pay-per-analysis para integração em plataformas
- Enterprise on-prem: $50-200k/ano para dados sensíveis
- Vertical templates: análise financeira, marketing, supply chain

**Esforço:** Médio — modelo funciona, mas UX precisa de polish. API already available.

**Combinações:**
- DeepAnalyze + chandra (#260) = documentos físicos → dados → análise automática
- DeepAnalyze + ChartGPU = análise + visualização WebGPU em tempo real
- DeepAnalyze + daily_stock_analysis (#246) = análise financeira profunda automatizada
- DeepAnalyze + json-render (#258) = análise → dashboard interativo gerado por AI
