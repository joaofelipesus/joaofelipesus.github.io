# joaofelipesus.github.io

Blog pessoal hospedado no GitHub Pages, gerado com Jekyll.

## Estrutura

```text
├── _posts/            textos do blog (YYYY-MM-DD-titulo.md)
├── _layouts/          templates HTML
│   ├── default.html   estrutura geral do site
│   └── post.html      estrutura de um post
├── assets/css/        CSS do site
├── about.md           página "Sobre"
├── index.md           página inicial
└── _config.yml        configuração do Jekyll
```

## Publicar um novo texto

```bash
vim _posts/2026-08-25-alguma-coisa.md

git add .
git commit -m "Adiciona nota sobre alguma coisa"
git push
```

O GitHub Pages publica a nova versão automaticamente.

## Filosofia

A estrutura deve permanecer simples. A prioridade é escrever, publicar e
continuar escrevendo. Tema, SEO, analytics, comentários e busca podem ser
adicionados depois, caso realmente sejam necessários.
