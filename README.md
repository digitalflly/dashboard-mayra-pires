# Dashboard Mayra Pires

Dashboard de análise de conteúdo — painel de página única (SPA) em React, sem
build/bundler, com dados servidos por Windsor.ai e calendário de produção do
Notion. Roda 100% no navegador a partir de um snapshot embutido e atualiza com
dados ao vivo via função serverless.

## Estrutura do repositório

```
Dashboard.dc.html   Página principal do dashboard (carrega support.js + design system)
support.js          Runtime dc (gerado a partir de dc-runtime/src/*.ts)
_ds/                Design System "Digital Flly" (tokens, componentes, fontes)
screenshots/        Capturas de tela do dashboard
uploads/            Materiais de referência e documentação técnica
  DOCUMENTACAO.md   Documentação técnica da arquitetura do dashboard
```

## Como visualizar

Abra `Dashboard.dc.html` num servidor estático (as folhas de estilo e o runtime
são carregados por caminhos relativos). Por exemplo:

```bash
python3 -m http.server 8000
# depois acesse http://localhost:8000/Dashboard.dc.html
```

## Documentação

A arquitetura, as fontes de dados e os cálculos estão detalhados em
[`uploads/DOCUMENTACAO.md`](uploads/DOCUMENTACAO.md). O design system tem seu
próprio README em `_ds/`.
