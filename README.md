# site-preto-teste

Site estático com fundo todo preto e a palavra "teste" no centro. Pronto para publicar no Cloudflare Pages.

## Estrutura

```
index.html   página única
_headers     cabeçalhos HTTP (opcional)
```

## Publicar no Cloudflare Pages (pelo painel)

1. Suba este repositório para o GitHub.
2. No painel da Cloudflare, vá em **Workers & Pages** > **Create** > **Pages** > **Connect to Git**.
3. Escolha o repositório `site-preto-teste`.
4. Configure o build:
   - **Framework preset:** None
   - **Build command:** (deixe vazio)
   - **Build output directory:** `/`
5. Clique em **Save and Deploy**.

O site fica disponível em `https://NOME-DO-PROJETO.pages.dev`. Para usar seu domínio, abra o projeto e vá em **Custom domains**.

## Publicar pela linha de comando (opcional)

```bash
npx wrangler pages deploy . --project-name=site-preto-teste
```

## Testar localmente

Abra o `index.html` no navegador ou rode:

```bash
npx serve .
```
