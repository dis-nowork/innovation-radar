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

### [google/langextract](https://github.com/google/langextract) ⭐ 23.9k | 🎯💎⚡🚀
**Problema:** Extrair informação estruturada de texto livre (notas clínicas, contratos, relatórios) requer pipelines NER complexos, fine-tuning, ou regex frágeis. Empresas gastam meses construindo extractors customizados.
**Solução:** Biblioteca Python do Google que usa LLMs para extrair dados estruturados com source grounding preciso (mapeia cada extração ao texto original) + visualização HTML interativa. Funciona com few-shot examples, sem fine-tuning.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Healthcare, legal, finance — todos precisam extrair dados de texto não-estruturado
- 💎 **Qualidade:** Source grounding elimina alucinações — cada fact vem com highlight no texto original
- ⚡ **Velocidade:** Chunking otimizado + processamento paralelo supera "needle in haystack" de docs longos
- 🚀 **Escala:** De domínio específico a qualquer domínio com few-shot examples — sem retreinamento
**TAM:** $5B+ (intelligent document processing + NLP extraction)
**Modelo de negócio:** SaaS de extração vertical (healthcare, legal, finance), API metered, enterprise on-prem
**Esforço:** Médio — core library pronta, precisa wrapper SaaS + integrations
**Combinações:** LangExtract + Docling (#89) = PDF→texto→extração estruturada end-to-end. LangExtract + CocoIndex (#95) = pipeline incremental de extração em larga escala

### [deepseek-ai/DeepSeek-OCR](https://github.com/deepseek-ai/DeepSeek-OCR) ⭐ 22.3k | 🎯⚡💸📈
**Problema:** OCR tradicional (Tesseract, ABBYY, AWS Textract) é caro, lento em documentos complexos, e perde contexto semântico. OCR "inteligente" requer integração de múltiplas ferramentas.
**Solução:** "Contexts Optical Compression" — modelo LLM-centric que investiga visão encoders de uma perspectiva centrada no LLM. ~2500 tokens/s em A100. DeepSeek-OCR2 já lançado (Jan 2026). Suportado em vLLM upstream.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo negócio digitaliza documentos — receitas, contratos, faturas
- ⚡ **Velocidade:** 2500 tokens/s throughput de produção
- 💸 **Custo:** Open-source vs Textract/ABBYY pricing ($1.50+ per 1000 pages)
- 📈 **Volume:** Batch processing nativo, streaming output, concurrency otimizada
**TAM:** $15B+ (OCR/IDP market, um dos maiores de enterprise AI)
**Modelo de negócio:** Managed OCR API (pay-per-page), on-prem enterprise, vertical solutions (healthcare records, legal discovery)
**Esforço:** Alto — requer GPU infra, mas vLLM integration já resolve serving
**Combinações:** DeepSeek-OCR + LangExtract (#128) = scan→OCR→extração estruturada. DeepSeek-OCR + Unstract (#94) = document processing pipeline completo

---

### [VectifyAI/PageIndex](https://github.com/VectifyAI/PageIndex) ⭐ 12.0k | 🎯💎⚡

**O que faz:** RAG sem vetores — constrói índice hierárquico em árvore de documentos e usa LLMs para reasoning-based retrieval. Inspirado no AlphaGo. Alcançou **98.7% accuracy no FinanceBench** (vs ~70-80% de vector RAG). Chat platform, MCP server e API disponíveis.

**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Vector RAG falha em documentos profissionais longos (contratos, relatórios financeiros, papers médicos) — similaridade ≠ relevância
- 💎 **98.7% accuracy** vs ~75% de vector RAG em benchmarks financeiros — salto qualitativo
- ⚡ **Sem chunking, sem embedding, sem vector DB** — pipeline drasticamente mais simples

**TAM:** $15B+ (enterprise search + document intelligence) — todo setor regulado (legal, financeiro, saúde)

**Modelo de negócio:** 
- SaaS: chat.pageindex.ai (já funcional)
- API/MCP: integração em workflows existentes
- Enterprise: on-prem para setores regulados (compliance)
- Vertical solutions: FinTech, LegalTech, HealthTech

**Esforço:** Baixo — self-host com código open-source, cloud já disponível

**Combinações:** 
- PageIndex + DeepSeek-OCR (#161) = scan→index→reasoning retrieval p/ documentos físicos
- PageIndex + Motia (#166) = backend workflow com RAG frontier embutido
- PageIndex + LangExtract (#158) = extração + retrieval reasoning = análise documental end-to-end
