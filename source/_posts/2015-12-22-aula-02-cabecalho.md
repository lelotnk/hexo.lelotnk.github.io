title: Aula 02 - Cabeçalho HTML
tags:
  - HTML
  - Curso de HTML Iniciante
categories: 'Curso de HTML5 do Zero!'
date: 2015-12-22 22:27:44
---


![HTML Heading](/images/posts/curso-html/heading.jpg)

No HTML, ao se falar em **cabeçalho** (em português) temos dois significados possíveis.

Podemos nos referir à tag `<head>` ou às tag `<h1>`, `<h2>`, [...] e `<h6>`.

Você entende a diferença entre esses dois tipos de cabeçalhos?

É muito fácil. Vem comigo.

<!-- more -->

Cabeçalhos são importantes pois definem informações suplementares sobre um documento, artigo ou outro conteúdo qualquer.

Num documento HTML não é diferente porém, como disse, temos dois tipos de **heading** que não tem nenhuma correlação entre si, exceto pelo seu significado semântico.

## O elemento **HEAD**

Na tag `<head>` é onde definimos informações **sobre o documento** HMTL.
Nessa tag as informações são definidas através de *metadados*, que são invisíveis ao leitor pelo navegador web.

Metadados significa *dados sobre dados*, um metadado HTML é um dado (informação) sobre o documento HTML. Esses dados são definidos através de **metatags**.

Lembra quando, na aula anterior, aprendemos a definir o *charset* do documento?
Fizemos isso definindo o *metadado charset* através de uma *metatag*.

```
<!DOCTYPE html>
<html>
<head>
    <title>Meu documento HTML</title>
    <meta charset="UTF-8">
</head>
<body>
</body>
</html>
```

Várias outras informações podem ser definidas através da tag `<meta>`.
Mas vamos dar uma olhada antes em outras tags que também definem metadados no elemento `<head>`.

### O elemento **TITLE**

O elemento `<title>` define o título do documento. Esse título não é visível no conteúdo do documento, mas é extremamente importante e obrigatório em todos os documentos HTML.

**Mas se ele não aparece no conteúdo por que devo definí-lo?**

* Ele aparece na aba ou no topo do seu navegador.
* Ele é utilizado como título quando alguém adiciona o documento aos favoritos.
* É utilizado como título nos resultados de páginas de buscadores como o Google ou Bing.

### O elemento **STYLE**

O elemento `<style>` é utilizado para definir informações de estilo (aparência visual) ao documento HTML.
Através dessa tag você defini como o documento deve ser renderizado pelo navegador. Algo como a cor do texto, tamanho ou alinhamento de um parágrafo, margens ou a cor de fundo do documento.

Para isso utilizamos uma linguagem de folhas de estilo chamada _**Cascading Style Sheets**_ (CSS), vamos aprender mais sobre isso em futuros posts mas segue um exemplo.

```
<style>
body {background-color:yellow;}
p {color:blue;}
</style>
```

> Experimente colocar esse elemento acima dentro da tag `<head>` de um documento HTML. Adicione ao menos um parágrafo no conteúdo, ok?

### O elemento **LINK**

O elemento `<link>` define um recurso externo relacionado ao documento HTML.
Olhe na aba do seu navegador quando você acessa algum web site. Provavelmente você verá um ícone ao lado do título da página. Esse ícone é definido através de um elemento `<link>`

Crie um documento HTML, adicione uma imagem chamada *favicon.png* na mesma pasta que seu documento e adicione o seguinte elemento a sua tag `<head>`.
```
<link rel="icon" href="favicon.png">
```

Também é muito comum fazer um relacionamento entre o seu documento HTML e um arquivo externo que contenha somente CSS, separando assim os códigos e organizando o que é estrutura HTML e o que é formatação visual em arquivos diferentes.

```
<link rel="stylesheet" href="estilos.css">
```

### O elemento **META**

Como já vimos mais acima, utilizamos a tag `<meta>` para definir algumas informações adicionais ao documento.
Essas informações são utilizadas pelos navegadores, por motores de busca ou algum outro sistema que leia o conteúdo de seu documento.

