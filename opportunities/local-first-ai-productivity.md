# 🏠 Local-First AI Productivity Stack

> Tema: A convergência entre privacidade, AI e produtividade pessoal/profissional.
> O movimento "local-first" está amadurecendo de filosofia para stack produtivo real.

---

## #406 — Zackriya-Solutions/meeting-minutes (Meetily)
- **GitHub:** https://github.com/Zackriya-Solutions/meeting-minutes
- **Stars:** 9.6k ⭐ | **Forks:** 831 | **Linguagem:** Rust | **Licença:** MIT
- **O que faz:** Meeting assistant 100% local — transcrição em tempo real (Parakeet/Whisper), speaker diarization, sumarização via Ollama. Nenhum dado sai da máquina.
- **Problema real:** Meeting AI tools (Otter.ai, Fireflies, Fathom) custam $15-30/mês/seat e enviam TUDO para cloud. GDPR/LGPD tornam isso tóxico para empresas reguladas. Custo médio de data breach: $4.4M (IBM 2024). Advogados, consultores de defesa, médicos não podem usar cloud meeting tools.
- **Eixos de inovação:**
  - 🎯 Problema real: compliance officers e profissionais regulados PRECISAM de meeting notes mas NÃO PODEM usar cloud
  - 💸 5-10x menor custo: zero custo operacional vs $15-30/seat/mês (Otter, Fireflies)
  - 💎 Qualidade: Parakeet TDT é 4x mais rápido que Whisper, speaker diarization nativo
