# Ykedin Sushi · site

Site de uma página do Ykedin Sushi (Jacobina e Capim Grosso, BA). HTML, CSS e JavaScript puros, sem build e sem dependências.

## Estrutura

- `site/` é a pasta publicada: `index.html` e `assets/` (fotos, logotipo, flor e vídeos já comprimidos).
- `tools/servidor.js` sobe uma pré-visualização local.
- `pacote-de-design.md` reúne as decisões de marca, texto e engenharia.

## Pré-visualizar

```bash
node tools/servidor.js
```

Depois abra http://localhost:5173 no navegador. Dar dois cliques no `index.html` também funciona, mas nesse caso a abertura aparece como imagem parada, porque o navegador bloqueia o vídeo em arquivos locais.

## Publicar

Suba o conteúdo de `site/` para a raiz da hospedagem (por exemplo, `public_html` na HostGator). O site está no ar em https://www.grupoykedin.com.br, publicado pela Vercel a cada envio ao GitHub. Se o domínio mudar, troque as URLs marcadas com `DEPLOY STEP` no `index.html`, o `robots.txt`, o `sitemap.xml` e o redirecionamento do `vercel.json`.
