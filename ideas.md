# Study Cycle - Brainstorm de Design

## Contexto
Aplicativo web de cronograma de estudos personalizado com Ciclo Contínuo de 9 sessões, timer, caderno de erros, dashboard de performance e edital verticalizado. Design moderno com dark mode, interface limpa e dashboard visual.

---

## Abordagem 1: Minimalismo Funcional com Acentos Dinâmicos (Probabilidade: 0.08)

**Design Movement:** Bauhaus Digital + Neomorfismo Suave

**Core Principles:**
- Clareza absoluta: cada elemento tem propósito visual e funcional
- Hierarquia através de espaçamento e peso tipográfico, não cores saturadas
- Acessibilidade como prioridade: alto contraste, tipografia legível, navegação intuitiva
- Profundidade sutil através de sombras suaves e elevações, não gradientes

**Color Philosophy:**
- Paleta: Cinza neutro (fundo), branco/off-white (cards), azul profundo (primário), verde menta (sucesso), laranja suave (alerta)
- Reasoning: Reduz fadiga visual em sessões longas de estudo; cores neutras permitem que dados e gráficos sejam protagonistas
- Dark mode: Fundo cinza muito escuro (quase preto), cards em cinza charcoal, acentos mantêm saturação

**Layout Paradigm:**
- Grid assimétrico: sidebar fixa (esquerda) com navegação principal; área central com conteúdo fluido
- Seções empilhadas verticalmente com breathing room (espaçamento gerado)
- Cards com elevação sutil (shadow-sm) em vez de bordas

**Signature Elements:**
- Indicador circular de progresso do ciclo (SVG animado, mostra sessão atual)
- Badges minimalistas para status (Em Progresso, Concluído, Pendente)
- Linhas divisoras suaves em vez de bordas pesadas

**Interaction Philosophy:**
- Transições suaves (300ms) em hover/focus
- Feedback imediato: ripple effect em botões, mudança de cor em inputs
- Confirmações visuais sem pop-ups intrusivos (toast notifications)

**Animation:**
- Timer conta regressivamente com mudança de cor gradual (verde → amarelo → vermelho)
- Progresso do ciclo anima suavemente ao avançar de sessão
- Gráficos animam ao carregar (entrada suave de barras/dados)

**Typography System:**
- Display: Poppins Bold 32px (títulos de página)
- Heading: Poppins SemiBold 20px (títulos de seção)
- Body: Inter Regular 14px (corpo de texto)
- Mono: JetBrains Mono 12px (dados numéricos, timestamps)
- Hierarquia: peso e tamanho, não cor

---

## Abordagem 2: Gamificação Vibrante com Progressão Visual (Probabilidade: 0.07)

**Design Movement:** Neumorphism Colorido + Micro-interactions Lúdicas

**Core Principles:**
- Engajamento através de feedback visual constante
- Progressão visível em cada ação (animações, sons visuais, badges)
- Cores vibrantes mas harmônicas para manter foco
- Elementos 3D suaves (pseudo-3D com sombras e gradientes)

**Color Philosophy:**
- Paleta: Fundo gradiente (azul profundo → roxo escuro), cards em vidro fosco (glassmorphism), acentos em gradientes (azul → ciano, verde → lima)
- Reasoning: Cria sensação de imersão e progresso; cores vibrantes motivam continuidade de estudos
- Dark mode: Fundo com gradiente sutil, cards translúcidos com backdrop blur

**Layout Paradigm:**
- Layout em grid 3 colunas (desktop) com cards flutuantes
- Sidebar retrátil com ícones grandes e coloridos
- Dashboard principal com widgets em tamanhos variados (masonry-like)

**Signature Elements:**
- Ícones grandes e coloridos para cada matéria
- Badges animadas com efeito de "pop" ao ganhar pontos
- Barra de progresso com gradiente animado
- Confete visual ao completar sessão (CSS animation)

**Interaction Philosophy:**
- Hover: cards elevam, sombra aumenta, cor muda
- Click: ripple effect colorido, feedback tátil visual
- Completar tarefa: animação de confete, som visual, badge aparece

**Animation:**
- Confete ao completar sessão (CSS keyframes)
- Barras de progresso crescem suavemente
- Números contadores animam de forma fluida (0 → valor final)
- Ícones giram levemente em hover

**Typography System:**
- Display: Montserrat Bold 36px (títulos, impactante)
- Heading: Montserrat SemiBold 22px (seções)
- Body: Poppins Regular 15px (legível, amigável)
- Accent: Poppins Bold 14px (destaques, badges)
- Hierarquia: peso, tamanho e cor

---

## Abordagem 3: Elegância Corporativa com Foco em Dados (Probabilidade: 0.06)

**Design Movement:** Data Visualization Premium + Swiss Design

**Core Principles:**
- Dados como protagonista: gráficos e métricas são o foco visual
- Elegância através de tipografia refinada e espaçamento generoso
- Profissionalismo: paleta restrita, sem excesso visual
- Usabilidade avançada: múltiplas visualizações de dados, filtros inteligentes

**Color Philosophy:**
- Paleta: Fundo branco/off-white, cards em tons de cinza claro, primário em azul navy, secundário em dourado/bronze
- Reasoning: Transmite profissionalismo e confiança; paleta restrita permite que dados brilhem
- Dark mode: Fundo cinza escuro, cards em cinza médio, acentos em dourado/bronze mantêm elegância

**Layout Paradigm:**
- Layout em 12 colunas com alinhamento preciso
- Sidebar com navegação em abas (tabs)
- Dashboard com widgets em grid regular (4 colunas)
- Espaçamento generoso (16px/24px entre elementos)

**Signature Elements:**
- Ícones minimalistas em estilo line-art
- Tabelas com alternância de cores de linha
- Gráficos em estilo corporativo (recharts com cores restritas)
- Números grandes e legíveis para KPIs principais

**Interaction Philosophy:**
- Hover: mudança sutil de cor/opacidade
- Click: feedback visual sem excesso
- Tooltips informativos em hover de gráficos
- Transições suaves e previsíveis

**Animation:**
- Gráficos animam ao carregar (entrada suave)
- Números contadores animam com easing elegante
- Transições entre abas suaves (fade + slide)
- Hover em gráficos mostra tooltip com animação suave

**Typography System:**
- Display: Playfair Display Bold 40px (títulos principais, elegância)
- Heading: Lato SemiBold 24px (seções)
- Body: Lato Regular 14px (corpo, legível)
- Data: IBM Plex Mono 13px (números, dados)
- Hierarquia: peso, tamanho e espaçamento

---

## Decisão Final

Será implementada a **Abordagem 1: Minimalismo Funcional com Acentos Dinâmicos**, pois oferece o melhor equilíbrio entre clareza visual, acessibilidade e funcionalidade para um aplicativo de estudos de longa duração. A paleta neutra reduz fadiga visual, a hierarquia clara facilita navegação, e as animações suaves fornecem feedback sem distração.

### Implementação:
- **Tipografia:** Poppins (títulos) + Inter (corpo) + JetBrains Mono (dados)
- **Cores:** Cinza neutro, azul profundo (#1e40af), verde menta (#10b981), laranja suave (#f97316)
- **Componentes:** Cards com elevação sutil, badges minimalistas, indicador circular de progresso
- **Animações:** Transições 300ms, timer com mudança de cor gradual, gráficos com entrada suave
