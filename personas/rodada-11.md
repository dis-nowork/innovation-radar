# 🔭 Rodada 12 — 2026-02-01 | Vida Adulta: Carro, Dinheiro, Documentos, Organização de Grupo

## 🔭 Rodada 12 — 2026-02-01 | Vida Adulta: Carro, Dinheiro, Documentos, Organização de Grupo

> **Ângulo:** Problemas que TODO adulto tem mas resolve com gambiarra — manutenção do carro, rachar conta, assinar documento, agendar reunião, investimentos, feedback de cliente. Ferramentas que existem mas são caras, feias ou complicadas demais.

**Termos pesquisados:** `vehicle maintenance tracker`, `expense splitting group`, `document signing open source`, `personal finance self hosted`, `scheduling poll meeting`, `survey platform open source`, `home inventory`, `portfolio tracker`

---

### 🎯 Achados

| # | Repositório | ⭐ | O que faz |
|---|-------------|-----|-----------|
| 65 | [hargata/lubelog](https://github.com/hargata/lubelog) | 2240 | Rastreador de manutenção veicular e consumo de combustível — self-hosted, bonito, funcional |
| 66 | [spliit-app/spliit](https://github.com/spliit-app/spliit) | ~4000 | Alternativa open-source ao Splitwise — rachar despesas com amigos e família |
| 67 | [docusealco/docuseal](https://github.com/docusealco/docuseal) | ~8000 | Alternativa open-source ao DocuSign — criar, preencher e assinar documentos digitais |
| 68 | [ghostfolio/ghostfolio](https://github.com/ghostfolio/ghostfolio) | ~5000 | Gestão de patrimônio open-source — acompanhar ações, ETFs, crypto com privacidade |
| 69 | [sysadminsmedia/homebox](https://github.com/sysadminsmedia/homebox) | ~3000 | Inventário doméstico — catalogar tudo que você tem em casa com etiquetas e locais |
| 70 | [lukevella/rallly](https://github.com/lukevella/rallly) | ~4000 | Alternativa open-source ao Doodle — enquetes de agendamento para encontrar o melhor horário |
| 71 | [formbricks/formbricks](https://github.com/formbricks/formbricks) | ~9000 | Alternativa open-source ao Qualtrics/Typeform — pesquisas in-app, email e link |

---

### 📋 Avaliação Detalhada

**65. LubeLogger — Manutenção do Carro**
- **Problema real:** Todo dono de carro deveria rastrear trocas de óleo, revisões, consumo de combustível. Ninguém faz. Resolve hoje: caixa de sapato com notas fiscais, ou simplesmente esquece até algo quebrar. 2.240 stars = muita gente sofre com isso.
- **Insight criativo:** O slogan diz tudo: "Nobody should deal with a homemade spreadsheet or a shoebox full of receipts." É um problema universal resolvido por ZERO apps bons e gratuitos. Os que existem são ou feios, ou cheios de ads, ou querem vender seguro.
- **Reposicionamento:** E se não fosse só carro? **"Manutenção de Tudo"** — carro, moto, casa, eletrodomésticos, bicicleta. Qualquer coisa que precisa de manutenção periódica. "O app que te lembra antes de quebrar." Para imobiliárias: rastrear manutenção de TODOS os imóveis da carteira.
- **Combinação:** LubeLogger + Warracker (#59) = **"Vida Útil"** — sabe quando seu carro precisa de revisão E quando a garantia da geladeira vence. Um app que cuida de tudo que estraga.

**66. Spliit — Rachar Despesas**
- **Problema real:** Viagem com amigos, república, casal que divide contas. Todo mundo usa Splitwise, mas ele virou bloatware com ads e paywall. Resolve hoje: planilha do Google, "anota aí que eu te pago depois" (spoiler: nunca paga).
- **Insight criativo:** Free, sem conta obrigatória, PWA que funciona offline. Scan de recibo com IA. O Splitwise começou assim e hoje cobra $3/mês pra funcionalidades básicas. Mercado provado, incumbente gordo.
- **Reposicionamento:** Para repúblicas de estudantes: "República Justa" — divide aluguel + contas + supermercado. Para condomínios pequenos: rachar custos de manutenção sem síndico profissional. Para viagens em grupo: "Tesoureiro de Viagem" — cria grupo, todo mundo loga gastos, no final calcula quem deve o quê.
- **Combinação:** Spliit + Biztro (#62) = **"Mesa Dividida"** — restaurante onde cada pessoa no grupo escaneia o QR, marca o que pediu, e paga sua parte via Pix. Fim da "vamos dividir igual" quando você pediu só uma salada.

**67. DocuSeal — Assinatura Digital**
- **Problema real:** Precisa assinar contrato de aluguel, acordo de freelancer, termo de consentimento. DocuSign cobra $10/mês. Adobe Sign idem. Resolve hoje: imprime, assina, escaneia, manda por email (em 2026!).
- **Insight criativo:** 12 tipos de campo, mobile-optimized, API com webhooks. Self-hosted = dados sensíveis ficam contigo. Para o Brasil: LGPD compliance trivial quando você controla o servidor.
- **Reposicionamento:** Para escolas: autorização de excursão digital. Para personal trainers/academias: termo de responsabilidade. Para fotógrafos: cessão de direito de imagem. Para qualquer MEI: contrato de prestação de serviço bonito e profissional em 2 minutos.
- **Combinação:** DocuSeal + Invio (#60) = **"Freelancer em 5 Minutos"** — cria proposta, cliente aprova e assina, invoice é gerada automaticamente. O fluxo proposta→contrato→cobrança inteiro sem sair do app.

**68. Ghostfolio — Gestão de Patrimônio**
- **Problema real:** Investidor pessoa física tem ações na corretora A, crypto na exchange B, renda fixa no banco C. Ninguém tem visão consolidada. Resolve hoje: planilha Excel atualizada manualmente (quando lembra).
- **Insight criativo:** Privacy-first, PWA, Zen Mode (mostra só o necessário). Suporta ações, ETFs, crypto, fundos. Para o Brasil: poderia integrar com B3 e calcular IR automaticamente.
- **Reposicionamento:** **"IRPF Invest"** — Ghostfolio + cálculo automático de imposto de renda sobre investimentos no Brasil. O problema não é acompanhar patrimônio — é declarar IR sem pagar contador. Cada compra e venda gera um evento fiscal. Se o app já rastreia transações, calcular DARF mensal e gerar declaração anual é extensão natural.
- **Combinação:** Ghostfolio + Maybe Finance (descontinuado, mas conceito vivo) = **"Saúde Financeira Total"** — não só investimentos, mas conta corrente + cartão de crédito + investimentos + dívidas em um lugar. Quanto sobra, quanto cresce, quanto deve.

**69. HomeBox — Inventário Doméstico (fork ativo)**
- **Problema real:** Igual ao NesVentory (#63), mas com comunidade maior e fork mantido ativamente. Catalogar o que você tem, onde está, quanto vale.
- **Insight criativo:** A versão original (hay-kot) foi arquivada mas o fork sysadminsmedia mantém vivo. Subreddit ativo, traduções via Weblate. Prova de que a comunidade QUER isso.
- **Reposicionamento:** Para mudanças: "Lista de Mudança Inteligente" — sabe exatamente quantas caixas, o peso estimado, e o que vai em cada uma. Para quem aluga no Airbnb: inventário do imóvel com fotos e estado de cada item.
- **Combinação:** HomeBox + LubeLogger = **"Vida de Adulto OS"** — tudo que você possui (HomeBox) + tudo que precisa de manutenção (LubeLogger) + tudo que vence (Warracker). O sistema operacional da vida adulta responsável.

**70. Rallly — Enquete de Agendamento**
- **Problema real:** Agendar churrasco com 10 amigos. Ou reunião com 5 colegas. Manda mensagem no grupo: "quando vocês podem?" — 47 mensagens depois, ninguém sabe nada. Doodle funciona mas é feio e cheio de ads.
- **Insight criativo:** Interface linda, sem login obrigatório, self-hostable. O nome é proposital (3 L's). Resolve um problema que TODO ser humano tem e que big tech ignora porque não dá pra monetizar com ads.
- **Reposicionamento:** Para igrejas/comunidades: agendar encontros, escalas de voluntários. Para professores: agendar bancas, reuniões de pais. Para condomínios: agendar uso de churrasqueira/salão de festas.
- **Combinação:** Rallly + Spliit = **"Rolê Perfeito"** — acha o melhor dia pro churrasco (Rallly) + racha os custos depois (Spliit). O app que organiza encontro de amigos de A a Z.

**71. Formbricks — Pesquisas e Feedback**
- **Problema real:** Quer ouvir seus clientes. Typeform cobra $25/mês. Google Forms é feio e limitado. Resolve hoje: "manda um zap perguntando" ou ignora completamente.
- **Insight criativo:** In-app surveys (aparece dentro do seu produto), link surveys, email surveys. Segmentação por comportamento. É a ferramenta que empresas de $100M usam, de graça pra quem tá começando.
- **Reposicionamento:** Para restaurantes: "Como foi sua experiência?" no QR da mesa. Para profissionais de saúde: formulário de anamnese digital bonito. Para professores: avaliação de aula que alunos realmente respondem porque é bonita. Para eventos: NPS pós-evento.
- **Combinação:** Formbricks + Biztro (#62) = **"Restaurante 360"** — cardápio digital + pedido + feedback pós-refeição. O dono do restaurante sabe O QUE vendeu, QUANTO faturou, e SE o cliente gostou.

---

### 🤪 Combinações Malucas

**1. LubeLogger + HomeBox + Warracker + DocuSeal = "Adulting OS"**
→ Um único app que: (a) sabe tudo que você tem (HomeBox), (b) rastreia manutenções de carro/casa (LubeLogger), (c) avisa quando garantias/documentos vencem (Warracker), (d) guarda contratos e assinaturas (DocuSeal). **Resolve:** "ser adulto é lembrar de 500 coisas que ninguém te ensinou" para qualquer pessoa que saiu da casa dos pais. O app que sua mãe queria que existisse quando você foi morar sozinho.

**2. Spliit + Rallly + Formbricks = "Social Planner"**
→ Organizar qualquer evento social: (a) encontra o melhor dia (Rallly), (b) divide os custos (Spliit), (c) coleta feedback depois (Formbricks). **Resolve:** "organizar aniversário/churrasco/viagem é um trabalho não-remunerado que ninguém quer fazer" para o amigo organizador do grupo. Um app que transforma o planejador do grupo em herói com zero esforço.

---

