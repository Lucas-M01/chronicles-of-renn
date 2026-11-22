# Site estático para demonstração do VoxNovel

O site usa HTML e CSS e pode ser aberto diretamente no navegador. A página inicial reúne a sinopse e o índice. Cada capítulo tem uma URL própria e o texto em inglês fica em parágrafos dentro de um elemento `article`.

A edição revisada terá dez capítulos. O índice dá acesso ao novo Capítulo 1 e sinaliza os demais como futuros. Os arquivos `chapter-2.html` e `chapter-3.html` ainda guardam os textos da edição anterior e ficam fora da navegação da edição revisada até serem substituídos.

## Editar o conteúdo

1. Em `index.html`, edite a sinopse em inglês na seção `synopsis`.
2. Para alterar o crédito de autoria, edite a linha `byline` na página inicial e nas páginas de capítulo.
3. Para revisar o texto original em inglês, edite o arquivo HTML do capítulo correspondente. Mantenha um `<p>...</p>` por parágrafo dentro de `<article>`. Ao colar texto, escreva `&amp;` para um `&` literal e `&lt;` para um `<` literal.
4. Ao adicionar um capítulo revisado, use `chapter-1.html` como modelo. Atualize o índice e os links dos capítulos vizinhos quando seus textos estiverem disponíveis.
5. Mantenha o crédito de direitos autorais e o aviso de autorização do VoxNovel no rodapé. Abra `index.html` no navegador para conferir o índice e a navegação.

## Publicar pelo GitHub Pages

1. Quando quiser publicar, coloque os arquivos na raiz da branch que será usada pelo GitHub Pages e envie essa branch ao repositório no GitHub. Inclua o arquivo vazio `.nojekyll`, que desativa o processamento pelo Jekyll.
2. No repositório no GitHub, abra **Settings → Pages**. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Selecione a branch que contém os arquivos, por exemplo `main`, escolha **/(root)** e clique em **Save**.
4. Após a publicação, abra **Visit site** em **Settings → Pages**. Para um site de projeto, o endereço padrão segue o formato `https://USUARIO.github.io/REPOSITORIO/`. Os caminhos relativos mantêm os links e o CSS dentro do subdiretório do projeto. [Documentação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Testar no VoxNovel

Use a URL publicada da página inicial ou de um capítulo, por exemplo `https://USUARIO.github.io/REPOSITORIO/chapter-1.html`. A compatibilidade com o VoxNovel, incluindo cadastro e navegação automática entre capítulos, depende de teste posterior no aplicativo.
