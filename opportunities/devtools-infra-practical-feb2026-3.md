# 🛠️ DevTools & Infraestrutura Prática — Fev 2026 (Rodada 3)

**Tema:** Ferramentas práticas que resolvem frustrações reais de DevOps, sysadmins e homelabbers — foco em UX bonita sobre infra madura.

---

## 1. Michael-A-Kuykendall/shimmy ⭐ 3.6k
**Link:** https://github.com/Michael-A-Kuykendall/shimmy
**O que faz:** Inference server LLM em Rust, single binary, zero config, OpenAI-API compatible — drop-in pra GGUF + SafeTensors com hot model swap, auto-discovery, GPU backends inclusos.

**Problema real:** Rodar LLMs localmente exige Ollama (Go, ecossistema fechado), vLLM (Python pesado), ou llama.cpp (complexo). Shimmy é 1 binário Rust que auto-descobre modelos do HuggingFace cache/Ollama/dirs locais e serve API OpenAI-compatible sem config.

**Eixos de inovação:**
- 🎯 **Problema real:** Devs/empresas que querem rodar LLMs locais com zero friction
- ⚡ **5x mais rápido em setup:** Download → `./shimmy serve` → pronto. Zero config files.
- 💸 **5x menor custo:** Free forever (promessa explícita), vs Ollama que caminha pra monetização

