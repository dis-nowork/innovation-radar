# Infraestrutura "Chata" + 3D/Video Acceleration — Feb 2, 2026 (Round 2)

## 1. PDFCraftTool/pdfcraft ⭐ 2.5k
**Link:** https://github.com/PDFCraftTool/pdfcraft
**Categoria:** Produtividade/PDF Tools
**Eixos:** 🎯💸🚀💎

### Problema Real
Ferramentas de PDF são um mercado bilionário dominado por incumbentes caros: Adobe Acrobat ($13-23/mês), Smallpdf ($12/mês), iLovePDF (freemium limitado). Milhões de pessoas carregam documentos sensíveis em servidores de terceiros diariamente.

### Por que é 5-10x melhor
- **💸 Custo:** 100% grátis, 90+ ferramentas vs Acrobat $276/ano
- **🎯 Problema real:** 100% client-side via WebAssembly — documentos NUNCA saem do dispositivo
- **🚀 Escala:** Workflow Editor visual (drag-and-drop) — encadear operações PDF em pipelines, 23+ templates pré-built
- **💎 Qualidade:** 90+ ferramentas profissionais: merge, split, compress, convert, watermark, OCR, encrypt, invoice processing
- Next.js 15 + React 19 + Tailwind — UI moderna, multi-idioma (8 langs incluindo PT)
- Batch processing, templates reusáveis

### TAM
$4-6B mercado global de PDF tools. Adobe Acrobat sozinho fatura $3B+/ano. Tens de milhões de SMBs e indivíduos pagam por PDF tools.

### Modelo de Negócio
- Self-hosted enterprise (compliance/on-premise)
- White-label para plataformas (real estate, legal, healthcare)
- Premium features (OCR avançado, batch unlimited, API)
- SaaS hosted com workflow builder

### Esforço: Baixo
Funcional, deployed, 90+ ferramentas. Precisa marketing e tier premium.

