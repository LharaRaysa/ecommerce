# Documentação Completa do Projeto - TechStore

**Versão:** 1.0  
**Data de Criação:** Novembro 2025  
**Desenvolvedora:** Lhara Raysa  
**Tipo de Projeto:** Portfólio Frontend  

---

## 1. Introdução

O **TechStore** é um e-commerce fictício de produtos de tecnologia desenvolvido exclusivamente com **HTML5, CSS3 e JavaScript Vanilla** (sem frameworks ou bibliotecas pesadas).

O objetivo principal deste projeto é demonstrar habilidades em desenvolvimento frontend moderno, criação de interfaces interativas, design responsivo e boas práticas de código para fins de **portfólio profissional**.

### Visão Geral
- **Nome do Projeto:** TechStore
- **Descrição:** Vitrine moderna de smartphones, notebooks, fones, smartwatches e acessórios com busca em tempo real e filtro por categorias.
- **Público-alvo:** Recrutadores de Frontend, desenvolvedores e potenciais clientes que buscam um e-commerce clean e funcional.
- **Status Atual:** Versão 1.0 (MVP - Minimum Viable Product)

---

## 2. Objetivos do Projeto

- Criar uma interface visualmente atraente e moderna
- Implementar interatividade fluida (busca e filtros) sem dependências externas
- Demonstrar domínio de **Flexbox**, **Grid Layout**, **CSS Variables** e manipulação do DOM com JavaScript puro
- Produzir um projeto responsivo e otimizado para portfólio
- Servir como base para futuras evoluções (carrinho, modal, integração com backend)

---

## 3. Requisitos Funcionais

| ID     | Descrição                                                                 | Prioridade | Status          |
|--------|---------------------------------------------------------------------------|------------|-----------------|
| RF-01  | Exibir produtos em formato de cards (grid responsivo)                     | Alta       | Implementado    |
| RF-02  | Busca em tempo real pelo nome do produto                                  | Alta       | Implementado    |
| RF-03  | Filtro por categorias (Todos, Smartphones, Notebooks, Fones, Acessórios, Smartwatches) | Alta       | Implementado    |
| RF-04  | Exibir nome, descrição, preço e imagem de cada produto                    | Alta       | Implementado    |
| RF-05  | Destaque visual no botão de categoria ativa                               | Média      | Implementado    |
| RF-06  | Seção Hero com promoção ("Black Friday Antecipada!")                      | Alta       | Implementado    |
| RF-07  | Botão "Ver Detalhes" em cada produto                                      | Média      | Implementado (visual) |
| RF-08  | Mensagem "Nenhum produto encontrado"                                      | Baixa      | Não implementado |

---

## 4. Requisitos Não Funcionais

- **Desempenho:** Filtros e busca devem ser instantâneos (menos de 100ms)
- **Responsividade:** Totalmente adaptável a desktop, tablet e mobile
- **Usabilidade:** Interface intuitiva, clean e com bons feedbacks visuais (hover, transições)
- **Acessibilidade:** Bom contraste de cores e navegação básica por teclado (pode ser aprimorado)
- **Manutenibilidade:** Código organizado, separado por responsabilidades (HTML / CSS / JS) e comentado
- **Compatibilidade:** Funciona nos principais navegadores modernos
- **Tecnologias:** Apenas HTML5 + CSS3 + JavaScript Vanilla + Font Awesome

---

## 5. Tecnologias Utilizadas

- **HTML5** — Estrutura semântica da página
- **CSS3** — Flexbox, CSS Grid, variáveis CSS (`:root`), animações, transições e hover effects
- **JavaScript Vanilla** — Manipulação do DOM, event listeners, filtros dinâmicos e renderização de produtos
- **Font Awesome 6** — Ícones (via CDN)
- **Unsplash** — Imagens dos produtos (links externos)

**Não foram utilizados:** Frameworks (React, Vue, etc.), pré-processadores CSS ou bibliotecas JS.

---

## 6. Estrutura de Arquivos

techstore/
├── index.html                 # Página principal
├── styles.css                 # Todos os estilos e design system
├── scripts.js                 # Lógica de busca, filtros e renderização
├── docs/
│   └── doc_completo_projeto.md   # Esta documentação
└── README.md                  # Página inicial do repositório

---

## 7. Funcionalidades Implementadas

- **Array de Produtos** → 8 produtos com id, nome, categoria, preço, preço original, desconto e descrição
- **Busca em Tempo Real** → Evento `input` filtra os produtos enquanto o usuário digita
- **Filtro por Categoria** → Botões com `data-categoria` e destaque do ativo
- **Renderização Dinâmica** → Função centralizada `mostrarProdutos()` que atualiza o grid
- **Design Moderno** → Gradiente no hero, cards com sombra e efeito de elevação no hover
- **Responsividade** → Grid com `auto-fill` e media queries parciais

---

## 8. Decisões de Design e Arquitetura

- Uso de **CSS Variables** para facilitar troca de cores e manutenção
- Separação clara de responsabilidades (HTML = estrutura, CSS = visual, JS = comportamento)
- Renderização via template string para simplicidade
- Event delegation e listeners eficientes
- Mobile-first parcialmente aplicado (pode ser melhorado)

---

## 9. Limitações da Versão Atual

- Preços sem formatação brasileira (ex: R$ 7.999,00)
- Desconto e preço original não são exibidos visualmente
- Botão "Ver Detalhes" não abre modal
- Não há carrinho de compras
- Responsividade ainda precisa de ajustes finos em mobile
- Sem mensagem de "nenhum resultado"

---

## 10. Roadmap / Próximas Versões

- Versão 1.1 → Formatação de preços + exibição de descontos
- Versão 1.2 → Modal de detalhes do produto
- Versão 2.0 → Carrinho de compras com localStorage + animações
- Versão 2.1 → Dark Mode + melhorias de acessibilidade
- Versão 3.0 → Integração com backend (futuro)

---

## 11. Como Executar o Projeto

1. Clone o repositório
2. Abra o arquivo `index.html` no navegador
3. Recomendado: Use a extensão **Live Server** do VS Code

---