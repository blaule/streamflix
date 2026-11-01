# StreamFlix

Site estático (página única) hospedado com GitHub Pages.

## Estrutura

- `index.html` — o site inteiro (HTML, CSS e JavaScript em um arquivo)
- `.nojekyll` — desativa o processamento Jekyll do GitHub Pages
- `.gitignore` — arquivos ignorados pelo Git

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `streamflix`), público.
2. Envie os arquivos deste projeto para o repositório:
   ```bash
   git init
   git add .
   git commit -m "Primeiro commit"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/streamflix.git
   git push -u origin main
   ```
3. No GitHub, vá em **Settings → Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e clique em **Save**.
5. Após alguns minutos, o site ficará em `https://SEU-USUARIO.github.io/streamflix/`.

## Observações

- A chave da API do TMDB, se usada no HTML, fica visível para qualquer visitante.
- Os cadastros feitos pelo painel admin são salvos apenas no `localStorage` do navegador de cada pessoa.
- Publique apenas conteúdo ao qual você tem direitos de exibição.