**TAM:** $2-5B (local AI inference market, crescendo 40%+ YoY)
**Modelo de negócio:** Open core — sponsors, enterprise support, hosted dashboard
**Esforço pra produtizar:** Baixo — já funciona como produto standalone
**Combinações:** Com Memori (#398) pra memória + Shimmy pra inferência = stack AI local completo

---

## 2. lintsinghua/DeepAudit ⭐ 4.4k
**Link:** https://github.com/lintsinghua/DeepAudit
**O que faz:** Multi-agent system de auditoria de código que encontra vulnerabilidades automaticamente — já descobriu 48 CVEs reais em 16 projetos open-source (Zentao, Dataease, H2o-3, etc). Suporta Ollama local.

**Problema real:** Pentest manual custa $20-100k por engagement e leva semanas. SAST tools (Snyk, SonarQube) geram toneladas de false positives. DeepAudit usa multi-agents que colaboram + sandbox PoC pra validar vulnerabilidades reais.

**Eixos de inovação:**
- 🎯 **Problema real:** 48 CVEs confirmados provam que funciona (CVSS 9.8 em vários)
- 💸 **10x menor custo:** $0 vs $20-100k por pentest manual
- ⚡ **10x mais rápido:** Horas vs semanas de pentest manual
- 🚀 **Escala:** Roda em qualquer codebase, Ollama pra privacidade total

**TAM:** $8-12B (application security testing market)
**Modelo de negócio:** Freemium — community open-source, enterprise com reporting compliance (SOC2, ISO 27001), SaaS hosted
**Esforço pra produtizar:** Médio — precisa melhorar reporting e integração CI/CD
**Diferencial vs Strix (#487):** DeepAudit foca em código-fonte (SAST), Strix foca em app running (DAST). Complementares.

---

## 3. control-theory/gonzo ⭐ 2.4k
**Link:** https://github.com/control-theory/gonzo
**O que faz:** TUI de análise de logs com AI insights, heatmaps, real-time streaming, Kubernetes nativo, OTLP receiver — inspirado em k9s mas pra logs.

**Problema real:** Log analysis é dominado por ferramentas caras (Datadog $23+/host, Splunk $150+/GB/dia) ou complicadas (ELK Stack setup infernal). Devs precisam de algo entre `tail -f` e Datadog. Gonzo é o "k9s dos logs" — poderoso mas roda no terminal.

**Eixos de inovação:**
- 🎯 **Problema real:** Todo dev/SRE sofre com log analysis
- 💸 **10x menor custo:** $0 vs Datadog/Splunk (economiza $2-50k/ano pra startups)
- 💎 **5x mais qualidade UX:** Heatmaps, AI insights, charts — tudo no terminal
- ⚡ **Rápido:** Go binary, real-time, zero setup externo

**TAM:** $4-8B (log management & observability)
**Modelo de negócio:** Open core — features enterprise (RBAC, teams, alerting avançado, retention policies)
**Esforço pra produtizar:** Médio — precisa de persistence/storage layer pra uso enterprise
**Combinações:** Com SigNoz (#96) ou Beszel (#183) pra monitoring stack completa

---

## 4. mostafa-wahied/portracker ⭐ 1.7k
**Link:** https://github.com/mostafa-wahied/portracker
**O que faz:** Ferramenta de monitoramento e discovery de portas/serviços — auto-descobre services rodando, suporta Docker + TrueNAS, P2P multi-server, UI moderna.

**Problema real:** Quem gerencia homelab ou servidores perde horas rastreando "que porta tá sendo usada?" em planilhas. Port conflicts causam downtime. Portracker auto-descobre tudo e dá visibilidade completa.

**Eixos de inovação:**
- 🎯 **Problema real:** Gestão de portas/serviços é dor real pra sysadmins e homelabbers
- ⚡ **10x mais rápido:** Auto-discovery vs rastrear manualmente com `netstat`/`ss`
- 💸 **Grátis:** Substitui processos manuais e ferramentas pagas de network discovery

**TAM:** $500M-1B (nicho dentro de network management)
**Modelo de negócio:** Open core — enterprise features (alerting, RBAC, compliance reporting, multi-team)
**Esforço pra produtizar:** Baixo — já é self-contained com SQLite embedded
**Combinações:** Com Scanopy (#201) pra topology + Portracker pra portas = visibilidade de rede completa

---

## 5. Adembc/lazyssh ⭐ 3.0k
**Link:** https://github.com/Adembc/lazyssh
**O que faz:** SSH manager TUI inspirado em lazydocker/k9s — navega, conecta, gerencia servidores do ~/.ssh/config com UI interativa, fuzzy search, tags, pin favorites.

**Problema real:** Devs e sysadmins gerenciam dezenas de servidores mas navegam SSH com aliases decorados ou scripts bash. Lazyssh traz a experiência lazydocker pro SSH.

**Eixos de inovação:**
- 🎯 **Problema real:** Todo dev com >5 servidores sofre com gestão SSH
- 💎 **5x mais qualidade UX:** De `ssh user@192.168.1.42 -p 2222 -i ~/.ssh/prod_key` pra 1 keypress
- ⚡ **Rápido:** Go binary, zero deps, lê ~/.ssh/config direto

**TAM:** $200M-500M (parte de remote access management)
**Modelo de negócio:** Difícil monetizar diretamente — melhor como entrada pra plataforma maior de server management
**Esforço pra produtizar:** Baixo — já funcional, precisa de file transfer GUI (roadmap)
**Combinações:** Com Termix (#294) pra management completo ou com Beszel (#183) pra monitoring

---

## 6. karol-broda/snitch ⭐ 2.9k
**Link:** https://github.com/karol-broda/snitch
**O que faz:** TUI bonita pra inspecionar conexões de rede — substitui `ss`/`netstat` com interface amigável, temas (Catppuccin, Dracula, etc), filtros, auto-refresh.

**Problema real:** `ss` e `netstat` outputs são criptografias pra humanos. Snitch faz a mesma coisa mas bonito e legível.

**Eixos de inovação:**
- 🎯 **Problema real:** Debug de rede é dor diária pra devs
- 💎 **5x mais qualidade:** De output ilegível pra TUI com temas e filtros
- ⚡ **Mesmo info, 5x mais rápido de entender:** Visual > texto cru

**TAM:** Ferramenta utilitária — valor como componente de stack maior
**Modelo de negócio:** Open-source puro — não monetizável isoladamente
**Esforço pra produtizar:** N/A — é tool de dev, não produto SaaS

---

## 7. surajverma/homehub ⭐ 1.1k
**Link:** https://github.com/surajverma/homehub
**O que faz:** Dashboard familiar all-in-one self-hosted — notas compartilhadas, lista de compras, chores, calendário, tracker de despesas, media downloader, recipe book, expiry tracker, PDF compressor, weather — tudo em uma PWA sem login, no-config.

**Problema real:** Famílias usam 10+ apps separados (Google Keep, Todoist, Splitwise, WhatsApp groups) pra organizar vida doméstica. HomeHub unifica tudo num dashboard privado que roda em Raspberry Pi.

**Eixos de inovação:**
- 🎯 **Problema real:** Famílias não têm hub digital unificado
- 💸 **10x menor custo:** $0 + Raspberry Pi vs $5-20/mês em apps separados
- 🚀 **Escala de funcionalidade:** 15+ ferramentas num único deploy Docker

**TAM:** $1-3B (family organization apps — Cozi, OurHome, etc)
**Modelo de negócio:** Freemium — hosting managed, add-ons, integrações smart home
**Esforço pra produtizar:** Médio — precisa de auth pra multi-família, mobile apps nativos
**Combinações:** Com Grocy (#26) pra estoque + HomeHub pra organização familiar = "Home OS"

---

## 8. Quenary/tugtainer ⭐ 1.1k
**Link:** https://github.com/Quenary/tugtainer
**O que faz:** Automação de updates de containers Docker com Web UI — multi-host, crontab, notificações, per-container config, linked containers, private registries.

**Problema real:** Manter containers atualizados é tedioso. Watchtower (16k⭐) é popular mas tem UX mínima e não suporta multi-host bem. Tugtainer dá controle granular com UI moderna.

**Eixos de inovação:**
- 🎯 **Problema real:** Todo homelabber/devops sofre com Docker updates
- 💎 **5x mais qualidade:** UI polida vs Watchtower CLI-only
- 🚀 **Multi-host:** Agente remoto pra gerenciar fleet de servidores Docker

**TAM:** $500M-1B (container management, parte do $8B Docker ecosystem)
**Modelo de negócio:** Open core — enterprise (audit logs, RBAC, rollback automático, compliance)
**Esforço pra produtizar:** Baixo-Médio — já funcional, precisa polir enterprise features
