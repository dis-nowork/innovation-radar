# Physical World Software — Negócios do Mundo Físico

> Análise: 2026-02-02 | Tema: Software para negócios que operam no mundo físico (logística, saúde, hospitalidade, varejo, manutenção)

## Contexto Estratégico

O mundo físico — hotéis, fábricas, clínicas, restaurantes, frotas — ainda roda em software dos anos 2000 ou planilhas. Esses verticais pagam $100-500+/mês por soluções proprietárias mediocres. A onda open-source está chegando nessas indústrias com 5-10 anos de atraso em relação ao mundo dev/tech.

---

## 1. inventree/InvenTree ⭐ 6.3k
**Link:** https://github.com/inventree/InvenTree
**Licença:** MIT

### Problema Real
Empresas de eletrônica, manufatura, makerspaces e até e-commerce precisam rastrear peças, componentes e estoque com precisão. Soluções existentes: Fishbowl ($329/mês), Cin7 ($349/mês), TradeGecko (descontinuado), ou SAP ($$$$).

### O que é
Sistema completo de gestão de inventário: rastreamento de peças por lote/serial, BOM (Bill of Materials), fornecedores, compras, localização em armazém. Python/Django backend + React frontend moderno (Mantine UI). REST API completa, mobile app nativa, sistema de plugins extensível.

### Eixos de Inovação
- 🎯 **Problema real:** PMEs de manufatura/eletrônica lutam com inventário em Excel ou sistemas caros
- 💸 **5-10x menor custo:** Grátis vs $329-349/mês (Fishbowl/Cin7) = economia de ~$4k/ano
- 💎 **Qualidade:** Stack moderna (React+Django), mobile app, API REST, plugin system — superior a muitos pagos
- 🚀 **Escala:** De hobbyista individual até empresa com múltiplos armazéns

### TAM
- Mercado global de inventory management software: ~$3.2B (2025), crescendo 8% ao ano
- 2M+ PMEs de manufatura só nos EUA precisam de gestão de inventário

### Modelo de Negócio
- **Open-core + Cloud hosting:** Já tem empresa comercial (inventree.org) com hosting gerenciado
- **Plugins premium:** Marketplace de extensões para verticais específicos
- **Enterprise:** Multi-tenant, SSO, audit logs, SLA

### Esforço para Produtizar: **Baixo** ✅
Já é product-grade. Instalação one-line. Docker. Mobile app. Comunidade ativa (6.3k stars, 450+ forks).

---

## 2. Grashjs/cmms (Atlas CMMS) ⭐ 496
**Link:** https://github.com/Grashjs/cmms
**Licença:** AGPL-3.0

### Problema Real
Técnicos de manutenção em fábricas, hospitais, hotéis, escolas e prédios comerciais usam papel/WhatsApp para rastrear ordens de serviço. Alternativas: UpKeep ($45/user/mês), Fiix ($40/user/mês), Limble ($28/user/mês).

### O que é
"Jira para técnicos" — CMMS completo self-hosted: work orders, preventive maintenance, equipment tracking, inventory de peças, purchase orders, analytics, Google Maps integration. Web + mobile. Docker one-click.

### Eixos de Inovação
- 🎯 **Problema real:** Manutenção industrial é 80% papel/WhatsApp no Brasil e LatAm
- 💸 **5-10x menor custo:** Grátis vs $28-45/user/mês — uma equipe de 10 técnicos economiza $3-5k/ano
- 🚀 **Escala:** De 1 prédio a campus multi-localidade

### TAM
- Mercado global de CMMS: ~$1.5B (2025), crescendo 10%+ ao ano
- Segmento mais underserved: PMEs com 5-50 técnicos que não justificam SAP PM

### Modelo de Negócio
- **Managed cloud:** Host por eles com pricing por user
- **Enterprise:** Multi-tenant, IoT integrations (sensores de vibração/temperatura), predictive maintenance com AI
- **Vertical editions:** Hospital, hotel, factory — cada um com workflows customizados

### Esforço para Produtizar: **Médio** ⚠️
Funcional mas com 496 stars = comunidade pequena. Precisa de polimento na UX mobile, offline mode para técnicos em campo, e integrações IoT.

