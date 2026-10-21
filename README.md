# Sebo Amazônia

Site estático do Sebo Amazônia, em Manaus. HTML, CSS e JavaScript puro, sem instalação de dependências, etapa de build ou variáveis de ambiente.

## Desenvolvimento

Com Python 3 instalado, execute na raiz do repositório:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

O servidor entrega `index.html`, `styles.css`, `script.js` e as imagens locais em `assets/`.

## Publicar na Vercel

1. Na Vercel, escolha **Add New → Project** e importe este repositório do GitHub.
2. Use **Framework Preset: Other** e a raiz do repositório como **Root Directory**.
3. Não configure comando de instalação nem de build. O `vercel.json` define a saída como a própria raiz (`.`).
4. Não são necessárias variáveis de ambiente. Clique em **Deploy**.
5. Após publicar, confira o menu no celular, as fotos e os links de WhatsApp e localização. O mapa incorporado depende de acesso ao Google Maps.

Depois de conectar o GitHub, novos pushes na branch de produção configurada na Vercel geram novos deploys. O domínio personalizado pode ser configurado em **Settings → Domains**.

## Arquivos

- `index.html`: conteúdo, contatos e links da loja.
- `styles.css`: layout responsivo, efeitos de hover, foco de teclado e preferência de movimento reduzido.
- `script.js`: menu móvel, incluindo fechamento por Escape e ao selecionar um link.
- `assets/`: as 25 fotos extraídas do HTML original, sem alterar os arquivos de imagem.
- `vercel.json`: configuração de publicação estática e cabeçalhos HTTP.

Os dados de endereço, horário e avaliações foram mantidos do arquivo fornecido. Confira se continuam atuais antes da publicação.
