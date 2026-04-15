# CLAUDE.md — CMMANAUS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** CMMANAUS
**Nicho:** Educação
**Keywords:** Criei esse blog a 3 anos sempre passando todo meu conhecimento de
**Paleta de cores:** rose | **Fonte:** outfit

Criei esse blog a 3 anos, sempre passando todo meu conhecimento de forma clara e gratuita para que todas as pessoas possam desfrutar desses meus anos nas salas de aula. Eu escrevo para todos os públicos, de todos os níveis de conhecimento, iniciante ou avançado. Sempre terei um espaço reservado para você. Sempre irei compartilhar todo o tipo de conteúdo que envolva educação. Para acompanhar esse rico e belo conteúdo, baste se inscrever em minha newsletter. Renata Padilha Olá! Meu nome é Renata Padilha, tenho 45 anos, sou fundadora do Cmanaus. Uma pessoa do bem com o objetivo de ajudar pais e crianças que buscam conteúdo e informação sobre educação. Sou Professora a mais de 20 anos, formada em pedagogia pela Faculdade Federal de Manaus. Trabalhei toda minha vida com o ensino militar. Este blog foi criado para transmitir meu conhecimento e experiências pessoais adquiridas ao longo dos anos nas salas de aula. Busquei sempre formar uma equipe de professores bem capacitados para me ajudar nessa jornada.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-H |
| Hero | Hero-B |
| Features | Features-D |
| About Section | About-B |
| Posts | Posts-F |
| Footer | Footer-B |
| Página Sobre | Sobre-G |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
