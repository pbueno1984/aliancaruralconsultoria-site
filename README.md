# aliancaruralconsultoria.com.br

Site estático da Aliança Rural Consultoria, publicado pelo GitHub Pages.

- `index.html`: página inicial
- `sigcar/index.html`: página do Plano SIGCAR (destino dos anúncios)
- `assinatura/index.html`: assinaturas (SIGCAR, Outorga, Licença, DAI, Regularidade Total), diagnóstico avulso e simulador. Preços gerados da planilha `modelo_precificacao_assinaturas.xlsx`
- `assets/`: logo, imagens (créditos no rodapé) e brasão
- `CNAME`: domínio próprio

## Publicar

Settings › Pages › Source: branch `main`, pasta `/ (root)`. Custom domain: `aliancaruralconsultoria.com.br`, marcar "Enforce HTTPS" quando liberar.

## DNS na Cloudflare (não mexer nos registros MX do e-mail)

Os servidores de nome do domínio estão na Cloudflare (o registro continua na GoDaddy).
Registros do site, todos em "DNS only" (nuvem cinza), apontando para o GitHub Pages:

| Tipo | Nome | Valor |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | pbueno1984.github.io |

Outros registros que não fazem parte deste site:
- MX `smtp.secureserver.net` / `mailstore1.secureserver.net`: e-mail da GoDaddy.
- CNAME `mapas` → Cloudflare Tunnel: área do cliente com os mapas, servida pelo
  servidor do escritório e protegida por login (Cloudflare Access). Criado pelo
  painel do túnel; não editar à mão.

## Não enviar para este repositório

O repositório é público e o histórico guarda tudo, mesmo o que for apagado depois.
Nunca enviar senhas, tokens, `.env`, a planilha de precificação, documentos ou mapas
de clientes.
