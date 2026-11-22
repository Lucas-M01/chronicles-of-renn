# Site estático para demonstração do VoxNovel

O site usa HTML e CSS e pode ser aberto diretamente no navegador. A página inicial reúne a sinopse e o índice. Cada capítulo tem uma URL própria e o texto em inglês fica em parágrafos dentro de um elemento `article`.

## Editar o conteúdo

1. Em `index.html`, edite a sinopse em inglês na seção `synopsis`.
2. Para alterar o crédito de autoria, edite a linha `byline` na página inicial e nas três páginas de capítulo.
3. Para revisar o texto original em inglês, edite o arquivo HTML do capítulo correspondente. Mantenha um `<p>...</p>` por parágrafo dentro de `<article>`. Ao colar texto, escreva `&amp;` para um `&` literal e `&lt;` para um `<` literal.
4. Mantenha o aviso de autorização do VoxNovel no rodapé. Se precisar ajustar a aparência, edite `styles.css`, que é compartilhado pelas quatro páginas.
5. Abra `index.html` no navegador e confira o índice e a navegação entre capítulos.

## Publicar pelo GitHub Pages

1. Quando quiser publicar, coloque os arquivos na raiz da branch que será usada pelo GitHub Pages e envie essa branch ao repositório no GitHub. Inclua o arquivo vazio `.nojekyll`, que desativa o processamento pelo Jekyll.
2. No repositório no GitHub, abra **Settings → Pages**. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Selecione a branch que contém os arquivos, por exemplo `main`, escolha **/(root)** e clique em **Save**.
4. Após a publicação, abra **Visit site** em **Settings → Pages**. Para um site de projeto, o endereço padrão segue o formato `https://USUARIO.github.io/REPOSITORIO/`. Os caminhos relativos mantêm os links e o CSS dentro do subdiretório do projeto. [Documentação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Testar no VoxNovel

Use a URL publicada da página inicial ou de um capítulo, por exemplo `https://USUARIO.github.io/REPOSITORIO/chapter-1.html`. A compatibilidade com o VoxNovel, incluindo cadastro e navegação automática entre capítulos, depende de teste posterior no aplicativo.
