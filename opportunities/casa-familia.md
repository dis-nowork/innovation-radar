# 🏠 Casa & Família — Gestão Doméstica e Vida Familiar

Ferramentas para simplificar a vida doméstica: receitas, compras, inventário, cuidados com bebês e organização do lar.

---

## 1. Mealie — Gerenciador de Receitas + Planejador de Refeições
⭐ **11.359 stars** | 🍴 Self-hosted | Vue + Python

**Link:** https://github.com/mealie-recipes/mealie

**Dor que resolve:** Famílias perdem receitas favoritas espalhadas em screenshots, links salvos, cadernos. Toda semana a mesma pergunta: "o que vamos comer?" vira 30 minutos de indecisão + compras desorganizadas.

**Como resolvem hoje (gambiarra):** Grupos de WhatsApp com receitas, screenshots no celular, favoritos no browser que nunca mais acham.

**Por que é não óbvio:** Não é "mais um app de receitas" — é um **sistema completo**: importa receita de qualquer URL automaticamente, planeja refeições da semana, e gera lista de compras organizada por seção do supermercado. O combo receita→planejamento→lista é o que faz funcionar.

**Reposicionamento:**
- **Nutricionistas** poderiam usar como plataforma para entregar planos alimentares personalizados aos pacientes
- **Escolas/creches** para planejar cardápio semanal e comunicar aos pais
- **Asilos/casas de repouso** para gestão de dietas especiais

**Modelo de negócio:** SaaS hosted ($5-15/mês família) ou white-label para nutricionistas ($29/mês)

**Combinação:** Mealie + IA generativa = "Manda foto da geladeira, recebe 3 receitas com o que tem + lista do que falta"

---

## 2. Grocy — ERP Doméstico (Estoque, Tarefas, Compras)
⭐ **8.679 stars** | 🏠 Self-hosted | PHP

**Link:** https://github.com/grocy/grocy

**Dor que resolve:** Você abre a geladeira e o iogurte venceu ontem. Compra leite mas já tinha 2 no armário. A pia entupiu mas ninguém lembra quando foi a última manutenção. Caos doméstico.

**Como resolvem hoje (gambiarra):** Lista mental, post-its na geladeira, app de notas genérico.

**Por que é não óbvio:** Se chama "ERP beyond your fridge" — e é sério. Controla estoque de casa (com validade!), gera listas de compras automáticas quando produto fica baixo, gerencia tarefas domésticas recorrentes (limpar filtro do ar condicionado a cada 3 meses), e rastreia equipamentos. É SAP, mas pra casa.

**Reposicionamento:**
- **Repúblicas de estudantes** — dividir compras, tarefas, estoque compartilhado
- **Pequenos restaurantes/food trucks** — gestão de estoque simplificada sem pagar Oracle
- **ONGs/abrigos** — controle de doações e suprimentos

**Modelo de negócio:** App mobile bonito com sync na nuvem ($3-8/mês), versão para pequenos negócios ($19/mês)

**Combinação:** Grocy + scanner de código de barras (BarcodeBody) + IA = "Passa o produto no scanner quando chega, o sistema já sabe a validade, avisa antes de vencer, e sugere receita com o que vai vencer"

---

## 3. BabyBuddy — Rastreador para Pais de Recém-nascidos
⭐ **~3.000+ stars** | 👶 Self-hosted | Python/Django

**Link:** https://github.com/babybuddy/babybuddy

**Dor que resolve:** Pais de recém-nascidos vivem em modo sobrevivência: "quando foi a última mamada?", "quantas fraldas trocou hoje?", "dormiu quantas horas?". Com privação de sono, ninguém lembra nada. Pediatra pergunta padrões e os pais não têm dados.

**Como resolvem hoje (gambiarra):** Anotação em papel, apps pagos tipo Huckleberry ($50/ano), ou simplesmente não rastreia e chuta no pediatra.

**Por que é não óbvio:** Integra com **Home Assistant** e **Alexa** — ou seja, o pai pode dizer "Alexa, registra mamada" enquanto segura o bebê. Tem até integração com balança inteligente para pesar mamadeiras. É nerd? Sim. Funciona? Absurdamente bem. E é 100% privado (seus dados ficam com você, não com uma big tech).

**Reposicionamento:**
- **Creches** — rastrear atividades de múltiplos bebês, gerar relatórios para pais
- **Cuidadores de idosos** — mesma lógica (medicação, alimentação, sono)
- **Pet daycares** — rastrear alimentação, brincadeiras, medicação de animais

