# 🛡️ Digital Sovereignty — Controle de Volta ao Usuário

> Repos que devolvem ao usuário controle sobre dados, mídia, e infraestrutura que hoje dependem de plataformas caras/invasivas.

---

## 83. OpenCut-app/OpenCut ⭐ 45.4k
**O que faz:** Editor de vídeo open-source para web, desktop e mobile. Alternativa direta ao CapCut.

**Problema real:** CapCut (ByteDance/TikTok) paywalled features básicas, força watermarks, e coleta dados massivamente. Criadores de conteúdo pequenos pagam $8-15/mês por funcionalidades simples. DaVinci Resolve é poderoso mas complexo demais pra edições rápidas.

**Eixos de inovação:**
- 🎯 **Problema:** 200M+ usuários de CapCut presos em paywall crescente
- 💸 **Custo:** $0 vs $8-15/mês (CapCut Pro) ou $300+ (Premiere)
- 🚀 **Escala:** Web-first = zero install, funciona em qualquer dispositivo

**TAM:** Mercado de edição de vídeo $4.2B (2025), crescendo 14% ao ano. Segmento "prosumer/creator" é ~$1.5B.

**Modelo de negócio:**
- Freemium: features avançadas (AI, templates, cloud storage)
- Enterprise: white-label para plataformas de mídia
- Marketplace: templates, efeitos, transições pagas

**Esforço pra produtizar:** Médio — timeline funciona, precisa polish em UX e features avançadas (color grading, audio mixing). Next.js + Zustand = stack moderna.

**Criado:** Jun 2025 → 45k stars em 7 meses = crescimento explosivo

---

## 84. resemble-ai/chatterbox ⭐ 22.1k
**O que faz:** Família de modelos TTS state-of-the-art open-source. Turbo (350M params), Multilingual (23+ idiomas), com paralinguistic tags ([laugh], [cough]).

**Problema real:** ElevenLabs cobra $5-99/mês. Voices.ai, Play.ht — todos SaaS caros. Devs de voice agents precisam de TTS de qualidade mas custo escala rápido ($0.15-0.30/1k chars).

**Eixos de inovação:**
- 💸 **Custo:** Self-hosted = $0 por char vs $0.15-0.30/1k chars (ElevenLabs)
- 💎 **Qualidade:** SoTA benchmarks, zero-shot voice cloning com 10s de áudio
- 🚀 **Escala:** Turbo model = 350M params, roda em GPU consumer, distilled decoder (10→1 step)

**TAM:** Mercado TTS $5.3B (2025), projetado $12B até 2030. Voice agents sozinhos ~$2B.

**Modelo de negócio:**
- Open-core: modelo grátis, API gerenciada paga (sub-200ms latency)
- Enterprise: fine-tuning, compliance, SLA
- Vertical: integração com call centers, gaming, audiobooks

**Esforço pra produtizar:** Baixo — modelos prontos, pip install. API wrapper = weekend project.

