# 🏠 Local-First Collaboration & Productivity

## colanode/colanode (#206)
- **Repo:** https://github.com/colanode/colanode
- **Stars:** 4.5k | **License:** Apache 2.0
- **Eixos:** 🎯💸🚀

### O que é
Workspace de colaboração open-source e local-first que unifica:
- **Chat real-time:** Mensagens instantâneas para times e indivíduos
- **Rich Text Pages:** Editor tipo Notion para docs, wikis, notes
- **Databases customizáveis:** Campos custom, views (table, kanban, calendar)
- **File management:** Armazenamento e compartilhamento em workspaces seguros

Arquitetura: SQLite local + sync em background + CRDTs (Yjs) para edição concorrente.

### Problema real
Slack ($8-15/user/mês) + Notion ($8-15/user/mês) = $16-30/user/mês. Para empresa de 50 pessoas = $800-1500/mês. Dados vivem em servidores de terceiros. Colanode unifica ambos em um produto self-hosted.

### Por que é 5-10x melhor
- **💸 Custo:** $0 vs $16-30/user/mês (Slack + Notion). Para 50 users = economia de $9.6k-18k/ano.
- **🚀 Escala:** De ferramenta individual para times inteiros. Multi-workspace, multi-server.
- **🎯 Problema real:** Soberania de dados. Funciona offline. Sem vendor lock-in.

### TAM
- Team collaboration software: $20B
- Knowledge management: $8B
- Self-hosted tools market crescendo 35% YoY

### Modelo de negócio
- **Self-hosted grátis** + **Managed hosting** ($5-15/user/mês, ainda 50% mais barato que Slack+Notion)
- **Enterprise:** SSO, audit logs, compliance, backup managed
- **Marketplace:** Plugins e integrações

### Esforço: Médio
Produto funcional com web app em app.colanode.com. Precisa maturar features enterprise.

---

## dtyq/magic (#208)
- **Repo:** https://github.com/dtyq/magic
- **Stars:** 4.5k | **License:** Open Source
- **Eixos:** 🎯⚡🚀

### O que é
Plataforma all-in-one de produtividade AI para empresas:
- **Super Magic:** AI Agent generalista para tarefas complexas (multi-agent, auto-planning, auto-correction)
- **Magic IM:** Sistema de mensagens enterprise que integra AI agents com comunicação interna
- **Magic Flow:** Orquestração visual de workflows AI
- **Teamshare OS (coming):** Office colaborativo online

Também open-sourced: Agentlang (framework p/ AI agents com linguagem natural), Magic Lens (HTML→Markdown)

### Problema real
Empresas usam 5-10 ferramentas separadas: Slack + ChatGPT + Zapier + Google Docs + Notion. Magic unifica tudo com AI nativa em cada componente. "100x produtividade" é o pitch.

### Por que é 5-10x melhor
- **⚡ Velocidade:** AI agents embutidos em cada ferramenta = sem alt-tab entre apps
- **🚀 Escala:** De single-user para enterprise inteiro. Framework extensível (Agentlang).

### TAM
- Enterprise productivity: $50B+
- AI workspace tools: novo mercado estimado em $10B+ até 2027

### Modelo de negócio
- Open-core: community grátis + enterprise (SSO, compliance, SLA)
- Managed cloud: pricing por seat
- Marketplace de AI agents e workflows

### Esforço: Alto
Projeto ambicioso com muitos componentes. Mas fundação sólida (PHP/Laravel backend, React frontend).

---

## crbnos/carbon (#207) — Manufacturing ERP
- **Repo:** https://github.com/crbnos/carbon
- **Stars:** 1.8k | **License:** Open Source
- **Eixos:** 🎯💸🚀

### O que é
ERP open-source especificamente para manufatura:
- ERP + MES (Manufacturing Execution System) + QMS (Quality Management System)
- API-first (Supabase + TypeScript + React)
- Projetado para: assembly complexa, job shops, configure-to-order
- Extensível com apps custom via API

### Problema real
ERPs para manufatura são caríssimos: SAP ($150-300/user/mês), Oracle ($175/user/mês), Epicor ($175/user/mês). Alternativas open-source como ERPNext são genéricas e não atendem complexidade de manufatura real. Carbon nasceu da frustração real de implementadores.

### Por que é 5-10x melhor
- **💸 Custo:** $0 vs $150-300/user/mês de SAP/Oracle. Para fábrica de 50 users = economia de $90k-180k/ano.
- **🚀 Escala:** API-first permite integração com qualquer sistema. Stack moderna (Supabase) vs monolitos legados.
- **🎯 Problema real:** "Vendor lock-in borders on extortion" — citação direta dos criadores.

### TAM
- Manufacturing ERP market: $12B (crescendo 8% YoY)
- SMB manufacturing (target principal): ~$4B
- Job shops nos EUA sozinhos: 30.000+ estabelecimentos

### Modelo de negócio
- Open-core: community grátis + módulos premium (QMS avançado, scheduling, analytics)
- Implementation services: consultoria de deploy ($5-20k por fábrica)
- Managed cloud: $50-100/user/mês (ainda 50%+ mais barato que incumbentes)

### Esforço: Alto
ERP é complexo por natureza. Mas stack moderna e API-first facilita extensão. Comunidade crescendo.
