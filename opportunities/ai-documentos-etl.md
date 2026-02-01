# 📄 AI/Documentos & ETL

Processamento de documentos, extração de dados, pipelines de transformação com AI.

### [docling-project/docling](https://github.com/docling-project/docling) ⭐ 51.8k | 🎯💸⚡💎
**Problema:** Empresas gastam centenas de horas/ano convertendo PDFs, DOCXs, slides em dados estruturados. Ferramentas pagas (Adobe Acrobat Pro, AWS Textract) são caras e limitadas por formato.
**Solução:** Parser universal open-source que converte PDF, DOCX, PPTX, XLSX, HTML, imagens e até áudio para formatos gen AI-ready (Markdown, JSON). Suporte a OCR, tabelas, fórmulas, layout avançado. Roda 100% local.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo workflow de RAG/AI começa com "parse o documento" — docling é a fundação
- 💸 **Custo:** $0 vs AWS Textract ($1.50/1000 páginas) ou Adobe ($240/ano)
- ⚡ **Velocidade:** `pip install docling` + 3 linhas de Python = conversão funcionando
- 💎 **Qualidade:** Entende layout, tabelas, fórmulas — não apenas "extrai texto bruto"
**TAM:** $4B+ (document processing market, crescendo 15% ao ano)
**Modelo de negócio:** Enterprise support, cloud hosted, integração com plataformas de AI
**Esforço:** Baixo — já é production-ready, integrações com LangChain/LlamaIndex/CrewAI prontas
**Combinações:** Docling + Unstract (#94) + CocoIndex (#95) = pipeline completo doc→estruturado→vector DB

---

### [Zipstack/unstract](https://github.com/Zipstack/unstract) ⭐ 6.1k | 🎯⚡🚀💸
**Problema:** Empresas recebem milhares de documentos não-estruturados (faturas, contratos, relatórios) que precisam virar dados estruturados. Hoje é manual ou requer devs caros.
**Solução:** Plataforma no-code que transforma docs não-estruturados em JSON via LLMs. Prompt Studio visual para definir schemas. Deploy como API ou ETL pipeline com um clique. Integra com n8n.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Empresas gastam $50-200k/ano em data entry manual
- ⚡ **Velocidade:** De semanas de dev para horas no visual Prompt Studio
- 🚀 **Escala:** Um schema serve para milhares de variações de documento
- 💸 **Custo:** Self-hosted grátis vs serviços de IDP (Intelligent Document Processing) a $25-100k/ano
**TAM:** $3B+ (intelligent document processing, 37% CAGR)
**Modelo de negócio:** Cloud edition com features enterprise (LLMChallenge, SSO, HITL)
**Esforço:** Médio — precisa orquestrar LLMs e storage, mas já tem Docker/cloud ready
**Combinações:** Unstract + Docling (#89) = parsing perfeito + extração estruturada. Unstract + n8n/Activepieces (#73) = automação end-to-end de documentos

---

### [cocoindex-io/cocoindex](https://github.com/cocoindex-io/cocoindex) ⭐ 6.0k | ⚡📈💸
**Problema:** Pipelines de dados para AI (vector indexing, knowledge graphs) são frágeis, lentos para atualizar, e exigem reprocessamento completo quando algo muda.
**Solução:** Framework declarativo de transformação de dados com core em Rust. Suporte nativo a processamento incremental — só reprocessa o que mudou. Data lineage out-of-box.
**Por que é 5-10x melhor:**
- ⚡ **Velocidade:** Core Rust = ordens de magnitude mais rápido que Python puro. Incremental = atualiza em segundos vs reindexar tudo
- 📈 **Volume:** Escala para datasets massivos mantendo freshness
- 💸 **Custo:** ~100 linhas de Python vs pipelines complexos com Airflow/dbt
**TAM:** $2B+ (data transformation/ETL for AI, mercado nascente mas explosivo)
**Modelo de negócio:** Cloud managed service, enterprise features
**Esforço:** Médio — requer Postgres, mas setup é straightforward
**Combinações:** CocoIndex + Docling (#89) + Graphiti (#91) = pipeline doc→transformação→knowledge graph com freshness automática

---
