# 💰 Financial Operations & Vertical SaaS Killers (2 fev 2026)

**Tema:** Software de gestão financeira e operacional open-source que substitui ferramentas SaaS caras (QuickBooks, Xero, SAP, Oracle WMS, monday.com).

**Insight central:** O mercado de accounting/ERP/WMS é dominado por software caro, feio e travado em vendor lock-in. A nova geração de ferramentas open-source combina UX moderna + self-hosting + AI para reduzir custos em 10-100x.

---

## 460 — akaunting/akaunting ⭐ 9.6k | 2.8k forks
**Link:** https://github.com/akaunting/akaunting
**O que faz:** Software de contabilidade online completo para pequenas empresas e freelancers. Dashboard, invoices, bills, bank feeds, relatórios, multi-empresa, multi-moeda. Built com Laravel + Vue + Tailwind, API RESTful, App Store modular.

**Problema real:** QuickBooks cobra $30-200/mês. Xero cobra $15-78/mês. FreshBooks $17-55/mês. Empresas pequenas no mundo inteiro gastam $500-2400/ano em contabilidade básica. Em países emergentes (Brasil, Índia, LatAm), isso é proibitivo — muitos usam Excel ou nada.

**Eixos de inovação:** 🎯💸🚀
- 🎯 Resolve: Contabilidade é obrigatória para qualquer negócio, mas ferramentas são caras
- 💸 5-10x menor custo: Self-hosted = $0/mês vs $30-200/mês. App Store gera receita para dev
- 🚀 Escala: De SMBs no primeiro mundo → milhões de micro-negócios em mercados emergentes

