# 🎨 Design Tools & Workflow Frameworks

## onlook-dev/onlook ⭐ 24.6k
**Link:** https://github.com/onlook-dev/onlook
**Eixos:** 🎯⚡💎

### Problema Real
Designers usam Figma ($12-75/editor/mês) para desenhar interfaces, depois devs recriam tudo em código. O "handoff" Figma→código é um buraco negro de produtividade — semanas perdidas traduzindo designs. Bolt.new, Lovable e V0 geram código mas não permitem edição visual precisa.

### Por que é 5-10x melhor
- **🎯 Problema real:** O gap design→código desperdiça milhões de horas/ano globalmente
- **⚡ Velocidade:** Edita diretamente no DOM do browser. Mudanças visuais = código real instantaneamente. Import de Figma e GitHub repos
- **💎 Qualidade:** Editor visual com profundidade de IDE — layers, components, branching, checkpoints. MCP support para AI avançada

### TAM
- Design tools: $15B+
- No-code/low-code: $30B+
- Público: Designers, devs frontend, product managers, agencies

### Modelo de Negócio
- **Freemium:** Editor local grátis → Cloud com deploy, collaboration, domains
- **Teams:** Real-time collaboration + comments = $15-30/seat/mês
- **Enterprise:** Self-hosted + SSO + brand management
- **Marketplace:** Templates, components, MCP plugins

### Esforço para Produtizar: Médio
Ainda em desenvolvimento ativo (🚧). Foco atual em Next.js + Tailwind. Precisa expandir para mais frameworks.

### Combinações
- + Penpot (design de alta fidelidade) → Onlook (implementação visual)
- + GrapesJS (web builder genérico) — público diferente mas complementar

---

## bytedance/flowgram.ai ⭐ 7.6k
**Link:** https://github.com/bytedance/flowgram.ai
**Eixos:** 🎯⚡🚀

### Problema Real
Toda plataforma de AI workflow (Dify, n8n, Langflow) precisa reinventar o canvas de nós + conexões. É complexo: drag & drop, forms, variáveis, layout automático, zoom, mini-mapa. Cada uma gasta meses construindo isso do zero.

### Por que é 5-10x melhor
- **🎯 Problema real:** Devs que querem criar plataformas de workflow gastam 50%+ do tempo no canvas, não na lógica de negócio
- **⚡ Velocidade:** Drop-in framework com canvas, forms, variable scope chain e materiais prontos (LLM, Condition, Code Editor). De meses para dias
- **🚀 Escala:** Da ByteDance — battle-tested em produção. Suporta free layout e fixed layout

### TAM
- Low-code platforms: $30B+
- AI workflow builders (emergente): $5B+ e crescendo rápido
- Público: Empresas construindo AI platforms, SaaS builders, internal tools teams

### Modelo de Negócio
- **Framework play:** O framework é grátis, mas ByteDance vende plataformas construídas com ele
- **Para empreendedores:** Base para criar AI workflow platforms white-label
- **Consulting/Services:** Customizações enterprise

### Esforço para Produtizar: Médio-Alto
É um framework, não um produto final. Precisa de wrapper de produto por cima. Mas isso é oportunidade — quem monta o melhor produto em cima vence.

### Combinações
- FlowGram (canvas) + FastMCP (MCP servers) + modelo LLM = plataforma de AI workflow completa em semanas, não meses
- FlowGram + ActivePieces core = AI automation platform customizável