### Combinações
- Com dots.ocr (#363) → PDF→structured data extraction
- Com Unstract (#94) → no-code document processing pipeline

---

## 2. HKUDS/Paper2Slides ⭐ 3.0k
**Link:** https://github.com/HKUDS/Paper2Slides
**Categoria:** EdTech/Produtividade Acadêmica
**Eixos:** 🎯⚡🚀💎

### Problema Real
Pesquisadores e estudantes gastam 4-8 horas transformando papers em apresentações. Com 5M+ papers publicados/ano, é um problema universal no mundo acadêmico e corporativo (relatórios→decks).

### Por que é 5-10x melhor
- **⚡ Velocidade:** Paper→slides em minutos vs horas de trabalho manual
- **💎 Qualidade:** RAG-powered extraction — captura figuras, dados, insights com precisão e traceabilidade
- **🚀 Escala:** Universal file support (PDF, Word, Excel, PPT, Markdown), parallel generation
- Custom styling por NL ("Studio Ghibli style", "minimalist blue"), temas built-in
- Session management com checkpoints — pause/resume sem perda
- Source-linked accuracy — rastreabilidade entre slide e fonte original
- Gera slides E posters

### TAM
130M+ researchers globalmente + 300M+ estudantes universitários. Mercado de academic tools $5B+.

### Modelo de Negócio
- Freemium SaaS (N slides grátis/mês, premium unlimited)
- Enterprise (corporate decks, consulting firms)
- API para plataformas acadêmicas (ResearchGate, arXiv)
- White-label para universidades

### Esforço: Baixo-Médio
CLI e web interface funcionais. Precisa hosted service e pricing tier.

### Combinações
- Com banana-slides (#154/354) → paper→AI-generated visual slides
- Com DeepTutor (#209) → study pipeline: paper→slides→quiz→flashcards

---

## 3. thu-ml/TurboDiffusion ⭐ 3.3k
**Link:** https://github.com/thu-ml/TurboDiffusion
**Categoria:** AI/Video Acceleration
**Eixos:** ⚡💸🚀

### Problema Real
Video diffusion models (Wan2.2, SORA) demoram 3-5 minutos para gerar 5s de vídeo em GPUs top. Isso torna interatividade impossível e custo de API proibitivo para escala.

### Por que é 5-10x melhor
- **⚡ Velocidade:** 100-200x aceleração end-to-end — 184s→1.9s para 5s de vídeo em RTX 5090
- **💸 Custo:** Quantização permite rodar em 4090 (consumer GPU). Elimina necessidade de H100s para inferência
- **🚀 Escala:** Transforma video gen de "batch overnight" para "real-time interactive"
- Combina SageAttention + Sparse-Linear Attention + rCM timestep distillation
- Suporta Wan2.1 e Wan2.2 (text→video e image→video)
- 480P e 720P

### TAM
$5-10B mercado de video generation. Com 100x speedup, video gen se torna viável para advertising, social media, e-commerce — mercados que hoje não usam por ser lento demais.

### Modelo de Negócio
- Inference acceleration as-a-service (API wrapper)
- Licensing para plataformas de video gen
- Hardware-optimized deployment consulting
- Integration SDK para apps de conteúdo

### Esforço: Médio
Research-grade mas com modelos publicados e pip install. Precisa productionize.

### Combinações
- Com Wan2.2 (#367) → video gen frontier a preço acessível
- Com InfiniteTalk (#368) → talking videos em real-time
- Com LTX-2 (#349) → audio+video generation acelerada

---

## 4. bellard/mquickjs ⭐ 5.4k
**Link:** https://github.com/bellard/mquickjs
**Categoria:** Runtime/Embedded Systems
**Eixos:** ⚡💸🚀

### Problema Real
IoT e embedded devices precisam de scripting mas não têm RAM para Node.js (100MB+) ou mesmo QuickJS regular. Wearables, sensores, microcontroladores ficam limitados a C hardcoded.

### Por que é 5-10x melhor
- **⚡ Velocidade:** Comparable speed ao QuickJS original com 10-100x menos memória
- **💸 Custo:** 10KB RAM, 100KB ROM — roda em microcontroladores $1-5
- **🚀 Escala:** JavaScript em QUALQUER device — de wearables a sensores industriais
- UTF-8 strings, tracing GC (não reference counting), VM sem CPU stack
- Bytecode compilation + persistent storage — compile uma vez, execute offline
- Cross-compile 32/64 bit
- Por Fabrice Bellard (FFmpeg, QEMU, JSLinux) — qualidade lendária

### TAM
14B+ IoT devices em 2026. Mercado de IoT runtime/edge computing $8B+.

### Modelo de Negócio
- OEM licensing para device manufacturers
- IoT platform integration (AWS IoT, Azure IoT Hub)
- Embedded scripting SDK para hardware companies
- Training/consulting para migração de firmware para JS

### Esforço: Médio-Alto
Motor de altíssima qualidade mas precisa ecosystem (package manager, tooling, IDE support).

---

## 5. apple/ml-sharp ⭐ 7.4k
**Link:** https://github.com/apple/ml-sharp
**Categoria:** AI/3D Vision
**Eixos:** 🎯💎⚡🚀

### Problema Real
Criar conteúdo 3D (e-commerce product views, real estate tours, gaming assets) requer photogrammetry com múltiplas fotos, scanners 3D caros ($10K+), ou artistas 3D ($50-200/h). Uma única foto não bastava.

### Por que é 5-10x melhor
- **⚡ Velocidade:** Single feedforward pass < 1 segundo (vs minutos/horas com NeRF/photogrammetry)
- **💎 Qualidade:** LPIPS -25-34%, DISTS -21-43% vs melhor modelo anterior. Estado da arte em robustez zero-shot
- **🚀 Escala:** Uma foto → 3D Gaussian Splat métrico com escala absoluta. Real-time rendering depois
- **🎯 Problema real:** Qualquer foto do celular → modelo 3D renderizável em tempo real
- Output compatível com 3DGS renderers padrão
- Apple research — provável integração em Vision Pro / ARKit

### TAM
$10B+ mercado de 3D content creation. E-commerce alone: 200M+ product listings que poderiam ter 3D views.

### Modelo de Negócio
- SaaS: upload foto → 3D model (e-commerce, real estate, insurance)
- API para plataformas (Shopify, Amazon, Airbnb)
- Game asset pipeline
- AR/VR content creation

### Esforço: Médio
Modelo funcional com CLI. Precisa API wrapper e pipeline de qualidade.

### Combinações
- Com Z-Image (#369) → gerar imagens AI + converter em 3D
- Com lingbot-world (#374) → world models com 3D objects gerados de fotos

---

## 6. stoolap/stoolap ⭐ 538
**Link:** https://github.com/stoolap/stoolap
**Categoria:** Infra/Database
**Eixos:** 💎⚡💸

### Problema Real
Developers precisam de databases embeddáveis mas SQLite não tem MVCC, cost-based optimizer, ou parallel execution. DuckDB é OLAP-focused. Não existe um "melhor dos dois mundos" para apps que precisam de OLTP + analytics.

### Por que é 5-10x melhor
- **💎 Qualidade:** Features que só PostgreSQL tem: MVCC, cost-based optimizer, parallel execution, time-travel queries (AS OF)
- **⚡ Velocidade:** Semantic query caching + adaptive query execution — features únicas
- **💸 Custo:** Embedded, zero deps, pure Rust, sem servidor
- AS OF time-travel queries (único entre embedded DBs)
- MVCC transactions (SQLite não tem)
- Memory-safe (Rust) vs SQLite (C com histórico de CVEs)

### TAM
SQLite está em 1T+ devices. Embedded DB market $3B+. Qualquer app que precisa de DB local.

### Modelo de Negócio
- Open-core (free embedded + enterprise features)
- Cloud managed service (stoolap-as-a-service)
- Consulting para migração SQLite→stoolap

### Esforço: Médio-Alto
Early-stage (538⭐) mas feature set impressionante. Precisa maturidade e ecosystem.

### Combinações
- Com qualquer agent framework → database embeddável com time-travel para audit
- Com SimpleMem (#371) → persistent memory store com SQL queries
