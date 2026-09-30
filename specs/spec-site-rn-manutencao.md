# SPEC — Site RN Manutenção e Serviços (Eletricista & Encanador)
**Versão:** 1.0  
**Data:** 30/09/2026  
**Autor:** Analista de Requisitos Sênior (IA)  
**Status:** Rascunho para Validação  

---

## 1. Visão Geral
Site institucional e landing page de alta conversão para a "RN Manutenção e Serviços" focada em serviços de eletricista e encanador. O objetivo principal é dominar o SEO local, atrair buscas de urgência ("eletricista perto de mim", "encanador urgente") e converter o visitante rapidamente através de botões de WhatsApp e ligação direta.

## 2. Contexto e Problema
A empresa atende residências, condomínios e comércios oferecendo soluções elétricas e hidráulicas com rapidez e segurança. Há uma necessidade latente de captar clientes no exato momento da urgência (ex: falta de luz, vazamento grave) através das buscas do Google. Isso exige um site com carregamento ultra-rápido, de alta confiança visual e com chamadas para ação (CTA) muito acessíveis no mobile (sem obstáculos).

## 3. Objetivos
- **OBJ-01:** Ranqueamento nas buscas locais do Google (SEO) para termos de urgência e serviços específicos.
- **OBJ-02:** Maximizar a conversão de acessos mobile, permitindo acionamento do serviço em menos de 3 segundos.
- **OBJ-03:** Transmitir credibilidade e profissionalismo através de design limpo, depoimentos, selos de qualidade e garantias por escrito.

## 4. Atores / Usuários
| Ator | Descrição | Permissões esperadas |
|------|-----------|----------------------|
| Cliente com Urgência | Precisa de resolução imediata (vazamento, sem luz) | Visualizar CTAs e acionar via WhatsApp/Ligação |
| Cliente Planejado | Busca orçamento para reformas, instalações e manutenção | Navegar por serviços, galeria e preencher formulário |
| Administrador | Proprietário (Roni) e equipe | Receber os contatos e orçamentos via WhatsApp/Email |

## 5. Requisitos Funcionais

### 5.1 Landing Page Principal (Home)
- **RF-01** [OBRIGATÓRIO]: O sistema deve exibir uma Hero Section com título de impacto e um botão gigante de emergência.
- **RF-02** [OBRIGATÓRIO]: O sistema deve possuir seções dedicadas e detalhadas para Serviços Elétricos e Serviços Hidráulicos.
- **RF-03** [OBRIGATÓRIO]: O sistema deve incluir uma seção de Atendimento de Urgência (Plantão).
- **RF-04** [OBRIGATÓRIO]: O sistema deve listar as Regiões Atendidas (Bairros/Cidades) focado em SEO Local.
- **RF-05** [OBRIGATÓRIO]: O sistema deve exibir uma seção de Depoimentos/Avaliações do Google para gerar prova social.
- **RF-06** [OBRIGATÓRIO]: O sistema deve exibir uma Galeria de Trabalhos Realizados (fotos de Antes e Depois).
- **RF-07** [OBRIGATÓRIO]: O sistema deve possuir um formulário simplificado de "Solicitar Cotação Rápida" (Nome, Bairro, Serviço).

### 5.2 Interações e CTAs
- **RF-08** [OBRIGATÓRIO]: O sistema deve exibir um Botão Flutuante de WhatsApp fixo (especialmente no mobile) com mensagem padrão pré-preenchida ("Olá Roni...").
- **RF-09** [OBRIGATÓRIO]: O sistema deve ter botões "Ligar Agora" com clique direto para chamadas telefônicas (`tel:`).

## 6. Requisitos Não Funcionais
- **RNF-01** Performance: O tempo de carregamento deve ser ultra-rápido, essencial para conexões instáveis de mobile na hora da urgência.
- **RNF-02** Design e Usabilidade: Cores principais devem ser Azul Marinho (confiança), Amarelo/Laranja (atenção/energia) e Branco. O layout deve ser estritamente Mobile-First.
- **RNF-03** SEO: Uso de marcação Schema.org para LocalBusiness, Electrician e Plumber; tags semânticas (H1, H2, H3); imagens otimizadas com alt text.
- **RNF-04** Segurança: O site deve ser hospedado com Certificado SSL (HTTPS) e seguir as diretrizes da LGPD nos formulários de contato.

## 7. Fluxos Principais (Happy Path)

**Fluxo 1: Chamado de Urgência Mobile**
1. Usuário pesquisa "encanador urgente" no Google e acessa a página.
2. O site carrega quase instantaneamente com o CTA de ligação visível.
3. Usuário clica no botão "Ligar Agora" ou "WhatsApp Flutuante".
4. O app de telefone/WhatsApp abre e o usuário inicia o atendimento com a empresa.

**Fluxo 2: Pedido de Orçamento Planejado**
1. Usuário acessa o site pesquisando sobre instalação elétrica.
2. Navega pelas seções de serviços e vê a galeria de antes/depois.
3. Preenche o formulário "Solicitar Cotação Rápida".
4. O usuário recebe feedback visual de sucesso e o Administrador recebe os dados por e-mail/WhatsApp.

## 8. Regras de Negócio
- **RN-01**: A garantia oferecida para mão de obra é de 90 dias (deve estar clara no site).
- **RN-02**: Todas as instalações devem mencionar o respeito às normas de segurança (NR-10).

## 9. Integrações e Dependências
| Sistema | Tipo de integração | Dados trocados |
|---------|--------------------|----------------|
| WhatsApp | Link direto (`wa.me`) | Texto pré-preenchido solicitando orçamento |
| Google Maps | Embed ou Link | Avaliações do Google Meu Negócio / Localização |

## 10. Critérios de Aceite
- [ ] Dado um usuário acessando via smartphone, quando ele rola a página, então o botão do WhatsApp deve permanecer visível na tela.
- [ ] Dado o preenchimento correto do formulário de contato, quando o usuário clica em enviar, então ele deve ver uma mensagem de sucesso e os dados devem ser enviados.
- [ ] Dado um teste no Google PageSpeed Insights, então o site deve pontuar na faixa verde de performance (90+).

## 11. Fora de Escopo
- Não haverá sistema de agendamento online automático (calendário).
- Não haverá área logada para clientes.
- Não haverá e-commerce/venda direta de produtos/peças pelo site.

## 12. Dúvidas e Pontos em Aberto
| # | Dúvida | Para quem | Status |
|---|--------|-----------|--------|
| 1 | Quais os principais bairros/cidades exatos atendidos para listagem focada no SEO local? | Cliente (Roni) | [REQUER DEFINIÇÃO] |
| 2 | O formulário deve enviar os dados para o e-mail informado ou também integrá-los para cair direto no WhatsApp? | Cliente (Roni) | [REQUER DEFINIÇÃO] |
| 3 | Tendo em vista a necessidade extrema de velocidade (carregar em < 3s), construiremos o site em HTML/CSS/JS nativo e leve, correto? | Cliente (Roni) | [AGUARDANDO CONFIRMAÇÃO] |

## 13. Histórico de Versões
| Versão | Data | Alteração |
|--------|------|-----------|
| 1.0 | 30/09/2026 | Criação inicial da Spec via briefing |