### Combinações Explosivas 💥
- **Atlas CMMS + InvenTree** = manutenção + inventário de peças integrado = solução completa para fábricas
- **Atlas CMMS + Traccar** = manutenção + rastreamento de frota = gestão completa de ativos móveis

---

## 3. Qloapps/QloApps ⭐ 11.9k
**Link:** https://github.com/Qloapps/QloApps
**Licença:** OSL-3.0

### Problema Real
Pequenos hotéis, pousadas e hostels pagam $100-500/mês para Cloudbeds, Little Hotelier, ou eZee — ou dependem 100% de OTAs (Booking.com cobra 15-25% de comissão). Precisam de: website, booking engine, PMS (property management).

### O que é
Plataforma completa para hotelaria: PMS, booking engine, website bonito, gestão de quartos/tarifas, multi-idioma. Baseado em PrestaShop (PHP), maduro e com marketplace de addons.

### Eixos de Inovação
- 🎯 **Problema real:** 80% dos pequenos hotéis no Brasil/LatAm não têm sistema próprio de reservas
- 💸 **5-10x menor custo:** Grátis vs $100-500/mês + elimina 15-25% de comissão OTA em reservas diretas
- 🚀 **Escala:** De pousada com 5 quartos a rede com 50+ propriedades

### TAM
- Mercado global de hotel management software: ~$4.5B (2025)
- ~700k hotéis independentes mundialmente que não usam software profissional
- Brasil: ~30k pousadas/hotéis pequenos = mercado local de R$500M+

### Modelo de Negócio
- **Addons marketplace:** Channel manager (Booking/Airbnb sync), payment gateways, revenue management
- **Managed hosting:** Setup + hosting por $30-50/mês (vs $200+ dos concorrentes)
- **White-label:** Para consultorias de turismo que atendem múltiplos hotéis

### Esforço para Produtizar: **Baixo** ✅
11.9k stars, Docker image, documentação extensa, marketplace ativo. Já é usado em produção por milhares de hotéis.

---

## 4. traccar/traccar ⭐ 6.9k
**Link:** https://github.com/traccar/traccar
**Licença:** Apache-2.0

### Problema Real
Frotas de entrega, táxi, transporte escolar e empresas de logística pagam $25-45/veículo/mês para Samsara, Verizon Connect, ou Omnitracs. Uma frota de 50 veículos = $15-27k/ano.

### O que é
Plataforma GPS tracking server mais madura do open-source: suporta 200+ protocolos de rastreadores GPS, web app, mobile apps (Android/iOS), geofencing, alertas, relatórios, manutenção de veículos. Java backend, 9.5k+ commits, 15+ anos de desenvolvimento.

### Eixos de Inovação
- 🎯 **Problema real:** Toda empresa com veículos precisa rastreamento — desde motoboy até transportadora
- 💸 **5-10x menor custo:** Servidor self-hosted + rastreador GPS ($20-50 cada) vs $25-45/veículo/mês
- 📈 **Volume:** Suporta milhares de dispositivos simultâneos, 200+ protocolos de hardware

### TAM
- Mercado global de fleet management: ~$25B (2025), crescendo 15%+ ao ano
- Segmento "SMB fleet" (5-100 veículos): ~$8B, mais underserved

### Modelo de Negócio
- **Managed hosting:** Traccar já oferece (traccar.org) — cloud hosting por device/mês
- **Enterprise features:** AI route optimization, fuel analytics, driver behavior scoring
- **White-label:** Para revendedores de rastreamento veicular (enorme no Brasil)
- **Vertical bundles:** Transporte escolar (com app para pais), delivery (com integração e-commerce)

### Esforço para Produtizar: **Baixo** ✅
Já é business. Empresa comercial (Traccar Ltd), apps móveis, hosting. O potencial está em AI layer + verticais.

---

## 5. opensourcepos/opensourcepos ⭐ 4.0k
**Link:** https://github.com/opensourcepos/opensourcepos
**Licença:** MIT

