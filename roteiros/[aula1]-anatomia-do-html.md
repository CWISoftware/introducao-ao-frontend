# Aula 1 - Anatomia do HTML

## Introdução - O que é HTML?

É uma linguagem de marcação utilizada na construção de páginas na Web. Documentos HTML são interpretados por navegadores
Uma página HTML é composta de vários Tags/Elementos/Components. De forma semântica e ordenada, é possível dispor conteúdos e criar interações com o usuário.
O básico estrutural de uma página HTML tem esta cara:
`<!DOCTYPE html>

<html lang="en">
    <head>
        <title>Anatomia do HTML</title>
    </head>
    <body>
        <p> Aqui podemos adicionar o conteúdo de texto do Parágrafo (sim, <p> = paragraph)</p> <!-- Comentários são feitos dessa forma no HTML -->
    </body>
</html>
`
Envoltou pela Tag <body></body> vai ficar todos os Elementos HTML da nossa página.
Mas descendo um pouco mais o nível temos as Tags:

## Sobre as Tags/Elementos

Uma tag HTML é dividida em três partes: o nome da tag, seu conteúdo e seus atributos.
Como exemplo a tag `<p atributo="valor do atributo"> Aqui vai o conteúdo do Paragrafo </p>`
outro exemplo é a tag `<img />` que só possui atributos e não necessita de conteúdo pois acessa uma midia e pode ter o fechamento reduzido '<img />'.

Aqui fica o link para TODOS os Elementos HTML disponíveis - https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element

## E como tudo isso se encaixa? O que/como o Navegador imterpreta?

A ferramenta mais importante para o desenvolvimento de paginas web é o Navegador
Todos os Navegadores de mercado (chrome, firefox, edge, safari) possuem ferramentas para desevolvedores de forma nativa.
Primeiro vamos abrir nossa página básica.
No Caso, usando o Google Chrome e apertando com o Botão direito + inspecionar elementos é possível ver o código por baixo dos panos. Em algumas páginas, de frameworks de frontend mais modernos pode ficar bem confusa a navegação na hierarquia de elementos. Mas aqui são somente os elementos básicos que já inserimos.
No desenrolar do treinamento vamos falando mais sobre a DevTools dos navegadores

## Encaixando HTML + Tags

Vou criar nossa primeira página HTML.

- Passo-a-passo:

  - A primeira divisão do HTML se faz entre Metatags e Tags de Interface/interação com o usuário.

    - Metatags são marcadores que usamos para informar o navegador sobre o documento, algumas configurações, linkar outros documentos, etc...
    - Tags de Interface literalmente interagem com o usuário e é o que os Navegadores realmente exibem para o usuário.

  - Vou adicionar alguns metatags para configurar o documento.

    - <!DOCTYPE html> - Define o tipo de documento, o idioma, o tipo de codificação, etc...
    - <meta /> - poder receber muitos atributos e precisam ser separados por contexto para que o navegador entenda.
      - <meta charset="utf-8"> - informa o tipo de caracteres que o documento usa.
      - <meta name="viewport" content="width=device-width, initial-scale=1.0"> - informa o tamanho da janela do navegador.
      - <meta http-equiv="X-UA-Compatible" content="ie=edge"> - informa que o navegador deve ser compatível com o IE.
      - <meta name="description" content=""> - informa uma descrição do documento.
      - <meta name="keywords" content=""> - informa palavras chave que o documento possui.
      - <meta name="author" content=""> - informa o autor do documento.
      - <meta name="robots" content="index, follow"> - informa ao navegador que o documento pode ser indexado pelo motor de busca.
      - meta etc...
    - <title> - Define o título do documento.
    - <link> - Define o link para outros documentos. Normalmente usado para incluir CSS ao documento.

  - Vamos para as tags de Interface

    - Dentro de Body adicionamos as tags de interface. Para isso é muito importante planejar a hierarquia e subdivisões que serão necessárias para que o navegador interprete corretamente.
      Lembrando que sempre que criamos interfaces para usuários é necessario pensar tbm em **Acessibilidade**. Não vou entrar a fundo na questão, mas desde o inicio deve ser considerado a acessibilidade
      e o minimo para isso é criação hierarquica do HTML e suas tags.

    - As tags de interface tbm se dividem em grupos e subgrupos.

      - Tags estruturais

        - <div> - divisão de conteúdo
        - <section> - divisão de conteúdo
        - <span> - elemento de texto
        - <h1>, <h2>, <h3>, <h4>, <h5>, <h6> - elementos de titulo
        - <p> - parágrafo
        - <ul> + <li> - listagem
        - <table> - tabelas de dados

      - Tags de formulários

        - <form> - formulário
        - <input> - campo de entrada
        - <button> - botão
        - <select> - caixa de seleção
        - <textarea> - área de texto

      - Tags de multimedia
        - <img /> - Imagem
        - <audio> - áudio
        - <video> - video

  - A composição das tags vai ajudar a formar os components e estruturar a página.

  - Criei um layout no figma e vou usar como referencia para a contrução da página HTML. Vou tentar abordar todas as tags que citei.

    Mas antes de continuar aconselho leia a documentação do HTML que é mantida pela Mozilla - https://developer.mozilla.org/pt-BR/docs/Web/HTML
    Contem toda informação técnica necessário sobre HTML. É um conteúdo bem extenso e muito interessante. Foi o que utilizei como base para este curso.

    - Iniciando - https://developer.mozilla.org/pt-BR/docs/Learn/HTML/Introduction_to_HTML/Getting_started
    - Anatomia do HTML - https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/HTML_basics

  APRESENTAR O LAYOUT

  - vou iniciar a criação da página com o layout do Figma.
    - ./conteudos/index-completo.html

  RESUMÃO

  - Vimos como é a Anatomia do HTML e suas Tags
  - Vimos que as tags se dividem em grupos e subgrupos

    - Metatags para informar o navegador sobre o documento e configurações
    - Tags para interface e interação com o usuário -

      - Tags estruturais

            - <div> - divisão de conteúdo
            - <span> - elemento de texto
            - <h1>, <h2>, <h3>, <h4>, <h5>, <h6> - elementos de titulo
            - <p> - parágrafo
            - <ul> + <li> - listagem
            - <table> - tabelas de dados

        - Tags de formulários

          - <form> - formulário
          - <input> - campo de entrada
          - <button> - botão
          - <select> - caixa de seleção
          - <textarea> - área de texto

        - Tags de multimedia

          - <img /> - Imagem
          - <audio> - áudio
          - <video> - video

  - Olhamos na prática a construção de uma página HTML
  - e agora vamos para a estilização da página com CSS.
