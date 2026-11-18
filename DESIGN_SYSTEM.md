# Design System & Arquitetura Visual — Site Juliana Garcia (Psicóloga)

## 1. Visão Geral & Conceito Estético
* **Estilo Visual:** Editorial orgânico, minimalista, acolhedor e sofisticado.
* **Atmosfera:** Transmitir segurança, calma, empatia e profissionalismo clínico.
* **Diretriz Dinâmica de Cores:** A estrutura, tipografia e espaçamentos deste documento seguem rigorosamente o layout de referência, **porém a paleta de cores definitiva deve ser extraída automaticamente dos arquivos de logomarca presentes na pasta do projeto** (substituindo os tokens de cor abaixo pelos tons correspondentes da marca da Juliana Garcia).

---

## 2. Tokens de Cores (Paleta extraída da logomarca)
*Os PNGs da pasta `Logomarca` foram inspecionados pixel a pixel. As cores sólidas recorrentes da identidade são púrpura `#A8518A`, azul-marinho `#333A5A` e branco `#FEFEFE`. As superfícies abaixo são tons de apoio derivados desses valores para preservar contraste e a atmosfera editorial da referência.*

* **Background Principal (`--bg-primary`):** Creme rosado muito claro (`#FCF9F8`) — usado nas seções principais e áreas de leitura.
* **Background Secundário / Superfície (`--bg-surface`):** Lavanda rosada suave (`#F3EBF0`) — usado em cards, badges de ícones e blocos de destaque suave.
* **Background de Encerramento (`--bg-footer-cta`):** Rosa-bege muito claro derivado da cor primária (`#F2E4EC`) — usado na faixa de chamada final antes do rodapé.
* **Cor Primária / Ação (`--color-primary`):** Púrpura exato da logomarca (`#A8518A`) — usada em botões principais (CTAs), palavras destacadas nos títulos e detalhes de foco.
* **Cor Secundária / Estrutura (`--color-secondary`):** Azul-marinho exato da logomarca (`#333A5A`) — usado em textos, navegação, fundos escuros e elementos de contraste.
* **Tons de Apoio (`--color-support`):** Branco de aplicação (`#FEFEFE`) e rosa névoa (`#EAD9E3`) — usados em contraste, estados suaves e detalhes decorativos.
* **Texto Principal (`--text-primary`):** Azul-marinho da marca (`#333A5A`) — alto conforto de leitura sem o peso do preto puro (`#000000`).
* **Texto Secundário (`--text-secondary`):** Azul ardósia suavizado (`#686879`) — usado em parágrafos descritivos, subtítulos e legendas.
* **Bordas & Divisores (`--border-subtle`):** Linhas finas em baixa opacidade (`rgba(51, 58, 90, 0.14)`).

---

## 3. Tipografia
* **Fonte para Títulos (Display / Headings):** Serifada editorial elegante (ex: `Cormorant Garamond`, `Playfair Display` ou `Lora`).
  * **Peso:** Regular (400) e Medium (500).
  * **Estilo:** Permite destaque semântico em palavras-chave dentro do título usando a `--color-primary` (ex: *"Cuidar da sua **mente** também é prioridade"*).
* **Fonte para Corpo e Interface (Sans-serif):** Humanista limpa e legível (ex: `Plus Jakarta Sans`, `DM Sans` ou `Inter`).
  * **Kicker / Eyebrow (Sobretítulos):** Caixa alta (`UPPERCASE`), tamanho `11px`–`12px`, `letter-spacing: 0.12em`, peso `600`.
  * **Corpo de Texto:** `15px`–`16px`, altura de linha (`line-height`) `1.65` para leitura fluida.
* **Assinatura Visual:** Fonte manuscrita/caligráfica fluida (ex: `Caveat`, `Alex Brush` ou arquivo SVG da assinatura) na seção "Sobre mim".

---

## 4. Layout, Grid & Espaçamento
* **Container Máximo:** `1140px` a `1200px` centralizado, com padding lateral responsivo (`24px` mobile / `48px` desktop).
* **Ritmo Vertical:** Espaçamento generoso entre seções (`80px` a `112px` no desktop; `56px` no mobile).
* **Arredondamento (Border Radius):**
  * **Fotos e Containers de Imagem:** `16px` a `20px` (cantos suaves e orgânicos).
  * **Botões:** `8px` a `10px` (retângulo levemente arredondado, moderno e discreto).
  * **Badges de Ícones:** `50%` (círculos perfeitos).

