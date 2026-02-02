# 🤖 AI Workforce, Video Generation & IoT — Fev 2026

## 362. eigent-ai/eigent ⭐ 11.9k
**Link:** https://github.com/eigent-ai/eigent
**Categoria:** AI/Workforce Desktop | **License:** Apache-2.0 | **Lang:** TypeScript

**Problema real:** Knowledge workers gastam 40-60% do tempo em tarefas repetitivas (email, data entry, report generation, scheduling). Ferramentas como Cowork (Anthropic) custam $25-50/mês/usuário e são cloud-only. PMEs e equipes reguladas precisam de alternativa local.

**O que faz:** Desktop app open-source que permite criar, gerenciar e deployar uma "workforce" de AI agents customizados. Cada agent pode usar MCP tools, executar tasks em paralelo, e ser orquestrado por um humano via chat. Built em cima do CAMEL-AI framework.

**Eixos de inovação:**
- 🎯 **Problema real:** Automação de tarefas repetitivas sem vendor lock-in
- 💸 **5-10x menor custo:** $0 self-hosted vs $25-50/user/mês (Cowork/Cluely)
- 🚀 **5-10x mais escala:** Multi-agent paralelo, não limitado a 1 chat por vez
- 💎 **Qualidade:** SSO, access control, enterprise features que alternativas não têm

