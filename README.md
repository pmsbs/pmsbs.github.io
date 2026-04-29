# pmsbs.github.io

Site institucional da Prefeitura Municipal de São Bento do Sapucaí - SP, desenvolvido com Jekyll e hospedado no GitHub Pages.

**Link ao vivo**: https://pmsbs.sp.gov.br/

## Desenvolvimento Local

### Pré-requisitos

- [Ruby](https://www.ruby-lang.org/) (versão compatível com Jekyll)
- [Jekyll](https://jekyllrb.com/)
- [Bundler](https://bundler.io/)

### Comandos

```bash
# Instalar dependências (se houver Gemfile)
bundle install

# Iniciar servidor de desenvolvimento
bundle exec jekyll serve

# Build para produção
bundle exec jekyll build
```

O servidor de desenvolvimento fica disponível em `http://localhost:4000` com live reload automático.

## Estrutura

| Diretório | Descrição |
|---|---|
| `_posts/` | Páginas de conteúdo (cada post é uma página do site) |
| `_layouts/` | Layouts HTML (apenas `default.html`) |
| `_sass/` | Módulos SCSS parciais |
| `assets/` | CSS compilado, imagens e outros recursos estáticos |

## Convenções

- Nome dos posts: `YYYY-MM-DD-slug.md`
- Todo post deve ter `layout: default` e `title` no front matter
- Cor primária: `#095B2E` (definida em `_sass/_base.scss`)
- Fonte: Roboto (Google Fonts)