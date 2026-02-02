# 🎙️ Voice AI Agents & Platforms

> Mercado de Voice AI estimado em $50B+ até 2030. Alternativas open-source começam a competir com Vapi, Bland.ai, Retell.

---

## 1. pipecat-ai/pipecat ⭐ 10.1k
**Link:** https://github.com/pipecat-ai/pipecat

**O que faz:** Framework open-source para construir AI de voz e multimodal conversacional. Suporta STT, TTS, LLM, VAD com arquitetura de pipelines modulares.

**Problema real:** Empresas pagam $0.10-0.30/minuto para plataformas como Vapi, Bland.ai, Retell para atendimento telefônico AI. Com volume, custos explodem.

**Eixos de inovação:**
- 🎯 Resolve: qualquer empresa que precisa de atendimento por voz (call centers, suporte, agendamento)
- ⚡ 5-10x mais rápido para prototipagem: pipeline modular plug-and-play
- 💸 5-10x menor custo: self-hosted, paga só APIs de STT/TTS/LLM

**TAM:** $15B+ (contact center AI market)

**Modelo de negócio:** Managed cloud (hospedagem), enterprise support, marketplace de integrações

**Esforço:** Médio — framework maduro, mas precisa de infra para escalar

**Combinações:** + Twilio/Plivo para telefonia + LiveKit para WebRTC = plataforma completa de voice AI

---

## 2. livekit/agents ⭐ 9.2k
**Link:** https://github.com/livekit/agents

**O que faz:** Framework para construir voice AI agents em tempo real com suporte a vídeo. Parte do ecossistema LiveKit (WebRTC infrastructure).

**Problema real:** Construir voice agents que funcionem em tempo real com latência <500ms é extremamente difícil. LiveKit resolve a infraestrutura.

**Eixos de inovação:**
- 🎯 Plataforma completa: do WebRTC ao agent logic
- ⚡ Latência ultra-baixa via infraestrutura WebRTC otimizada
- 🚀 Escala: já usado em produção por empresas grandes

**TAM:** $20B+ (real-time communication + AI agents)

**Modelo de negócio:** LiveKit Cloud (hosted), enterprise licensing

**Esforço:** Baixo-Médio — ecossistema maduro com exemplos e SDKs

---

## 3. akdeb/ElatoAI ⭐ 1.4k
**Link:** https://github.com/akdeb/ElatoAI

**O que faz:** Voice AI agents rodando em ESP32 (microcontrolador ~$5). Conversas de 15+ minutos com modelos multimodais. Para brinquedos, companions, dispositivos IoT.

**Problema real:** Brinquedos AI e companions são caros ($100-300) e dependem de cloud proprietário. ElatoAI roda em hardware de $5-15.

**Eixos de inovação:**
- 🎯 Problema real: mercado de AI toys/companions explodindo
- ⚡ Conversas realtime em hardware mínimo
- 🚀 Escala massiva: ESP32 custa centavos em volume
- 💎 Qualidade: suporta modelos SOTA (Gemini, OpenAI, ElevenLabs)

**TAM:** $10B+ (smart toys + AI companions + elder care devices)

**Modelo de negócio:** Kit hardware, firmware licensing, cloud companion service

**Esforço:** Médio — precisa de produto físico + supply chain

**Combinações:** + Supabase para backend + ElevenLabs para voz = produto consumer completo

---

## 4. index-tts/index-tts ⭐ 18.4k
**Link:** https://github.com/index-tts/index-tts

**O que faz:** IndexTTS2 — sistema TTS zero-shot de nível industrial desenvolvido pela Bilibili. Primeira TTS autoregressiva com controle preciso de duração de síntese + desacoplamento emoção/timbre. Suporta dois modos: duração controlada (p/ dubbing) e geração livre (prosódia natural). Fine-tune de Qwen3 para controle emocional por texto.

**Problema real:** Dubbing de vídeo profissional custa $50-200/minuto com voice actors. Ferramentas TTS existentes não controlam duração (dessincronizam com vídeo) nem emoção independentemente do timbre.

**Eixos de inovação:**
- 🎯 Dubbing automático preciso — enorme demanda de criadores YouTube, streamers, empresas de localização
- 💎 SOTA em WER, similaridade de speaker e fidelidade emocional — supera CosyVoice, XTTS
- ⚡ Controle de duração que nenhum concorrente autoregressivo oferece
- 🚀 Zero-shot: clona qualquer voz com poucos segundos de referência

**TAM:** $8B+ (localization/dubbing market) + $30B+ (content creation tools)

**Modelo de negócio:** API comercial (já tem email p/ licensing), self-hosted freemium, integração em plataformas de edição de vídeo

**Esforço:** Baixo-Médio — modelo pronto, precisa de wrapper API + UI

**Combinações:** + OpenCut (editor vídeo) + DeepSeek-OCR (legendas) = pipeline completo de localização de conteúdo automático

---

## 5. QwenLM/Qwen3-TTS ⭐ 6.5k
**Link:** https://github.com/QwenLM/Qwen3-TTS

**O que faz:** Série TTS do Alibaba/Qwen com modelos 0.6B e 1.7B. Suporta voice clone, voice design por NL (descreva a voz desejada em texto), streaming ultra-low-latency com arquitetura Dual-Track. 10 idiomas (incluindo português), múltiplos dialetos. Codebook LM end-to-end sem DiT.

**Problema real:** TTS de qualidade é dominado por ElevenLabs ($5-330/mês) e PlayHT. Modelos open-source até agora tinham latência alta ou qualidade limitada.

**Eixos de inovação:**
- 🎯 Voice design por texto natural — "voz masculina grave, confiante, sotaque brasileiro" → gera voz
- 💸 Open-source completo vs ElevenLabs: custo zero de API, roda local
- 💎 Qualidade comparável a ElevenLabs com modelo 1.7B
- 🚀 Streaming nativo com latência ultra-baixa, ideal p/ aplicações real-time

**TAM:** $5B+ (TTS market) — crescendo 15% ao ano

**Modelo de negócio:** DashScope API (Alibaba Cloud), self-hosted freemium, fine-tuning services

**Esforço:** Baixo — modelos HuggingFace prontos, Gradio UI inclusa, vLLM suportado

**Combinações:** + Pipecat (voice AI framework) + LiveKit (WebRTC) = plataforma completa de voice agents com TTS frontier

---
