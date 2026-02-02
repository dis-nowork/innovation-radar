# Edge AI, Creative Tools & Local-First Collaboration
> Rodada: 2026-02-02 | Tema: TTS ultra-leve, video editing AI-native, sandboxing de agents, knowledge bases locais, SDKs de sync

---

## 424. ekwek1/soprano ⭐1.2k
**Link:** https://github.com/ekwek1/soprano
**Categoria:** Voice AI / TTS
**Problema real:** TTS de qualidade requer modelos enormes (1B+ params) e GPUs caras. Edge/mobile ficam de fora.
**Solução:** Modelo de 80M params que entrega qualidade competitiva com 20x realtime em CPU e 2000x em GPU. Streaming lossless, OpenAI-compatible API.
**Eixos de inovação:**
- ⚡ **Velocidade:** 2000x realtime em GPU é absurdo — ordens de magnitude acima de F5-TTS, Bark, etc.
- 💸 **Custo:** 80M params roda em hardware consumer. Substitui ElevenLabs ($22-$99/mês) por self-hosted zero-cost
- 💎 **Qualidade:** "95% fewer hallucinations" no v1.1, qualidade comparável a modelos 10-100x maiores
- 🚀 **Escala:** De nicho GPU → qualquer device. Edge/IoT/mobile viável
**TAM:** Mercado TTS ~$5B (2025), crescendo 15%/ano. Cada app com voz é cliente potencial.
**Modelo de negócio:** Cloud TTS API (Soprano-as-a-Service), Enterprise fine-tuning support, premium voices marketplace
**Esforço:** Baixo — já tem WebUI, CLI, OpenAI-compatible endpoint, fine-tuning toolkit
**Combinações:** + lue (eBook→audiobook), + meeting notes (transcrição→narração), + chatbots (voz ultra-rápida)

---

## 425. gausian-AI/Gausian_native_editor ⭐1.1k
**Link:** https://github.com/gausian-AI/Gausian_native_editor
**Categoria:** Creative Tools / Video
**Problema real:** Editors de vídeo AI (CapCut, Runway) são cloud-locked e caros. DaVinci Resolve é pesado. Não existe editor nativo leve focado em workflow AI-first.
**Solução:** Editor nativo em Rust com WGPU preview, integração ComfyUI local, timeline editing, export pro (FCPXML/EDL), screenplay helpers com LLM.
**Eixos de inovação:**
- 🎯 **Problema real:** Criadores de conteúdo AI precisam de editor que entenda o workflow: gerar→editar→exportar
- 💎 **Qualidade:** Rust + WGPU = performance nativa, preview GPU-acelerado
- ⚡ **Velocidade:** Proxy gen (ProRes/NVENC/VAAPI), hardware decode, startup rápido vs Electron-based
**TAM:** Mercado de video editing ~$4B. AI video creators é o segmento de maior crescimento.
**Modelo de negócio:** Freemium (features pro: multi-track audio, advanced effects), plugin marketplace, enterprise
**Esforço:** Médio — funcional mas early-stage. Precisa polish de UX e mais efeitos
**Combinações:** + ComfyUI workflows customizados, + soprano (narração TTS integrada), + huobao-drama (pipeline end-to-end)

---

## 426. boxlite-ai/boxlite ⭐894
**Link:** https://github.com/boxlite-ai/boxlite
**Categoria:** AI / Agent Infrastructure
**Problema real:** AI agents precisam executar código untrusted. Docker não isola de verdade (shared kernel). VMs tradicionais são pesadas demais. E2B/Modal são cloud-only e caros.
**Solução:** Micro-VMs embeddable com kernel próprio por Box, OCI-compatible, sem daemon, sem root, async-first, SDKs em Python/Node/Rust.
**Eixos de inovação:**
- 🎯 **Problema real:** Todo agent framework precisa de sandbox. É infra fundamental.
- 💎 **Qualidade:** Hardware-level isolation (próprio kernel) vs Docker (namespace apenas)
- ⚡ **Velocidade:** Lightweight, fast-starting, high concurrency
- 🚀 **Escala:** Embeddable como library — qualquer app vira multi-tenant code execution
**TAM:** Agent infra é mercado ~$10B+. Todo coding agent, CI/CD, e plataforma no-code precisa disso.
**Modelo de negócio:** Open core + managed BoxLite Cloud, enterprise support, agent platform partnerships
**Esforço:** Médio — SDKs funcionais, precisa scaling stories e managed offering
**Combinações:** + qualquer agent framework (LangGraph, CrewAI), + coding agents (Claude Code, Codex), + multi-tenant SaaS

