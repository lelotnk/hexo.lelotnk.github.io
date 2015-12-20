title: Introdução ao HTML
date: 2015-12-20 02:29:07
categories: Curso de HTML5 do Zero!
tags:
- HTML
- Curso de HTML Iniciante
---

O que você acha de aprender a programar aplicações Web? Sites? Jogos?

O HTML é a linguagem mais falada na web. Quase tudo que você vê na web é escrito em HMTL. Se você tem interesse em começar no desenvolvimento web do zero, a sua hora chegou! ;)

Vamos começar uma série de aulas sobre o HTML5.

Essa primeira aula é de introdução.
Você vai aprender o que é o HTML, como poderá fazer e testar os exercícios práticos em seu próprio computador.


Então vá pegar uma xícara de café, sente-se confortavelmente e vamos começar!

<!-- more -->

## O que é o HMTL?

HTML é uma **linguagem de marcação** utilizada para descrever documentos web (Páginas Web ou Web Site).

O nome HTML é uma abreviação da expressão inglesa HyperText Markup Language, que significa Linguagem de Marcação de Hipertexto.

**Mas o que é uma linguagem de marcação?**

Bem, Linguagens de Marcação são utilizadas para definir formatos, ou seja, uma maneira padronizada para exibir elementos em um documento.
Diferente das *linguagens de programação*, a de marcação não possui estruturas de controle condicionais ou de repetição e também não são capazes de realizar operações matemáticas.
As linguagens de marcação utilizam marcadores, mais conhecido como **tags**, para trazer um significado a um elemento que ao ser lido por um sistema ou programa capaz de entendê-lo, irá saber exatamente como esse elemento deve ser exibido visualmente.

## TAGs HTML

Bom, já sabemos que um documento HTML é descrito por uma ou diversas **tags**, certo?

