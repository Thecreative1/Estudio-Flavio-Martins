---
name: Estúdio Flávio Martins
description: Um laboratório digital português onde os projetos são a demonstração.
colors:
  night-ink: "oklch(13% 0.025 250)"
  midnight-surface: "oklch(18% 0.035 250)"
  warm-paper: "oklch(94% 0.02 95)"
  signal-lime: "oklch(84% 0.20 135)"
  hot-coral: "oklch(70% 0.19 28)"
  electric-blue: "oklch(72% 0.16 235)"
  soft-line: "oklch(82% 0.03 240 / 0.18)"
typography:
  display:
    fontFamily: "Chakra Petch, Segoe UI, sans-serif"
    fontSize: "clamp(3.7rem, 10vw, 9.8rem)"
    fontWeight: 700
    lineHeight: 0.84
    letterSpacing: "-0.055em"
  body:
    fontFamily: "Sora, Segoe UI, sans-serif"
    fontSize: "clamp(1rem, 1.25vw, 1.15rem)"
    fontWeight: 400
    lineHeight: 1.65
rounded:
  sm: "6px"
  md: "14px"
  lg: "24px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "32px"
  lg: "64px"
  xl: "128px"
components:
  button-primary:
    backgroundColor: "{colors.signal-lime}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.sm}"
    padding: "14px 20px"
  button-ghost:
    backgroundColor: "{colors.midnight-surface}"
    textColor: "{colors.warm-paper}"
    rounded: "{rounded.sm}"
    padding: "14px 20px"
---

# Design System: Estúdio Flávio Martins

## 1. Overview

**Creative North Star: "Oficina de futuros úteis"**

A página sente-se como entrar no espaço de trabalho de alguém que domina sistemas e gosta de os pôr a mexer. É escura porque o visitante explora uma montra digital luminosa num ambiente de portátil, não porque “tecnologia” tenha de ser dark. Tipografia muito grande, superfícies recortadas e microinterfaces reais transformam cada projeto numa pequena demonstração.

O sistema é energético, mas tem disciplina: cada movimento ajuda a ler, cada cor identifica um projeto e cada detalhe interativo reage à pessoa. Rejeita grelhas repetidas de cartões, estética SaaS copiada, glassmorphism decorativo e efeitos que não contam nada.

**Key Characteristics:**

- Escala tipográfica cinematográfica e assimétrica.
- Preto azulado tintado, papel quente e cor de sinalização.
- Projetos encenados como produtos vivos, não como thumbnails.
- Movimento ligado ao scroll, cursor e estado, sempre com redução disponível.
- Copy curta, direta e em português europeu.

## 2. Colors

A base noturna transforma verde, coral e azul em sinais funcionais, enquanto o papel quente evita o contraste clínico de branco puro.

### Primary

- **Signal Lime** (`oklch(84% 0.20 135)`): ações principais, estado disponível e detalhes que pedem interação.

### Secondary

- **Hot Coral** (`oklch(70% 0.19 28)`): AutoRetoma, chamadas editoriais e momentos de calor.
- **Electric Blue** (`oklch(72% 0.16 235)`): OndeCortar, mapas, dados e relações espaciais.

### Neutral

- **Night Ink** (`oklch(13% 0.025 250)`): fundo principal.
- **Midnight Surface** (`oklch(18% 0.035 250)`): superfícies funcionais.
- **Warm Paper** (`oklch(94% 0.02 95)`): texto principal e secções de inversão.
- **Soft Line** (`oklch(82% 0.03 240 / 0.18)`): divisores e contornos discretos.

**The Signal Rule.** Verde significa ação ou disponibilidade. Não é decoração espalhada.

## 3. Typography

**Display Font:** Chakra Petch (com Segoe UI)
**Body Font:** Sora (com Segoe UI)

**Character:** O display parece mecânico e construído; o corpo mantém a leitura humana. A diferença de escala faz mais trabalho do que a ornamentação.

### Hierarchy

- **Display** (700, `clamp(3.7rem, 10vw, 9.8rem)`, 0.84): uma ideia dominante por viewport.
- **Headline** (700, `clamp(2.5rem, 6vw, 6.3rem)`, 0.95): títulos de projeto e secção.
- **Title** (650, `clamp(1.35rem, 2.4vw, 2.2rem)`, 1.05): capacidades e itens selecionados.
- **Body** (400, `clamp(1rem, 1.25vw, 1.15rem)`, 1.65): máximo de 70 caracteres por linha.
- **Label** (700, 0.78rem, 0.08em): metadados curtos e numeração.

**The One Loud Line Rule.** Cada ecrã tem uma frase dominante; o resto ajuda-a.

## 4. Elevation

O sistema é estratificado por cor e oclusão. Sombras amplas aparecem apenas em previews de produto que precisam de se separar do palco; superfícies editoriais mantêm-se planas.

### Shadow Vocabulary

- **Stage Shadow** (`0 32px 90px oklch(5% 0.025 250 / 0.46)`): janelas de projeto em destaque.
- **Signal Glow** (`0 0 42px oklch(84% 0.20 135 / 0.18)`): hover e foco de ações primárias.

**The Flat Stage Rule.** O palco é plano; só o objeto demonstrado levanta.

## 5. Components

### Buttons

- **Shape:** retângulos técnicos com cantos de 6px.
- **Primary:** Signal Lime sobre Night Ink, `14px 20px`, peso 700.
- **Hover / Focus:** deslocação de 2px, glow controlado e foco visível de 2px.
- **Ghost:** superfície escura com contorno Soft Line; inverte para Warm Paper no hover.

### Chips

- **Style:** palavras curtas em linha, sem cápsulas excessivamente redondas. Fundos transparentes e divisores discretos.

### Cards / Containers

- **Corner Style:** 14px em janelas, 6px em controlos.
- **Background:** Midnight Surface ou cores específicas do projeto.
- **Shadow Strategy:** Stage Shadow apenas nos previews grandes.
- **Border:** 1px Soft Line.
- **Internal Padding:** fluido entre 20px e 48px.

### Inputs / Fields

- **Style:** fundo Night Ink, contorno Soft Line, raio de 6px.
- **Focus:** contorno Signal Lime e halo discreto.
- **Error / Disabled:** mensagem explícita; nunca depender apenas da cor.

### Navigation

Barra fina e persistente, marca à esquerda, índice curto ao centro e contacto evidente à direita. No telemóvel, preserva a marca e o contacto e reduz os atalhos.

### Project Stage

Cada projeto de destaque ocupa uma composição única com uma miniinterface reconhecível, cor própria, contexto, responsabilidades e um link direto. O palco responde ao ponteiro com inclinação subtil, nunca dificulta a leitura.

## 6. Do's and Don'ts

### Do:

- **Do** mostrar ferramentas, mapas, pesquisa, dados e estados em miniinterfaces reais.
- **Do** usar Signal Lime apenas para ações e disponibilidade.
- **Do** manter texto corrido entre 65 e 70 caracteres por linha.
- **Do** transformar movimento em progressão narrativa e oferecer `prefers-reduced-motion`.
- **Do** preservar uma voz direta, portuguesa e segura.

### Don't:

- **Don't** criar o portfólio genérico de agência ou um catálogo interminável de serviços.
- **Don't** usar grelhas repetidas de cartões, estética SaaS copiada ou promessas vagas.
- **Don't** usar gradient text, glassmorphism decorativo ou listas de ícones em caixas idênticas.
- **Don't** usar `border-left` ou `border-right` espesso como acento.
- **Don't** usar efeitos sem relação com o conteúdo ou uma página que pareça uma template produzida por IA.
