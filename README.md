# Hamburgueria e Açaí Nova aliança delivery

Landing page estática, responsiva e pronta para Cloudflare Pages.

## Conteúdo

- `index.html`: página única em português do Brasil.
- `styles.css`: identidade visual, layout responsivo e acessibilidade.
- `script.js`: atualização automática do ano no rodapé.
- `assets/ilustracao-gastronomica.webp`: ilustração gastronômica gerada por IA. Não representa produtos específicos nem fotografias reais da empresa.
- `_headers`: cabeçalhos de segurança e cache para Cloudflare Pages.
- `robots.txt`: permite indexação pública.

## Testar localmente

Abra `index.html` no navegador. Para um servidor local, dentro desta pasta execute:

```bash
python3 -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Publicar no Cloudflare Pages pelo celular

A forma mais simples é o **Direct Upload** (envio direto). A documentação oficial confirma que o painel aceita um arquivo ZIP ou uma pasta de arquivos estáticos.

1. Baixe o ZIP deste projeto e mantenha-o no celular.
2. Entre em https://dash.cloudflare.com/ e faça login.
3. Abra **Workers & Pages**.
4. Selecione **Create application** → **Get started** → **Drag and drop your files** (os nomes podem variar um pouco conforme o idioma da conta).
5. Nomeie o projeto, por exemplo `nova-alianca-delivery`.
6. Selecione e envie `hamburgueria-nova-alianca-cloudflare.zip`.
7. Selecione **Deploy site**. A Cloudflare fornecerá um endereço `*.pages.dev` quando o deploy terminar.

Este projeto é estático: não precisa de comando de build nem instalação de dependências. Se a interface pedir uma pasta, extraia o ZIP e envie a pasta `nova-alianca-cloudflare` que contém `index.html`.

**Importante:** a Cloudflare informa que um projeto criado com Direct Upload não pode ser convertido depois em um projeto com integração Git. Se você pretende usar GitHub com deploy automático, é melhor criar um projeto separado já com Git integration.

Documentação oficial: https://developers.cloudflare.com/pages/get-started/direct-upload/

## Antes de divulgar

- Confirme com a empresa se a nota 4,7 e as 60 avaliações continuam atuais.
- Confirme o endereço e o telefone/WhatsApp.
- A ilustração é conceitual e deve permanecer identificada como gerada por IA; substitua-a por fotos reais somente com autorização do proprietário.
- Horários, produtos, cardápio, preços e condições de entrega foram omitidos porque não foram confirmados.
- Adicione domínio próprio somente depois de registrá-lo e configurá-lo na Cloudflare.

## Dados usados

WhatsApp: `+5511943725396`  
Maps: https://www.google.com/maps/search/?api=1&query=Hamburgueria%20e%20A%C3%A7a%C3%AD%20Nova%20alian%C3%A7a%20delivery&query_place_id=ChIJ_3KCejE3zpQRFfm7ZtG64qs