Uma TAG é definida por uma **palavra chave** envolvida por **[chevrons](https://pt.wikipedia.org/wiki/Chevron_%28tipografia%29)**, mais conhecidos como sinais matemáticos **menor que** (<) e **maior que** (>).

```
<palavrachave>Conteúdo da TAG</palavrachave>
```

* Uma tag geralmente é escrita em par, como `<p></p>`;
* A primeira tag `<p>` é chamada de *tag de abertura*, e a segunda tag `</p>`é chamada de *tag de fechamento*;
* A *tag de fechamento* é escrita exatamente igual a tag de abertura, porém com uma barra antes de seu nome: `</p>`;
* O HTML não diferencia letras maiúsculas e minúsculas em suas tags. Portanto `<P></P>` funcionará exatamente igual a `<p></p>`. Porém é **recomendado** e amplamente utilizado a escrita minúscula em todas as tags de um documento;

## Estrutura básica de uma página HTML

Abaixo segue um exemplo de como é a estrutura básica de um documento HTML.
Vamos entender passo a passo, ok?

```
<!DOCTYPE html>
<html>
    <head>
        <title>Título da Página</title>
    </head>
<body>

<h1>Meu Primeiro Título</h1>
<p>Este é o meu primeiro parágrafo</p>

</body>
</html>
```

Explico:
* **DOCTYPE** é a declaração que define o tipo/versão do documento HTML. Você verá outras versões diferentes do HTML5 mais abaixo. O importante aqui é saber que essa declaração deve ser a primeira coisa num documento HTML. Assim o seu navegador entenderá como ele deve renderizar as tags html do documento e exibi-las na tela.
* `<html></html>` define o início e o fim de um documento HMTL. Tudo que estiver dentro dessas tags é o documento HTML propriamente dito.
* `<head></head>` provê algumas informações sobre o documento. Essas informações são invisíveis na tela do navegador. Mas são muito importantes.
* `<title></title>` é uma das informações descritas no `<head>`. Essa tag define o título do documento.
* `<body></body>` define o conteúdo visível do documento. É o que você está vendo na tela do navegador.
* `<h1></h1>` é uma tag que define um título/cabeçalho do conteúdo do documento.
* `<p></p>` é uma tag que define um parágrafo. Trocando seis por meia dúzia, o que você escrever dentro dessa tag, o navegador interpretará como um parágrafo de texto.

Com essas poucas tags um navegador saberá que esse documento possui um título *Título da Página*, possui um conteúdo com um cabeçalho e, logo após, um parágrafo.

Existem centenas de outras tags que vamos aprender no decorrer das aulas.

Abaixo é uma outra visualização da estrutura básica de um documento HTML.

<div style="width:99%;border:1px solid grey;padding:3px;margin:0;background-color:#ddd">&lt;html&gt;<div style="width:90%;border:1px solid grey;padding:3px;margin:20px">&lt;head&gt;<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;title&gt;Título da Página&lt;/title&gt;</div>&lt;/head&gt;</div><div style="width:90%;border:1px solid grey;padding:3px;margin:20px;background-color:#fff">&lt;body&gt;<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;h1&gt;Meu Primeiro Título&lt;/h1&gt;</div><div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;p&gt;Este é o meu primeiro parágrafo.&lt;/p&gt;</div><div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;p&gt;Este também é um outro parágrafo&lt;/p&gt;</div>&lt;/body&gt;</div>&lt;/html&gt;</div>

## A declaração DOCTYPE

Como vimos antes, o DOCTYPE define o tipo/versão do documento web.
Isso porque existem outros tipos de documentos diferentes de HTML circulando por aí, e também em relação a versão, existem tags que são aceitas numa versão que não são aceitas em outra. Ou a maneira de escrever também pode mudar de vesão para versão.
Então, para mostrar o conteúdo corretamente o navegador precisa saber de que tipo é o documento e qual a versão ele deve utilizar.

### Tipos mais comuns de DOCTYPE

* **HTML5**:
    `<!DOCTYPE html>`
* **HTML 4.01**:
    `<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">`
* **XHTML 1.0**:
    `<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">`

### Outras versões do HTML

* **HTML**: lançada em 1991
* **HTML 2.0**: lançada em 1995
* **HTML 3.2**: lançada em 1997
* **HTML 4.01**: lançada em 1999
* **XHTML**: lançada em 2000
* **HTML5**: lançada em 2014

Nessas aulas nós vamos trabalhar com a versão mais recente, o **HTML5**.

## Ferramentas necessárias

### Navegador
A primeira coisa que você vai precisar é algo que você já está utilizando para ler isto aqui. Um navegador.

Os mais conhecidos são:

| [Mozila Firefox](http://www.mozilla.com/firefox/) | [Google Chrome](https://www.google.com/chrome/browser/desktop/) | [Apple Safari](http://www.apple.com/br/safari/) | [Opera](http://www.opera.com/browser/) |
|:-:|:-:|:-:|:-:|
| ![Mozilla Firefox](/images/posts/ff.png) | ![Google Chrome](/images/posts/chrome.png) | ![Apple Safari](/images/posts/safari.png) | ![Opera](/images/posts/opera.png) |

É importante que você possua vários, senão todos, navegadores para poder testar seus códigos pois existem algumas pequenas diferenças na rederização dos documentos de navegador para navegador.

O Chrome é o que vou utilizar nessas aulas pois é o que, hoje, possui o melhor suporte a versão 5 do HTML.

### Editor
Outra ferramenta necessária é um editor de texto. Existem muitas opções disponíveis, desde o mais simples até o mais profissional.

É possível escrever HTML com editores nativos do seu sistema operacional, como o **Bloco de Notas** do Windows, o **Gedit** do Ubuntu ou o **TextEdit** do Mac.

Também existem IDE's, do inglês Integrated Development Environment, ou Ambiente de Desenvolvimento Integrado que é como um editor de texto porém com muitas outras ferramentas integradas para facilitar e agilizar o trabalho.

Mas como estamos começando a estudar a linguagem, vamos utilizar um editor de texto que é nem tão simples como o Notepad ou TextEdit, e também nem tão complexo quanto uma IDE que faria algumas coisas automaticamente para você.

Vou utilizar nessas aulas o Sublime Text, porém sugiro essas duas boas opções:

| [Sublime Text](http://www.sublimetext.com/) | [Notepad++](https://notepad-plus-plus.org/) |
|:-:|:-:|
| <a href="http://www.sublimetext.com/"><img src="/images/posts/sublime-text.png" alt="Sublime Text" width="100" /></a> | <a href="https://notepad-plus-plus.org/"><img src="/images/posts/notepad.png" alt="Notepad++" width="100" /></a> |

## Primeiro Teste

Bom, vamos ao nosso primeiro teste para ver se está tudo Ok?

### Abra o seu editor
Como eu disse antes, aqui estou usando o Sublime Text 3.
![Passo 1](/images/posts/curso-html/passo-1.png)

### Escreva algum código HTML

![Passo 2](/images/posts/curso-html/passo-2.png)

### Salve o documento HTML

Eu estou usando o sistema operacional OSX dos computadores Mac.
Mas na verdade não importa se é Windows, Mac ou Linux. O que você deve fazer é criar uma pasta, para deixar tudo organizado, e salvar o seu arquivo com a extensão **.html**.

Vamos aproveitar aqui e fechar um acordo?
1. Sempre utilize letras minúsculas em seus arquivos e pastas.
2. Não utilize acentuação e troque espaços em branco por hífen. Assim "Arquivo Com Acentuação" ficaria "arquivo-com-acentuacao".

Isso não é uma regra rígida, porém é uma atitude altamente recomendada e utilizada pelos profissionais da área, evitando assim outras dores de cabeça quando algum sistema for ler o seu arquivo.
![Passo 3](/images/posts/curso-html/passo-3.png)

### Verifique o documento no navegador

![Passo 4](/images/posts/curso-html/passo-4.png)

Ok. Tudo funcionou como esperado, certo?
Se você encontrou algum problema com os caracteres do seu texto que possuem acentuação, não se preocupe. Isso é um problema de **charset** que vamos resolver em seguida ok?

Por enquanto é só.

Na próxima aula vamos falar sobre o *charset* e começar ver algumas tags básicas do HTML.

Grande abraço, e bons estudos. ;)