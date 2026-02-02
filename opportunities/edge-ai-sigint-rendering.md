# Edge AI, SIGINT & High-Performance Rendering
> Análise: 2 Fev 2026 — Tema: Ferramentas que eliminam dependências pesadas (GPU, browser, cloud)

---

## 1. Lightricks/LTX-2 ⭐ 3.4k
**Link:** https://github.com/Lightricks/LTX-2
**Problema real:** Geração de vídeo com áudio requer múltiplos modelos separados (vídeo + TTS + sync). Serviços como Runway/Pika cobram $$$, sem áudio, e são black-box.
**O que faz:** Primeiro modelo DiT (Diffusion Transformer) que gera vídeo E áudio sincronizados num único modelo. 19B params, text-to-video e image-to-video, com spatial/temporal upscalers, LoRA trainer, e pipeline modular.

### Eixos de Inovação
- 🎯 **Problema real:** Criadores de conteúdo precisam de vídeo+áudio e hoje usam 3-4 ferramentas separadas
- 💎 **Qualidade:** Primeiro modelo unificado audio+video — elimina dessincronização e artifacts de compositing
- 🚀 **Escala:** LoRA training permite fine-tuning para domínios específicos (e-commerce, educação, marketing)
- ⚡ **Velocidade:** Pipeline distilled permite inference rápida, FP8 quantization

### TAM & Modelo de Negócio
- **TAM:** Video generation market ~$1.5B+ (2026), crescendo 30%+ ao ano
- **Modelo:** API as a service, LoRA marketplace (vende styles/domains), enterprise licensing, white-label para plataformas de conteúdo
- **Esforço:** Médio-Alto (requer GPU inference infra, mas pipeline é bem modular)

### Combinações
- + DeepSeek-OCR-2 → extrai texto de vídeos e re-gera com edições
- + Pocket TTS → voice-over local + vídeo gerado = content pipeline completo
- + Qwen3-ASR → transcrição automática de vídeos gerados para legendas

---

## 2. kyutai-labs/pocket-tts ⭐ 2.9k
**Link:** https://github.com/kyutai-labs/pocket-tts
**Problema real:** TTS decente requer GPU ou APIs caras (ElevenLabs $5-99/mês). Desenvolvedores mobile/edge não têm opção local viável.
**O que faz:** Modelo TTS de 100M params que roda em CPU puro (2 cores), 6x real-time no MacBook Air M4, 200ms latência p/ primeiro chunk, streaming, voice cloning, roda no browser via WASM.

### Eixos de Inovação
- 🎯 **Problema real:** TTS local viável elimina dependência de cloud para apps de voz
- 💸 **Custo:** $0 vs ElevenLabs/Play.ht ($5-330/mês) — economia total
- ⚡ **Velocidade:** 200ms first chunk, 6x real-time — viável para conversação
- 🚀 **Escala:** Roda no browser = deploy para milhões sem infra de GPU

### TAM & Modelo de Negócio
- **TAM:** TTS market ~$5B+ (2026), explosão com AI assistants
- **Modelo:** Freemium SDK (voice cloning premium, mais vozes, multi-idioma quando sair), embedded licensing para hardware, enterprise support
- **Esforço:** Baixo-Médio (já funciona como pip install, falta multi-idioma)

### Combinações
- + Qwen3-ASR → speech-to-speech pipeline 100% local, zero cloud
- + LTX-2 → gera vídeo com narração sem GPU dedicada para TTS
- + qualquer chatbot → assistente de voz local para IoT/smart home

---

## 3. hipcityreg/situation-monitor ⭐ 2.4k
**Link:** https://github.com/hipcityreg/situation-monitor
**Problema real:** Traders, analistas, jornalistas e equipes de risco precisam monitorar múltiplas fontes (news, mercados, geopolítica) em tempo real. Hoje usam Bloomberg Terminal ($24k/ano) ou cobrem manualmente 10+ tabs.
**O que faz:** Dashboard TypeScript real-time que agrega notícias globais, dados de mercado e eventos geopolíticos com alertas e visualização unificada.

### Eixos de Inovação
- 🎯 **Problema real:** Monitoramento multi-fonte é caro (Bloomberg) ou manual (10 tabs abertas)
- 💎 **Qualidade:** Visualização unificada com correlação news↔markets
- 🚀 **Escala:** De uso individual para war rooms corporativas

### TAM & Modelo de Negócio
- **TAM:** Market intelligence ~$30B+, Bloomberg Terminal sozinho ~$10B revenue
- **Modelo:** Freemium (dashboards básicos grátis), enterprise (custom feeds, alertas, API), data add-ons
- **Esforço:** Médio (precisa de curadoria de fontes, infra de streaming)

### Combinações
- + Dexter (financial research agent) → análise automática de eventos detectados
- + Daily Stock Analysis → combina monitoramento macro com análise micro por ação
- + LLM summarization → briefings automáticos de situação

---

## 4. deepseek-ai/DeepSeek-OCR-2 ⭐ 1.9k
**Link:** https://github.com/deepseek-ai/DeepSeek-OCR-2
**Problema real:** OCR tradicional trata imagem como grid de pixels. Documentos complexos (tabelas, diagramas, handwriting) falham em abordagens convencionais.
**O que faz:** "Visual Causal Flow" — novo paradigma de encoding visual inspirado em como humanos leem (fluxo causal), evolução do DeepSeek-OCR-1 que já era SOTA. vLLM inference, Apache-2.0.

