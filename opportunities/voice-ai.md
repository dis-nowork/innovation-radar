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
