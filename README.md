# ♻️ EcoTech

> Aplicação web para mapeamento de ecopontos e conscientização sobre o descarte adequado de Resíduos de Equipamentos Eletroeletrônicos (REEE).

Projeto desenvolvido como requisito acadêmico para a disciplina de Introdução ao Desenvolvimento Web do curso de Ciência da Computação (Universidade Federal da Fronteira Sul - UFFS, Campus Chapecó).

---

## 🎯 Sobre o Projeto

O acelerado avanço tecnológico gera um volume crescente de lixo eletrônico. O **EcoTech** atua na redução da barreira informacional, conectando a intenção de descarte responsável por parte do cidadão à infraestrutura de coleta existente em Chapecó e região.

Este projeto está diretamente alinhado ao **ODS 12 (Consumo e Produção Responsáveis)** da ONU (Meta 12.5), atuando na conscientização da população e no fomento à logística reversa de componentes como baterias, monitores, placas e periféricos.

---

## 🎨 Paleta de Cores e Identidade Visual (Sprint 2)

A identidade visual foi projetada para unir a sobriedade da área tecnológica ao dinamismo da sustentabilidade ambiental, priorizando a legibilidade e o alto contraste (padrão WCAG):

| Cor | Código Hexadecimal | Aplicação Principal |
| :--- | :--- | :--- |
| **Verde Esmeralda** | `#10B981` | Botões de ação (CTAs), destaques visuais, ícones e links ativos. |
| **Azul Noturno (Slate)** | `#1E293B` | Tipografia principal, títulos, bordas estruturais e ícones secundários. |
| **Cinza Neve** | `#F8FAFC` | Plano de fundo (*background*) geral das páginas para reduzir a fadiga visual. |
| **Branco Puro** | `#FFFFFF` | Superfície de destaque dos *cards*, barra de navegação e caixa de busca. |
| **Âmbar Alerta** | `#D97706` | Indicadores visuais de atenção e alerta de risco à saúde/toxicidade. |

**Justificativa e Contraste:** A combinação do texto em Azul Noturno (`#1E293B`) sobre os fundos Cinza Neve (`#F8FAFC`) e Branco (`#FFFFFF`) proporciona uma taxa de contraste superior a 12:1 (nível AAA da diretriz WCAG), garantindo leitura confortável tanto em ambientes internos (desktop) quanto sob luz solar em dispositivos móveis (*mobile-first*). O Verde Esmeralda (`#10B981`) guia o olhar do usuário diretamente para as ações principais de localização de ecopontos.

---

## 🗂️ Estrutura de Pastas e Páginas

~~~text
ecotech/
├── src/
│   └── css/
│       ├── input.css      # Diretivas do Tailwind CSS v4 e estilos customizados
│       └── output.css     # Folha de estilo externa compilada e vinculada aos HTMLs
├── index.html             # Página Inicial (Hero section, impacto ambiental e navegação)
├── guia.html              # Guia de Descarte segmentado por categorias de hardware
├── ecopontos.html         # Busca, protótipo de mapa e catálogo de pontos de coleta
├── .gitignore             # Exclusão da pasta node_modules do versionamento
├── package.json           # Dependências de desenvolvimento (@tailwindcss/cli)
└── README.md              # Documentação técnica do projeto
~~~

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 Semântico:** Estruturação com `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` e `<footer>`, além de atributos de acessibilidade (`aria-label` e `sr-only`).
* **CSS3 & Tailwind CSS v4:** Estilização em folha externa (`./src/css/output.css`) compilada via `@tailwindcss/cli`, utilizando abordagem *Mobile-First* e microinterações de *hover*.

---

## 🚀 Como Executar o Projeto Localmente

1. Clone o repositório:
   ~~~bash
   git clone https://github.com/flplz/ecotech.git
   ~~~
2. Acesse o diretório do projeto:
   ~~~bash
   cd ecotech
   ~~~
3. Abra o arquivo `index.html` diretamente no navegador ou utilize a extensão **Live Server** no VS Code.
4. *(Opcional — apenas para recompilar o CSS durante edições)*:
   ~~~bash
   npm install
   npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --watch
   ~~~

---

## 📅 Progresso das Sprints

- [x] **Sprint 1:** Concepção do projeto, fundamentação teórica, alinhamento com a ODS 12 e prototipação (*wireframes* de baixa fidelidade).
- [x] **Sprint 2:** Estruturação semântica das páginas principais interligadas (`index.html`, `guia.html`, `ecopontos.html`), estilização com folha de estilo externa, definição da paleta de cores e atualização do repositório.
- [ ] **Sprint 3:** Refinamento final de responsividade, validação de dados dos ecopontos e testes de usabilidade.

---

Desenvolvido por **Felipe Fagundes Pacheco** ([flplz](https://github.com/flplz)) — Ciência da Computação (UFFS Chapecó)