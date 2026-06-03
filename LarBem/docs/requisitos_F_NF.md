# 📋 Especificação de Requisitos – Projeto LarBEM

Este documento detalha os Requisitos Funcionais (RF) e Não Funcionais (RNF) para o desenvolvimento da plataforma digital e institucional do **Lar Bem Elizabeth**. O mapeamento das necessidades listadas abaixo foi consolidado através de reuniões de alinhamento com a diretoria da instituição, criação de wireframes, guias de identidade visual e gerenciamento ágil via quadro Kanban.

---

## 🛠️ Requisitos Funcionais (RF)

Os Requisitos Funcionais descrevem as ações, recursos e interações que a plataforma deve oferecer aos seus usuários e à comunidade.

| ID | Requisito | Descrição | Referência (Card) |
| :--- | :--- | :--- | :--- |
| **RF01** | **Apresentação do Bazar Solidário** | O sistema deve conter uma seção dedicada ao bazar institucional ("Temos um Bazar!"), detalhando os produtos vendidos (roupas, calçados e acessórios) e instruindo a comunidade sobre os critérios de doação. | #28 |
| **RF02** | **Carrossel Dinâmico de Categorias** | O catálogo do bazar deve conter um componente de carrossel de imagens interativo para exibição dos produtos por categorias (ex: "brinquedos"), navegável por setas laterais controladas via JavaScript. | #28 / #26 / #40 |
| **RF03** | **Direcionamento para WhatsApp ("Saiba Mais")** | O sistema deve possuir um botão Neubrutalista no Bazar que direcione o usuário para o WhatsApp oficial do LarBEM, permitindo demonstrar interesse de compra ou agendar doações. | *README* / #40 |
| **RF04** | **Formulário de Contato Direto** | O sistema deve possuir um formulário funcional contendo os campos obrigatórios: *Seu nome*, *Seu e-mail*, *Assunto* e *Sua mensagem*, com validação de preenchimento antes do envio. | #10 / #13 |
| **RF05** | **Seção de Voluntariado** | O sistema deve possuir uma área dedicada ("Faça Parte da Nossa História!") com textos de engajamento e um botão que redirecione o usuário para a página de inscrição de voluntários. | #45 / #37 |
| **RF06** | **Menu de Navegação Superior** | O cabeçalho deve possuir botões interativos para ancoragem e acesso rápido às seções essenciais do site: *Sobre Nós*, *Nosso Brechó*, *Seja um Voluntário*, *Seja um Doador* e *Contatos*. | *README* / #31 |
| **RF07** | **Apresentação Institucional (Home)** | A primeira dobra do site deve exibir de forma fixa o logotipo oficial, o título "Larbem.", o nome "Lar Batista Elizabeth Mein" e o resumo histórico de sua fundação em 1954. | #29 / #22 / #13 |
| **RF08** | **Seção de Valores da ONG** | O sistema deve apresentar uma grade com 4 blocos de informações textuais e iconográficas detalhando as diretrizes da ONG: *Dignidade e Respeito*, *Afetividade e Proteção*, *Empoderamento Feminino* e *Justiça Social*. | #29 / #13 / #32 |
| **RF09** | **Seção de Serviços Prestados** | O sistema deve listar de forma clara as 4 principais frentes de atuação e acolhimento contínuo oferecidas às meninas atendidas pela instituição. | #29 / #13 |
| **RF10** | **Seção de Doações (Como Ajudar)** | O sistema deve expor de forma fixa os dados bancários oficiais validados para captação de recursos (Banco do Brasil, Caixa Econômica e PIX). | #40 / #13 / #47 |
| **RF11** | **Funcionalidade Copiar Chave PIX** | Na seção de doações, o sistema deve permitir a cópia rápida do CNPJ da chave PIX para a área de transferência do dispositivo do usuário, sem gerar redirecionamentos externos. | #40 |
| **RF12** | **Canais de Comunicação e Localização** | O sistema deve disponibilizar de forma textual e linkada o endereço físico em Recife, telefone fixo, e-mail institucional e links para as redes sociais (Facebook e Instagram). | #10 / #13 |
| **RF13** | **Rodapé de Propriedade Intelectual** | A base do site deve exibir uma barra de rodapé contendo o ano vigente, declaração de direitos autorais da ONG e os créditos nominais dos desenvolvedores (Amanda Aziz e Mozart Moura). | #44 |
| **RF14** | **Seção de Notícias (Futuro)** | O sistema deve prever uma estrutura modular ou aba voltada para a publicação de futuros eventos, comunicados e novidades da instituição. | #51 / #37 |
| **RF15** | **Espaço para Anúncios (Futuro)** | O layout deve reservar áreas específicas integradas para banners de parceiros comerciais, visando monetização para manutenção do servidor. | #46 |
| **RF16** | **Formulário de Satisfação (Futuro)** | O sistema deve implementar uma ferramenta de coleta de feedback e avaliação dos usuários para melhoria contínua da experiência digital. | #50 / #47 |

