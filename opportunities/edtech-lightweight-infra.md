# 🎓 EdTech & Lightweight Infrastructure Tools

Ferramentas que democratizam educação com AI e substituem SaaS caro com soluções leves self-hosted.

---

### [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) ⭐ 9.9k | 🎯💎⚡💸
**Problema:** Estudantes pagam caro por tutoria particular ou usam ChatGPT genérico sem personalização por documento. Não existe "tutor AI" que realmente entenda SEUS materiais.
**Solução:** Tutor AI personalizado que:
- Faz RAG massivo sobre seus documentos (textbooks, papers, manuais)
- Gera visualizações interativas de conceitos complexos
- Cria exercícios e provas personalizadas baseadas no seu nível
- Deep research com síntese cross-domain
- Multi-agent: RAG + web search + code execution

**Eixos de Inovação:**
- 🎯 Problema real: 1.5B estudantes globalmente, tutoria particular custa $40-100/h
- 💎 Qualidade: Multi-agent architecture com citações precisas, muito além de "chat com PDF"
- ⚡ Velocidade: Setup em minutos via Docker, começa a estudar imediatamente
- 💸 Custo: Self-hosted, custo = LLM API (~$0.01-0.10 por sessão vs $40+/h tutoria)

**TAM:** $100B+ (edtech global), segmento de tutoring/test prep vale ~$15B
**Modelo:** Freemium SaaS (hosted) + enterprise para universidades + white-label
**Esforço:** Médio — já tem v0.6, Docker pronto, precisa polish de UX e onboarding
**Combinações:** + KittenTTS (leitura em voz alta) + VibeVoice (multilíngue) = tutor multimodal completo

---

### [KittenML/KittenTTS](https://github.com/KittenML/KittenTTS) ⭐ 9.6k | 🎯💸⚡💎
**Problema:** TTS de qualidade requer GPU cara (modelos de 1-10GB) ou APIs pagas ($4-24/1M chars). Dispositivos edge/mobile ficam de fora.
**Solução:** TTS realista com apenas 15M parâmetros (<25MB), roda sem GPU. `pip install` e pronto.

**Eixos de Inovação:**
- 🎯 Problema real: Acessibilidade, e-learning, assistentes de voz em edge devices
- 💸 Custo: Zero — roda local, sem API. vs ElevenLabs ($5-99/mês)
- ⚡ Velocidade: Modelo nano = inferência rápida mesmo em CPU
- 💎 Qualidade: State-of-the-art para o tamanho, 8 vozes expressivas (M/F)

**TAM:** $7B+ (TTS market), segmento edge/embedded crescendo 25%/ano
**Modelo:** Commercial license para embeddar em produtos + premium voices + fine-tuning service
**Esforço:** Baixo — já é pip installable, pronto para integrar
**Combinações:** + DeepTutor = tutor que fala + Meeting AI tools = transcrição+resposta em edge

---

### [tiagozip/cap](https://github.com/tiagozip/cap) ⭐ 4.8k | 🎯💸⚡💎
**Problema:** reCAPTCHA/hCaptcha são pesados (500KB+), rastreiam usuários, quebram UX com puzzles visuais, não funcionam para APIs M2M.
**Solução:** CAPTCHA baseado em proof-of-work SHA-256. 20KB, zero tracking, invisível, funciona para humanos E máquinas amigáveis.

**Eixos de Inovação:**
- 🎯 Problema real: Todo site precisa anti-bot. GDPR torna tracking-based CAPTCHAs problemáticos
- 💸 Custo: 100% grátis e self-hosted vs Cloudflare Turnstile/hCaptcha enterprise pricing
- ⚡ Velocidade: 250x menor que hCaptcha, carrega em milliseconds, zero friction para usuário
- 💎 Qualidade: Privacy-first by design, customizável via CSS, invisible mode, standalone Docker

**TAM:** $12B+ (web security/anti-bot market)
**Modelo:** Open-core — standalone mode com analytics dashboard como premium, enterprise support
**Esforço:** Baixo — já production-ready, Apache 2.0
**Combinações:** + VoidAuth = stack completo de auth+anti-bot self-hosted

---

### [usertour/usertour](https://github.com/usertour/usertour) ⭐ 1.9k | 🎯💸🚀
**Problema:** Onboarding de usuários em SaaS custa $249-999/mês (Appcues, Userflow, Chameleon). Startups early-stage não podem pagar mas precisam desesperadamente de bom onboarding.
**Solução:** Plataforma completa de onboarding in-app: tours, checklists, surveys. Self-hosted, open-source.

**Eixos de Inovação:**
- 🎯 Problema real: 40-60% dos trial users abandonam por onboarding ruim
- 💸 Custo: Self-hosted grátis vs $249-999/mês nos incumbentes
- 🚀 Escala: Multi-environment (prod/staging), version control, custom targeting — features enterprise

**TAM:** $3B+ (digital adoption platforms)
**Modelo:** Open-core — self-hosted free, cloud hosted premium, enterprise com analytics avançado
**Esforço:** Médio — bom mas jovem, precisa mais integrações e templates
**Combinações:** + analytics platform = ciclo completo de product-led growth

---

### [operacle/checkcle](https://github.com/operacle/checkcle) ⭐ 2.3k | 🎯💸💎
**Problema:** Monitoring completo (Datadog, PagerDuty) custa $15-23/host/mês. PMEs e freelancers DevOps precisam de algo completo mas acessível.
**Solução:** Monitoring full-stack self-hosted — uptime, SSL, DNS, server metrics, incident management, status pages, alertas multi-canal.

**Eixos de Inovação:**
- 🎯 Problema real: Todo serviço online precisa monitoring. Custos escalam rápido
- 💸 Custo: Self-hosted grátis vs Datadog $15-23/host ou UptimeRobot $7-54/mês
- 💎 Qualidade: Feature-set comparable a soluções pagas — distributed checks, SSL monitoring, status pages

**TAM:** $6B+ (monitoring/observability market)
**Modelo:** Open-core — community free, enterprise com SLA monitoring, compliance reports, SSO
**Esforço:** Baixo-Médio — Docker one-liner, PocketBase backend, UI pronta
**Combinações:** + Pulse (Proxmox/Docker) + Beszel (server metrics) = observabilidade completa self-hosted

---

### [voidauth/voidauth](https://github.com/voidauth/voidauth) ⭐ 1.8k | 🎯💸💎
**Problema:** Self-hosters precisam de SSO para dezenas de apps. Authelia/Authentik são complexos. Auth0/Okta custam $2-13/user/mês.
**Solução:** SSO simples e elegante — OIDC, ForwardAuth, passkeys, convites, self-registration, encryption-at-rest.

**Eixos de Inovação:**
- 🎯 Problema real: Identity é o #1 pain point de self-hosting
- 💸 Custo: Grátis vs Auth0 ($240/mês para 1000 users) ou Okta ($1,500+/mês)
- 💎 Qualidade: UX moderna, passkeys nativos, simpler que Authentik/Keycloak

**TAM:** $20B+ (identity/access management market)
**Modelo:** Open-core — community free, enterprise com audit logs, SCIM provisioning, compliance
**Esforço:** Baixo — Docker compose, Postgres/SQLite, UI pronta
**Combinações:** + Cap (CAPTCHA) = auth+anti-bot stack + Checkcle (monitoring) = full self-hosted infra
