# Physical World Software & Infrastructure Primitives (02 Fev 2026, noite #2)

## Tema: Indústrias offline massivas + infra que habilita novos modelos

---

## 436. funstory-ai/BabelDOC ⭐ 7.6k
**Link:** https://github.com/funstory-ai/BabelDOC
**Eixos:** 🎯💸💎⚡

### Problema Real
Pesquisadores, estudantes e profissionais precisam ler papers e documentos em idiomas que não dominam. Tradução de PDF científico é um pesadelo: Google Translate perde formatação, equações, tabelas. Serviços como DocTranslator cobram $15-30/doc. Pesquisadores chineses, japoneses, coreanos, brasileiros sofrem diariamente.

### Por que é 5-10x melhor
- **🎯 Problema:** ~7M papers publicados/ano + bilhões de docs corporativos. Nenhuma solução preserva layout + traduz bem.
- **💸 Custo:** Grátis (self-hosted) vs $15-30/doc. 1000 páginas grátis na versão online.
- **💎 Qualidade:** Preserva equações LaTeX, tabelas, imagens, layout. Visão bilíngue lado-a-lado (original+tradução). Integração com Immersive Translate.
- **⚡ Velocidade:** Pipeline automatizado vs copiar-colar manual.

### TAM
- Translation services market: $65B+
- Academic publishing: ~7M papers/ano ($10B+ market)
- Corporate document translation: $15B+
- Público-alvo imediato: 50M+ pesquisadores + estudantes de pós-graduação

### Modelo de Negócio
- **Freemium SaaS:** X páginas grátis/mês, planos $10-50/mês
- **API:** $0.01-0.05/página para integração em plataformas acadêmicas
- **Enterprise:** Tradução de documentação técnica em volume
- **Já tem SaaS:** Integrado ao Immersive Translate (>1M users)

### Esforço: Baixo
Já tem produto online + API + CLI. Monetização via volume pricing.

