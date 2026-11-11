# Design system — Clareando

## Direção de arte

Fotografia editorial / fine art: minimalista, sofisticada, acolhedora e atemporal. As imagens conduzem a narrativa; interface, tipografia e ornamentos devem apoiar o conteúdo, sem competir com ele.

## Princípios

1. **Imagem em primeiro lugar:** priorizar fotografias expressivas e autorizadas.
2. **Respiro:** usar margens generosas e ritmo vertical calmo.
3. **Calor sem excesso:** tons neutros com acentos dourados discretos.
4. **Clareza:** textos legíveis, navegação previsível e chamadas diretas.
5. **Atemporalidade:** evitar efeitos e tendências visuais que envelheçam rapidamente.

## Cores

| Token | Valor | Uso |
|---|---|---|
| `color-background` | `#FAF8F5` | Fundo principal off-white. Alternativa de fundo: `#F7F4EF`. |
| `color-surface` | `#EFECE6` | Cards, blocos e áreas de apoio. |
| `color-accent` | `#D4A373` | Acento dourado suave / golden hour. |
| `color-accent-alt` | `#C59B27` | Variação de destaque, usar com moderação. |
| `color-text` | `#1C1917` | Textos principais e títulos. |

Usar `#1C1917` sobre os fundos claros para leitura. Não usar os dourados como cor de texto pequeno sem validar contraste; reservar para detalhes, ícones, bordas e elementos decorativos. Verificar contraste de todos os estados interativos antes da publicação.

## Tipografia

- **Títulos:** `Playfair Display` ou `Cormorant Garamond`, com fallback serifado.
- **Corpo e interface:** `Inter` ou `Plus Jakarta Sans`, com fallback sans-serif.
- Criar hierarquia por tamanho, peso e espaçamento; evitar longos blocos em caixa alta.
- Manter corpo confortável para leitura em celular e altura de linha generosa.
- Carregar apenas pesos realmente utilizados e configurar fallbacks para reduzir mudanças de layout.

## Layout e espaçamento

- Composição editorial com conteúdo centralizado e largura de leitura limitada.
- Usar áreas amplas de imagem e margens generosas em telas grandes.
- Reduzir margens sem comprimir conteúdo em telas pequenas.
- Usar espaçamento consistente em múltiplos de uma unidade-base definida na implementação.
- Alternar áreas de imagem, texto e fundo neutro para criar ritmo visual.

## Fotografia e galeria

- Grade de portfólio estilo galeria/masonry, com proporções variadas e alinhamento consistente.
- Destacar retratos em preto e branco, ensaios ao ar livre e cobertura de eventos emocionais.
- Manter a edição coerente sem uniformizar artificialmente diferentes histórias ou tons de pele.
- Usar recortes responsivos que preservem rostos e o assunto principal.
- Disponibilizar ampliação com controles acessíveis, fechamento claro e navegação por teclado, se houver lightbox.
- Comprimir imagens e carregar sob demanda as que estiverem fora da primeira dobra, preservando qualidade visual.
- Obter autorização para publicação e fornecer texto alternativo adequado.

## Componentes

### Cabeçalho

Marca Clareando, navegação principal e chamada de contato. Em telas pequenas, menu com rótulo acessível, foco visível e fechamento por teclado.

### Botões e links

- CTA primário com contraste forte e texto explícito.
- CTA secundário discreto, mantendo área de toque confortável.
- Estados visíveis de hover, foco, pressionado e desabilitado.
- Não comunicar estado apenas por cor.

### Cards de serviço/experiência

Fundo `#EFECE6`, espaçamento interno generoso, título serifado e descrição curta em sans-serif. Não destacar uma experiência como “mais popular” sem decisão da marca.

### Formulário

Rótulo persistente em cada campo, instruções claras, validação compreensível e confirmação apenas após envio real. Informar campos obrigatórios, preservar os dados em caso de erro e oferecer aviso de privacidade.

## Responsividade e acessibilidade

- Projetar mobile-first e validar em larguras pequenas, médias e grandes.
- Garantir navegação por teclado, ordem de foco lógica, foco claramente visível e títulos semânticos.
- Usar texto redimensionável, contraste adequado e alvos de toque confortáveis.
- Respeitar `prefers-reduced-motion`; animações devem ser sutis e não essenciais.
- Não usar imagem como único meio de transmitir informação.
- Verificar contraste de texto, botões e controles em todos os estados.

## Movimento

Transições suaves e breves apenas quando ajudam a orientar a atenção. Evitar movimento automático na galeria; qualquer carrossel deve permitir controle e pausa.

## Tokens adicionais para implementação

Definir na camada de interface, conforme o projeto:

- raios de borda discretos e consistentes;
- sombras suaves apenas para separar superfícies quando necessário;
- largura máxima de leitura e pontos de quebra orientados pelo conteúdo;
- escalas de tipografia, espaçamento e duração de transições.

Os valores de implementação devem ser ajustados e validados no site real, sem alterar a paleta e a direção visual definidas neste documento.
