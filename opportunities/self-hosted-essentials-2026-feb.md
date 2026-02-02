# 🏠 Self-Hosted Product Essentials (Fev/2026 — Rodada 2)

> Tema: Produtos self-hosted maduros que resolvem problemas reais do dia-a-dia — knowledge management, monitoring, infraestrutura.

---

## 1. karakeep-app/karakeep ⭐ 23.1k
- **Link:** https://github.com/karakeep-app/karakeep
- **Forks:** 1.0k | **Licença:** AGPL-3.0 | **Criado:** Fev/2024

### O que faz
App self-hosted para salvar TUDO — links, notas, imagens — com AI auto-tagging e busca full-text. Substitui Raindrop.io ($5.50/mês), Pocket (descontinuado), e Instapaper ($3/mês).

### Problema Real
Knowledge workers salvam links/notas em 5+ lugares (browser bookmarks, Notion, Pocket, email drafts). Nada tem search decente. Pocket morreu. Raindrop.io cobra por features básicas.

### Eixos de Inovação
- 🎯 **Problema real:** Fragmentação de bookmarks/notas é universal — afeta 100% dos knowledge workers
- 💸 **5-10x menor custo:** $0 vs. $5.50-10/mês (Raindrop Pro, Instapaper, Readwise)
- 💎 **5-10x mais qualidade:** AI auto-tagging + full-text search + imagens vs. bookmarks burros do browser
- 🚀 **5-10x mais escala:** Self-hosted = sem limites, sem vendor lock-in, dados seus

### TAM: $4B+ (personal knowledge management + bookmarking)

### Modelo de Negócio
- **Managed hosting:** $3-5/mês (vs $5.50-10 incumbentes)
- **Team/Enterprise:** $5-8/user/mês com shared collections, SSO
- **AI premium:** Summarization, auto-categorization avançada, knowledge graph
- **Mobile apps:** Premium features no mobile (offline sync, widget)

### Esforço para Produtizar: Baixo
Produto maduro com 23k stars. Precisa de cloud hosting + pricing page.

### Combinações
- Karakeep + Docmost (#134) = Knowledge base pessoal + wiki profissional unificados
- Karakeep + Kreuzberg (#36) = Importa qualquer formato (PDF, PPTX) + AI tagging
- Karakeep + Crawl4AI (#111) = Salva artigos completos com extraction inteligente

---

## 2. glanceapp/glance ⭐ 31.6k
- **Link:** https://github.com/glanceapp/glance
- **Forks:** 1.2k | **Licença:** AGPL-3.0 | **Criado:** Abr/2024

### O que faz
Dashboard self-hosted que agrega todos seus feeds em um lugar — RSS, Reddit, YouTube, weather, monitoring, bookmarks, calendário. Startpage pessoal linda e customizável.

### Problema Real
Informação fragmentada em 10+ apps/sites. Não existe "tela única" que mostre tudo que importa. Google Reader morreu. Feedly cobra $6-12/mês por features premium.

### Eixos de Inovação
- 🎯 **Problema real:** Information overload e fragmentação de feeds afeta todos
- 💸 **5-10x menor custo:** $0 vs. Feedly Pro ($6/mês), Inoreader ($5/mês)
- 💎 **5-10x mais qualidade:** Dashboard visual integrado vs. reader de RSS simples — weather, monitoring, stocks tudo junto
- 🚀 **5-10x mais escala:** Go binary leve, roda em qualquer lugar, extensível

### TAM: $3B+ (RSS readers + personal dashboards + digital wellness)

### Modelo de Negócio
- **Managed hosting:** $2-5/mês com widgets premium
- **Enterprise/Team:** Dashboard de equipe, feeds compartilhados
- **Widget marketplace:** Widgets customizados por integração
- **White-label:** Dashboard customizável para empresas

### Esforço para Produtizar: Baixo
Go binary pronto. Precisa de managed offering e widgets marketplace.

### Combinações
- Glance + Karakeep = Dashboard + save para leitura posterior numa experiência unificada
- Glance + TrendRadar (#251) = Feed pessoal + monitoring de tendências AI-powered
- Glance + Beszel (#215) = Dashboard pessoal + server monitoring em um painel

---

## 3. bluewave-labs/Checkmate ⭐ 9.0k
- **Link:** https://github.com/bluewave-labs/Checkmate
- **Forks:** ~500 | **Licença:** AGPL-3.0 | **Criado:** Abr/2024

### O que faz
Monitoring full-stack self-hosted com visualizações bonitas — uptime, hardware, response times, incidents. Compete com Better Uptime ($20-85/mês), UptimeRobot ($7-54/mês), e Datadog (absurdo).

### Problema Real
Startups e PMEs pagam $50-500/mês em monitoring que muitas vezes é overkill. Alternativas gratuitas são feias ou limitadas.

### Eixos de Inovação
- 🎯 **Problema real:** Monitoring é caro e complexo demais pra maioria das empresas
- 💸 **5-10x menor custo:** $0 vs. $20-500/mês (Better Uptime, Datadog, Pingdom)
- 💎 **5-10x mais qualidade:** Visualizações modernas e bonitas vs. UIs feias de ferramentas legacy

### TAM: $5B+ (monitoring + observability for SMBs)

### Modelo de Negócio
- **Managed hosting:** $10-30/mês (vs $20-85 incumbentes)
- **Enterprise:** Multi-tenant, API, custom integrations, SLA
- **Status page premium:** Branded status pages
- **Alerts add-on:** SMS, phone call, PagerDuty integration

### Esforço para Produtizar: Baixo
Produto funcional. Precisa de managed hosting e advanced features.

### Combinações
- Checkmate + Beszel (#215) = Server monitoring (hardware) + service monitoring (uptime) unificados
- Checkmate + Scanopy (#201) = Auto-discovery de rede + monitoring automático
- Checkmate + Glance = Dashboard pessoal com status dos serviços inline

---

## 4. certimate-go/certimate ⭐ 8.1k
- **Link:** https://github.com/certimate-go/certimate
- **Forks:** ~500 | **Licença:** MIT | **Criado:** Ago/2024

### O que faz
Ferramenta self-hosted de gestão completa do ciclo de vida de certificados SSL — issuance, deployment, renewal tudo visual e automático. Suporta múltiplos provedores cloud.

### Problema Real
SSL certificates são dor de cabeça constante — expiram, precisam renovar manualmente, deploy em múltiplos servidores é tedioso. Certbot é CLI-only e frágil.

### Eixos de Inovação
- 🎯 **Problema real:** 30%+ dos sites sofrem com SSL expiration issues
- ⚡ **5-10x mais rápido:** Setup visual vs. CLI manual do certbot
- 💸 **5-10x menor custo:** $0 vs. DigiCert ($200+/ano) ou managed SSL services
- 🚀 **5-10x mais escala:** De "um cert por vez" pra "gerencie 1000 certs visual"

### TAM: $2B+ (SSL/TLS certificate management)

### Modelo de Negócio
- **Managed service:** $5-20/mês por domínio (vs $50-200 incumbentes)
- **Enterprise:** Multi-team, audit logs, compliance (PCI-DSS)
- **Integration marketplace:** Plugins pra AWS, GCP, Azure, Cloudflare
- **API:** Certificate-as-a-Service pra SaaS companies

### Esforço para Produtizar: Baixo
Produto funcional com UI visual. Precisa de managed offering.

### Combinações
- Certimate + Dokploy (#6) = PaaS com SSL management integrado
- Certimate + Pangolin (#216) = VPN/proxy com certificate automation
- Certimate + 1Panel (#71) = Server management + SSL lifecycle visual

---
