# Checklist de Requisitos — RN Manutenção e Serviços

**Verificado em:** 30/09/2026 — `landing-page-rn-manutencao.html` (todas as linhas conferidas no código)

## Estrutura e Seções (Copy e Design)
- [x] Hero Section (Cabeçalho) com título de impacto e botão gigante de emergência (`.btn-hero` + pulso)
- [x] Seção "Sobre Nós" (Roni, diferenciais da empresa, garantia de 90 dias) — `#sobre`
- [x] Seção "Serviços Elétricos" (Instalações, chuveiros, quadros, curto-circuito) — `#servicos`
- [x] Seção "Serviços Hidráulicos" (Vazamentos, desentupimento, torneiras) — `#servicos`
- [x] Seção "Atendimento de Urgência" (24h / Plantão rápido) — faixa com imagem de fundo + `tel:`
- [x] Seção "Regiões Atendidas" (Áreas de foco para SEO Local: Natal + RMR) — `#regioes` + ItemList schema
- [x] Seção "Depoimentos" (Prova social) — `#depoimentos` (placeholders marcados com `<!-- PLACEHOLDER -->`)
- [x] Seção "Galeria de Fotos" (Antes e Depois) — `#galeria`
- [x] Seção "Contato e Orçamento" (Formulário simplificado de 3 campos: Nome, Bairro, Serviço) — `#contato`
- [x] Rodapé (Links úteis, redes sociais, políticas de garantia e privacidade / LGPD)

## Funcionalidades e Interações
- [x] Botão Flutuante de WhatsApp (Fixo e com mensagem padrão configurada)
- [x] Botões de "Ligar Agora" utilizando o atributo de chamada `tel:` (nav, faixa 24h, rodapé)
- [x] Formulário de contato funcional enviando os dados corretos (JS monta Nome/Bairro/Serviço → `wa.me` + mensagem de sucesso + aviso LGPD)

## Requisitos Técnicos
- [x] Design Mobile-first de altíssimo contraste
- [x] Cores fiéis implementadas: Azul Marinho, Amarelo/Laranja e Branco
- [x] Performance ultra-rápida (Core Web Vitals para 3G/4G) — imagens comprimidas (≈560 KB total), `loading="lazy"`, `width`/`height` anti-CLS, `fetchpriority="high"` no hero
- [x] SEO Técnico: Schema.org (LocalBusiness, Electrician, Plumber, ItemList de regiões)
- [x] SEO On-page: Meta tags adequadas e hierarquia semântica de Headings (1×H1, 7×H2, 4×H3)

## Pendências do Cliente (marcadas no HTML com comentários)
- [ ] Depoimentos reais (substituir os 3 placeholders)
- [ ] Fotos reais de antes/depois na galeria
- [ ] URLs das redes sociais (Instagram/Facebook)
- [ ] Confirmar termos da garantia e dados de contato do titular (LGPD)
