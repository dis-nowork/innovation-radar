# On-Device AI, Quant Trading Local-First & IoT Reverso — Fev 2026

## 1. neuphonic/neutts ⭐ 4.7k
**Link:** https://github.com/neuphonic/neutts
**Licença:** Apache 2.0 (Air) / NeuTTS Open License 1.0 (Nano)

### Problema Real
TTS de qualidade está preso em APIs web caras ($15-50/M chars). Edge devices (toys, assistentes, carros) precisam de voz natural sem latência de rede nem custos de API. Players como ElevenLabs cobram $5-330/mês.

### Eixos de Inovação
- 🎯 **Problema:** TTS on-device era terrível (robótico) ou inexistente
- 💸 **Custo:** Zero custo por inferência vs $0.015-0.03/1K chars em APIs cloud
- ⚡ **Velocidade:** 45 tok/s num Galaxy A25, 19K tok/s em RTX 4090 — real-time mesmo em celular
- 💎 **Qualidade:** "Best-in-class realism for their size" — voice clone com 3 segundos de áudio
- 🚀 **Escala:** GGML quantizado roda em Raspberry Pi, celulares, laptops — bilhões de dispositivos

### TAM
- TTS market: $4.5B (2024) → $12B (2030)
- Embedded voice agents market: $8B+
- AI toys/companions: $3B+

### Modelo de Negócio
- **Open-core:** Modelo base gratuito, versões enterprise com mais idiomas/vozes
- **Hardware licensing:** Licenciar para fabricantes de toys/dispositivos IoT
- **Voice marketplace:** Marketplace de vozes clonadas/customizadas
- **API premium:** Neuphonic.com já tem API cloud como upsell

### Esforço para Produtizar: Baixo
Já está pronto para deploy. Só inglês por agora (ponto de entrada para contribuições multi-idioma).

### Combinações Poderosas
- + ElatoAI (ESP32 voice agents) = AI toys com voz natural e offline
- + Open-AutoGLM = Phone agent com voz em edge, sem cloud
- + Whisper.cpp = Pipeline STT+TTS 100% on-device

---

## 2. RohanAdwankar/oxdraw ⭐ 2.2k
**Link:** https://github.com/RohanAdwankar/oxdraw
**Licença:** MIT

### Problema Real
Diagramas gerados por AI (Mermaid) ficam feios e bagunçados. Pra ajustar layout, você precisa exportar para Lucidchart/Excalidraw — perdendo a versionabilidade do code. Nenhuma ferramenta une diagram-as-code com edição visual persistente.

### Eixos de Inovação
- 🎯 **Problema:** Gap entre diagrams-as-code (Mermaid) e tools visuais (Lucidchart)
- 💎 **Qualidade:** Posições salvas como comments no .mmd — versionável + bonito
- ⚡ **Velocidade:** AI Codemap gera diagrama de codebase inteiro automaticamente

### TAM
- Diagram tools market: $3B+ (Lucidchart, Miro, draw.io)
- Developer documentation: $1.5B
- AI-generated architecture docs: emergente

### Modelo de Negócio
- **Freemium SaaS:** Editor web hosted (free para público, paid para teams)
- **Enterprise:** Integração CI/CD (auto-gerar docs de PRs)
- **VS Code extension:** Premium com AI codemap

### Esforço para Produtizar: Médio
CLI Rust funciona, editor React beta. Precisa: multi-user collab, cloud sync, mais tipos de diagrama.

### Combinações
- + beautiful-mermaid = Output renderizado bonito
- + spec-kit/OpenSpec = Diagramas auto-gerados de specs executáveis

---

## 3. SamsungSAILMontreal/TinyRecursiveModels ⭐ 6.3k
**Link:** https://github.com/SamsungSAILMontreal/TinyRecursiveModels
**Licença:** Research

### Problema Real
Reasoning AI = modelos gigantes = custos enormes. GPT-4 custa $30/M tokens para raciocínio. Este paper prova que um modelo de 7M params atinge 45% no ARC-AGI-1 via recursão — sem LLMs massivos.

### Eixos de Inovação
- 🎯 **Problema:** Reasoning caro e centralizado
- 💸 **Custo:** 7M params vs 200B+ params — ordens de magnitude mais barato para treinar e rodar
- ⚡ **Velocidade:** Modelos tiny rodam em qualquer GPU consumer
- 💎 **Qualidade:** 45% ARC-AGI-1 com fração do custo — desafia "bigger is better"

### TAM
- Edge AI inference: $15B+ (2030)
- Embedded reasoning: Emergente (robótica, IoT, dispositivos médicos)

