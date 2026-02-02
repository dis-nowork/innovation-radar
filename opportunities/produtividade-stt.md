# 🎙️ Produtividade — Speech-to-Text

## cjpais/Handy ⭐ 13.8k
**Link:** https://github.com/cjpais/Handy
**Stack:** Tauri (Rust + React/TypeScript)

### Problema Real
Ditado por voz em desktop é dominado por soluções cloud (Dragon $15/mês, Google/Apple built-in mas mediocres, Whisper CLI = terminal only). Não existe um app desktop bonito, offline-first, open-source para speech-to-text universal.

### Eixos de Inovação
- 🎯 **Problema real:** Acessibilidade — pessoas com lesões, RSI, dislexia precisam de STT confiável
- 💸 **5-10x custo:** Gratuito vs Dragon ($15/mês), Otter.ai ($10/mês)
- 💎 **5-10x qualidade:** Whisper Turbo/Large + Parakeet V3, GPU acceleration, VAD filtering

### TAM
- Speech recognition market: ~$12B em 2025
- Desktop STT: subconjunto significativo — profissionais, escritores, developers, acessibilidade

### Modelo de Negócio
- **Premium models:** Modelos especializados (médico, jurídico, técnico) como download pago
- **Enterprise:** Vocabulário customizado, compliance, integração com EMR/EHR
- **Plugin marketplace:** Extensões (auto-formatting, tradução, ações por comando de voz)
- **Mobile companion:** App mobile sincronizado com desktop

### Esforço para Produtizar: Baixo-Médio
App funcional com instaladores para Win/Mac/Linux. Falta: vocabulário custom, plugin system, mobile.

### Combinações
- **+ OpenCut:** STT → legendas automáticas em vídeos
- **+ hyprnote:** STT desktop + STT reuniões = produtividade completa
- **+ VibeVoice:** Pipeline bidirecional: voz→texto→voz