---

## 5. Componentes & Elementos Gráficos

### A. Elementos Decorativos (Line Art)
* Ilustrações botânicas minimalistas (folhagens e ramos em traço fino `1px`–`1.5px`) posicionadas de forma sutil ao fundo com baixa opacidade (`10%` a `15%`).
* Símbolo da Psicologia ($\Psi$) estilizado em traço fino ou marca d'água discreta na seção final.

### B. Botões (CTAs)
* **Botão Primário:** Fundo `--color-primary`, texto branco (`#FFFFFF`), ícone do WhatsApp integrado à esquerda, padding `14px 28px`, transição suave de escurecimento (`hover:brightness-90`).
* **Selo de Confiança (Abaixo do CTA Hero):** Ícone de escudo/verificação + texto pequeno (`13px`) reforçando sigilo e acolhimento.

### C. Cards de Especialidades ("Como posso te ajudar")
* Layout em grid `2x2` (desktop) / `1 coluna` (mobile), sem bordas pesadas ou sombras fortes.
* **Estrutura interna:**
  1. Círculo (`48px x 48px`) em `--bg-surface` contendo ícone minimalista em linha fina (`stroke-width: 1.5`).
  2. Título da abordagem/demanda em fonte serifada (`20px`).
  3. Breve descrição acolhedora de 2 a 3 linhas.

---

## 6. Arquitetura de Seções (Landing Page)

1. **Header (Navegação Superior):**
   * Esquerda: Logomarca da **Juliana Garcia** (extraída da pasta do projeto).
   * Centro: Links limpos (`Início`, `Sobre`, `Atendimentos`, `Contato`) com indicador sutil no item ativo.
   * Direita: Botão compacto `"Agendar consulta"` com ícone do WhatsApp.
2. **Hero Section (Split 50/50):**
   * Coluna Esquerda: Kicker (`SAÚDE MENTAL • AUTOCONHECIMENTO • EQUILÍBRIO`), Headline de impacto com palavra-chave destacada na cor primária, subtítulo explicativo (atendimento online ou presencial), CTA principal e selo de sigilo.
   * Coluna Direita: Fotografia profissional da Juliana Garcia (da pasta do projeto) com cantos arredondados e enquadramento acolhedor.
3. **Seção "Sobre mim" (Split Assimétrico 40/60):**
   * Coluna Esquerda: Foto vertical secundária da Juliana em ambiente de consultório/acolhimento.
   * Coluna Direita: Título `"Sobre mim"`, 2 parágrafos humanizados sobre propósito e abordagem terapêutica, assinatura estilizada e registro profissional (`Psicóloga | CRP XX/XXXXX`).
4. **Seção "Como posso te ajudar" (Grid 2x2):**
   * Título centralizado/alinhado + 4 pilares principais (ex: *Ansiedade*, *Estresse*, *Autoestima*, *Relacionamentos* — ajustáveis conforme o perfil da Juliana).
5. **Banner CTA Final & Rodapé:**
   * Faixa em tom suave (`--bg-footer-cta`) com ícone de coração em linha fina, frase de acolhimento (*"Você não precisa enfrentar isso sozinho(a)."*), botão centralizado de agendamento e contatos diretos (WhatsApp e Instagram).
   * Rodapé minimalista com direitos autorais e CRP.

---

## 7. Diretrizes de Implementação para o OpenCode
1. **Assets Locais:** Listar e utilizar os arquivos de imagem e logotipo já presentes no diretório do projeto.
2. **Extração de Cores:** Analisar a paleta dominante da logomarca da Juliana Garcia antes de escrever o CSS/Tailwind config, aplicando-a aos tokens da Seção 2.
3. **Responsividade & Performance:** Garantir adaptação fluida para mobile, otimização de carregamento das fotos e links diretos (`https://wa.me...`) configuráveis para o WhatsApp da profissional.