### Modelo de Negócio
- **Licensing:** Licenciar a abordagem recursiva para empresas de edge AI
- **Training platform:** SaaS para treinar tiny reasoning models customizados
- **Embedded SDK:** SDK para fabricantes de dispositivos

### Esforço para Produtizar: Alto
É research paper, não produto. Precisa: engenharia pesada para generalizar além de ARC-AGI, benchmarks em tarefas reais, SDK usável.

### Impacto Estratégico
Muda o paradigma de "jogar mais compute" para "usar recursão inteligente". Se a abordagem generalizar, pode democratizar AI reasoning para dispositivos edge.

---

## 4. nexmoe/VidBee ⭐ 6.1k
**Link:** https://github.com/nexmoe/VidBee
**Licença:** MIT

### Problema Real
yt-dlp é poderoso mas CLI-only. GUI alternatives são pagas ($20-40) ou buggy. Content creators que fazem curadoria de vídeos precisam de RSS auto-download para acompanhar canais sem esforço manual.

### Eixos de Inovação
- 🎯 **Problema:** Download de vídeos é complicado para não-técnicos
- 💎 **Qualidade:** UI moderna React + fila com pause/resume (vs apps feios como JDownloader)
- 💸 **Custo:** Grátis vs $20-40 de alternativas pagas (4K Video Downloader, etc)

### TAM
- Video download tools: $500M+ (apps pagos + freemium)
- Content curation: $2B+ (ferramentas de criadores)

### Modelo de Negócio
- **Freemium desktop:** Base gratuita, premium com batch processing avançado
- **Cloud service:** VidBee Cloud com downloads agendados
- **Content creator tool:** Integração com editores de vídeo

### Esforço para Produtizar: Baixo
Já funciona como app desktop. RSS auto-download é diferencial real. Precisa: auto-update, performance polish.

---

## 5. medusalix/FreeMDU ⭐ 1.0k
**Link:** https://github.com/medusalix/FreeMDU
**Licença:** GPL-3.0

### Problema Real
Miele (e outros fabricantes premium) trancam diagnóstico de appliances atrás de software proprietário + adaptadores caros ($100+). Owners pagam $150+ por visita técnica para erros simples que poderiam auto-diagnosticar.

### Eixos de Inovação
- 🎯 **Problema:** Repair monopoly de fabricantes de eletrodomésticos (direito a reparo)
- 💸 **Custo:** ESP32 €10 + firmware grátis vs adaptador proprietário €100+ software exclusivo
- 🚀 **Escala:** MQTT→Home Assistant = integra com ecossistema smart home existente

### TAM
- Smart home appliance market: $80B+
- Right-to-repair movement: crescente (legislação EU/US)
- Miele installed base: 100M+ appliances globalmente

### Modelo de Negócio
- **Hardware kit:** Vender kit diagnóstico pré-montado ($25-40)
- **SaaS diagnostic:** App mobile com interpretação de erros + guias de reparo
- **Expand to other brands:** Bosch, Siemens, Samsung (mesmo padrão IR)
- **Home automation integration:** Premium Home Assistant add-on

### Esforço para Produtizar: Médio
Protocolo reverse-engineered funciona para devices listados. Precisa: suporte a mais modelos, app mobile amigável, guias de reparo.

### Impacto Estratégico
Exemplifica o movimento right-to-repair. Se expandir para múltiplas marcas, cria plataforma horizontal de diagnóstico de appliances.

---

## 6. brokermr810/QuantDinger ⭐ 649
**Link:** https://github.com/brokermr810/QuantDinger
**Licença:** AGPL-3.0

### Problema Real
Plataformas quant (QuantConnect, Alpaca) são cloud-first = suas strategies expostas. TradingView cobra $15-60/mês. PineScript é limitado. Quem quer privacidade total sobre strategies precisa construir infra própria.

### Eixos de Inovação
- 🎯 **Problema:** Traders sérios não confiam em cloud com suas strategies
- 💸 **Custo:** Self-hosted grátis vs $15-180/mês em plataformas SaaS
- 💎 **Qualidade:** Visual Python (não PineScript limitado) + AI multi-agent research integrado
- 🚀 **Escala:** Multi-market (stocks, crypto, forex) + multi-user com PostgreSQL

### TAM
- Algorithmic trading platforms: $3B+ (2025)
- Retail quant trading: $1.5B
- AI-assisted trading tools: $800M+

### Modelo de Negócio
- **Open-core:** Base AGPL, enterprise com features premium (risk management, compliance)
- **Marketplace:** Vender/alugar strategies entre users
- **Data feeds:** Parcerias com data providers
- **Managed hosting:** "QuantDinger Cloud" para quem não quer self-host

### Esforço para Produtizar: Médio
Docker compose funciona. Precisa: polish UX, mais conectores de corretoras, documentação, compliance features.