```
<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">
```
> **keywords** são palavras chaves muito utilizadas por motores de buscas para entender do que se trata o seu documento.

```
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint, molestiae.">
```
> **description**, como o nome sugere, é uma breve descrição sobre o conteúdo do documento. Também muito utilizada por motores de busca e ao compartilhar links em redes sociais.

```
<meta charset="UTF-8">
```
> Este você já sabe, certo? O **charset** define a codificação de caracteres do documento.

```
<meta name="author" content="Marco Aurélio Tanaka">
```
> **author** define o autor do documento.

```
<meta http-equiv="refresh" content="30">
```
> **refresh** fará o documento ser atualizado automaticamente a cada 30 segundos.

```
<meta http-equiv="refresh" content="15;url=http://www.dominio.com.br/pagina.html">
```
> Escrito dessa maneira, a tag fará o documento ser redirecionado automaticamente para o endereço especificado em **url** após 15 segundos.

### O elemento **SCRIPT**

Este elemento `<script>` é utilizado para definir uma ação ou comportamento ao documento através da linguagem de programação **Javascript**.

Javascript é uma linguagem muito importante e bastante utilizada na web hoje. Vamos falar muito dela aqui no blog em outras séries.

Apenas como exemplo, tente executar esse documento abaixo em seu navegador.
Ele escreverá "Olá Javascript!" num parágrafo de seu documento, que será identificado através de seu atributo **id**. Veja:

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Meu documento HTML</title>

    <script>
    function digaOla()
    {
        document.getElementById('meu-paragrafo').innerHTML = "Olá Javascript!";
    }
    </script>
</head>
<body>
    <h1>Exemplo de Javascript</h1>

    <p id="meu-paragrafo">Eu sou um parágrafo.</p>

    <button onclick="digaOla()">Diga: Olá!</button>
</body>
</html>
```

### O elemento **BASE**

O elemento `<base>` especifica o endereço (URL) utilizado por todos os endereços relativos contidos dentro de um documento.

Então se você possui um link com o endereço `/exemplo.html`, ele será prefixado com o conteúdo da tag `<base>`.

Experimente este exemplo:

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Meu documento HTML</title>
    <base target="_blank" href="http://www.exemplo.com.br/">
</head>
<body>
    <h1>Exemplo da tag BASE</h1>
    <a href="/teste.html">Clique aqui!</a>
</body>
</html>
```
> Portanto, qualquer outro link com endereço absoluto (que comece com "http") não irá obedecer essa regra da tag `<base>`.

### Como verificar?

Bom, já que o conteúdo de `<head>` fica invisível, como posso verificar ser escrevi corretamente?

Para isso é necessário que você leia o código fonte da documento.

Para fazer isso em seu navegador você deve clicar com o botão direito do mouse em algum local vazio da página e selecionar "*Ver código-fonte da página*" ou algo semelhante.

![Código-fonte da página](/images/posts/curso-html/codigo-fonte.png)

## Cabeçalhos de Conteúdo

**Ok, mas e as tags `<h1>` até `<h6>`?**

Bom, talvez você já tenha percebido em nossos exemplos.

Essas tags definem um título/cabeçalho ao **conteúdo** ou uma seção do conteúdo, diferente da tag `<head>` que diz respeito ao documento.

Existem 6 níveis de títulos no HTML, sendo o `<h1>` o mais relevante e o `<h6>` o menos relevante.

Veja as opções
```
<h1>Título Nível H1</h1>
<h2>Título Nível H2</h2>
<h3>Título Nível H3</h3>
<h4>Título Nível H4</h4>
<h5>Título Nível H5</h5>
<h6>Título Nível H6</h6>
```
> <h1 class="no-nav">Título Nível H1</h1>
> <h2 class="no-nav">Título Nível H2</h2>
> <h3 class="no-nav">Título Nível H3</h3>
> <h4 class="no-nav">Título Nível H4</h4>
> <h5 class="no-nav">Título Nível H5</h5>
> <h6 class="no-nav">Título Nível H6</h6>

---

Bom pessoal, é isso que temos para falar sobre cabeçalhos. Bem fácil não?

Nas próximas aulas vamos continuar vendo mais elementos HTML.

Até mais!


---

* https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element
