# Clareando — Clara Fernandes

Landing page do estúdio fotográfico Clareando, com portfólio, especialidades, experiências e solicitação de orçamento.

## Estrutura do projeto

```text
.
├── site/                       # Site estático pronto para publicação
├── README.md
└── render.yaml                 # Configuração de publicação no Render
```

## Visualizar localmente

Na raiz do projeto, execute:

```bash
python -m http.server 8000 --directory site
```

Abra `http://localhost:8000`.

O site usa Tailwind CSS e Alpine.js via CDN e Google Fonts, então esses recursos externos precisam de conexão à internet. O formulário prepara uma mensagem para o WhatsApp oficial `+55 84 99674-0734`; o envio só acontece após confirmação no aplicativo. Instagram: `@clareandofotografia`.

## Publicação

O Render publica o conteúdo de `site/` como site estático. Os documentos de trabalho e as imagens originais não fazem parte deste repositório público.