---

## ⚙️ Requisitos Não Funcionais (RNF)

Os Requisitos Não Funcionais especificam os critérios de qualidade, restrições tecnológicas, desempenho, design e usabilidade que o sistema deve cumprir.

| ID | Categoria | Descrição | Referência (Card) |
| :--- | :--- | :--- | :--- |
| **RNF01** | **Tecnologia / Stack** | O frontend deve ser construído estritamente com tecnologias nativas da Web: HTML5, CSS3 e JavaScript Vanilla, sem a dependência de frameworks ou bibliotecas complexas de terceiros. | #8 |
| **RNF02** | **Responsividade** | A interface da plataforma deve ser totalmente adaptável, quebrando layouts multi-colunas em fluxos verticais únicos para garantir usabilidade em smartphones, tablets e desktops. | #42 / #43 |
| **RNF03** | **Estilo Visual (UI/UX)** | A interface deve seguir rigorosamente a estética do *Neubrutalismo*: uso de paleta vibrante com roxo, rosa e laranja, bordas pretas espessas, cantos arredondados nos botões/cards e sombras pretas sólidas projetadas sem desfoque (blur). | #30 / #32 / #33 |
| **RNF04** | **Animações Dinâmicas** | O sistema deve conter elementos de microinteração e animações fluidas via CSS/JS, incluindo uma barra de texto rotativa contínua (*marquee*) no corpo da página. | #26 |
| **RNF05** | **Hospedagem e CI/CD** | O deploy do projeto deve ser automatizado e hospedado na plataforma Vercel (`larbem.vercel.app`), com gatilhos de atualização automática vinculados ao branch principal do GitHub. | #24 |
| **RNF06** | **Acessibilidade** | O site deve seguir boas práticas de acessibilidade na web, utilizando estruturação semântica de tags HTML (header, section, main, footer) e contraste legível de cores para os textos. | *README* |
| **RNF07** | **Mantenabilidade e Organização** | O código-fonte deve ser limpo e estruturado em uma arquitetura modular de pastas bem definidas divididas por escopo (`/css`, `/js`, `/assets`). | #44 |
| **RNF08** | **Confiabilidade de Conteúdo** | Todas as informações textuais de impacto social e imagens reais aplicadas no layout (incluindo as molduras estilo *Polaroid*) devem passar por curadoria e aprovação direta da diretoria da instituição. | #13 / #22 |
| **RNF09** | **Infraestrutura / Domínio** | O sistema deve estar configurado para responder corretamente sob o endereço web oficial definido para a marca LarBEM Elizabeth. | #23 |
| **RNF10** | **Simplicidade de Execução** | O projeto deve permitir execução local imediata sem necessidade de instalação de dependências ou gerenciadores de pacotes (como npm ou yarn), funcionando via abertura direta do `index.html`. | *README* |

---
> **Nota:** Este documento serve como guia para a equipe de desenvolvimento (Amanda e Mozart) e para a validação final do projeto de extensão.
