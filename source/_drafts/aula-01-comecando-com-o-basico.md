title: Aula 01 - Começando com o básico
tags:
  - HTML
  - Curso de HTML Iniciante
categories: 'Curso de HTML5 do Zero!'
date: 2015-12-20 19:46:07
---

No post anterior fizemos uma introdução ao HTML.

Agora vamos ver algumas coisas básicas para o desenvolvimento.

Vamos entender o **charset**, falar sobre aninhamento e identação, e também ver algumas tags básicas.

Vem comigo!

<!-- more -->

## Charset

Charset, ou Character Sets, é o tipo de codificação de caracteres utilizada por um documento HTML. São como tabelas de caracteres possíveis.

Vamos a um exemplo.
Crie um arquivo **.html** e abra em seu navegador com o seguinte conteúdo:
```
Olá Mundo!
```

Provavelmente você verá o seguinte resultado:

![Olá Mundo!](http://placehold.it/500x300?text=Olá Mundo!)

Esse erro aconteceu porque o seu navegador está utilizando a codificação padrão **ANSI (Windows-1252)** para interpretar o seu documento.

O problema é que nessa codificação não existe o caractere **á** (a com acento).

Isso porquê o o padrão ANSI é da língua inglesa que não possui acentos.
Nós utilizamos o idioma **pt-br** (Português Brasil), uma língua latina que possui caracteres acentuados.

Para trabalhar com nosso idioma, nós utilizamos um outro padrão. O **UTF-8**.

**Os charset's mais conhecidos são:**

- **ASCII** que foi o primeiro padrão de codificação de caracteres. Esse padrão define 127 caracteres alfanuméricos diferentes. Números (0-9), letras americanas (A-Z), e alguns caracteres especiais: ! $ + - ( ) @ < >;
- **ANSI** (Windows-1252) é a codificação original do Windows. Ele suporta 256 caracteres diferentes;
- **ISO-8859-1** é o charset padrão do HTML 4. Ele também suporta 256 caracteres diferentes;
- **UTF-8** (Unicode) é o padrão que suporta quase todos os caracteres e simbolos existentes. Tornou-se o padrão do HTML5 por causa das limitações dos padrões ANSI e ISO.

### Especificando o CHARSET

Para dizer ao navegador qual o padrão de codificação utilizado em seu documento, utilize o seguinte elemento:

- **HTML 5** `<meta charset="UTF-8">`
- **HTML 4** `<meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">`

Vamos corrigir então o nosso documento, adicionando a estrutura básica de um documento HTML e também já colocando o nosso **charset**.
Se você não se sente a vontade com essa estrutura básica, volte ao nosso primeiro post de **Introdução ao HTML**.

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Documento</title>
</head>
<body>
    <p>Olá Mundo!</p>
</body>
</html>
```

![Olá Mundo!](http://placehold.it/500x300?text=Olá Mundo!)

## Elementos HTML

Aposto que você já sabe isso, mas só para recapitular.

Um elementro HTML é escrito por uma **tag de abertura**, uma **tag de fechamento** e o conteúdo entre as tags.

```
<tag>Conteúdo da Tag</tag>
```

Um **elemento** HTML é **tudo** desde a tag de abertura e a tag de fechamento.

```
<p>Meu primeiro parágrafo</p>
```

| Tag de Abertura | Conteúdo      | Tag de Fechamento |
|-----------------|---------------|-------------------|
| &lt;h1&gt;      | Meu cabeçalho | &lt;/h1&gt;       |
| &lt;p&gt;       | Meu parágrafo | &lt;/p&gt;        |
| &lt;br /&gt;    |               |                   |

> Lembrando que alguns elementos não possuem tag de fechamento

## Elementos Aninhados

Elementos HTML podem ser aninhados, ou seja, podem conter outros elementos.
Na verdade, todo documento HTML é feito por elementos aninhados.
Este exemplo abaixo contém 4 elementos:

```
<!DOCTYPE html>
<html>
<body>

<h1>Meu Cabeçalho</h1>
<p>Meu primeiro parágrafo.</p>

</body>
</html> 
```

O elemento `<html>` define o documento HTML. Ele possui uma tag de abertura `<html>` e uma tag de fechamento `</html>`.
O conteúdo deste elemento `<html>` é outro elemento html, o `<body>` que por sua vez, possui outros dois elementos `<h1>` e `<p>`.
Neste exemplo os elementos `<h1>` e `<p>` não possuem outros elementos como conteúdo, mas apenas um texto puro: "Meu Cabeçalho" e "Meu primeiro parágrafo." respectivamente.

### Tag de fechamento

A regra é clara:
> A primeira tag a ser aberta deve ser a última a ser fechada

Logo, este exemplo abaixo não deve existir:

```
<html> <body> </html> </body>
```

O correto, é claro, você já sabe:

```
<html> <body> </body> </html>
```

Todos os navegadores mostram corretamente um elemento ainda que você esqueça da tag de fechamento.
Este exemplo abaixo funcionará corretamente:

```
<html>
<body>

<p>Meu primeiro parágrafo.
<p>Meu segundo parágrafo.

</body>
</html> 
```

Porém nunca confie nisto. Com certeza você terá problemas ou algum resultado inesperado se você esquecer a tag de fechamento. **Sempre** feche seu elemento corretamente, a não ser que ele não possua uma tag de fechamento.

### Elementos vazios

Elementos que não possuem conteúdo são chamados de **Elementos vazios**.

`<br>` é um elemento vazio e não possui uma tag de fechamento. Essa tag define uma quebra de linha.

Esses elementos podem ser fechados na própria tag de abertura: `<br />`.
O HTML5 não requer que você feche um elemento vazio, mas caso seu código precise passar por uma validação mais rígida, você deveria fechar todos os elementos.

## Indentação de Tags

Indentar nada mais é que organizar seu código, fazer com que ele fique mais bonito.

Mas não é só estética, eles podem ajudar muito na leitura e manutenção do código, pois fica mais fácil de encontrar determinada informação num código corretamente indentado.

Para fazer a indentação, temos que usar de espaços em branco (ou TAB) em nosso código HTML.

As tags correspondentes (de abertura e fechamento) devem ficar na mesma linha vertical, e as tags internas (aninhadas) devem ficar a frente.

Este código **NÃO** está indentado:

```
<!DOCTYPE html>
<html>
<body>
<h1>Meu Cabeçalho</h1>
<p>Meu primeiro parágrafo.</p>
</body>
</html>
```

Este também **NÃO** está indentado:

```
<!DOCTYPE html><html><body><h1>Meu Cabeçalho</h1><p>Meu primeiro parágrafo.</p></body></html>
```

Este **SIM**, está corretamente indentado:

```
<!DOCTYPE html>
<html>
<body>
    <h1>Meu Cabeçalho</h1>
    <p>Meu primeiro parágrafo.</p>
    <ul>
        <li>Primeiro Item da Lista</li>
        <li>Segundo Item da Lista</li>
        <li>Terceiro Item da Lista</li>
    </ul>
</body>
</html>
```

## Elementos Básicos e Atributos de Tags HTML

Todas as tags HTML podem ter atributos. Os atributos adicionam informações a tag.
Os atributos devem sempre ser escritos na tag de abertura. Nunca na tag de fechamento.

### O Atributo LANG

Para definir o idioma do documento utilize o atributo **lang** na tag `<html>`.

Esse atributo é importante para os leitores de tela (por acessibilidade) os motores de busca (Google, Bing, Yahoo e etc).

```
<!DOCTYPE html>
<html lang="pt-br">
<body>
    <h1>Meu Cabeçalho</h1>
    <p>Meu primeiro parágrafo.</p>
</body>
</html>
```

As duas primeiras letras define o idioma (pt = Português) e, se houver um dialéto utilize duas outras letras (br = Brasil).

### O Atributo TITLE

Vamos adicionar um atributo **title** na tag `<p>`.

```
<p title="Título do meu parágrafro">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi, explicabo.
</p>
```

> <p title="Título do meu parágrafro">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi, explicabo.</p>

Posicione o ponteiro do mouse em cima do parágrafo acima e veja o comportamento desse atributo. Ele mostra o conteúdo do atributo title.

### Elemento de Link e o Atributo HREF

O atributo **href** é utilizado em conjunto com a tag `<a>`. Esta tag define um link e, é neste atributo que a referência do link é definida.

```
<a href="http://www.google.com.br" target="_blank">Link para o Google</a><br>
<a href="http://www.facebook.com" target="_blank">Link para o Facebook</a><br>
<a href="http://www.twitter.com" target="_blank">Link para o Twitter</a>
```

> <a href="http://www.google.com.br" target="_blank">Link para o Google</a>
> <a href="http://www.facebook.com" target="_blank">Link para o Facebook</a>
> <a href="http://www.twitter.com" target="_blank">Link para o Twitter</a>

Perceba que eu também adicionei um atributo **target**. Este atributo possui opções já pré-definidas. As duas mais comuns são:
- **_blank**: o link se abrirá em uma nova janela;
- **_self**: o link será aberto na mesma janela;

Eu também adicionei uma tag `<br>` após os dois primeiros links para fazer uma quebra de linha e facilitar a leitura.

### Elemento de Imagem e seus Atributos

Um elemento de imagem é definido pela tag `<img>`, porém essa tag precisa de outros atributos para funcionar.

- **src** (source ou fonte) é onde você define o caminho da imagem;
- **width** é onde você define uma largura opcional da imagem;
- **height** é onde você define uma altura opcional da imagem;
- **alt** é onde especifica um texto alternativo para ser utilizado quando o elemento não puder ser mostrado. Por exemplo, quando o caminho *src* não existir. Este atributo também é lido por leitores de tela. Então um usuário, por exemplo, cego poderá "ouvir" o conteúdo dessa imagem.

```
<img src="sunrise.jpg" width="640" height="426"> 
```

![Pôr do Sol](/images/posts/curso-html/sunrise.jpg)

> Para funcionar você precisa ter um arquivo de imagem com o mesmo nome definido no atributo **src** na mesma pasta que o seu arquivo html

### Algumas dicas

#### Utilize caracteres minúsculos

Assim como os elementos HTML, os atributos podem ser escritos com letras maiúsculas ou minúsculas. `title` e `Title` funcionam igualmente.

Porém recomendo que utilizem **sempre** caracteres minúsculos.

#### Sempre utilize aspas

O HTML5 não requer que você utilize aspas para delimitar um atributo.
O exemplo abaixo funciona corretamente:

```
<a href=http://www.google.com.br>Google</a>
```

Porém se seu atributo possui espaços em branco no conteúdo, é necessário utilizar aspas. O exemplo abaixo pode não funcionar corretamente

```
<p title=Meu Parágrafo>
```

Portanto minha recomendação é: Sempre utilize aspas em seus atributos.

#### Aspas (") ou Apóstrofe (')?

As aspas são as mais utilizadas para delimitar uma atributo. Porém a apóstrofe também pode ser utilizada.

Quando um atributo contém aspas em seu conteúdo, é necessário delimitar o atributo com apóstrofe

```
<p title='Atributo title "com aspas" também funciona'>
```

O contrário também é verdadeiro;

```
<p title="Atributo title 'com aspas' também funciona">
```

---

Bom, por enquanto é só.

Nessa aula vimos sobre **Charset**, **aninhamento de elementos**, **indentação de tags** e também vimos alguns elementos básicos com alguns de seus atributos mais utilizados.

Nas próximas aulas vamos estudar mais detalhadamente os elementos HTML.

Até a próxima! ;)