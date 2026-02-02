# 🎬 Creative Tools — Video & Media

## OpenCut-app/OpenCut ⭐ 45.4k
**Link:** https://github.com/OpenCut-app/OpenCut
**Forks:** ~alto (projeto viral)
**Criado:** 2025

### Problema Real
CapCut (ByteDance) se tornou o editor de vídeo dominante para criadores de conteúdo, mas está progressivamente colocando features básicas atrás de paywall. Criadores de conteúdo pequenos/médios (dezenas de milhões) precisam de um editor simples, gratuito e sem marca d'água.

### Eixos de Inovação
- 🎯 **Problema real:** Paywalls crescentes em CapCut + preocupações de privacidade (dados indo para ByteDance)
- 💸 **5-10x menor custo:** Gratuito vs CapCut Pro ($7.99/mês), Adobe Premiere ($22.99/mês)
- 🚀 **5-10x mais escala:** Web + desktop + mobile, nenhum outro editor open-source cobre todas as plataformas
- 💎 **Qualidade:** Timeline multi-track, preview real-time, sem watermarks

### TAM
- Mercado de edição de vídeo: ~$4.7B em 2025, crescendo 14% ao ano
- CapCut: 200M+ usuários — capturar 1% = 2M usuários

### Modelo de Negócio
- **Freemium:** Editor gratuito + efeitos/templates premium
- **Enterprise/White-label:** Empresas querendo editor embutido
- **Marketplace:** Templates, transições, efeitos vendidos por criadores
- **Cloud rendering:** Processing pesado na nuvem como upsell

### Esforço para Produtizar: Médio
Stack moderna (Next.js + Zustand), mas edição de vídeo no browser tem limitações de performance. Precisa de investimento em codec/rendering.

### Combinações
- **+ index-tts ou Qwen3-TTS:** Auto-narração de vídeos
- **+ banana-slides:** Pipeline completo: slides → vídeo → edição
- **+ Handy (STT):** Legendas automáticas offline

---

## chatfire-AI/huobao-drama ⭐ 6.9k
**Link:** https://github.com/chatfire-AI/huobao-drama
**Forks:** 1,272 | **License:** CC BY-NC-SA 4.0
**Criado:** Jan 2026 | **Stack:** Go + Vue3

### Problema Real
Short dramas/curtas são o conteúdo de maior crescimento em plataformas (TikTok, Reels, Kuaishou). Produzir um curta-metragem exige roteirista + designer + animator + editor — semanas de trabalho e milhares de dólares. Creators individuais e pequenas agências de marketing ficam de fora.

### Eixos de Inovação
- 🎯 **Problema real:** Produção de vídeo narrativo é cara e lenta. Agências cobram $5-50k por curta.
- ⚡ **5-10x mais rápido:** Uma frase → roteiro + personagens + storyboard + vídeo final. Minutos vs semanas.
- 💸 **5-10x menor custo:** Self-hosted, paga só API do LLM + modelo de imagem/vídeo.
- 🚀 **5-10x mais escala:** Permite produção em massa de conteúdo narrativo. Uma pessoa faz o que um estúdio faz.

### TAM
- Short-form video market: $100B+ (TikTok alone ~$20B receita/ano)
- AI video generation: $2B+ em 2025, crescendo 35%/ano
- Mercado de marketing content: $400B+ global

### Modelo de Negócio
- **SaaS cloud:** $29-199/mês por volume de produção
- **Enterprise/White-label:** Agências de marketing embutem na própria plataforma
- **Marketplace:** Templates de estilos visuais e gêneros de drama
- **API:** Pay-per-video para integrações

### Esforço para Produtizar: Médio
Arquitetura DDD bem feita (Go backend, Vue3 frontend). Precisa de UX polish e mais modelos de vídeo. A licença CC BY-NC-SA limita uso comercial direto — precisaria licença dual ou fork.

### Combinações
- **+ OpenCut:** Edição pós-produção do vídeo gerado
- **+ Qwen3-TTS:** Narração AI nos idiomas locais
- **+ chandra (OCR):** Importar roteiros físicos/impressos e gerar drama direto
