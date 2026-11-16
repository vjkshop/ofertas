# Landing Page VJKShop

Arquivos prontos para hospedagem estática. Abra `index.html` no navegador para conferir.

## Publicar no Cloudflare Pages

1. No Cloudflare Dashboard, abra **Workers & Pages** > **Create** > **Pages** > **Upload assets** (a interface pode variar).
2. Envie o conteúdo da pasta `vjkshop-site` (ou o ZIP, se o painel aceitar).
3. A página abre direto em `/` com os dois links funcionando.

## Links usados
- Telegram: https://t.me/VJKShop
- WhatsApp: https://chat.whatsapp.com/C8wWEFZkuzw6RbzSBs4nAs?s=cl&p=a&iam=2

## Mensuração de campanhas
Os botões disparam o evento `join_group_click`, com parâmetros `platform` (whatsapp ou telegram) e `placement` (hero, final ou sticky).
Se você instalar Meta Pixel, será enviado `fbq('trackCustom','JoinGroupClick',...)`. Com GA4, será enviado `gtag('event','join_group_click',...)`.
**Sem Pixel/GA4 conectado, os eventos não são coletados por nenhum serviço externo.** Não inventamos números de vendas, descontos, membros ou provas sociais.

**Importante:** o evento conta o clique no convite, não a confirmação da entrada no aplicativo. Configure eventos e consentimento de cookies conforme os rastreadores usados.

## Personalização
- `index.html` possui todo HTML, CSS e JS.
- `assets/vjkshop-logo.webp` usa a imagem enviada.
- `assets/og-vjkshop.jpg` é uma prévia para compartilhamento (metadados OG apontam para o caminho relativo; depois de publicar, pode ser necessário usar a URL absoluta).
- Fontes externas (Google Fonts) têm fallback seguro caso não carreguem.