- **TAM:** $5.2B (mercado de meeting intelligence, Grand View Research). Enterprise compliance segment é ~30% = ~$1.5B
- **Modelo de negócio:** Freemium — Community (MIT, local) + Meetily PRO (templates, GDPR compliance tools, exports, auto-detection). Enterprise: deployment on-prem com SSO + audit trails.
- **Esforço pra produtizar:** Baixo — já tem versão PRO vendendo, downloads pra macOS/Windows
- **Combinações:** + Rowboat (#411) para transformar meeting notes em knowledge graph automático. + Hyprnote (#407) como frontend complementar.

---

## #407 — fastrepl/hyprnote
- **GitHub:** https://github.com/fastrepl/hyprnote
- **Stars:** 7.6k ⭐ | **Forks:** 515 | **Linguagem:** TypeScript | **Licença:** GPL-3.0
- **O que faz:** AI notepad especificamente para meetings. Captura áudio in/out do computador (sem bot na call), transcreve em tempo real, gera summaries baseados nos seus memos. Roda offline com Ollama/LM Studio.
- **Problema real:** Ninguém quer um bot entrando na call ("Otter.ai is recording"). É constrangedor, assusta clientes, e em muitas empresas é proibido. Hyprnote escuta diretamente o áudio do sistema — invisível.
- **Eixos de inovação:**
  - 🎯 Problema real: o constrangimento do bot na call é uma barreira ENORME de adoção
  - 💎 5-10x qualidade UX: não é transcritor passivo, é notepad ativo onde você anota o importante e AI completa o resto
  - 💸 Custo: local processing, zero API costs
- **TAM:** Same $5.2B meeting intelligence, mas com approach que destranca o segmento "people who refuse bots" (~40% do mercado)
- **Modelo de negócio:** Freemium desktop app + Pro features (templates, integrations, cloud sync opcional). Enterprise: managed deployment.
- **Esforço pra produtizar:** Médio — macOS beta, Windows/Linux Q1 2026. Precisa polimento, mas UX já é forte.
- **Combinações:** Complementar ao Meetily (#406) — Meetily é o engine, Hyprnote é o UX layer. Juntos = meeting AI perfeito.

---

## #408 — elie222/inbox-zero
- **GitHub:** https://github.com/elie222/inbox-zero
- **Stars:** 10.0k ⭐ | **Forks:** 1,190 | **Linguagem:** TypeScript | **Licença:** Custom (AGPL-like)
- **O que faz:** AI email assistant que organiza inbox, pre-drafta replies no seu tom, categoriza senders, bulk unsubscribe, cold email blocker, meeting briefs, auto-filing de attachments.
- **Problema real:** Profissionais gastam 28% do dia gerenciando email (McKinsey). Soluções como Fyxer ($12/mês) e SaneBox ($7/mês) são caras e limitadas. Inbox Zero é open-source com AI rules em plain English ("if recruiter email, archive and label").
- **Eixos de inovação:**
  - 🎯 Problema real: email overload afeta literalmente BILHÕES de trabalhadores
  - 💸 5-10x menor custo: self-hostable vs $7-12/mês de alternatives comerciais
  - 🚀 Escala: "Cursor Rules for email" — plain English rules escalam pra qualquer workflow
- **TAM:** $2.8B (email management market). Addressable: knowledge workers = 1.2B pessoas
- **Modelo de negócio:** Hosted SaaS (getinboxzero.com) com freemium + paid tiers. Self-hosted para enterprises.
- **Esforço pra produtizar:** Baixo — já é produto rodando, Next.js + Prisma, deploy via Vercel
- **Combinações:** + Rowboat (#411) para ter contexto de email em meetings. + Twenty CRM (#5) para auto-log de comunicação com leads.

---

## #409 — blinkospace/blinko
- **GitHub:** https://github.com/blinkospace/blinko
- **Stars:** 9.3k ⭐ | **Forks:** 655 | **Linguagem:** TypeScript | **Licença:** GPL-3.0
- **O que faz:** Self-hosted personal AI note tool. Quick capture (tipo Flomo), rich text, AI-powered search e organização, RAG sobre suas notas, multimodal (imagens, arquivos). Deploy com Docker em 1 comando.
- **Problema real:** Obsidian não tem AI nativo. Notion é cloud-first e cobra $8-10/mês. Apple Notes é limitado. Nenhuma ferramenta de notas combina: (1) self-hosted, (2) AI nativo, (3) quick capture, (4) rich text. Blinko faz as 4.
- **Eixos de inovação:**
  - 🎯 Problema real: profissionais precisam de notas com AI sem entregar dados para Big Tech
  - 💸 5-10x menor custo: self-hosted vs Notion ($8-10/seat/mês)
  - 💎 Qualidade: quick capture + AI search + RAG é UX superior a qualquer note app existente
- **TAM:** $1.4B (note-taking apps market). Segment "AI-enhanced PKM" crescendo 40%+ ao ano.
- **Modelo de negócio:** Self-hosted open-source + hosted premium tier. Enterprise: SSO + team features.
- **Esforço pra produtizar:** Baixo — Docker deploy funcional, UI polida, comunidade ativa
- **Combinações:** + Hyprnote (#407) para meeting notes auto-flowing para Blinko. + Reor (#27) como alternativa Obsidian-like.

---

## #410 — colanode/colanode
- **GitHub:** https://github.com/colanode/colanode
- **Stars:** 4.6k ⭐ | **Forks:** 260 | **Linguagem:** TypeScript | **Licença:** Apache-2.0
- **O que faz:** Workspace local-first que combina Slack (chat real-time) + Notion (pages/wikis/databases) + Google Drive (file management). CRDTs via Yjs para edição colaborativa. Self-hosted, SQLite local, sync em background.
- **Problema real:** Empresas pagam $15-25/user/mês por Slack + Notion + Drive separados. São 3 apps, 3 logins, dados fragmentados. Para SMBs isso é $500-5000/mês. Colanode unifica tudo com dados locais.
- **Eixos de inovação:**
  - 🎯 Problema real: fragmentação de ferramentas de colaboração é dor universal
  - 💸 5-10x menor custo: self-hosted vs $15-25/user/mês (Slack $7 + Notion $8 + Drive $6)
  - 🚀 Escala: de "3 apps separados" para "1 plataforma" — simplificação massiva
- **TAM:** $15.5B (collaboration tools market, incluindo Slack $1.5B, Notion ~$1B, cloud storage ~$13B)
- **Modelo de negócio:** Hosted app (app.colanode.com) freemium + self-hosted. Enterprise: SSO, compliance, audit, SLA.
- **Esforço pra produtizar:** Médio-Alto — ambicioso (3 produtos em 1), mas foundation sólida com CRDTs. Precisa de AI features pra se diferenciar.
- **Combinações:** + Meetily (#406) para meeting transcripts no workspace. + Inbox Zero (#408) para email no mesmo lugar. = "Digital HQ" all-in-one local-first.

---

## #411 — rowboatlabs/rowboat
- **GitHub:** https://github.com/rowboatlabs/rowboat
- **Stars:** 4.3k ⭐ | **Forks:** 371 | **Linguagem:** TypeScript | **Licença:** Apache-2.0
- **O que faz:** AI coworker local-first que ingere email (Gmail) e meeting notes (Granola, Fireflies), organiza em vault Obsidian-compatible de Markdown com backlinks, e usa esse knowledge graph para draftar emails, preparar meetings, organizar arquivos, e executar ações.
- **Problema real:** AI assistants atuais (ChatGPT, Claude) NÃO TÊM memória persistente do seu trabalho. Cada sessão começa do zero. Rowboat mantém "long-lived knowledge" — contexto que se acumula e compõe ao longo do tempo, não "retrieval that starts cold every time".
- **Eixos de inovação:**
  - 🎯 Problema real: AI sem memória é uma ferramenta; AI com memória é um coworker
  - 💎 5-10x qualidade: knowledge compounds over time vs cold retrieval. Notas são plain Markdown, editáveis, inspecionáveis
  - 🚀 Escala: de "AI que responde perguntas" para "AI que conhece seu trabalho e age proativamente"
- **TAM:** $6.8B (AI personal assistant market, crescendo 30%+ ao ano)
- **Modelo de negócio:** Desktop app freemium + premium (mais integrações, team features). Enterprise: shared organizational memory.
- **Esforço pra produtizar:** Médio — macOS app funcional, precisa Windows/Linux. Core é sólido (Obsidian vault = portabilidade infinita).
- **Combinações:** + Meetily (#406) como source de meeting notes. + Inbox Zero (#408) como source de email intelligence. + Blinko (#409) como note capture layer. = **"AI Chief of Staff" que conhece tudo do seu trabalho**.

---

### [run-llama/notebookllama](https://github.com/run-llama/notebookllama) ⭐ 1.8k | 🎯💸💎

**O que é:** Alternativa open-source ao Google NotebookLM. Upload docs, faz perguntas com citações. Backed by LlamaCloud. By LlamaIndex team.

**Problema real:** NotebookLM é proprietário do Google, dados vão pro Google, sem customização, e pode ser descontinuado a qualquer momento. Researchers e empresas querem RAG notebook privado.

**Eixos de inovação:**
- 🎯 **Problema real:** NotebookLM lock-in — seus documentos no Google sem portabilidade
- 💸 **Custo:** Self-hostable, use seu próprio LLM (Ollama), $0 vs Google lock-in
- 💎 **Qualidade:** LlamaIndex RAG pipeline é state-of-art, citações com source grounding

**TAM:** Knowledge management software = $645B by 2030. NotebookLM segment (research + learning) = $5-10B

**Modelo de negócio:**
- Open-core: self-host grátis, LlamaCloud managed = paid tier
- Enterprise: SSO, audit, compliance, fine-tuned models
- API: embed notebook-as-a-service em outros produtos

**Esforço para produtizar:** Baixo — by LlamaIndex (empresa established), já tem produto managed

---

### [RICHQAQ/PasteMD](https://github.com/RICHQAQ/PasteMD) ⭐ 3.9k | 🎯💎⚡

**O que é:** Tray app que resolve o problema #1 de quem usa AI: copiar respostas do ChatGPT/DeepSeek para Word/Excel sem quebrar formatação. Markdown→DOCX via Pandoc, one-click paste.

**Problema real:** TODO MUNDO que usa AI para trabalho sofre isso. Fórmulas LaTeX viram lixo, tabelas quebram, headers somem. Afeta milhões de knowledge workers diariamente.

**Eixos de inovação:**
- 🎯 **Problema real:** Friction #1 entre AI output e ferramentas de trabalho (Word/Excel/WPS)
- 💎 **Qualidade:** Smart detection (HTML, Markdown, LaTeX), auto-fix de fórmulas, app extensions por janela
- ⚡ **Velocidade:** One-click vs reformatar manualmente (5-30min por documento)

**TAM:** ~1B knowledge workers usando AI × $5-10/ano tool = $5-10B

**Modelo de negócio:**
- Freemium: paste básico grátis, templates/batch/enterprise = paid
- OEM: integrar em AI chatbots como feature (Jasper, Copy.ai)
- Enterprise: policy controls, approved formatting

**Esforço para produtizar:** Baixo — já funciona, precisa apenas SaaS wrapper e cross-platform (atualmente Windows-focused)

**Combinações:**
- + BentoPDF → pipeline AI→formatação→PDF completo
- + Obsidian/Notion plugins → markdown-first workflow