### Eixos de Inovação
- 🎯 **Problema real:** OCR de documentos complexos ainda é unreliable e caro
- 💎 **Qualidade:** Paradigma "visual causal flow" = encoding mais natural, menos erros em layouts complexos
- ⚡ **Velocidade:** vLLM backend = high-throughput batch processing

### TAM & Modelo de Negócio
- **TAM:** Document AI market ~$8B+ (2026)
- **Modelo:** API processing (pay-per-page), enterprise on-prem, vertical solutions (legal, medical, finance)
- **Esforço:** Médio (modelo pronto, falta productização e pipeline end-to-end)

### Combinações
- + OCR-1 → ensemble para confidence scoring
- + RAG pipelines → melhor ingestão de documentos para knowledge bases
- + LTX-2 → OCR extrai→edita→re-gera conteúdo visual

---

## 5. QwenLM/Qwen3-ASR ⭐ 1.1k
**Link:** https://github.com/QwenLM/Qwen3-ASR
**Problema real:** ASR multilíngue de qualidade requer Whisper large (pesado) ou APIs pagas (Google/AWS/Azure). Modelos open-source não cobrem dialetos e idiomas menores.
**O que faz:** Família de modelos ASR (0.6B/1.7B) que suporta 52 idiomas + dialetos, language detection automática, timestamp prediction, streaming inference, e um modelo de forced alignment para 11 idiomas. SOTA entre open-source ASR.

### Eixos de Inovação
- 🎯 **Problema real:** Transcrição multilíngue confiável é cara e limitada em idiomas
- 💎 **Qualidade:** SOTA open-source, competitivo com APIs proprietárias
- 🚀 **Escala:** 52 idiomas num único modelo = cobertura global
- 💸 **Custo:** Self-hosted grátis vs Google Speech-to-Text ($0.006-0.024/15s)

### TAM & Modelo de Negócio
- **TAM:** Speech recognition market ~$25B+ (2026)
- **Modelo:** API as a service (multi-tenant), edge deployment licensing, vertical (call centers, medical transcription, legal), subtitle generation SaaS
- **Esforço:** Baixo-Médio (modelos prontos, Docker, vLLM support)

### Combinações
- + Pocket TTS → pipeline speech-to-speech completo e local
- + Meeting transcription tools → transcrição multilíngue automática
- + Content platforms → legendas automáticas em 52 idiomas

---

## 6. smittix/intercept ⭐ 1.1k
**Link:** https://github.com/smittix/intercept
**Problema real:** Ferramentas SIGINT (SDR, pager decode, ADS-B, AIS) são fragmentadas — cada protocolo requer setup e tool separados. Profissionais de segurança gastam horas configurando.
**O que faz:** Plataforma unificada web-based que integra: POCSAG/FLEX pager decode, 433MHz sensor capture, ADS-B aircraft tracking, AIS vessel tracking, ACARS messages, WiFi/BT scanning, satellite tracking, Meshtastic, remote agents. Funciona offline para deployments em campo.

### Eixos de Inovação
- 🎯 **Problema real:** SIGINT fragmentada = horas de setup por protocolo
- 💸 **Custo:** $0 vs hardware+software proprietário ($10k-100k+)
- 🚀 **Escala:** De uma antena local para rede distribuída com remote agents
- 💎 **Qualidade:** Interface unificada com 12+ protocolos vs ferramentas CLI isoladas

### TAM & Modelo de Negócio
- **TAM:** SIGINT/SDR market ~$15B+ (defense), $2B+ (commercial/hobbyist)
- **Modelo:** Hardware bundles (Raspberry Pi + SDR + Intercept pré-configurado), enterprise licensing (defense/gov), premium plugins, remote agent management
- **Esforço:** Médio (depende de hardware SDR, mas software é plug-and-play)

### Combinações
- + Situation Monitor → SIGINT + OSINT unificados numa intelligence platform
- + AI analysis → classificação automática de sinais capturados
- + Meshtastic mesh → rede de sensores distribuída autônoma

---

## 7. 1jehuang/mermaid-rs-renderer ⭐ 749
**Link:** https://github.com/1jehuang/mermaid-rs-renderer
**Problema real:** Mermaid-cli usa Puppeteer/Chromium = lento (2-3s por diagrama), pesado, frágil em CI/CD. Impossível usar em batch ou real-time.
**O que faz:** Renderer Mermaid em Rust puro — 500-1600x mais rápido, zero dependência de browser, font cache, suporta flowchart/class/state/sequence. Um diagrama em ~3ms vs ~2.5s.

### Eixos de Inovação
- ⚡ **Velocidade:** 500-1600x mais rápido — de segundos para milissegundos
- 💸 **Custo:** Elimina Chromium headless = menos RAM, CPU, e complexidade em CI
- 💎 **Qualidade:** Renderização nativa sem artifacts de browser rendering

### TAM & Modelo de Negócio
- **TAM:** Developer tools / documentation market (diagramming ~$2B+)
- **Modelo:** CLI tool gratuito, SaaS rendering API (pay-per-render, batch pricing), plugin para ferramentas de documentação, enterprise Confluence/Notion integration
- **Esforço:** Baixo (CLI pronto, falta mais diagram types e integrações)

### Combinações
- + AI code agents → geração de diagramas em tempo real durante code review
- + Documentation platforms → rendering instantâneo de diagramas em wikis
- + CI/CD pipelines → geração de architecture diagrams automáticos em PRs
