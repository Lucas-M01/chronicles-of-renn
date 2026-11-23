# Site estático para demonstração do VoxNovel

O site usa HTML e CSS, tem tema escuro e pode ser aberto diretamente no navegador. A página inicial (`index.html`) é o catálogo. Cada história tem uma página com índice de capítulos e informações da obra. Cada capítulo tem uma URL própria e o texto fica em parágrafos dentro de um elemento `article`.

*The Raven That Cast No Shadow* tem uma página própria (`the-raven-that-cast-no-shadow.html`) e dez capítulos em inglês, de `chapter-1.html` a `chapter-10.html`.

*O Último Sobrevivente da Expedição* tem uma página própria (`o-ultimo-sobrevivente-da-expedicao/index.html`) e dez capítulos em português na mesma pasta.

*O Dragão que Pediu para Morrer* tem uma página própria (`o-dragao-que-pediu-para-morrer/index.html`) e vinte capítulos em português brasileiro na mesma pasta.

## Adicionar uma história

1. Crie uma pasta para a nova história, por exemplo `nova-historia/`, com um `index.html` próprio e os arquivos dos capítulos. Use a página e os capítulos do corvo como modelo.
2. Nos arquivos da nova pasta, vincule o tema por `../styles.css`. Use `../index.html` para voltar ao catálogo e caminhos relativos à pasta nos links entre capítulos.
3. Adicione um item na lista `story-catalog` do catálogo raiz com um link para `nova-historia/index.html`.

## Editar o conteúdo

1. Na página da história, edite a sinopse na seção `synopsis`.
2. Para alterar o crédito de autoria, edite a linha `byline` no catálogo, na página da história e nos capítulos conforme necessário.
3. Para revisar o texto original, edite o arquivo HTML do capítulo correspondente. Mantenha um `<p>...</p>` por parágrafo dentro de `<article>`. Ao colar texto, escreva `&amp;` para um `&` literal e `&lt;` para um `<` literal.
4. Use `<hr>` entre cenas e `<em>` ou `<strong>` para os destaques do original. Se mudar os títulos ou a ordem dos capítulos, confira o índice e os links entre as páginas.
5. Mantenha o crédito de direitos autorais e o aviso de autorização do VoxNovel no rodapé. Abra `index.html` no navegador para conferir o índice e a navegação.

## Publicar pelo GitHub Pages

1. Quando quiser publicar, coloque os arquivos na raiz da branch que será usada pelo GitHub Pages e envie essa branch ao repositório no GitHub. Inclua o arquivo vazio `.nojekyll`, que desativa o processamento pelo Jekyll.
2. No repositório no GitHub, abra **Settings → Pages**. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Selecione a branch que contém os arquivos, por exemplo `main`, escolha **/(root)** e clique em **Save**.
4. Após a publicação, abra **Visit site** em **Settings → Pages**. Para um site de projeto, o endereço padrão segue o formato `https://USUARIO.github.io/REPOSITORIO/`. Os caminhos relativos mantêm os links e o CSS dentro do subdiretório do projeto. [Documentação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Testar no VoxNovel

Use a URL publicada de uma história ou de um capítulo, por exemplo `https://USUARIO.github.io/REPOSITORIO/chapter-1.html`. A compatibilidade com o VoxNovel, incluindo cadastro e navegação automática entre capítulos, depende de teste posterior no aplicativo.
