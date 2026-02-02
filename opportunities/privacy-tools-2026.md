# 🔒 Privacy-First Tools (Fev 2026)

## BentoPDF — PDF Toolkit Privacy-First
- **Repo:** [alam00000/bentopdf](https://github.com/alam00000/bentopdf)
- **Stars:** 11.0k ⭐ | **Criado:** 2025
- **Eixos:** 🎯💸💎

### Problema Real
Ferramentas de PDF online (ILovePDF, SmallPDF, Adobe Acrobat) fazem upload dos seus documentos para servidores. Para empresas com dados sensíveis (contratos, RH, financeiro), isso é inaceitável. Adobe Acrobat Pro custa $20/mês.

### Inovação
**100% client-side** — zero upload, todo processamento no browser:
- 50+ ferramentas: merge, split, edit, convert, compress, sign, OCR, watermark
- Suporta PDF→Word, PDF→Imagem, HTML→PDF, EPUB/MOBI conversion
- WASM-powered: PyMuPDF, Ghostscript, CPDF carregados como módulos opcionais
- Self-hostable, Docker/Podman ready
- Dual license: AGPL-3.0 (grátis) + Commercial ($49 lifetime)

### Por que 5-10x melhor:
- **🎯 Problema:** 100% dos escritórios usam PDFs, maioria depende de SaaS inseguro
- **💸 Custo:** $0 (AGPL) ou $49 one-time vs $240/ano Adobe
- **💎 Qualidade:** Feature-complete, UI limpa, sem watermarks

### TAM
- PDF tools market: $3B+ (Adobe só faz $2B+/ano em Document Cloud)
- Compliance-driven demand: GDPR, LGPD, HIPAA

### Modelo de Negócio
- AGPL-3.0 gratuito para uso open-source
- Commercial license $49 lifetime para empresas
- Enterprise deployment consulting

---

## AltSendme — File Transfer Sem Cloud
- **Repo:** [tonyantony300/alt-sendme](https://github.com/tonyantony300/alt-sendme)
- **Stars:** 5.3k ⭐ | **Criado:** 2025
- **Eixos:** 🎯💸💎

### Problema Real
Enviar arquivos grandes é um inferno: WeTransfer (2GB limit grátis, $12/mês pro), Google Drive (storage limit), Dropbox (storage limit). Todos fazem upload para cloud = lento + privacy issues.

### Inovação
**Peer-to-peer direto** usando [Iroh](https://iroh.computer) (moderno, não WebRTC):
- E2E encrypted com QUIC + TLS 1.3 (forward secrecy)
- Sem contas, sem sign-up, sem dados pessoais
- Qualquer tamanho, qualquer formato
- Transferências resumable
- NAT traversal automático (QUIC hole punching + relay fallback)
- Multi-gigabit capable
- Desktop app (macOS, Windows, Linux)

### Por que 5-10x melhor:
- **🎯 Problema:** Transferir 50GB+ é pesadelo hoje
- **💸 Custo:** $0 vs WeTransfer Pro $12/mês ou Dropbox $12/mês
- **💎 Qualidade:** E2E encrypted by default, BLAKE3 integrity verification

### TAM
- File sharing/transfer: $8B+ market
- Enterprise file transfer: $2B+

### Modelo de Negócio
- Open-source gratuito (core)
- Premium features (mobile, web, advanced relay)
- Enterprise relay infrastructure
- SaaS managed relay for corporations

---

## Scanopy — Network Topology Auto-Discovery
- **Repo:** [scanopy/scanopy](https://github.com/scanopy/scanopy)
- **Stars:** 4.0k ⭐ | **Criado:** 2025
- **Eixos:** 🎯💸⚡

### Problema Real
Documentar rede é pesadelo: MSPs gastam horas em Visio/draw.io desenhando manualmente, diagramas ficam desatualizados em semanas. Network discovery tools enterprise (SolarWinds, ManageEngine) custam $2-10k/ano.

### Inovação
- **Auto-discovery:** Scan redes, identifica hosts, serviços e conexões automaticamente
- **200+ service definitions:** Auto-detecta databases, web servers, containers, monitoring
- **Docker integration:** Descobre serviços containerizados
- **Distributed scanning:** Daemons em múltiplos segmentos de rede
- **Zero upkeep:** Scheduled scans mantêm documentação atualizada automaticamente
- **Multi-user:** Org management com RBAC

### Por que 5-10x melhor:
- **🎯 Problema:** Diagramas de rede desatualizados → incidents, security gaps
- **💸 Custo:** Self-hosted grátis vs $2-10k/ano em enterprise tools
- **⚡ Velocidade:** Setup em minutos, auto-atualização vs horas de documentação manual

### TAM
- Network monitoring & management: $15B+
- MSP tools: $5B+
- Homelab/prosumer: Growing fast

### Modelo de Negócio
- AGPL-3.0 self-hosted (grátis)
- Commercial license (proprietary use)
- Scanopy Cloud (managed hosting)
