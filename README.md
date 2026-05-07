# Seção de Depoimentos em Formato de Grade

Projeto desenvolvido como exercício de estudo de **CSS Grid** e **Flexbox**, recriando um layout de seção de depoimentos (testimonials) com 5 cards dispostos em grade.

---

## 📸 Preview

![Preview do Projeto](./img/preview.jpg)

---

## 🚀 Tecnologias Utilizadas

- **HTML5** — Estrutura semântica com `<article>`, `<header>`, `<main>`
- **CSS3** — Estilização completa com:
  - CSS Grid (layout em grade)
  - Flexbox (alinhamento interno dos cards)
  - CSS Custom Properties (variáveis de cor)
  - Media Queries (responsividade)
  - Google Fonts (Barlow Semi Condensed)

---

## 🗂️ Estrutura do Projeto

```
📁 projeto
├── index.html          # Estrutura HTML dos 5 cards
├── README.md
└── css/
    ├── base.css        # Estilos globais e configuração do grid principal
    ├── articles.css    # Estilos específicos de cada card
    ├── variable.css    # Variáveis CSS (cores)
    └── reset.css       # Reset de estilos padrão do navegador
```

---

## 🧩 Layout em Grade

O layout usa `grid-template-areas` para posicionar cada card de forma nomeada:

```
┌──────────┬──────────┬──────────┬──────────┐
│  daniel  │  daniel  │ jonathan │   kira   │
├──────────┼──────────┼──────────┤          │
│ jeanette │ patrick  │ patrick  │   kira   │
└──────────┴──────────┴──────────┴──────────┘
```

- **Daniel** — ocupa 2 colunas, fundo roxo com ícone de aspas
- **Jonathan** — 1 coluna, fundo cinza escuro
- **Jeanette** — 1 coluna, fundo branco
- **Patrick** — ocupa 2 colunas, fundo azul escuro
- **Kira** — 1 coluna, ocupa 2 linhas (fundo branco)

---

## 🎨 Paleta de Cores

| Variável | Cor | Uso |
|---|---|---|
| `--purple-500` | `hsl(263, 55%, 52%)` | Fundo card Daniel |
| `--grey-500` | `hsl(217, 19%, 35%)` | Fundo card Jonathan |
| `--dark-blue` | `hsl(219, 29%, 14%)` | Fundo card Patrick e padrão |
| `--white` | `hsl(0, 0%, 100%)` | Fundo cards Jeanette e Kira |
| `--purple-300` | `hsl(264, 82%, 80%)` | Borda dos avatares |

---

## 📱 Responsividade

O layout se adapta a diferentes tamanhos de tela via **media queries**:

| Largura | Layout |
|---|---|
| `> 1024px` | 4 colunas (layout completo) |
| `≤ 1024px` | 2 colunas (tablet) |
| `≤ 640px` | 1 coluna (mobile) |

---

## 💡 Conceitos Aprendidos

- Definição de áreas nomeadas com `grid-template-areas`
- Uso de `grid-area` para posicionar elementos no grid
- `grid-row: span 2` para fazer um elemento ocupar múltiplas linhas
- Cascata CSS e sobrescrita de estilos
- Organização de arquivos CSS por responsabilidade
- Contraste de texto em fundos claros e escuros

---

## 🔗 Créditos

Desafio baseado no [Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7).