**Modelo de negócio:** App mobile polido com sync ($4/mês), versão creche/daycare ($15/mês por unidade)

**Combinação:** BabyBuddy + IA preditiva = "Baseado nos últimos 7 dias, seu bebê provavelmente vai acordar às 3h20 — se alimentar agora às 22h, pode ganhar +40min de sono"

---

## 4. HomeBox — Inventário Doméstico
⭐ **~7.000+ stars** | 📦 Self-hosted | Go + Vue

**Link:** https://github.com/sysadminsmedia/homebox

**Dor que resolve:** "Onde coloquei o carregador extra?", "A garantia da TV venceu?", "Quanto gastei em eletrônicos esse ano?". Ninguém sabe o que tem em casa, onde está, ou quanto vale.

**Como resolvem hoje (gambiarra):** Não resolvem. Compram duplicatas por não achar coisas. Perdem garantias. Não sabem o valor total dos bens para seguro.

**Por que é não óbvio:** Parece "inventário de nerd", mas o killer feature é **seguro residencial**. Qualquer pessoa que tem seguro precisa listar bens e valores em caso de sinistro. HomeBox faz isso automaticamente + organiza por cômodo + rastreia garantias + mantém recibos. É literalmente dinheiro economizado quando algo dá errado.

**Reposicionamento:**
- **Imobiliárias/Airbnb** — inventário de imóveis mobiliados com fotos
- **Empresas pequenas** — controle de patrimônio/ativos simplificado
- **Mudanças** — catalogar tudo antes de mudar, verificar se chegou tudo

**Modelo de negócio:** App com OCR de notas fiscais ($5/mês), versão Airbnb/imobiliária ($12/mês por imóvel)

---

## 5. social-to-mealie — Importador de Receitas de Redes Sociais
⭐ **155 stars** | 🔗 Bridge tool | Node.js

**Link:** https://github.com/GerardPolloRebozado/social-to-mealie

**Dor que resolve:** Você vê um Reel/TikTok de receita incrível. Salva. Nunca mais acha. Ou acha mas precisa assistir o vídeo inteiro de novo pra lembrar os ingredientes. Receitas de vídeo são impossíveis de seguir na cozinha.

**Como resolvem hoje (gambiarra):** Salvam o vídeo, tentam transcrever manualmente, ou desistem e pedem pizza.

**Por que é não óbvio:** Usa **IA (Whisper + GPT)** pra transcrever o vídeo, extrair ingredientes e passos, e importar direto pro Mealie formatado como receita. Funciona com Instagram, TikTok, YouTube Shorts, Facebook, Pinterest. Tem até atalho pra iOS (compartilha → vira receita).

**Reposicionamento:**
- **Qualquer tipo de "vídeo tutorial → texto estruturado"**: aulas de yoga, tutoriais de maquiagem, DIY
- **Criadores de conteúdo** — transcrever seus próprios vídeos em posts de blog automaticamente
- **Educação** — converter videoaulas em material escrito acessível

**Modelo de negócio:** Plugin/extensão de browser ($3/mês) que funciona com qualquer rede social + qualquer tipo de conteúdo, não só receitas

---

## 6. KitchenOwl — Lista de Compras Inteligente + Receitas
⭐ **3.036 stars** | 🦉 Self-hosted | Flutter + Flask

**Link:** https://github.com/TomBursch/kitchenowl

**Dor que resolve:** A lista de compras da família é um caos — cada pessoa adiciona coisas em apps diferentes, ninguém sincroniza, alguém compra algo que já tem, e a receita do jantar precisa de 3 coisas que ninguém lembrou de anotar.

**Como resolvem hoje (gambiarra):** Lista no WhatsApp da família, Google Keep compartilhado, gritar da cozinha "compra leite!".

**Por que é não óbvio:** É **Flutter** (mobile-first, funciona offline) com lista compartilhada em tempo real. Mas o diferencial é a integração: escolhe receitas → ingredientes vão automaticamente pra lista → lista organizada por seção do supermercado. Família inteira no mesmo app. Simples, rápido, sem fricção.

**Reposicionamento:**
- **Repúblicas estudantis** — lista compartilhada com divisão de custos
- **Personal chefs/nutricionistas** — montar listas de compras para clientes
- **Cuidadores** — compras organizadas para idosos que moram sozinhos

**Modelo de negócio:** App mobile freemium (grátis até 2 pessoas, $3/mês família ilimitada), versão nutricionista com branding ($15/mês)

---

*Adicionado em: 2026-02-01 | Ângulo: Pais & Famílias — organização doméstica*
