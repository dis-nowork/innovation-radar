# 🛠️ DevTools

Extração documental, geração de código, TTS, MCP tooling, coding agents.

### [kreuzberg-dev/kreuzberg](https://github.com/kreuzberg-dev/kreuzberg) ⭐ 5.7k | 🎯⚡💸
**Problema:** Extrair texto de PDFs, imagens, DOCX, etc. exige múltiplas libs e muita gambiarra.
**Solução:** Uma lib Python que extrai texto de 50+ formatos com OCR embutido (Rust = rápido).
**Por que é superior:** ⚡ Rust backend = 5x mais rápido que PyPDF. 💸 Grátis vs APIs pagas de OCR. 🎯 Todo pipeline de dados precisa.

---

### [enoch3712/ExtractThinker](https://github.com/enoch3712/ExtractThinker) ⭐ 1.5k | 🎯⚡
**Problema:** Extrair dados estruturados de contratos/faturas exige regex frágil ou trabalho manual.
**Solução:** ORM para documentos: define schema, LLM extrai os campos. Contratos viram queries.
**Por que é superior:** ⚡ Horas de regex → minutos com schema. 🎯 Toda empresa processa documentos.

---

### [gofireflyio/aiac](https://github.com/gofireflyio/aiac) ⭐ 3.8k | ⚡💸
**Problema:** Escrever Terraform/Pulumi/Docker configs é repetitivo e propenso a erros.
**Solução:** Gera IaC com linguagem natural: descreve o que quer, recebe o código pronto.
**Por que é superior:** ⚡ Minutos vs horas escrevendo YAML. 💸 Menos erros de infra = menos downtime.

---

### [Zyphra/Zonos](https://github.com/Zyphra/Zonos) ⭐ 7.2k | 💸🚀
**Problema:** TTS de qualidade (ElevenLabs) custa $5-99/mês por voz.
**Solução:** TTS open-weight qualidade comercial — 200k+ horas de treino, roda local.
**Por que é superior:** 💸 Grátis vs $99/mês. 🚀 Roda local = sem API, sem limites, privacidade total.

---


### [jlowin/fastmcp](https://github.com/jlowin/fastmcp) ⭐ 22.5k | 🎯⚡🚀
**Problema:** Criar MCP servers é complexo — serialização, validação, error handling, protocol compliance. O SDK oficial é verboso.
**Solução:** Framework Pythonic que abstrai toda complexidade MCP em decorators simples. FastMCP 1.0 foi incorporado ao SDK oficial; hoje powera 70% de todos MCP servers.
**Por que é superior:** ⚡ De dias → horas pra criar um MCP server. 🚀 1M+ downloads/dia, se tornou o padrão de facto. 🎯 Todo dev que quer expor tools pra AI precisa disso.
**TAM:** MCP ecosystem estimado em bilhões. Todo SaaS, API, database eventualmente terá MCP server.
**Modelo de negócio:** Já da Prefect (empresa madura). Upsell: Prefect Cloud pra orquestração. MCP hosting managed.
**Esforço:** Baixo (já produtizado). Oportunidade: managed MCP hosting, marketplace de servers, enterprise support.
**Licença:** Apache-2.0 | 1.7k forks

---

### [oraios/serena](https://github.com/oraios/serena) ⭐ 19.6k | 🎯⚡💎
**Problema:** Coding agents (Claude Code, Codex, Gemini CLI) desperdiçam tokens lendo arquivos inteiros e fazendo grep cego. Em codebases grandes, isso é ineficiente e caro.
**Solução:** Toolkit que dá capacidades de IDE ao LLM via MCP — retrieval semântico por símbolo (find_symbol, find_referencing_symbols, insert_after_symbol). O agent navega como um dev sênior, não como um estagiário com grep.
**Por que é superior:** 💎 Qualidade muito superior: edições precisas por símbolo vs string replacement. ⚡ 5-10x menos tokens = 5-10x menor custo. 🎯 Todo dev usando AI coding agents se beneficia.
**TAM:** AI coding tools market $2B+ e crescendo 100%+ a.a.
**Modelo de negócio:** Freemium (MIT). Plugin JetBrains já lançado. Enterprise: self-hosted com suporte, custom language packs.
**Esforço:** Baixo-Médio. Já funcional com Claude Code, Gemini CLI, Cursor, VSCode.
**Combinação:** Serena + FastMCP = coding agents que são IDE-aware E eficientes em tokens.
**Licença:** MIT | 1.3k forks

---
