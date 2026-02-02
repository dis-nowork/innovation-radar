# 🎬 Content Creation & AI Research Tools

## OpenCut — Editor de Vídeo Open-Source (CapCut Killer)
- **Repo:** [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) — ⭐ 45.4k | Next.js + Zustand
- **Problema real:** CapCut paywallou features básicas. Editores profissionais (Premiere, DaVinci) são complexos demais pra criadores casuais. Mercado de edição de vídeo simples ficou num limbo entre "grátis mas limitado" e "pago e complicado".
- **Eixos:** 🎯💸🚀
  - 🎯 Criadores de conteúdo (TikTok, YouTube Shorts, Reels) = centenas de milhões de usuários
  - 💸 100% grátis vs CapCut Pro ($8-10/mês) e similares
  - 🚀 Web + desktop + mobile = alcance massivo
- **TAM:** Mercado de video editing software: $4.2B (2024) → $7.6B (2030). Segmento "prosumer" é o que mais cresce
- **Modelo de negócio:** Freemium (templates premium, cloud rendering, assets), marketplace de plugins, cloud storage
- **Esforço:** Médio — funcional mas ainda em desenvolvimento ativo. Timeline multi-track já existe. Faltam efeitos avançados, transições AI
- **Combinações:** + Chatterbox TTS (narração automática) + Whisper (legendas auto) = pipeline completa de criação de conteúdo

---

## Chatterbox TTS — Text-to-Speech Estado da Arte
- **Repo:** [resemble-ai/chatterbox](https://github.com/resemble-ai/chatterbox) — ⭐ 22.1k | Python
- **Problema real:** ElevenLabs custa $5-99/mês. Serviços de TTS comerciais cobram por caractere. Criadores, devs e empresas precisam de voz sintética de qualidade sem custos recorrentes altos.
- **Eixos:** 💸💎⚡
  - 💸 Custo zero (self-hosted) vs $5-99/mês de ElevenLabs/WellSaid
  - 💎 SoTA quality — zero-shot cloning, 23+ idiomas, tags paralinguísticas ([laugh], [cough])
  - ⚡ Turbo model (350M params): baixa latência, ideal pra voice agents em produção
- **TAM:** Mercado de TTS: $5.0B (2024) → $12.4B (2030). Voice AI agents é o segmento mais quente
- **Modelo de negócio:** Open-core (modelo grátis + API managed com SLA/latência garantida), enterprise licensing
- **Esforço:** Baixo — pip install, modelos pré-treinados no HuggingFace, API simples
- **Combinações:** + LiveKit/Pipecat (voice agents) + OpenCut (narração automática) + Open Notebook (podcasts AI)

---

## Strix — AI Hacker Autônomo para Security Testing
- **Repo:** [usestrix/strix](https://github.com/usestrix/strix) — ⭐ 19.6k | Python + Docker
- **Problema real:** Pentest manual custa $10-50k por engagement. SAST/DAST tradicionais têm >50% de falsos positivos. Empresas (especialmente startups) ficam vulneráveis por não poder pagar security testing frequente.
- **Eixos:** 🎯💸⚡🚀
  - 🎯 Toda empresa com webapp precisa de security testing — mercado universal
  - 💸 Self-hosted vs $10-50k por pentest manual ou $500-2000/mês de ferramentas comerciais
  - ⚡ Horas vs semanas de pentest manual. Validação real com PoCs, não falsos positivos
  - 🚀 CI/CD integration = security em cada PR, não 1x por quarter
- **TAM:** Mercado de application security: $10.3B (2024) → $25B+ (2030)
- **Modelo de negócio:** Open-core (CLI grátis + managed cloud com dashboards, compliance reports, team features), per-scan pricing
- **Esforço:** Baixo/Médio — Docker + API key de LLM. Resultados imediatos. Enterprise precisa de integração com compliance frameworks
- **Combinações:** + CI/CD (GitHub Actions nativo) + Serena (code understanding) = security scanning que entende contexto semântico do código

---

## Open Notebook — NotebookLM Open-Source com Multi-Model
- **Repo:** [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) — ⭐ 19.1k | Python + Next.js + SurrealDB
- **Problema real:** Google NotebookLM é cloud-only, Google-models-only, sem API, sem customização. Pesquisadores, estudantes e empresas querem pesquisa AI com dados privados.
- **Eixos:** 🎯💸💎
  - 🎯 Qualquer pessoa que faz pesquisa (acadêmicos, analistas, estudantes, jornalistas)
  - 💸 Paga só custo de AI (ou roda local com Ollama = grátis) vs NotebookLM Plus ($7.99/mês)
  - 💎 16+ providers, 1-4 speakers em podcasts (vs 2 no Google), REST API completa, customizável
- **TAM:** Mercado de knowledge management: $7.5B (2024), research tools + education = mercado enorme
- **Modelo de negócio:** Self-hosted grátis, managed cloud (hosting + indexação), enterprise (SSO, audit logs, compliance)
- **Esforço:** Médio — Docker compose funcional. UI já boa. Precisa melhorar citations e UX para não-técnicos
- **Combinações:** + Chatterbox TTS (vozes customizadas nos podcasts) + DeepResearch agents (pesquisa automatizada)

---

## Microsoft VibeVoice — Voice AI Frontier Open-Source
- **Repo:** [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) — ⭐ 22.7k | Python
- **Problema real:** ASR (speech-to-text) comercial cobra por minuto e tem limites de duração. Empresas com muitas horas de áudio (call centers, podcasts, legal) gastam fortunas em transcrição.
- **Eixos:** 💸💎📈
  - 💸 Open-source vs serviços de transcrição ($0.01-0.05/min = $600-3000 por 1000h)
  - 💎 60 minutos de áudio em um único passe, com identificação de speaker + timestamps. 50+ idiomas
  - 📈 Volume massivo de processamento sem limites de API
- **TAM:** Mercado de speech recognition: $12.9B (2024) → $35B+ (2030)
- **Modelo de negócio:** Open-source (modelo livre) + managed API da Microsoft para escala. Oportunidade: wrap em SaaS vertical (transcrição legal, médica, media)
- **Esforço:** Médio — requer GPU. Fine-tuning code disponível. Integração com vLLM para inferência rápida
- **Combinações:** + Open Notebook (pesquisa em áudio/vídeo) + Strix (transcrição de meetings de security review)

---

## Dyad — AI App Builder Local (Lovable/v0/Bolt Killer)
- **Repo:** [dyad-sh/dyad](https://github.com/dyad-sh/dyad) — ⭐ 19.5k | TypeScript/Electron
- **Problema real:** Lovable, v0, Bolt são cloud-only e cobram $20-100/mês. Privacidade é zero (seu código vai pro servidor deles). Power users querem controle total.
- **Eixos:** 🎯💸
  - 🎯 Devs e power users que querem gerar apps com AI mas sem lock-in ou custos de plataforma
  - 💸 Grátis (usa suas próprias API keys) vs $20-100/mês de Lovable/Replit
- **TAM:** Mercado de low-code/no-code: $32B (2024), AI app builders é a fronteira mais quente
- **Modelo de negócio:** Open-core (Apache 2.0 base + FSL pro features), templates marketplace, enterprise
- **Esforço:** Baixo — download e usar. Cross-platform (Mac, Windows)
- **Combinações:** + OpenCut (gerar apps de edição de vídeo) + Strix (security scan dos apps gerados)