### Problema Real
Pequenos varejistas, cafeterias, mercearias pagam $60-99/mês para Square POS, Toast ($69/mês), ou Lightspeed ($89/mês). Em mercados emergentes, muitos ainda usam caderno.

### O que é
POS web-based completo: gestão de estoque, vendas, clientes, fornecedores, VAT/GST, barcode, recibos, gift cards, rewards, mesas de restaurante, multi-user com permissões, reporting, SMS, multilíngue.

### Eixos de Inovação
- 🎯 **Problema real:** Todo comércio precisa de PDV — mercado universal
- 💸 **5-10x menor custo:** Grátis vs $60-99/mês — economia de $720-1200/ano por loja
- 🚀 **Escala:** De quiosque a rede de lojas

### TAM
- Mercado global de POS software: ~$15B (2025)
- ~30M pequenos comércios mundialmente sem PDV digital

### Modelo de Negócio
- **Hardware bundles:** Vender com impressora térmica + gaveta + leitor de barcode
- **Managed cloud:** Hosting + backup + suporte por $15-30/mês
- **Vertical editions:** Restaurante (kitchen display, delivery integration), varejo (e-commerce sync), salão de beleza

### Esforço para Produtizar: **Médio** ⚠️
Stack legada (PHP/CodeIgniter 4, Bootstrap 3). Funcional mas precisa de modernização da UX e mobile-first redesign para competir com Square/Toast.

---

## 6. openemr/openemr ⭐ 4.7k
**Link:** https://github.com/openemr/openemr
**Licença:** GPL-2.0

### Problema Real
Clínicas e consultórios pagam $140-500+/provedor/mês para AdvancedMD, athenahealth, DrChrono. Muitos médicos no Brasil/LatAm usam prontuário em papel ou planilhas.

### O que é
O EHR open-source mais popular do mundo: prontuário eletrônico, agendamento, faturamento eletrônico, prescrições, CID-10, FHIR API, portal do paciente, telemedicina. 20+ anos de desenvolvimento, ONC certified (EUA).

### Eixos de Inovação
- 🎯 **Problema real:** Saúde digital é mandatória em muitos países — clínicas precisam de EHR
- 💸 **5-10x menor custo:** Grátis vs $140-500/provedor/mês = economia massiva para clínicas
- 📈 **Volume:** Usado em 40+ países, suporta múltiplos idiomas e regulações

### TAM
- Mercado global de EHR: ~$40B (2025), crescendo 5% ao ano
- Segmento clínicas independentes/pequenas: ~$12B

### Modelo de Negócio
- **Implementation services:** Setup, customização, integração com labs/farmácias
- **Managed hosting + compliance:** HIPAA/LGPD hosting gerenciado
- **Vertical modules:** Dermatologia (fotos), ortopedia (imagens), odontologia (odontograma)
- **AI layer:** Transcrição de consultas (Whisper), AI diagnostic suggestions, drug interaction checking

### Esforço para Produtizar: **Alto** ⛔
Complexidade regulatória enorme (certificações, compliance). Stack legada. Mas o moat é gigante — quem implementa vira indispensável.

---

## Comparativo Rápido

| Repo | ⭐ | Custo Substitui | Economia/ano | TAM | Esforço | Score |
|------|-----|-----------------|-------------|-----|---------|-------|
| InvenTree | 6.3k | Fishbowl $329/mo | ~$4k | $3.2B | Baixo | ⭐⭐⭐⭐⭐ |
| Atlas CMMS | 496 | UpKeep $45/user/mo | ~$5k (10 users) | $1.5B | Médio | ⭐⭐⭐⭐ |
| QloApps | 11.9k | Cloudbeds $200/mo | ~$2.4k + OTA savings | $4.5B | Baixo | ⭐⭐⭐⭐⭐ |
| Traccar | 6.9k | Samsara $35/vehicle/mo | ~$21k (50 vehicles) | $25B | Baixo | ⭐⭐⭐⭐⭐ |
| OSPOS | 4.0k | Square $69/mo | ~$828 | $15B | Médio | ⭐⭐⭐ |
| OpenEMR | 4.7k | athena $140/provider/mo | ~$1.7k | $40B | Alto | ⭐⭐⭐⭐ |
