# 🎙️ Voice AI & Meeting Intelligence

## microsoft/VibeVoice (#203)
- **Repo:** https://github.com/microsoft/VibeVoice
- **Stars:** 22.8k | **Org:** Microsoft Research
- **Eixos:** 🎯💎⚡🚀

### O que é
Família de modelos open-source de voz frontier da Microsoft:
- **VibeVoice-ASR (7B):** Speech-to-text que processa 60min de áudio em single pass, gerando transcrições estruturadas com Who (speaker), When (timestamps) e What (conteúdo). 50+ idiomas nativos. Finetunable.
- **VibeVoice-TTS (1.5B):** Text-to-speech long-form até 90 minutos com 4 speakers distintos (código removido por uso indevido, mas weights disponíveis).
- **VibeVoice-Realtime (0.5B):** TTS streaming em tempo real com vozes multilíngues (9 idiomas + 11 estilos inglês).

### Problema real
Soluções de ASR (Google Speech, Azure STT, AWS Transcribe) cobram por minuto e não lidam bem com áudio longo. Whisper é popular mas não faz diarização nativa. VibeVoice unifica tudo: transcrição + diarização + timestamps em um modelo só.

### Por que é 5-10x melhor
- **💎 Qualidade:** Modelo 7B dedicado vs Whisper (1.5B max). Diarização nativa sem pipeline separado.
- **⚡ Velocidade:** Single-pass 60min vs chunking necessário em Whisper. vLLM inference suportado.
- **🚀 Escala:** 50+ idiomas nativos. Finetuning disponível. Inference otimizada.

### TAM
- Mercado de speech recognition: $26B em 2026
- Meeting transcription: $6B em 2026
- Contact center analytics: $15B

### Modelo de negócio
- **API as a Service:** Hosting managed do modelo (ASR + TTS) — $0.005/min vs $0.024/min do Google
- **On-premise enterprise:** Deploy privado pra hospitais, tribunais, call centers
- **SDK/White-label:** Integrar em apps de terceiros

### Esforço: Médio-Alto
Modelos pesados (7B ASR), precisa GPU. Mas finetuning disponível e vLLM suportado facilita deploy.

---

## Zackriya-Solutions/meeting-minutes (#204) — Meetily
- **Repo:** https://github.com/Zackriya-Solutions/meeting-minutes
- **Stars:** 9.6k | **License:** Open Source
- **Eixos:** 🎯💸⚡💎

### O que é
AI meeting assistant privacy-first que roda 100% local:
- Transcrição live com Parakeet/Whisper (4x mais rápido que Whisper padrão)
- Speaker diarization
- Summarization via Ollama (local) ou Claude/Groq/OpenRouter
- macOS + Windows + Linux
- Versão PRO: templates, exports PDF/DOCX, auto-detecção de meetings, GDPR compliance

### Problema real
Otter.ai ($17/mês), Fireflies ($19/mês), Fathom ($19/mês) cobram caro e enviam dados pra cloud. Empresas reguladas (saúde, jurídico, governo, defesa) não podem usar. Meetily resolve com processamento 100% local.

### Por que é 5-10x melhor
- **💸 Custo:** $0/mês vs $17-19/mês de alternativas. PRO a ~$9/mês.
- **⚡ Velocidade:** 4x mais rápido que Whisper padrão via Parakeet
- **💎 Qualidade:** Privacidade total — custo médio de breach é $4.4M (IBM 2024). Isso não tem preço.

### TAM
- Meeting transcription tools: $6B
- Enterprise meeting productivity: $15B
- Compliance-mandated local processing: crescendo 40% YoY

### Modelo de negócio
Já implementado: Community Edition (grátis forever) + PRO (templates, exports, GDPR). Enterprise (custom deploy, SSO, audit trails).

### Esforço: Baixo
Já tem produto funcional com PRO tier. Rust-based = performance. Multi-platform.

---

## fastrepl/hyprnote (#205)
- **Repo:** https://github.com/fastrepl/hyprnote
- **Stars:** 7.6k | **License:** Open Source
- **Eixos:** 🎯💸💎

### O que é
AI notepad especificamente projetado para meetings:
- Escuta áudio do sistema diretamente (sem bot entrando na call — diferencial enorme!)
- Transcrição realtime enquanto você anota memos
- Após meeting: crafts summaries personalizados baseados nos seus memos
- Roda offline com LM Studio ou Ollama
- macOS (beta), Windows/Linux Q1 2026

### Problema real
Ferramentas como Otter/Fathom adicionam um bot na call (constrangedor em reuniões sensíveis). Hyprnote captura áudio do sistema = invisível. Além disso, combina notas manuais com transcrição automática pra summaries mais úteis.

### Por que é 5-10x melhor
- **💎 Qualidade UX:** Sem bot na call! Captura áudio do OS diretamente. Combina memos humanos + AI = summaries muito mais relevantes.
- **💸 Custo:** Grátis e local-first.

### TAM
- Note-taking apps market: $2B
- Meeting productivity: $6B
- Overlap com PKM (second brain) market

### Modelo de negócio
- Freemium: app grátis + cloud sync/AI premium
- Team/Enterprise: summaries compartilhados, templates, integração CRM
- Marketplace de plugins

### Esforço: Baixo-Médio
Produto já funcional em macOS. Windows/Linux em desenvolvimento.

---

## 🔗 Combinações Poderosas

### VibeVoice + Meetily = Meeting Intelligence Platform
Usar VibeVoice-ASR como engine de transcrição dentro do Meetily = qualidade de ASR frontier + privacidade total + custo zero. Diarização nativa do VibeVoice elimina pipeline extra.

### Hyprnote + Reor (PKM) = Knowledge Worker OS
Meeting notes que alimentam automaticamente um segundo cérebro local. Tudo que você discutiu em meetings → pesquisável e conectado ao seu conhecimento.

### Meetily + Evolution API (WhatsApp) = Sales Intelligence
Transcrever calls de vendas automaticamente + enviar summaries via WhatsApp para o time. CRM intelligence grátis.