**Combinações letais:**
- Chatterbox + Pipecat (#66) + LiveKit Agents (#67) = voice agent stack completo, $0 de TTS
- Chatterbox + ScreenPipe (#86) = personal AI com voz que "ouve e vê" tudo

---

## 85. usestrix/strix ⭐ 19.6k
**O que faz:** AI agents autônomos que fazem pentest real — rodam código, encontram vulns, geram PoCs reais. CLI-first, CI/CD integration.

**Problema real:** Pentest manual custa $10k-50k+ por engagement e leva semanas. Ferramentas SAST (Snyk, SonarQube) geram montanhas de false positives. Startups simplesmente não testam segurança.

**Eixos de inovação:**
- 🎯 **Problema:** 90%+ de startups nunca fazem pentest real (muito caro)
- 💎 **Qualidade:** PoCs reais validados vs falsos positivos de SAST/DAST
- ⚡ **Velocidade:** Horas vs semanas de pentest manual

**TAM:** Mercado de application security testing $13.7B (2025). Pentest-as-a-Service ~$3B.

**Modelo de negócio:**
- Freemium: scan básico grátis, enterprise features pagas
- Per-scan: pay-per-pentest com relatórios compliance (SOC2, ISO 27001)
- CI/CD integration: pricing por repo/pipeline

**Esforço pra produtizar:** Baixo — CLI pronto, Docker-based, CI/CD templates incluídos. Precisa LLM provider key.

**Criado:** Ago 2025 → 19.6k stars em 6 meses. Segurança + AI = hype real.

---

## 86. mediar-ai/screenpipe ⭐ 16.6k
**O que faz:** Rewind.ai open-source — grava tela + microfone 24/7, 100% local, com OCR e indexação. API developer-friendly para construir "pipes" (plugins).

**Problema real:** Rewind.ai cobrava $20/mês e foi descontinuado. Microsoft Recall gerou escândalo de privacidade. Pessoas querem "memória digital" mas sem mandar dados pra cloud.

**Eixos de inovação:**
- 🎯 **Problema:** Memória digital sem sacrificar privacidade
- 💸 **Custo:** $0 vs $20/mês (Rewind) — e Rewind nem existe mais
- 💎 **Qualidade:** 100% local, extensível via pipes, integra com qualquer LLM

**TAM:** Mercado de "personal AI/digital memory" nascente, estimado $5-10B até 2028. Adjacent ao mercado de PKM ($2B).

**Modelo de negócio:**
- Freemium: core grátis, cloud sync/backup pago
- Marketplace: pipes (plugins) pagos
- Enterprise: compliance logging, meeting summarization, knowledge capture

**Esforço pra produtizar:** Médio — app Tauri funcional, precisa polish em UX. Rust core = performance sólida.

**Combinações:**
- ScreenPipe + Khoj (#77) = AI brain que lembra TUDO que você viu/ouviu
- ScreenPipe + Chatterbox (#84) = assistente pessoal com voz que te conhece profundamente

---

## 87. Billionmail/BillionMail ⭐ 13.4k
**O que faz:** Mail server + email marketing completo, self-hosted. Inclui Postfix, Dovecot, Rspamd, RoundCube. "8 minutos da instalação ao primeiro envio."

**Problema real:** Mailchimp cobra $13-350/mês e limita envios. SendGrid $15-90/mês. Para quem tem lista grande (100k+), custo escala absurdamente. Listmonk (#14, 18.9k ⭐) resolve parte mas não inclui mail server.

**Eixos de inovação:**
- 🎯 **Problema:** Email marketing caro demais para PMEs/creators com listas grandes
- 💸 **Custo:** $0 + custo do VPS (~$5-20/mês) vs $100-500/mês no Mailchimp
- 📈 **Volume:** "Billion emails" — sending ilimitado, sem throttle artificial
- 🚀 **Escala:** Inclui mail server completo (não precisa SES/SendGrid)

**TAM:** Mercado de email marketing $15.7B (2025). PMEs gastam em média $300-500/mês.

**Modelo de negócio:**
- Open-core: community grátis, managed hosting pago
- Add-ons: deliverability monitoring, IP warm-up, advanced analytics
- White-label: agências oferecem como próprio

**Esforço pra produtizar:** Baixo — stack completa, install script, Docker. Desafio: deliverability e reputação de IP.

**Vs Listmonk (#14):** BillionMail é mais ambicioso — inclui mail server inteiro. Listmonk precisa de SMTP externo.

---

## 88. Fission-AI/OpenSpec ⭐ 21.5k
**O que faz:** Spec-driven development (SDD) — escreva specs estruturadas e AI coding assistants (Claude Code, Cursor, etc.) executam com muito mais precisão. "Context engineering" como disciplina.

**Problema real:** AI coding agents erram muito quando recebem instruções vagas. Devs gastam mais tempo corrigindo output de AI do que seria escrever do zero. Falta uma interface padrão entre humanos e AI coders.

**Eixos de inovação:**
- 🎯 **Problema:** AI coding assistants são imprevisíveis sem contexto estruturado
- ⚡ **Velocidade:** Specs bem escritas = 5-10x menos iterações com AI
- 💎 **Qualidade:** Output de AI vai de "50% correto" para "90%+ correto"

**TAM:** Mercado de AI coding tools $32B (2025), crescendo 45% ao ano. Adjacente: developer productivity tools $20B.

**Modelo de negócio:**
- Open-core: framework grátis, templates premium de specs por vertical
- IDE integration: plugins pagos para VS Code, JetBrains
- Enterprise: spec libraries, team workflows, quality gates

**Esforço pra produtizar:** Médio — conceito sólido, precisa integração profunda com IDEs e CI/CD.

**Criado:** Jan 2025 → 21.5k stars = validação massiva da tese de "context engineering"

---

### [docmost/docmost](https://github.com/docmost/docmost) ⭐ 18.9k | 🎯💸💎
**Problema:** Confluence custa $5.75-11/user/mês. Notion similar. Empresas pagam $1000+/mês pra documentação colaborativa. Dados ficam em cloud de terceiros — compliance/GDPR é nightmare.
**Solução:** Wiki/docs colaborativa open-source com real-time editing, Excalidraw/Draw.io/Mermaid, spaces, permissions, comments, page history, search, file attachments. Self-hosted.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Toda equipe precisa de wiki/docs — mercado de 100M+ knowledge workers
- 💸 **Custo:** $0 vs $5-11/user/mês. Empresa de 100 pessoas economiza $7000-13000/ano
- 💎 **Qualidade:** UX limpa, real-time collab, diagramas integrados — paridade com Notion/Confluence em features core
**TAM:** $10B+ (collaboration/knowledge management market)
**Modelo de negócio:** Cloud managed, enterprise features (SSO, audit logs, advanced permissions), suporte premium
**Esforço:** Baixo-Médio — 18.9k stars, projeto maduro com AGPL license, Docker deploy
**Combinações:** Docmost + Colanode (#114) = Notion+Slack completo. Docmost + Khoj (#77) = docs com AI search nativo

---

### [better-auth/better-auth](https://github.com/better-auth/better-auth) ⭐ 25.8k | 🎯💸💎
**Problema:** Auth0 cobra $23-240/mês por features avançadas. Clerk similar. NextAuth/Lucia são incompletos — 2FA, multi-tenant, RBAC requerem centenas de linhas extras. Auth é o maior time-sink de todo novo projeto.
**Solução:** Framework de auth TypeScript mais completo. Plugin ecosystem: 2FA, multi-tenant, organizations, passkeys, social login, RBAC. Framework-agnostic (Next, Nuxt, Svelte, Hono, Express). MIT license.
**Por que é 5-10x melhor:**
- 🎯 **Problema real:** Todo app precisa de auth — é o primeiro feature de 100% dos projetos
- 💸 **Custo:** $0 vs $23-240/mês (Auth0/Clerk). Sem vendor lock-in
- 💎 **Qualidade:** Plugin system = 2FA, multi-tenant, passkeys com 3 linhas. Comparado com NextAuth que requer 200+ linhas pra mesma coisa
**TAM:** $8B+ (identity & access management market, growing 12% YoY)
**Modelo de negócio:** Open-source core (MIT) + managed service (Better Auth Cloud) + enterprise plugins + consulting
**Esforço:** Baixo — npm install, TypeScript nativo, docs excelentes, 25.8k stars = comunidade ativa
**Combinações:** Better-auth + Supabase = BaaS completo. Better-auth + qualquer SaaS starter = auth resolvido em 10 min
