# AI Personal Productivity & Local-First Tools

## gavrielc/nanoclaw ⭐2.8k
**Categoria:** AI/Personal Assistant
**Link:** https://github.com/gavrielc/nanoclaw
**Eixos:** 🎯💎💸🚀

### Problema
OpenClaw/Clawdbot são poderosos mas complexos (52+ módulos, 45+ deps). Usuários avançados querem um assistente pessoal AI que entendam completamente, com isolamento real de segurança (containers OS-level, não permissões app-level).

### Análise
- Codebase mínimo que se entende em 8 minutos
- Roda em Apple Containers (macOS) ou Docker
- WhatsApp I/O, cada grupo com filesystem isolado
- Claude Agent SDK nativo (sem hacks de ToS)
- Filosofia "fork and customize" — sem configuração, muda o código
- Skills como transformações (ex: `/add-telegram` modifica seu fork)

### Modelo de Negócio
- Hosting gerenciado ($9-29/mês) — "NanoClaw Cloud"
- Templates/skills marketplace p/ customizações comuns
- Consultoria de setup p/ empresas que querem assistentes internos

### TAM
- 5M+ devs que usam Claude Code querem assistente pessoal
- Mercado de personal AI assistant: $2-5B até 2027

---

## anthropics/knowledge-work-plugins ⭐1.3k
**Categoria:** AI/Enterprise Productivity
**Link:** https://github.com/anthropics/knowledge-work-plugins
**Eixos:** 🎯💎🚀

### Problema
Empresas gastam meses customizando AI para cada departamento. Cada equipe (vendas, jurídico, finanças, marketing) tem workflows únicos com ferramentas específicas. Integrar tudo é caríssimo.

### Análise
- 11 plugins oficiais da Anthropic: productivity, sales, customer-support, product-management, marketing, legal, finance, data, design, people, IT
- Cada um com connectors pré-configurados (Slack, Jira, Notion, HubSpot, Salesforce, Intercom, etc.)
- Slash commands e sub-agents especializados por função
- Open-source para customização por empresa
- Padrão emergente: "plugin marketplace" para AI assistants empresariais

### Modelo de Negócio
- Vertical SaaS: plugins customizados por indústria ($500-5000/mês)
- Marketplace de plugins terceiros com comissão
- Serviço de integração enterprise ($10k-50k setup)

### TAM
- Enterprise AI assistants: $15-30B mercado
- Cada departamento de Fortune 500 = $50-200k/ano em AI tooling

---

## mindfold-ai/Trellis ⭐1.6k
**Categoria:** DevTools/AI Framework
**Link:** https://github.com/mindfold-ai/Trellis
**Eixos:** 🎯💎⚡🚀

### Problema
Dev teams usando Claude Code/Cursor perdem tempo repetindo contexto, não conseguem paralelizar sessions, e não compartilham best practices de forma consistente.

### Análise
- Auto-injection de specs em toda conversa AI (write once, apply forever)
- Parallel sessions em worktrees Git isolados — multiple features simultâneas
- Team sync: um dev escreve best practice, toda equipe se beneficia
- Session persistence no repo — AI lembra contexto entre sessões
- Custom workflows via slash commands
- npm package, setup em 30 segundos

### Modelo de Negócio
- Free para devs individuais
- Team plan $15/dev/mês (sync, analytics, dashboard)
- Enterprise $50/dev/mês (SSO, audit log, custom integrations)

### TAM
- 10M+ devs usando AI coding tools
- Developer productivity tools: $5-10B mercado

---

## npmx-dev/npmx.dev ⭐1.2k
**Categoria:** DevTools/Registry Browser
**Link:** https://github.com/npmx-dev/npmx.dev
**Eixos:** 🎯💎⚡

### Problema
npmjs.com é lento, cluttered, sem features modernas (dark mode, code browsing, vulnerability warnings inline, keyboard navigation). Devs JS/TS gastam tempo desnecessário navegando packages.

### Análise
- Drop-in URL replacement (troca npmjs.com por npmx.dev)
- Code viewer inline com syntax highlighting
- Vulnerability warnings do OSV database
- Install size (incluindo transitive deps)
- Outdated dependency indicators
- Provenance badges, JSR availability
- Keyboard shortcuts, infinite search

### Modelo de Negócio
- Free tier público
- Pro $5/mês (dashboard pessoal, favoritos, alertas)
- Enterprise (registry privado, analytics, compliance)

### TAM
- 17M+ devs npm. Qualquer % = massivo
- Comparar com npm alternativas: Yarn, pnpm ecossistema

---

## Nagi-ovo/gemini-voyager ⭐4.7k
**Categoria:** AI/Browser Extension
**Link:** https://github.com/Nagi-ovo/gemini-voyager
**Eixos:** 🎯💎⚡

### Problema
Google Gemini web UI carece de organização (sem folders, sem timeline), export limitado, sem prompt library, e features como Mermaid rendering não existem nativamente.

### Análise
- Timeline visual entre mensagens, star momentos-chave
- Folders 2 níveis com drag-and-drop
- Prompt Vault cross-site (Gemini, AI Studio, custom sites)
- Export JSON/Markdown/PDF com imagens
- NanoBanana: remoção lossless de watermarks
- Deep Research: extrai links e processos de pesquisa
- Batch delete, LaTeX/MathML copy

### Modelo de Negócio
- Extension free + Pro features ($4.99/mês)
- API de prompt management cross-platform
- Enterprise: compliance e audit trail de conversas AI

### TAM
- 100M+ usuários Gemini. Chrome Web Store = distribuição massiva
- AI UX enhancement tools: mercado emergente $500M+

---

## legeling/PromptHub ⭐526
**Categoria:** Produtividade/AI Tools
**Link:** https://github.com/legeling/PromptHub
**Eixos:** 🎯💸💎

### Problema
Profissionais gastam horas reescrevendo prompts. Não existe version control, não dá pra testar mesmo prompt em múltiplos modelos, e ferramentas pagas (PromptLayer, etc.) mandam dados pra cloud.

### Análise
- Desktop app Electron cross-platform
- Version control com diff visual entre versões
- Template variables `{{var}}` com substituição dinâmica
- Multi-model parallel testing (OpenAI, DeepSeek, Ollama, etc.)
- WebDAV sync (Nextcloud, etc.) — dados locais mas sincronizáveis
- Master password + pasta privada encriptada
- 7 idiomas, 3 views (card/gallery/list)

### Modelo de Negócio
- Free open-source desktop
- Cloud sync premium $5/mês (team collab, analytics)
- Enterprise: shared prompt library com permissões

### TAM
- Todo profissional que usa AI regularmente (~500M pessoas)
- Prompt management SaaS: $200-500M mercado emergente
