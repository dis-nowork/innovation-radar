# 🏋️ Fitness & Profissionais Solo

> Foco: Personal trainers, nutricionistas, fisioterapeutas — profissionais que gerenciam alunos/pacientes com WhatsApp + planilha.

---

## Oportunidade 1: wger — Plataforma de Treino (Reposicionada)

- **Repo:** [wger-project/wger](https://github.com/wger-project/wger) ⭐ 5.572 | 🍴 ~850
- **O que é:** Tracker de treino/nutrição/peso, self-hosted, feito pro indivíduo
- **Dor que resolve:** Personal trainers criam treinos em PDF ou WhatsApp. O aluno perde. O trainer não tem visibilidade da execução.
- **Gambiarra atual:** Planilha do Google compartilhada, PDF no WhatsApp, apps pagos caros (TrainerHub, Nexur)
- **Por que é não óbvio:** Todos os apps de treino são B2C (focam no aluno). O wger, por ser self-hosted com API REST, pode ser reposicionado como B2B: o **trainer** hospeda e gerencia **todos** os alunos numa única instância.
- **Reposicionamento:** Personal trainer → fisioterapeuta (exercícios de reabilitação), nutricionista (planos alimentares), preparador físico de times amadores
- **Modelo:** SaaS multi-tenant. R$49/mês personal básico, R$149/mês com white-label (app com logo do trainer)
- **Teste dos 10 segundos:** "Um app onde o personal cria treinos e acompanha todos os alunos numa tela só"

---

## Oportunidade 2: EasyAppointments + WhatsApp = Agendamento Automático

- **Repo:** [alextselegidis/easyappointments](https://github.com/alextselegidis/easyappointments) ⭐ 4.029
- **O que é:** Agendador de consultas/sessões, self-hosted, com painel admin
- **Dor que resolve:** Personal trainer passa o DIA respondendo WhatsApp: "tem horário terça?", "posso trocar pra quinta?", "quanto tá a aula?"
- **Gambiarra atual:** Responde um por um no WhatsApp. Alguns usam Google Calendar compartilhado. A maioria só lembra de cabeça.
- **Por que é não óbvio:** Existem mil agendadores. Mas NENHUM se integra nativamente com WhatsApp de forma self-hosted. A combinação EasyAppointments + [evolution-api](https://github.com/EvolutionAPI/evolution-api) (já mapeado na categoria Comunicação) cria um bot que agenda direto na conversa do WhatsApp.
- **Reposicionamento:** Personal trainer → barbeiro, manicure, dentista solo, advogado, psicólogo, qualquer profissional liberal brasileiro que vive no WhatsApp
- **Modelo:** R$29/mês com bot WhatsApp incluso. R$79/mês com cobrança automática (Pix via API)
- **Combinação crítica:** evolution-api + easyappointments + gateway de Pix = o aluno agenda, confirma e paga sem o profissional tocar no celular
- **Teste dos 10 segundos:** "O aluno manda 'quero agendar' no WhatsApp e o bot resolve tudo — horário, confirmação e pagamento"

---

## Oportunidade 3: workout-tracker — Treino Outdoor com Visibilidade Remota

- **Repo:** [jovandeginste/workout-tracker](https://github.com/jovandeginste/workout-tracker) ⭐ 1.192
- **O que é:** Tracker de treino com foco em atividades GPX (corrida, ciclismo, caminhada)
- **Dor que resolve:** Assessorias de corrida online explodiram pós-pandemia. O assessor manda planilha, o aluno corre, e depois manda print do Strava. O assessor fica catando prints em 50 conversas.
- **Gambiarra atual:** Print do Strava no WhatsApp. Assessor monta relatório manualmente em planilha.
- **Por que é não óbvio:** O Strava é social (focado no atleta mostrar pros amigos). Não é ferramenta de TRABALHO do assessor. Esse repo, por ser self-hosted, permite o assessor ter dashboard unificado de TODOS os alunos com métricas reais.
- **Reposicionamento:** Corrida → ciclismo, triathlon, grupos de caminhada para idosos (mercado crescente), reabilitação cardiovascular (fisioterapia)
- **Modelo:** R$39/mês por assessor (até 30 alunos). R$99/mês ilimitado + relatórios automáticos PDF
- **Teste dos 10 segundos:** "O assessor de corrida vê todos os treinos dos alunos num painel só, sem ficar catando print no WhatsApp"

---

## Oportunidade 4: Habitica — Gamificação de Treino por Assinatura

- **Repo:** [HabitRPG/habitica](https://github.com/HabitRPG/habitica) ⭐ 13.642
- **O que é:** Habit tracker gamificado — seus hábitos viram um RPG com XP, níveis, itens
- **Dor que resolve:** A maior dor do personal não é criar treino — é fazer o aluno FAZER o treino. Aderência é o problema #1.
- **Gambiarra atual:** Personal manda mensagem motivacional. Grupo de WhatsApp com fotos. Ranking manual em planilha.
- **Por que é não óbvio:** Habitica é genérico (qualquer hábito). Ninguém fez um Habitica ESPECÍFICO para fitness com o personal como "mestre do jogo". O trainer cria as quests (treinos), o aluno executa e sobe de nível. Rankings entre alunos.
- **Reposicionamento:** Fitness → educação (professor gamifica tarefas), fisioterapia (paciente ganha pontos por fazer exercícios), nutrição (desafios semanais de dieta)
- **Modelo:** Freemium. Grátis para personal com até 5 alunos. R$59/mês ilimitado. R$149/mês com app white-label.
- **Teste dos 10 segundos:** "Seus alunos ganham XP e sobem de nível quando fazem o treino. Ranking entre eles pra criar competição"

---

## Oportunidade 5: BeaverHabits — Check-in Minimalista de Aluno

- **Repo:** [daya0576/beaverhabits](https://github.com/daya0576/beaverhabits) ⭐ 1.654
- **O que é:** Habit tracker minimalista, self-hosted, sem gamificação — só o essencial
- **Dor que resolve:** O personal quer saber: o aluno treinou ou não? Bebeu água? Dormiu bem? Seguiu a dieta? Hoje, descobre só quando o aluno aparece na aula.
- **Gambiarra atual:** Pergunta no WhatsApp. O aluno mente ou esquece de responder.
- **Por que é não óbvio:** Não precisa de app complexo. Um check-in diário de 3 perguntas (treinou? dieta? sono?) compartilhado com o personal já resolve 80% do acompanhamento remoto.
- **Reposicionamento:** Personal → psicólogo (check-in diário de humor), nutricionista (diário alimentar simplificado), médico (acompanhamento pós-operatório)
- **Modelo:** R$19/mês por profissional. Simplicidade é o valor — sem feature creep.
- **Teste dos 10 segundos:** "O aluno marca 3 checkboxes por dia. O personal vê tudo num painel. Acabou."

---

## 🔗 Conexões Inesperadas

### Conexão 1: evolution-api + easyappointments + Pix API = "Secretária Virtual WhatsApp"
**Problema:** Profissionais liberais brasileiros perdem 2h/dia gerenciando agenda pelo WhatsApp
**Produto:** Bot WhatsApp que agenda, confirma, cobra (Pix) e lembra — tudo automático
**Público:** Personal trainers, barbeiros, dentistas solo, psicólogos, advogados
**Por que não existe:** Os agendadores são web-first. O Brasil é WhatsApp-first. Ninguém fez a ponte self-hosted.

### Conexão 2: wger + habitica (conceito) = "Coach RPG"
**Problema:** Aderência ao treino. 70% dos alunos desistem em 3 meses.
**Produto:** Plataforma onde o personal cria treinos (wger) e o aluno os completa num sistema gamificado (XP, ranking, conquistas). O personal vira "mestre" do RPG fitness dos alunos.
**Público:** Personal trainers com público jovem (18-35), academias que querem reter alunos
**Por que não existe:** wger é sério/funcional. Habitica é genérico. Ninguém uniu fitness tracking profissional + gamificação controlada pelo trainer.

---

*Scan: 01/02/2026 — Foco: Personal trainers e profissionais de saúde solo*