**TAM:** $15B+ (productivity software + AI assistants)
**Modelo de negócio:** Open core (community free) + Enterprise (SSO, audit logs, managed hosting)
**Esforço:** Médio — já tem UI polida, falta integrações verticais
**Combinações:** + MCP servers (#315 n8n-mcp, #118 mcp-chrome) = workforce que opera em qualquer ferramenta
**Competidores:** Cowork ($25/mês), Cluely ($280/mês), openwork (#92)

---

## 363. rednote-hilab/dots.ocr ⭐ 7.1k
**Link:** https://github.com/rednote-hilab/dots.ocr
**Categoria:** AI/Document Parsing | **License:** MIT | **Lang:** Python

**Problema real:** Document parsing requer pipelines complexos: detector de layout (YOLO) → OCR engine → table extractor → formula parser. Cada component falha de forma diferente, e a integração é frágil. ABBYY cobra $500k+/ano enterprise. AWS Textract cobra por volume.

**O que faz:** Um ÚNICO modelo VLM de 1.7B params que faz layout detection + OCR + table extraction + formula recognition + reading order, tudo com um prompt swap. SOTA no OmniDocBench em EN, ZH e multilíngue. By RedNote (Xiaohongshu — 300M+ MAU).

**Eixos de inovação:**
- 🎯 **Problema real:** Substitui pipelines multi-model por 1 modelo
- 💎 **5-10x qualidade:** SOTA em benchmarks — supera modelos 10x maiores (Gemini 2.5 Pro comparável em fórmulas)
- ⚡ **5-10x mais rápido:** 1 forward pass vs pipeline de 4-5 models sequenciais
- 💸 **Custo:** MIT, self-hostável, 1.7B roda em GPU consumer

**TAM:** $15B+ (Intelligent Document Processing — ABBYY, Kofax, AWS Textract)
**Modelo de negócio:** API managed, enterprise on-prem, integração em SaaS (contabilidade, legal, healthcare)
**Esforço:** Médio — modelo pronto, precisa wrapping (API, batch processing, webhooks)
**Combinações:** + Unstract (#94) + CocoIndex (#95) = pipeline doc intelligence completa em 1 stack
**Diferencial vs DeepSeek-OCR (#129):** dots.ocr unifica layout+OCR; DeepSeek foca em compressão óptica

---

## 364. boson-ai/higgs-audio ⭐ 7.9k
**Link:** https://github.com/boson-ai/higgs-audio
**Categoria:** Voice AI/Foundation Model | **License:** Apache-2.0 | **Lang:** Python

**Problema real:** TTS de alta qualidade com expressividade (emoções, ritmo natural, multi-speaker) requer modelos enormes e caros. ElevenLabs cobra $0.15-0.30/1k chars. Vídeo dubbing profissional custa $50-200/min.

**O que faz:** Foundation model de áudio treinado em 10M+ horas. V2.5 condensa tudo em 1B params. Gera diálogos multi-speaker, adapta prosódia automaticamente em narração, faz humming melódico com voz clonada, e gera speech com música de fundo simultaneamente. 75.7% win rate vs GPT-4o-mini-tts em "Emotions" no EmergentTTS-Eval.

**Eixos de inovação:**
- 🎯 **Problema real:** TTS expressivo é caro e bloqueado por APIs
- 💎 **5-10x qualidade:** Win rate 75% vs GPT-4o-mini-tts; capacidades emergentes (multi-speaker dialogue, music+speech, live translation)
- 🚀 **Escala:** V2.5 1B params = roda em hardware acessível, deploy at scale

**TAM:** $8B+ (TTS market + localization + content creation)
**Modelo de negócio:** API managed ($), enterprise license, integração em plataformas de criação de conteúdo
**Esforço:** Médio — requer GPU inferencing, mas Docker pronto
**Combinações:** + InfiniteTalk (#368) + OpenCut (#83) = pipeline dubbing automatizado completo

---

## 365. JerryZLiu/Dayflow ⭐ 5.7k
**Link:** https://github.com/JerryZLiu/Dayflow
**Categoria:** Produtividade/Time Tracking | **License:** MIT | **Lang:** Swift

**Problema real:** Knowledge workers não sabem onde gastam tempo. RescueTime ($12/mês) e Timing ($9/mês) são caros, cloud-dependent, e privacy-invasive. Freelancers precisam trackear horas para faturamento mas odeiam timers manuais.

**O que faz:** App macOS nativo que monitora sua tela, usa AI (Gemini/Ollama/Claude) para entender o que você está fazendo, e gera timeline do dia automaticamente. 25MB, <1% CPU, 100MB RAM. 100% local com modelos locais.

**Eixos de inovação:**
- 🎯 **Problema real:** Time tracking passivo para freelancers/profissionais
- 💸 **5-10x menor custo:** $0 vs $9-12/mês (Timing/RescueTime)
- 💎 **Qualidade:** AI summarization dá contexto, não só "tempo no Chrome"

**TAM:** $3B+ (time tracking + workforce analytics)
**Modelo de negócio:** Freemium desktop (grátis local, pago para cloud sync/teams), enterprise (workforce analytics)
**Esforço:** Baixo — já funciona como produto, falta cross-platform (Windows/Linux)
**Combinações:** + Screenpipe (#86) para capture + Dayflow para summarization = combo letal

---

## 366. francescopace/espectre ⭐ 6.2k
**Link:** https://github.com/francescopace/espectre
**Categoria:** IoT/Smart Home | **License:** GPL-3.0 | **Lang:** Python (ESPHome)

**Problema real:** Motion detection em smart homes depende de sensores PIR (limitados, ângulo estreito), câmeras (invasão de privacidade), ou sensores mmWave ($30-50/unidade). Para eldercare e segurança residencial, precisa cobrir casa inteira com múltiplos sensores caros.

**O que faz:** Transforma Wi-Fi em sensor de movimento usando Channel State Information (CSI). Um ESP32 de €10 detecta movimento analisando perturbações nos sinais Wi-Fi. Abordagem 100% matemática (sem ML), integração nativa com Home Assistant via ESPHome. Setup em 10-15 minutos.

**Eixos de inovação:**
- 🎯 **Problema real:** Home security/eldercare sem câmeras
- 💸 **5-10x menor custo:** €10 ESP32 vs $30-50/sensor mmWave (ou $200+ câmeras)
- ⚡ **5-10x mais rápido setup:** 10-15 min vs horas de instalação de câmeras
- 🚀 **Escala:** WiFi já existe em toda casa — cada roteador é potencial sensor

**TAM:** $5B+ (home security) + $15B+ (eldercare monitoring)
**Modelo de negócio:** Kit de hardware + firmware, SaaS de monitoramento (eldercare), white-label para builders
**Esforço:** Baixo — produto funciona, precisa packaging comercial
**Combinações:** + Home Assistant + ElatoAI (#70) = casa inteligente que detecta movimento por Wi-Fi e conversa por voz

---

## 367. Wan-Video/Wan2.2 ⭐ 14.0k
**Link:** https://github.com/Wan-Video/Wan2.2
**Categoria:** AI/Video Generation | **License:** Apache-2.0 | **Lang:** Python

**Problema real:** Geração de vídeo com qualidade cinematográfica requer Sora ($200/mês), Runway ($76/mês), ou Kling (pago). Nenhum modelo open-source combina estética cinematic + 720P@24fps + roda em GPU consumer.

**O que faz:** Modelos MoE de video generation com qualidade cinematográfica (Alibaba/DAMO). Wan2.2 5B model gera 720P@24fps e roda em 4090 consumer. Suporta T2V, I2V, animate (character animation), speech-to-video, e vídeos com música sincronizada. +83% mais dados de treino que v2.1.

**Eixos de inovação:**
- 🎯 **Problema real:** Vídeo cinematográfico acessível para criadores
- 💎 **5-10x qualidade:** MoE architecture + aesthetic data labeling = TOP entre modelos open E closed
- 🚀 **Escala:** 5B model em 4090 = democratiza geração de vídeo pro-level

**TAM:** $10B+ (video creation tools + advertising + entertainment)
**Modelo de negócio:** API service, SaaS de criação de vídeo, enterprise licensing
**Esforço:** Alto — requer GPU heavy, mas inference pipeline existe
**Combinações:** + InfiniteTalk (#368) para dubbing + Higgs-Audio (#364) para voz = studio de produção AI completo

---

## 368. MeiGen-AI/InfiniteTalk ⭐ 4.7k
**Link:** https://github.com/MeiGen-AI/InfiniteTalk
**Categoria:** AI/Talking Video | **License:** Apache-2.0 | **Lang:** Python

**Problema real:** Dubbing de vídeo é um processo manual que custa $50-200/minuto. Talking head videos para courses/marketing são caros (Synthesia $22-67/mês com limitações). Vídeos de duração longa perdem sincronização labial com métodos existentes.

**O que faz:** Modelo de geração de talking videos de duração ILIMITADA com lip-sync perfeito. Suporta: áudio→vídeo (dubbing), imagem→vídeo (foto vira talking head), continuação de vídeo (estende cenas). By Meituan (food delivery giant — massive video needs).

**Eixos de inovação:**
- 🎯 **Problema real:** Dubbing e talking head videos são caros/limitados
- 💎 **Qualidade:** Unlimited-length = sem degradação em vídeos longos (outros modelos falham >30s)
- ⚡ **Velocidade:** Audio-driven = resultado rápido sem iteração manual
- 🚀 **Escala:** Uma foto + áudio = vídeo; um vídeo + novo áudio = dubbing em qualquer idioma

**TAM:** $8B+ (video dubbing + localization + e-learning + marketing)
**Modelo de negócio:** API de dubbing pay-per-minute, SaaS para criadores, enterprise licensing
**Esforço:** Médio — modelo pronto, precisa wrapping e UX
**Combinações:** + Higgs-Audio (#364) para TTS + dots.ocr (#363) para transcrição de legendas = pipeline de localização de vídeo completa e automatizada