### Combinações
- + pdf-craft (#441): Scanned book → OCR → tradução → EPUB bilingue
- + DeepTutor (#419): Upload paper em qualquer idioma → tutor inteligente

---

## 437. droidrun/droidrun ⭐ 7.6k
**Link:** https://github.com/droidrun/droidrun
**Eixos:** 🎯⚡🚀

### Problema Real
Automatizar ações em celular é uma necessidade massiva: testes de QA, onboarding automatizado, acessibilidade para idosos, RPA mobile. Appium é complexo, requer programação. Ferramentas pagas (Test.ai, Functionalize) custam $500-2k/mês. Usuários normais não conseguem automatizar tarefas repetitivas no celular.

### Por que é 5-10x melhor
- **🎯 Problema:** 6B+ smartphones, nenhuma forma simples de automatizar tarefas. "Siri/Google Assistant" fazem pouco.
- **⚡ Velocidade:** NL → ação. "Reserve um Airbnb em Lisboa para março" vs escrever scripts Appium.
- **🚀 Escala:** De devs que sabem Appium → qualquer pessoa com linguagem natural. Multi-LLM (OpenAI/Anthropic/Gemini/Ollama/DeepSeek).

### TAM
- Mobile testing market: $7B+ (crescendo 15%/ano)
- RPA market: $12B+ (UiPath, Automation Anywhere)
- Digital accessibility: $30B+
- Consumer automation: Nascente mas enorme

### Modelo de Negócio
- **Developer SDK:** Grátis open-source, Pro com analytics/tracing ($20/mês)
- **Enterprise:** QA automation fleet + reporting ($500/mês/team)
- **Consumer app:** "Automate your phone" app com templates ($5-10/mês)
- **API as a service:** Mobile automation-as-a-service

### Esforço: Médio
Framework funcional. Gap: iOS support (em progresso), consumer-friendly UI, cloud fleet management.

### Combinações
- + Open-AutoGLM (#418): Phone agent completo (Android+iOS+Harmony)
- + browser-use (#1): Web + Mobile automation unificada

---

## 438. useplunk/plunk ⭐ 4.8k
**Link:** https://github.com/useplunk/plunk
**Eixos:** 🎯💸🚀

### Problema Real
Email marketing/transacional é essencial para todo negócio, mas caro. SendGrid: $20-500/mês. Resend: $20-100/mês. Mailgun: similar. Startups e pequenos negócios gastam $200-5000/ano só em email. Diferente de listmonk (#14) que é só newsletter, Plunk faz TUDO: transacional + campaigns + automations.

### Por que é 5-10x melhor
- **🎯 Problema:** Todo SaaS precisa de email. É custo recorrente que escala com growth.
- **💸 Custo:** AWS SES = $0.10/1000 emails vs SendGrid $0.001/email. Plunk = self-hosted wrapper sobre SES.
- **🚀 Escala:** De pagar por email → custo quase zero por email. Automations + segmentation + analytics inclusos.

### TAM
- Email marketing: $12B+
- Transactional email: $5B+
- Total addressable: $17B+ (growing 10%/year)

### Modelo de Negócio
- **Open core (AGPL):** Self-hosted grátis
- **Cloud hosted:** $10-100/mês (Plunk Cloud)
- **Enterprise:** Dedicated infrastructure, compliance, SSO
- **Addons:** Templates marketplace, integration marketplace

### Esforço: Baixo
Produto maduro com UI, API, workflows. Monetização clara via hosted version.

### Combinações
- + BillionMail (#87): Plunk (transacional + campaigns) + BillionMail (mail server)
- + chatwoot (#7): Atendimento omnichannel + email marketing unificado

---

## 439. opencloud-eu/opencloud ⭐ 4.7k
**Link:** https://github.com/opencloud-eu/opencloud
**Eixos:** 🎯💸💎

### Problema Real
Google Drive, Dropbox, OneDrive = data em servidores americanos. Com GDPR, NIS2, e regulações globais, empresas europeias (e de qualquer país com leis de proteção de dados) PRECISAM de alternativas soberanas. Nextcloud existe mas é pesado, complexo, e monolítico. OpenCloud é Go-based, no-database (filesystem), e muito mais leve.

### Por que é 5-10x melhor
- **🎯 Problema:** Soberania digital é mandatória em EU, Brasil (LGPD), e outros. Multis+ empresas.
- **💸 Custo:** Self-hosted grátis vs $6-18/user/mês (Google Workspace/M365).
- **💎 Qualidade:** Go backend = leve e rápido. No database = zero manutenção. Apache 2.0 = sem vendor lock.

### TAM
- Enterprise file sharing: $15B+
- Cloud storage: $100B+
- Sovereign cloud (EU): $10B+ (crescendo 30%/ano com regulação)

### Modelo de Negócio
- **Open core (Apache 2.0):** Self-hosted grátis, enterprise features pagas
- **Managed hosting:** $5-15/user/mês
- **Compliance packages:** GDPR, NIS2, HIPAA certifications
- **Integrations:** App marketplace

### Esforço: Médio
Early stage mas com equipe EU dedicada e funding. Precisa: mobile apps, integrations, enterprise features.

### Combinações
- + documenso (#17): File management + assinatura digital = suite documental soberana
- + PandaWiki (#193): Knowledge base + file management = intranet completa

---

## 440. oomol-lab/pdf-craft ⭐ 4.8k
**Link:** https://github.com/oomol-lab/pdf-craft
**Eixos:** 🎯💎⚡💸

### Problema Real
Milhões de livros escaneados (Internet Archive, bibliotecas universitárias, acervos pessoais) estão presos em PDF imagem — sem busca, sem cópia, sem acessibilidade. OCR genérico (Tesseract) falha em tabelas, equações, footnotes. Serviços profissionais (ABBYY) custam $100-500/ano. pdf-craft usa DeepSeek OCR para converter scanned books em Markdown/EPUB com estrutura preservada.

### Por que é 5-10x melhor
- **🎯 Problema:** 130M+ livros já publicados, maioria só em PDF scan. Pesquisadores, estudantes, bibliófilos sofrem.
- **💎 Qualidade:** DeepSeek OCR para tabelas, equações LaTeX, footnotes. TOC gerado automaticamente. Output limpo.
- **⚡ Velocidade:** GPU-accelerated, 100% local. Sem LLM na v1.0 = muito mais rápido.
- **💸 Custo:** Grátis + local vs ABBYY $100+/ano.

### TAM
- OCR software: $13B+ (growing 14%/year)
- Digital publishing/ebook: $20B+
- Academic digitization: $5B+
- Accessibility (leis de acessibilidade): Mandatório em muitos países

### Modelo de Negócio
- **SaaS:** Online converter (já tem demo). Pay-per-page ou subscription.
- **API:** Integração com libraries, publishers, universities
- **Enterprise:** Batch digitization para editoras e universidades
- **Bundled com EPUB stores:** Converter + vender ebooks remasterizados

### Esforço: Baixo-Médio
Produto funcional com demo online. Precisa: scaling, API robusta, batch processing.

### Combinações
- + BabelDOC (#436): Scanned book → OCR → tradução bilíngue → EPUB
- + LEANN (#195): Livro digitalizado → indexado no RAG pessoal → searchable knowledge base
- + DeepTutor (#419): Livro scan → OCR → upload → AI tutor

---

## 441. farmOS/farmOS ⭐ 1.2k
**Link:** https://github.com/farmOS/farmOS
**Eixos:** 🎯💸🚀

### Problema Real
570M fazendas no mundo, maioria gerenciando operações em papel, WhatsApp e planilhas. Software agrícola (Granular, FarmLogs, AgriWebb) custa $500-5000/ano. Fazendas familiares (80% do total mundial) não podem pagar. farmOS é o ÚNICO farm management system open-source maduro, com backing de Cornell University, USDA, e Vermont.

### Por que é 5-10x melhor
- **🎯 Problema:** 570M fazendas, <5% usam software dedicado. Gap absurdo.
- **💸 Custo:** Grátis vs $500-5000/ano. Hosting via Farmier = affordable.
- **🚀 Escala:** De nicho americano → global. Suporta qualquer tipo de fazenda. API aberta.

### TAM
- Farm management software: $4B+ (growing 12%/year)
- Precision agriculture: $12B+
- Global agriculture: $10T+ industry

### Modelo de Negócio
- **Managed hosting (Farmier):** $10-50/mês (já existe)
- **Enterprise/coop:** Custom modules, integrations com IoT, ERP agrícola
- **Data marketplace:** Aggregated farm data (anonymized) para seguradoras, governo
- **Government contracts:** Compliance reporting (USDA, EU CAP)
- **IoT integration:** Sensores + Farm-Data-Relay-System + farmOS

### Esforço: Médio
Produto maduro (10+ anos). Precisa: mobile app moderna, AI features, IoT dashboard. Drupal-based (arquitetura pesada).

### Combinações
- + Fields2Cover (745⭐): Path planning para veículos autônomos + gestão de fazenda
- + microsoft/farmvibes-ai (830⭐): ML geoespacial + farm records
- + kepler.gl (#19): Visualização geoespacial das áreas plantadas

---

## Insights Estratégicos

### Insight: "Software de Trilhões" — as indústrias que GitHub ignora são as maiores oportunidades
**Padrão:** Agricultura ($10T), construção ($13T), imobiliário ($3.6T), saúde ($10T) — juntas representam >$35 trilhões. No GitHub, os melhores repos dessas áreas têm 500-1200 stars. Compare com yet-another-todo-app frameworks com 10k+.

**Por que importa:** O gap entre tamanho do mercado e atenção dos developers é absurdamente grande. farmOS (1.2k⭐) endereça um mercado de $4B+. microrealestate (1.0k⭐) endereça $30B+. Qualquer startup que pegue um desses repos e construa uma UX moderna + AI features + mobile app tem vantagem de 5-10 anos.

**Gap MASSIVO:** Ninguém combinou AI + esses repos de vertical software. Imagina: farmOS + satellite imagery AI + weather prediction + yield optimization = "Precision Farm OS" — vale $1B+. Ou: microrealestate + AI tenant screening + smart pricing + maintenance prediction = "Smart Landlord OS" — outro $1B+.

### Insight: "Document Processing Pipeline" está se completando — de scan a knowledge
**Padrão:** pdf-craft (#440) converte scan→text. BabelDOC (#436) traduz. LEANN (#195) indexa em RAG. DeepTutor (#419) responde perguntas. dots.ocr (#363) faz layout parsing. Cada um resolve um pedaço. Juntos formam: **Scanned Book → OCR → Translate → Index → AI Tutor**.

**Por que importa:** Isso democratiza acesso ao conhecimento global. Um estudante brasileiro pode pegar um textbook japonês escaneado, converter para EPUB, traduzir para português, indexar no RAG pessoal, e ter um tutor AI que responde perguntas citando o livro. Custo: $0. Antes: impossível.

**Oportunidade de $10B:** Quem montar este pipeline como produto (upload PDF → "conhecimento pronto") captura o mercado de educação + pesquisa + treinamento corporativo. É a "Netflix do conhecimento técnico" — acesso a qualquer livro/paper em qualquer idioma, com AI tutor incluído.
