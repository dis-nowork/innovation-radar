# 🏗️ Self-Hosted Automation Platforms & AI Task Execution — Feb 2026

## Tema: A Convergência de AI Agents + Self-Hosting + Workflow Automation

O padrão emergente: ferramentas que combinam **AI agents que executam tarefas reais** com **self-hosting** (dados nunca saem do controle do usuário). Não é mais "chatbot que responde perguntas" — é "agente que faz o trabalho".

---

## 520. jonesphillip/weft ⭐ 466
**Link:** https://github.com/jonesphillip/weft

### O que é
Task board pessoal onde **AI agents trabalham nas suas tarefas**. Cria uma task, atribui a um agent, e ele executa. Gmail, Google Docs/Sheets, GitHub, code execution em Cloudflare Sandbox, MCP remoto.

### Problema Real
Profissionais gastam horas em tarefas repetitivas (emails, planilhas, PRs). Zapier/Make automatizam fluxos, mas são caros ($20-100/mês), não têm AI agent inteligente, e seus dados passam por servidores terceiros. Weft é **self-hosted, AI-first, e human-in-the-loop** (approval antes de ações destrutivas).

### Eixos de Inovação
- 🎯 **Problema real:** Automação de tarefas com AI agents — o "AI assistant que realmente FAZ coisas"
- 💎 **Qualidade:** Human-in-the-loop com approval granular; não é automação cega
- ⚡ **Velocidade:** Parallel agents — múltiplas tarefas simultâneas
- 🚀 **Escala:** De manual (1 humano = 1 tarefa) para automático (N agents = N tarefas paralelas)

### TAM
- Automação de workflows: $15B+ (2025)
- Personal AI assistants: mercado nascente, estimado $5B+ até 2028
- Compete com: Zapier, Make, Monday.com (mas AI-first + self-hosted)

### Modelo de Negócio
- Open-source self-hosted (free)
- Cloud hosted com metering por execuções de agent
- Enterprise: SSO, team boards, audit logs, compliance
- Premium integrations marketplace

### Esforço para Produtizar: **Médio**
Já roda em Cloudflare Workers. Precisa: mais integrations, team features, mobile app.