**TAM:** $15B+ (global accounting software market, growing 8% YoY)
**Modelo de negócio:** Open-core + App Store (plugins pagos $29-199), hosting gerenciado, white-label para contadores
**Esforço pra produtizar:** Baixo — já é produto maduro com 7+ anos de desenvolvimento
**Combinações:**
- + TaxHacker (#461): Scanning de recibos AI + contabilidade estruturada
- + Lago (#23): Usage-based billing + contabilidade = stack financeira completa
- + Docuseal (#29): Contratos assinados → faturamento automático

---

## 461 — vas3k/TaxHacker ⭐ 1.1k | 140 forks
**Link:** https://github.com/vas3k/TaxHacker
**O que faz:** App de contabilidade self-hosted com AI para freelancers/indies. Upload fotos de recibos, invoices, PDFs → AI extrai automaticamente: nome do produto, valores, itens, datas, merchants, impostos. Conversão automática de moedas (incluindo crypto!), multi-projeto, import/export, categorias customizáveis com prompts AI personalizados.

**Problema real:** Freelancers gastam 5-10h/mês organizando recibos e notas para o contador. Ferramentas como Expensify ($5-12/user/mês), Dext ($30/mês), Shoeboxed ($18-36/mês) cobram por OCR que AI moderna faz melhor. Na época do imposto, é um caos de PDFs e fotos desorganizados.

**Eixos de inovação:** 🎯💎⚡💸
- 🎯 Resolve: Tax filing para freelancers é nightmare — recibos em 10 idiomas, 5 moedas
- 💎 Qualidade: AI (GPT-4/Gemini) extrai dados melhor que OCR tradicional + prompts customizáveis
- ⚡ Velocidade: Foto → dados estruturados em segundos vs horas de data entry manual
- 💸 Custo: Self-hosted + bring-your-own-API-key vs $18-36/mês de SaaS

**TAM:** $2.5B (expense management software) + 60M+ freelancers globais
**Modelo de negócio:** Freemium hosted, enterprise self-hosted, integração com contabilidade
**Esforço pra produtizar:** Médio — early stage, precisa polish e integrações (bank feeds, contadores)
**Combinações:**
- + Akaunting (#460): Receipt scanning → contabilidade completa
- + Midday (#16): Financial OS freelancer + tax automation = stack completa
- + BeeCount: AI receipt + bookkeeping pessoal = finanças pessoais 360°

---

## 462 — mayswind/ezbookkeeping ⭐ 4.1k | 414 forks
**Link:** https://github.com/mayswind/ezbookkeeping
**O que faz:** App de finanças pessoais lightweight, self-hosted, com UI mobile-first (PWA). Suporta: multi-moeda, conversão automática, categorias 2-nível, recurring transactions, location tracking, gráficos analíticos, AI receipt recognition, MCP support. Import/export: CSV, OFX, QFX, QIF, GnuCash, Beancount, Firefly III. Backend em Go (ultra-leve, roda em Raspberry Pi).

**Problema real:** YNAB custa $14.99/mês ($180/ano). Mint foi descontinuado. Apps de finanças pessoais ou são caros (YNAB, Copilot), ou fecharam (Mint), ou são ruins/invasivos (banco apps). Pessoas querem controle simples sobre gastos sem vender dados.

**Eixos de inovação:** 🎯💸
- 🎯 Resolve: Controle financeiro pessoal é necessidade universal — Mint morreu, YNAB é caro
- 💸 5-10x menor custo: $0 vs $180/ano (YNAB). Roda em Raspberry Pi/NAS sem custo de hosting

**TAM:** $1.5B (personal finance software) + 2B+ adultos sem ferramenta de orçamento
**Modelo de negócio:** Freemium cloud, premium features (AI, sync avançado), white-label para bancos
**Esforço pra produtizar:** Baixo — produto maduro, PWA funcional, multi-plataforma
**Combinações:**
- + Actual Budget (#10): Duas abordagens complementares (envelope vs tracking)
- + TaxHacker (#461): Tracking pessoal + organização fiscal = personal finance completa
- + Ghostfolio (#30): Gastos diários + investimentos = wealth management open-source total

---

## 463 — ever-co/ever-gauzy ⭐ 3.5k | 725 forks
**Link:** https://github.com/ever-co/ever-gauzy
**O que faz:** Plataforma de gestão empresarial completa: ERP + CRM + HRM + ATS + PM. Features: time tracking, employee monitoring, onboarding, proposals, invoicing, inventory, equipment sharing, goals/KPI, knowledge base, multi-org. Stack: NestJS + Angular, headless API, multi-tenant.

**Problema real:** Empresas de 10-200 funcionários precisam de 5-8 ferramentas separadas: monday.com ($8-16/user), BambooHR ($8-22/user), Freshdesk ($15-79/user), Harvest ($12/user)... = $50-130/user/mês. Integração entre elas é um pesadelo. SAP/Oracle é para enterprises de 1000+.

**Eixos de inovação:** 🎯💸🚀
- 🎯 Resolve: SMBs pagam $50-130/user/mês em 5+ ferramentas desconectadas
- 💸 5-10x menor custo: Tudo-em-um self-hosted vs $600-1560/user/ano
- 🚀 Escala: De ferramenta individual → plataforma completa que serve todo ciclo de negócio

**TAM:** $50B+ (ERP market) + $15B (HRM) + $15B (project management)
**Modelo de negócio:** Open-core, enterprise license, managed hosting, marketplace de plugins
**Esforço pra produtizar:** Alto — plataforma ambiciosa, muitas features = manutenção complexa
**Combinações:**
- + Twenty CRM (#5): CRM mais polido + ever-gauzy HRM/PM = back-office completo
- + Akaunting (#460): Gauzy operations + Akaunting finance = mini-SAP open-source
- + ActivePieces (#73): Automação de workflows entre módulos

---

## 464 — GreaterWMS/GreaterWMS ⭐ 4.2k | 1.1k forks
**Link:** https://github.com/GreaterWMS/GreaterWMS
**O que faz:** Sistema de gestão de armazém (WMS) completo, originado dos processos de logística da Ford Asia Pacific. Features: inbound/outbound, picking, stock management, barcode scanning, compartilhamento de espaço de armazém, app mobile. Reescrevendo em Rust + Python (Bomiot framework) para v3.0.

**Problema real:** WMS enterprise (SAP WM, Oracle WMS, Manhattan) custa $100k-1M+ de implementação + $5k-50k/mês de licença. Médias empresas de logística, e-commerce e manufatura precisam de WMS mas não podem pagar SAP. Usam Excel ou sistemas caseiros frágeis.

**Eixos de inovação:** 🎯💸🚀
- 🎯 Resolve: Logística/armazém é core de qualquer empresa que vende produtos físicos
- 💸 5-10x menor custo: $0 vs $100k+ implementação + $5-50k/mês
- 🚀 Escala: De Excel → sistema profissional; de 1 armazém → rede de armazéns

**TAM:** $4B (WMS market, growing 15% YoY com e-commerce boom)
**Modelo de negócio:** Enterprise support, customização, SaaS managed, white-label para 3PLs
**Esforço pra produtizar:** Médio-Alto — reescrita Rust em andamento, precisa integrações (Shopify, WooCommerce, etc.)
**Combinações:**
- + Fleetbase (#54): WMS + fleet management = supply chain completa
- + InvenTree (#76): WMS para armazéns + InvenTree para inventário de peças
- + Ever-Gauzy (#463): ERP + WMS = operação física completa

