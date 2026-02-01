# 🔭 Rodada 13 — 2026-02-01 | Família, Corpo, Despensa e Condomínio

## 🔭 Rodada 13 — 2026-02-01 | Família, Corpo, Despensa e Condomínio

> **Ângulo:** Problemas de famílias inteiras — não de indivíduos. Bebês, receitas, academia, saúde pessoal, gestão de condomínio. Nichos onde as soluções existem mas são ruins, caras, ou ignoram quem mais precisa.

**Termos pesquisados:** `babybuddy`, `grocy`, `mealie`, `wger workout`, `fasten health`, `endurain fitness`, `open condo property management`, `family organizer`

---

### 🎯 Achados

| # | Repositório | ⭐ | O que faz |
|---|-------------|-----|-----------|
| 72 | [babybuddy/babybuddy](https://github.com/babybuddy/babybuddy) | 2649 | Rastreador de bebê — sono, mamadas, fraldas, tempo de barriga. Ajuda pais a prever necessidades |
| 73 | [grocy/grocy](https://github.com/grocy/grocy) | 8679 | ERP doméstico — gestão de despensa, validades, lista de compras, tarefas e receitas |
| 74 | [mealie-recipes/mealie](https://github.com/mealie-recipes/mealie) | 11359 | Gerenciador de receitas + planejador de refeições + lista de compras. Importa receitas por URL |
| 75 | [wger-project/wger](https://github.com/wger-project/wger) | 5566 | Gerenciador de treinos, nutrição e peso — tracker fitness completo com API REST |
| 76 | [fastenhealth/fasten-onprem](https://github.com/fastenhealth/fasten-onprem) | 2590 | Agregador de prontuário médico pessoal/familiar — conecta com hospitais, seguros, clínicas |
| 77 | [endurain-project/endurain](https://github.com/endurain-project/endurain) | 1726 | Alternativa self-hosted ao Strava — tracking de corrida/ciclismo com controle total dos dados |
| 78 | [open-condo-software/condo](https://github.com/open-condo-software/condo) | 299 | SaaS open-source de gestão de condomínio — chamados, moradores, pagamentos, marketplace de serviços |
| 79 | [actualbudget/actual](https://github.com/actualbudget/actual) | 24626 | Finanças pessoais local-first — orçamento por envelope, sync entre devices, importação bancária |

---

### 📋 Avaliação Detalhada

**72. BabyBuddy — Rastreador de Bebê**
- **Problema real:** Pais de recém-nascido estão exaustos e precisam rastrear mamadas, fraldas, sono — pra identificar padrões e prever necessidades. Resolve hoje: anotando no celular, perguntando pro parceiro "que horas foi a última mamada?", ou simplesmente não rastreando e adivinhando.
- **Insight criativo:** 2.649 stars + integração com Home Assistant + hardware dedicado (BabyPod, keypads ESP32). Isso prova que pais tech-savvy QUEREM dados sobre seus bebês. Mas o mercado real é 100x maior: TODOS os pais de primeira viagem estão perdidos.
- **Reposicionamento:** O BabyBuddy é para geeks. E se fizesse uma versão "Meu Bebê" com UX de TikTok? Ao invés de dashboard, **stories diárias**: "Hoje o João dormiu 2h a mais que ontem 🎉" e "Padrão detectado: ele mama mais às terças 🍼". Transforma dados frios em narrativa emocional. Pediatra recebe relatório bonito no WhatsApp antes da consulta.
- **Combinação:** BabyBuddy + Mealie (#74) = **"Família 0-3 Anos"** — rastreia o bebê E planeja as refeições da casa (porque pais de recém-nascido não têm tempo pra pensar em jantar). Sugere receitas rápidas baseadas no nível de sono dos pais.

**73. Grocy — ERP da Casa**
- **Problema real:** Comida vencendo na geladeira. Comprar o que já tem. Esquecer de comprar o que falta. Resolve hoje: abrindo a geladeira e cheirando, ou mandando foto pelo WhatsApp "a gente tem leite?".
- **Insight criativo:** 8.679 stars e subreddit ativo. O conceito é genial: ERP para casa. Mas a execução peca na UX — é pensado para quem gosta de scanear barcodes. O usuário real quer falar "acabou o leite" pro celular e pronto.
- **Reposicionamento:** **"Despensa Inteligente"** — versão simplificada com foco em 3 dores: (1) "o que tá vencendo?" com notificação, (2) "o que preciso comprar?" com lista automática, (3) "o que posso cozinhar com o que tenho?" conectado ao Mealie. Para o Brasil: integração com apps de supermercado (iFood Market, Rappi) = compra direto da lista.
- **Combinação:** Grocy + LubeLogger (#65) = **"Manutenção de Tudo"** — a geladeira vence, o óleo do carro vence, o filtro de água vence. UM app que sabe tudo que precisa ser trocado/reposto na sua vida.

**74. Mealie — Receitas + Planejamento de Refeições**
- **Problema real:** "O que vamos comer hoje?" é a pergunta mais repetida da humanidade. Resolve hoje: perguntando no grupo do WhatsApp, abrindo o iFood, ou comendo a mesma coisa de sempre.
- **Insight criativo:** 11.359 stars (!) — é um dos repos self-hosted mais populares que existe. Importar receita por URL é killer feature. Mas o planejamento de refeições ainda é manual. O salto: IA que conhece suas preferências, restrições alimentares, orçamento, e o que tem na despensa (Grocy) e SUGERE o cardápio da semana.
- **Reposicionamento:** Para nutricionistas — "monte o plano alimentar do paciente em 5 min" ao invés de planilha Excel. Para escolas/creches — "cardápio semanal que atende 300 crianças com restrições diferentes". Para personal chefs — "cardápio personalizado para cada cliente".
- **Combinação:** Mealie + Grocy + Actual (#79) = **"Vida Doméstica OS"** — sabe o que tem na despensa (Grocy), sugere o que cozinhar (Mealie), e calcula quanto você gasta em comida por semana (Actual). O triângulo mágico: despensa→receita→orçamento.

**75. wger — Fitness Tracker Completo**
- **Problema real:** Quem treina na academia precisa anotar exercícios, séries, peso. Apps como Strong cobram $5/mês. Resolve hoje: bloco de notas do celular, planilha, ou memória ("acho que fiz 3x12 com 40kg semana passada...").
- **Insight criativo:** 5.566 stars, apps mobile reais (Android/iOS/F-Droid), exercício wiki, nutrição integrada. É basicamente o que Strong/Hevy cobram, mas grátis e self-hosted. O gap: não tem inteligência — não sugere progressão, não detecta platô, não adapta treino.
- **Reposicionamento:** **"Personal Trainer de Bolso"** — wger como base de dados + IA que analisa seus logs e diz: "Você não aumentou peso no supino há 4 semanas. Tenta mudar pra inclinado." Para academias pequenas: o dono da academia dá acesso ao sistema pros alunos, vira diferencial competitivo vs. Smart Fit.
- **Combinação:** wger + Endurain (#77) = **"Corpo Total"** — treinos na academia (wger) + corrida/bike ao ar livre (Endurain) em UM lugar. Hoje quem corre E treina musculação precisa de 2 apps. Ninguém quer isso.

**76. Fasten Health — Prontuário Pessoal**
- **Problema real:** Seu histórico médico está espalhado em 10 clínicas, 3 seguros, e 2 hospitais. Quando você precisa (emergência, novo médico, viagem), não tem nada organizado. Resolve hoje: pasta de exames no Google Drive, ou "vou pedir pro outro médico mandar".
- **Insight criativo:** Self-hosted, agrega dados de múltiplos provedores automaticamente via integração. O criador fez porque teve um problema médico sério e percebeu que NINGUÉM tem controle do próprio histórico. 2.590 stars = dor real comprovada.
- **Reposicionamento:** Para famílias com idosos — **"Saúde da Família"** — filhos cuidam dos pais à distância. Prontuário do pai/mãe/avó em um lugar, com alertas de medicamentos e próximas consultas. Para expatriados: leva seu histórico médico de um país pro outro sem depender de burocracia.
- **Combinação:** Fasten Health + BabyBuddy (#72) = **"Ciclo de Vida"** — começa rastreando o bebê (mamadas, vacinas), evolui para o prontuário infantil, depois adolescente, adulto, e eventualmente cuidado de idosos. UM app de saúde que acompanha a pessoa do nascimento à velhice. A família inteira num só sistema.

**77. Endurain — Strava Alternativo**
- **Problema real:** Corredores e ciclistas usam Strava, mas o plano gratuito foi castrado. Funções básicas agora são pagas ($5/mês). Resolve hoje: paga o Strava e reclama, ou usa Garmin Connect (feio).
- **Insight criativo:** 1.726 stars e crescendo rápido. Integra com Strava E Garmin Connect (importa dados). Suporta .gpx, .tcx, .fit. Privacy-first. É o tipo de projeto que cresce quando o incumbente fica ganancioso — e o Strava tá fazendo exatamente isso.
- **Reposicionamento:** Para corridas e provas locais — "Cronômetro de Corrida Comunitária". Organizador de prova de 5km de bairro usa Endurain como plataforma: atletas veem seus tempos, rotas, evolução. Sem precisar de chip caro. Para assessorias de corrida: personal de corrida acompanha todos os alunos em um painel.
- **Combinação:** Endurain + Rallly (#70, enquete de agendamento) = **"Pelotão"** — grupo de corrida que combina o melhor horário (Rallly), corre junto (Endurain rastreia), e depois compara tempos e evolução. Social fitness para grupos locais.

**78. Condo — Gestão de Condomínio**
- **Problema real:** Gestão de condomínio no Brasil é um CAOS. Síndico gerencia na planilha, morador reclama no grupo do WhatsApp, ata de assembleia é papel. Resolve hoje: sistema proprietário caro (Superlógica, TownSq ~R$3-5/unidade/mês) ou planilha + WhatsApp.
- **Insight criativo:** Open-source com tickets, contatos de moradores, rastreamento de pagamentos, marketplace de serviços e sistema de mini-apps. Bem arquitetado. O gap no Brasil: condomínios pequenos (10-30 unidades) não têm orçamento pra software pago, mas têm TODOS os mesmos problemas.
- **Reposicionamento:** **"Meu Condomínio"** — versão brasileira simplificada: (1) livro de ocorrências digital, (2) reserva de salão/churrasqueira (Rallly-style), (3) comunicados do síndico, (4) boleto e prestação de contas, (5) votação digital em assembleia. Cobra R$1/unidade/mês e atende 100 mil condomínios pequenos que ninguém serve.
- **Combinação:** Condo + Formbricks (#71, pesquisas) = **"Condomínio Democrático"** — morador vota em melhorias, responde pesquisas de satisfação, síndico tem dados reais pra tomar decisões. Fim do "quem grita mais na assembleia decide."

**79. Actual Budget — Finanças Pessoais Local-First**
- **Problema real:** Controlar dinheiro. O problema mais universal da humanidade depois de "o que comer". Resolve hoje: não controla (maioria), planilha (minoria dedicada), ou apps como Mobills/Organizze que querem seus dados bancários.
- **Insight criativo:** 24.626 stars (!!) — É o 2º repo de finanças mais popular do GitHub. Local-first = seus dados nunca saem do seu dispositivo. Método envelope = orçamento por categorias. Sync entre devices. Importação bancária. Isso é Mint/YNAB grátis e privado.
- **Reposicionamento:** **"Finanças de Casal"** — a maioria dos apps de finanças é individual. Mas casais têm contas conjuntas E individuais. Actual já suporta isso mas não posiciona assim. O produto: "cada um vê seus gastos + juntos veem o orçamento da casa". Para famílias: mesada dos filhos como sub-orçamento. Para repúblicas: funciona como Spliit (#66) mas com visão mensal.
- **Combinação:** Actual + Ghostfolio (#68) + Grocy (#73) = **"Dinheiro da Família"** — orçamento do dia-a-dia (Actual) + investimentos de longo prazo (Ghostfolio) + quanto gasta em comida (Grocy). A visão COMPLETA das finanças familiares: ganha, gasta, investe, come.

---

### 🤪 Combinações Malucas

**1. BabyBuddy + Mealie + Grocy + Actual = "FamilyOS — O Sistema Operacional da Família"**
→ Um hub que: (a) rastreia o bebê (sono, mamadas, vacinas — BabyBuddy), (b) planeja o que comer (Mealie), (c) sabe o que tem na despensa e o que comprar (Grocy), (d) controla o orçamento familiar (Actual). **Resolve:** "ser família é gerenciar 50 coisas sem nenhum sistema" para qualquer casal com filhos pequenos. Cada módulo é opcional — começa com o que precisa, adiciona conforme a vida complica. É o ERP que toda família precisa mas nunca teve.

**2. Fasten Health + wger + Endurain = "Saúde 360°"**
→ Prontuário médico completo (Fasten) + treinos e nutrição (wger) + atividades ao ar livre (Endurain). **Resolve:** "meu médico não sabe que eu corro 3x por semana e meu personal não sabe que tenho hérnia de disco" para qualquer pessoa que se exercita e vai ao médico. Na consulta, o médico vê não só exames, mas hábitos reais: sono, exercício, nutrição. Decisão médica informada por dados de vida real, não por "como você se sente?".

---
