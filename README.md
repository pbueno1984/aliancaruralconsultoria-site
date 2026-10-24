# aliancaruralconsultoria.com.br

Site estático da Aliança Rural Consultoria, publicado pelo GitHub Pages.

- `index.html`: página inicial
- `sigcar/index.html`: página do Plano SIGCAR (destino dos anúncios)
- `assinatura/index.html`: Plano SIGCAR por Assinatura, com preços por imóvel rural e simulador
- `assets/`: logo, imagens (créditos no rodapé) e brasão
- `CNAME`: domínio próprio

## Publicar

Settings › Pages › Source: branch `main`, pasta `/ (root)`. Custom domain: `aliancaruralconsultoria.com.br`, marcar "Enforce HTTPS" quando liberar.

## DNS na GoDaddy (não mexer nos registros MX do e-mail)

| Tipo | Nome | Valor |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | pbueno1984.github.io |
