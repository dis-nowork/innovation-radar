# AI para Educação, Conteúdo e Geração de Mídia

> Atualizado: 2026-02-02

## 📚 deepseek-ai/DeepSeek-OCR
- **Stars:** 22.3k | **Forks:** 2.0k | **Licença:** MIT
- **Link:** https://github.com/deepseek-ai/DeepSeek-OCR
- **Problema real:** OCR enterprise custa caro (AWS Textract ~$1.50/1000 páginas, Google Document AI similar). Empresas processam milhões de documentos/mês.
- **O que faz:** "Context Optical Compression" — modelo vision-language que faz OCR free, 2500 tok/s em A100, suporte vLLM nativo, batch PDF processing. DeepSeek-OCR2 lançado Jan/2026.
- **Eixos:** 🎯💸⚡💎 — Free vs serviços pagos ($$$), velocidade alta com vLLM, qualidade DeepSeek-tier
- **TAM:** $13B+ (mercado global de OCR/IDP 2025)
- **Modelo de negócio:** Hosting managed (OCR-as-a-Service), enterprise fine-tuning, vertical solutions (legal, medical, finance)
- **Esforço:** Médio — precisa infraestrutura GPU, mas vLLM facilita deploy
- **Combinações:** + Karakeep (bookmarks) = bookmark anything com OCR perfeito. + formulários = IDP completo

## 📚 HKUDS/DeepTutor
- **Stars:** 9.9k | **Forks:** ~800 | **Licença:** MIT
- **Link:** https://github.com/HKUDS/DeepTutor
- **Problema real:** Tutoria particular custa $50-100/h. Estudantes precisam de ajuda personalizada mas não podem pagar. Professores não escalam.
- **O que faz:** Upload docs/papers → knowledge base com RAG multi-agent, gerador de exercícios, visualização interativa, deep research, suporte multi-LLM (Gemini free, OpenAI, Claude, Ollama). Docker-ready.
- **Eixos:** 🎯💸💎🚀 — Substitui tutor humano $50-100/h por custo quase zero, qualidade personalizada, escala infinita
- **TAM:** $120B+ (mercado global de tutoria privada)
- **Modelo de negócio:** Freemium SaaS (plano free com Gemini, pro com Claude/GPT-4), B2B para escolas/universidades, white-label para edtechs
- **Esforço:** Baixo-Médio — já tem Docker, frontend Next.js 16, multi-provider. Precisa polimento UX e onboarding
- **Combinações:** + DeepSeek-OCR = upload qualquer material impresso e estudar. + TOON = economia de tokens no pipeline RAG

## 📚 vercel-labs/json-render
- **Stars:** 9.8k | **Forks:** ~500 | **Licença:** MIT
- **Link:** https://github.com/vercel-labs/json-render
- **Problema real:** AI gerando UI é imprevisível e inseguro. Empresas querem que usuários criem dashboards/widgets via prompt mas precisam de guardrails.
- **O que faz:** Framework que define catálogo de componentes (Zod schemas), AI só gera JSON válido dentro do catálogo, streaming progressivo, actions declarativas (AI declara intenção, app executa).
- **Eixos:** 🎯💎⚡ — Resolve o problema #1 de AI-generated UI (previsibilidade), 10x mais rápido que custom parsing, qualidade enterprise
- **TAM:** $50B+ (mercado de BI/dashboards + low-code)
- **Modelo de negócio:** Core open-source + Vercel hosting premium, SDK enterprise com analytics, marketplace de component catalogs
- **Esforço:** Baixo — lib React pronta, integra com qualquer LLM provider
- **Combinações:** + qualquer SaaS = "descreva o que quer ver" como feature. Killer para internal tools, BI, CMS

## 📚 chatfire-AI/huobao-drama
- **Stars:** 6.9k | **Forks:** ~600 | **Licença:** CC-BY-NC-SA
- **Link:** https://github.com/chatfire-AI/huobao-drama
- **Problema real:** Produção de short-form video custa $5-50k por episódio. Criadores de conteúdo não têm budget. Short dramas viralizam mas são caros de produzir.
- **O que faz:** Pipeline completo: script → parse personagens → gerar retratos AI → storyboard → text-to-video → composição final com FFmpeg. DDD em Go, frontend Vue3.
- **Eixos:** 🎯⚡🚀💸 — De semanas para horas, de $5-50k para quase zero, escala de nicho para massa
- **TAM:** $20B+ (short-form video market, growing 20%+ YoY)
- **Modelo de negócio:** SaaS com créditos de geração, marketplace de templates/personagens, white-label para produtoras, API para plataformas de conteúdo
- **Esforço:** Médio — precisa GPUs para geração, mas arquitetura modular (providers plugáveis)
- **Combinações:** + NVIDIA PersonaPlex (voz) = short dramas com vozes naturais. + x-algorithm (recommendation) = geração + distribuição

## 📚 ZhuLinsen/daily_stock_analysis
- **Stars:** 8.9k | **Forks:** ~1.2k | **Licença:** MIT
- **Link:** https://github.com/ZhuLinsen/daily_stock_analysis
- **Problema real:** Análise de ações custa (Bloomberg $24k/ano, serviços premium $50-200/mês). Investidores individuais não têm acesso a análise AI quality.
- **O que faz:** Análise diária automatizada via LLM (Gemini grátis) — multi-fonte (AkShare, YFinance, etc), dashboard decisório com pontos de compra/venda, disciplina de trading embutida, push multi-canal (Telegram, WeChat, email), roda 100% em GitHub Actions = zero custo.
- **Eixos:** 🎯💸🚀 — Bloomberg quality por $0/mês, escala de manual para automático
- **TAM:** $35B+ (mercado de financial data & analytics)
- **Modelo de negócio:** Freemium (análise básica free, deep analysis pro), copy-trading signals, B2B para corretoras, white-label
- **Esforço:** Baixo — já funciona end-to-end, fork + configure = rodando

## 📚 toon-format/toon
- **Stars:** 22.4k | **Forks:** ~988 | **Licença:** MIT
- **Link:** https://github.com/toon-format/toon
- **Problema real:** LLM tokens custam dinheiro. JSON é verboso. Empresas gastam milhares/mês em tokens desnecessários enviando dados estruturados para LLMs.
- **O que faz:** Token-Oriented Object Notation — formato compacto, lossless, drop-in replacement para JSON em prompts LLM. Combina indentação YAML + layout tabular CSV. Economia de 30-60% tokens em arrays uniformes.
- **Eixos:** ⚡💸📈 — 2-3x menos tokens (= 2-3x mais barato), mesmo throughput de dados, mais volume no context window
- **TAM:** $100B+ (mercado de AI/LLM infrastructure)
- **Modelo de negócio:** SDK premium com analytics de economia, enterprise middleware, integração com proxies/gateways LLM
- **Esforço:** Baixo — TypeScript SDK pronto, spec estável, plug-and-play
- **Combinações:** + qualquer app que manda dados para LLM = economia automática. + DeepTutor/stock_analysis = mais dados no contexto por menos $
