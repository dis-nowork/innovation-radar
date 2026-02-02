# 🛠️ Self-Hosted Professional Tools — Fev 2026

Ferramentas self-hosted que substituem SaaS caros para profissionais e equipes.

---

## 288. KartikLabhshetwar/better-shot ⭐ 1.4k
- **Link:** https://github.com/KartikLabhshetwar/better-shot
- **Problema real:** CleanShot X ($29) domina screenshots no macOS. Designers, devs e content creators pagam por captura+edição+anotação. Alternativas free são feias ou limitadas.
- **Eixos:** 🎯💸💎
  - 🎯 Resolve dor real — screenshots profissionais são workflow diário pra milhões
  - 💸 Grátis vs $29 — zero cost
  - 💎 Feature parity alta — region/fullscreen/window capture, backgrounds, shadows, annotations, OCR via Vision framework
- **TAM:** ~$200M (screenshot/screen recording tools market)
- **Modelo:** Open-source + premium features, sponsorships
- **Esforço:** Baixo — já funcional, Tauri+React, macOS-native
- **Stack:** Tauri, React, macOS Vision framework, Homebrew
- **Combinações:** Com openscreen (screen recording) = suite completa de captura visual

---

## 289. hcavarsan/pipedash ⭐ 1.0k
- **Link:** https://github.com/hcavarsan/pipedash
- **Problema real:** Times usam 3-5 CI/CD providers simultaneamente (GitHub Actions, GitLab, Jenkins, ArgoCD...). Verificar status = abrir 5 tabs. Não existe dashboard unificado self-hosted.
- **Eixos:** 🎯💎⚡💸
  - 🎯 Pain point universal em DevOps — "onde está minha build?"
  - 💎 UI unificada com trigger/re-run/cancel de qualquer provider
  - ⚡ Background polling com atualização instantânea
  - 💸 Grátis vs ferramentas enterprise de observabilidade CI/CD ($$$)
- **TAM:** ~$2B (CI/CD tooling market, observability)
- **Modelo:** Open-source core + Enterprise (SSO, teams, audit logs, SLA monitoring)
- **Esforço:** Médio — plugin system extensível, já suporta 7 providers
- **Stack:** Tauri, Rust, React, TypeScript, SQLite/PostgreSQL
- **Diferencial:** Desktop + Web + iOS app, tokens criptografados localmente

---

## 290. majcheradam/ocrbase ⭐ 802
- **Link:** https://github.com/majcheradam/ocrbase
- **Problema real:** Empresas processam milhares de PDFs/documentos. APIs de OCR (AWS Textract, Google Document AI) custam $1.50-$5/1000 páginas. Resultados nem sempre estruturados.
- **Eixos:** 🎯⚡📈💸
  - 🎯 Extração de dados de documentos é workflow crítico (finance, legal, healthcare)
  - ⚡ Queue-based processing p/ milhares de documentos
  - 📈 PaddleOCR-VL open-weight = escala sem custo por página
  - 💸 Self-hosted = custo fixo de infra vs por-página
- **TAM:** ~$15B (document processing/intelligent document processing market)
- **Modelo:** Open-source self-hosted + Managed API (pay-per-page) + Enterprise on-prem
- **Esforço:** Médio — SDK TypeScript pronto, React hooks, WebSocket
- **Stack:** PaddleOCR-VL-0.9B, TypeScript SDK, Docker, Bun
- **Combinações:** Com LLMs (parse→summarize→extract) = pipeline completa de doc intelligence

---

## 291. obot-platform/obot ⭐ 585
- **Link:** https://github.com/obot-platform/obot
- **Problema real:** MCP servers estão explodindo (milhares disponíveis) mas não existe plataforma enterprise pra hospedar, descobrir, autenticar e auditar uso. É como npm sem npmjs.com.
- **Eixos:** 🎯💎🚀
  - 🎯 Gap real — enterprises querem MCP mas não têm governança
  - 💎 Solução completa: hosting + registry + gateway + chat client
  - 🚀 Escala de nicho (devs individuais) pra massivo (enterprise IT)
- **TAM:** ~$5B+ (API management/gateway market, growing com MCP adoption)
- **Modelo:** Open-source + Enterprise (SSO, compliance, SLA, support)
- **Esforço:** Médio-Alto — plataforma complexa mas bem arquitetada
- **Stack:** Go, Docker, Kubernetes, OAuth 2.1
- **Diferencial:** Único a oferecer hosting+registry+gateway+client integrados

---

## 292. the-momentum/open-wearables ⭐ 456
- **Link:** https://github.com/the-momentum/open-wearables
- **Problema real:** Devs de health apps precisam integrar Garmin+Fitbit+Oura+Whoop+Strava separadamente. Cada um tem OAuth diferente, formatos diferentes, APIs diferentes. Meses de trabalho.
- **Eixos:** 🎯💸🚀💎
  - 🎯 Integração multi-wearable é o maior gargalo de health app development
  - 💸 Self-hosted = sem vendor lock-in, sem custo por API call
  - 🚀 Uma API unificada substitui 6+ integrações separadas
  - 💎 Dados normalizados + AI health insights layer
- **TAM:** ~$10B (digital health platform market, wearables data analytics)
- **Modelo:** Open-source core + Managed hosting + Enterprise (HIPAA, white-label)
- **Esforço:** Médio — FastAPI+React, Docker, integrações OAuth já implementadas
- **Stack:** FastAPI, React, TanStack, Docker
- **Combinações:** Com AI health models = plataforma de saúde preditiva personalizada

---

## 293. tinykit-studio/tinykit ⭐ 358
- **Link:** https://github.com/tinykit-studio/tinykit
- **Problema real:** Lovable ($40/mês), Replit ($25/mês), v0 cobram por AI generation. Não dá pra self-hospedar. Dados ficam com eles. Freelancers/agências querem controle.
- **Eixos:** 🎯💸🚀
  - 🎯 App building com AI é mercado explosivo
  - 💸 Self-hosted = custo do LLM (BYOLLM) vs $40/mês
  - 🚀 Multi-app em 1 servidor, domain mapping, escala de uso pessoal a agência
- **TAM:** ~$8B (low-code/no-code platform market)
- **Modelo:** Open-source + Cloud hosted + Agency plan (white-label)
- **Esforço:** Médio — early alpha mas funcional, PocketBase simplifica infra
- **Stack:** Svelte, PocketBase, Docker, BYOLLM (OpenAI/Anthropic/Gemini)
- **Diferencial:** Time travel (snapshots), realtime DB embutido, CMS built-in
