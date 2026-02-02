# 🧠 AI & Produtividade Pessoal

## khoj-ai/khoj ⭐ 32.4k
**Link:** https://github.com/khoj-ai/khoj
**Eixos:** 🎯💸🚀💎 (4 eixos!)

### Problema Real
Pessoas e empresas têm documentos espalhados (PDFs, Notion, Word, Markdown) e querem buscar/conversar com eles usando AI. Soluções como ChatGPT Plus ($20/mês) ou Perplexity Pro ($20/mês) não acessam seus docs privados. Notion AI cobra $10/mês por membro.

### Por que é 5-10x melhor
- **🎯 Problema real:** Todo knowledge worker precisa de busca semântica nos próprios docs
- **💸 Custo:** Self-hosted = custo de infra apenas. vs $20/mês/usuário dos incumbentes
- **🚀 Escala:** De personal AI (single user) a enterprise (multi-tenant). Funciona com qualquer LLM (local ou cloud)
- **💎 Qualidade:** Agents customizáveis com personalidade, tools e knowledge bases. Deep research mode integrado

### TAM
- Knowledge management: $47B+ (2025)
- AI assistants: $15B+
- Público: Knowledge workers, equipes, consultores, pesquisadores

### Modelo de Negócio
- **Freemium:** App cloud grátis com limites → planos pagos ($10-15/mês)
- **Enterprise:** On-premises + SSO + compliance = $50-200/seat/mês
- **White-label:** API para empresas embutirem AI search em seus produtos

### Esforço para Produtizar: Baixo
Já tem cloud app funcional, Docker compose, enterprise tier. Muito maduro.

### Combinações
- + OpenObserve (monitoring da plataforma)
- + Penpot (docs de design como knowledge base)
- + InvenTree (busca semântica em inventário)

---

## Freika/dawarich ⭐ 7.9k
**Link:** https://github.com/Freika/dawarich
**Eixos:** 🎯💸

### Problema Real
Google matou o Timeline gratuito e mudou para armazenamento on-device. Milhões de pessoas perderam acesso ao histórico de localização. Alternativas pagas não existem — é Google ou nada.

### Por que é 5-10x melhor
- **🎯 Problema real:** Google removeu feature amada. Vácuo de mercado
- **💸 Custo:** Self-hosted = grátis vs dados vendidos ao Google

### TAM
- Location intelligence: $25B+
- Self-hosted apps market: $5B+
- Público: Privacy-conscious users, famílias, viajantes, fotógrafos

### Modelo de Negócio
- **Cloud managed:** Dawarich Cloud (já existe) — hosting fácil por $5-10/mês
- **Patronage:** Ko-fi + Patreon (modelo atual)
- **Enterprise:** Fleet tracking, employee location compliance

### Esforço para Produtizar: Médio
Já tem cloud, mas precisa de mobile app melhor e onboarding mais simples.

---

## fastrepl/hyprnote ⭐ 7.6k
**Link:** https://github.com/fastrepl/hyprnote
**Eixos:** 🎯💸⚡

### Problema Real
Meeting notes são um inferno: ou você toma notas e perde a conversa, ou presta atenção e esquece os detalhes. Ferramentas como Otter.ai ($16.67/mês), Fireflies ($18/mês) e Krisp ($8/mês) resolvem parcialmente, mas:
- Adicionam bots invasivos nas chamadas
- Dependem de cloud (privacidade zero)
- Custo acumula ($100-200/ano por pessoa)

### Como Resolve
- **Captura de áudio local** — ouve som entrando/saindo do computador, sem bot na call
- **Transcrição real-time** com diarização de speakers
- **Notepad integrado** — jota enquanto ouve, AI completa o resto pós-meeting
- **100% offline** via LM Studio ou Ollama
- macOS hoje, Windows/Linux Q1 2026

### Por que é 5-10x Melhor
- **🎯 Problema real:** Todo knowledge worker com >3 reuniões/semana sofre isso
- **💸 Custo:** $0 vs $100-200/ano (Otter/Fireflies)
- **⚡ Velocidade:** Zero setup — instala via brew, não precisa conectar calendário nem integrar

### TAM
- 300M+ knowledge workers globalmente com reuniões regulares
- Mercado de meeting intelligence: ~$3B em 2025
- Freemium → teams → enterprise: modelo provado (Otter faz $100M+ ARR)

### Modelo de Negócio
- Open-core: versão local grátis, cloud sync + team features pagos
- Enterprise: compliance, SSO, admin console

### Esforço para Produtizar: Baixo-Médio
App Tauri pronto, UX polida, falta Windows/Linux + team features

### Combinações
- + meeting-minutes (#144): engine Rust para transcrição + Hyprnote como UI/UX layer
- + open-notebook (#142): resumos de meeting → knowledge base pessoal
