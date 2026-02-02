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