### Combinações
- **+ ocrbase (#521):** Agent processa documentos automaticamente
- **+ LogTide (#523):** Observabilidade das execuções de agents
- **+ Doppelganger (#524):** Browser automation como tool dos agents

---

## 521. majcheradam/ocrbase ⭐ 807
**Link:** https://github.com/majcheradam/ocrbase

### O que é
API de OCR que transforma PDFs em Markdown/JSON estruturado. Powered by PaddleOCR-VL (open-weight). Queue-based para processar milhares de docs. TypeScript SDK com React hooks e WebSocket real-time.

### Problema Real
Empresas gastam $$$$ em OCR SaaS (ABBYY, AWS Textract, Google Document AI — $1.50-3.00 por 1000 páginas). Dados sensíveis (contratos, faturas, prontuários) saem para clouds terceiros. ocrbase: **self-hosted, open-weight model, structured extraction com schemas tipados**.

### Eixos de Inovação
- 🎯 **Problema real:** Extração de dados de PDFs é universal (legal, finance, healthcare, logistics)
- ⚡ **Velocidade:** Queue-based processing, WebSocket real-time updates
- 📈 **Volume:** Projetado para milhares de documentos simultâneos
- 💸 **Custo:** Self-hosted = custo de infra apenas; vs $1.50-3/1000 pags em SaaS

### TAM
- Document processing/OCR: $20B+ (2025)
- Compete com: AWS Textract, Google Document AI, ABBYY, Docsumo
- Target: PMEs que processam 1000+ docs/mês

### Modelo de Negócio
- Self-hosted free (MIT)
- Cloud API com metering por página
- Enterprise: SLA, suporte, custom models
- Vertical solutions (legal, healthcare, accounting templates)

### Esforço para Produtizar: **Baixo**
Já tem SDK, Docker deploy, API pronta. Precisa: mais modelos, pre-built schemas por vertical.

---

## 522. tinykit-studio/tinykit ⭐ 359
**Link:** https://github.com/tinykit-studio/tinykit

### O que é
Lovable/v0/Replit open-source e self-hosted. Builder agentic com PocketBase (realtime DB), CMS inline (edita texto sem tocar código), design system visual, time travel (snapshot por mudança), multi-app num servidor via domain routing.

### Problema Real
Lovable/v0/Replit cobram $20-50/mês por app. Freelancers e pequenos negócios querem criar web apps rapidamente sem depender de plataformas caras. Tinykit: **self-hosted, multi-app (centenas num servidor), PocketBase embutido, BYOLLM**.

### Eixos de Inovação
- 🎯 **Problema real:** Criar web apps sem programar é caro ($20-50/mês por plataforma)
- 💸 **Custo:** Self-hosted = um servidor pra centenas de apps (vs $20-50/mês CADA no Lovable)
- 🚀 **Escala:** Domain routing = multi-tenant num servidor; de 1 app pra N apps
- 💎 **Qualidade:** Time travel, CMS inline, design system — features que SaaS cobram extra

### TAM
- No-code/low-code platforms: $25B+ (2025)
- Compete com: Lovable, v0, Replit, Bolt
- Target: freelancers, agencies, SMBs que constroem apps para clientes

### Modelo de Negócio
- Self-hosted free (MIT)
- Managed cloud com tiers (por apps, storage, bandwidth)
- Agency plan: white-label, client management
- Template/plugin marketplace

### Esforço para Produtizar: **Médio**
Alpha stage. Precisa: auth, backend jobs, more LLM providers, template marketplace.

---

## 523. logtide-dev/logtide ⭐ 314
**Link:** https://github.com/logtide-dev/logtide

### O que é
Datadog/Splunk/ELK killer open-source. GDPR-first (EU cloud ou self-hosted). TimescaleDB + Fastify (muito mais leve que Java stacks). Features: logs explorer, distributed tracing, error groups, SIEM dashboard, alertas, Fluent Bit integration.

### Problema Real
Datadog cobra **$0.10/GB ingestão + $1.70/M indexed logs**. Para uma startup processando 100GB/mês = ~$170/mês SÓ de logs. ELK é "gratuito" mas precisa de cluster Elasticsearch que devora RAM. LogTide: **TimescaleDB (PostgreSQL) = fração do custo, fração da complexidade**.

### Eixos de Inovação
- 🎯 **Problema real:** Observabilidade é cara demais para SMBs/startups
- 💸 **Custo:** Self-hosted free; cloud free em alpha; vs Datadog ($170+/mês para 100GB)
- ⚡ **Velocidade:** 5min Docker setup (vs dias configurando ELK)
- 🚀 **Escala:** De "não monitoramos porque é caro" para "monitoramos tudo por $0"

### TAM
- Observability/monitoring: $40B+ (2025)
- Compete com: Datadog, Splunk, ELK, Grafana Loki, SigNoz
- Target: startups, SMBs, europeus (GDPR), equipes <50 devs

### Modelo de Negócio
- Self-hosted free (MIT)
- EU cloud: freemium → tiers por volume
- Enterprise: SSO, RBAC, compliance certifications
- Managed EU hosting premium (GDPR selling point)

### Esforço para Produtizar: **Médio**
Alpha estável. Precisa: mais maturidade, APM, RUM, mais integrações.

---

## 524. mnemosyne-artificial-intelligence/doppelganger ⭐ 237
**Link:** https://github.com/mnemosyne-artificial-intelligence/doppelganger

### O que é
Plataforma self-hosted de browser automation com visual block editor. Playwright-based, com Task API + CLI, proxy rotation, captures (screenshots/recordings), audit trails. Zero dependência de cloud.

### Problema Real
Browserbase, Apify, PhantomBuster cobram $50-500/mês. Dados scraped passam por servidores terceiros. Selenium/Playwright raw demanda dev skills. Doppelganger: **visual editor (no-code), self-hosted, auditable, proxy management built-in**.

### Eixos de Inovação
- 🎯 **Problema real:** Scraping/automation é caro em SaaS e complexo com código raw
- 💎 **Qualidade:** Block editor visual + audit trails + captures automáticas
- 💸 **Custo:** Self-hosted free (vs $50-500/mês em SaaS)
- 🚀 **Escala:** De "dev que escreve scripts" para "qualquer um monta automação visual"

### TAM
- Web scraping/automation: $8B+ (2025)
- Compete com: Apify, PhantomBuster, Browserbase, Browserbear
- Target: marketing teams, data teams, agencies, lead gen

### Modelo de Negócio
- Self-hosted free (MIT)
- Cloud hosted com metering por execução
- Enterprise: team features, scheduling, compliance
- Marketplace de automações prontas (templates)

### Esforço para Produtizar: **Baixo-Médio**
Funcional, Docker deploy. Precisa: mais blocks, scheduling avançado, team features.

---

## 525. hellodigua/ChatLab ⭐ 4.1k
**Link:** https://github.com/hellodigua/ChatLab

### O que é
Análise local-first de histórico de chats (WeChat, Telegram, WhatsApp). SQL queries sobre conversas, AI Agent para insights, "reviver memórias sociais". Electron desktop, 100% local.

### Problema Real
Pessoas têm **anos de conversas** em mensageiros mas zero capacidade de buscar/analisar (busca nativa é péssima). Empresas de social analytics processam seus dados em cloud. ChatLab: **tudo local, SQL power, AI para insights**.

### Eixos de Inovação
- 🎯 **Problema real:** Busca em mensageiros é terrível; memórias sociais são inacessíveis
- 💎 **Qualidade:** SQL + AI Agent vs busca por keyword nativa dos apps
- 💸 **Custo:** Free e local (vs zero alternativas comparáveis)

### TAM
- Personal productivity/digital memory: mercado nascente
- Bilhões de usuários de mensageiros com anos de conversas
- Potencial para enterprise (compliance, audit de comunicações)

### Modelo de Negócio
- Free open-source (desktop app)
- Premium: mais connectors (Slack, Discord, email), AI models avançados
- Enterprise: compliance, audit, team communication analytics
- API: integração com CRM/customer success tools

### Esforço para Produtizar: **Médio**
Desktop app funcional. Precisa: mais connectors, onboarding simplificado, enterprise features.