---

## 427. MrSibe/KnowNote ⭐865
**Link:** https://github.com/MrSibe/KnowNote
**Categoria:** Local-First AI / Knowledge
**Problema real:** NotebookLM do Google é poderoso mas cloud-locked, sem controle de LLM, dados vão pro Google. Alternativas open-source pedem Docker.
**Solução:** Desktop app Electron que faz o que NotebookLM faz — upload docs, build knowledge base, Q&A com citações — mas 100% local, sem Docker, multi-provider LLM.
**Eixos de inovação:**
- 🎯 **Problema real:** Estudantes/pesquisadores querem NotebookLM sem entregar dados ao Google
- 💸 **Custo:** Free + usa LLMs que você já tem (Ollama local = $0)
- 💎 **Qualidade:** RAG com sqlite-vec, citações precisas, suporta PDF/DOCX/PPTX/web pages
**TAM:** EdTech/knowledge management ~$8B. Qualquer estudante, pesquisador, profissional de conhecimento.
**Modelo de negócio:** Freemium desktop, premium features (team sync, advanced analytics), enterprise (compliance/on-prem)
**Esforço:** Baixo-Médio — app funcional, precisa polish e features avançadas (collaboration, podcasts)
**Combinações:** + soprano (podcast generation como NotebookLM), + Ollama (full offline), + synckit (collaboration)

---

## 428. Dancode-188/synckit ⭐627
**Link:** https://github.com/Dancode-188/synckit
**Categoria:** DevTools / Collaboration
**Problema real:** Adicionar colaboração real-time a apps é projeto de meses. CRDTs são complexos. Liveblocks/Yjs requerem setup significativo. Liveblocks cobra $2K+/mês.
**Solução:** SDK batteries-included: 3 linhas de código para sync, rich text com CRDTs (Peritext+Fugue), undo/redo, cursors, presence. React/Vue/Svelte. 154KB.
**Eixos de inovação:**
- 🎯 **Problema real:** Devs querem collab features sem virar especialistas em CRDTs
- 💸 **Custo:** Open source vs Liveblocks $99-$2K+/mês
- 🚀 **Escala:** Qualquer app web vira colaborativo. De single-user para multi-user em horas
- 💎 **Qualidade:** Peritext+Fugue são state-of-art em CRDTs para rich text
**TAM:** Real-time collaboration SDK ~$2B. Todo SaaS com editing precisa disso.
**Modelo de negócio:** Open core + managed sync servers, enterprise (on-prem, SLA, SSO), premium adapters
**Esforço:** Médio — SDK funcional, precisa managed infra e enterprise features
**Combinações:** + KnowNote (knowledge base colaborativa), + qualquer editor (code, docs, design)

---

## 429. superstarryeyes/lue ⭐669
**Link:** https://github.com/superstarryeyes/lue
**Categoria:** Produtividade / Reading
**Problema real:** Audiobooks custam $15-20 cada (Audible). TTS readers existentes soam robóticos. Kindle/Kobo têm TTS ruim.
**Solução:** eBook reader terminal com TTS audiobook-quality (Edge TTS + Kokoro local), word highlighting sincronizado, multi-formato (EPUB/PDF/DOCX/HTML/RTF/TXT/MD), speed control, smart persistence.
**Eixos de inovação:**
- 🎯 **Problema real:** Pessoas querem consumir livros em áudio sem pagar Audible preço por livro
- 💸 **Custo:** $0 vs $15/audiobook no Audible ($180/ano no plano)
- 💎 **Qualidade:** Word-level highlighting sync com voz é UX de primeiro mundo
**TAM:** Audiobook market ~$7B (2025), ebook ~$15B. Intersection é enorme.
**Modelo de negócio:** Premium voices, mobile app, library management, premium UI themes
**Esforço:** Baixo — funcional, precisa app mobile/desktop GUI (Electron/Tauri) para mass adoption
**Combinações:** + soprano (TTS local ultra-rápido), + KnowNote (study tool integrado)
