title: Parágrafos HTML, Estilos e Formatação
date: 2016-01-08 19:51:26
tags:
  - HTML
  - Curso de HTML Iniciante
categories: 'Curso de HTML5 do Zero!'
---

Um parágrafo é definido através da tag `<p>`. A utilização é extremamente simples. Vamos lá.

```
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro. Id cum sapiente, commodi ad asperiores.</p>
```

> <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro. Id cum sapiente, commodi ad asperiores.</p>

Se tratando de parágrafos, você nunca terá certeza de como ele será renderizado na tela em relação às quebras de linhas.
Isso por que o texto é ajustado na tela de acordo com o tamanho de espaço disponível para ele. Portanto em telas pequenas ele ser encaixará de uma maneira, e em telas grandes de outra.

Vamos continuar que temos mais coisas para ver sobre parágrafos.

<!-- more -->

## Quebra de linha

Se você quiser forçar uma quebra de linha, utilize a tag `<br>`. Essa tag não possui o seu par de fechamento. É um elemento vazio.

Veja:

```
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p>
```

> <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p>

Mas qual a diferença entre quebrar linha com dois parágrafos (`<p>`) ou com um `<br>`?

Bem, além de ser preciso considerar a semântica do texto, os navegadores adicionam por padrão uma margem nas tags `<p>` que não existe nas tags `<br>`. A diferença visual fica assim:

```
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p>
```

> <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<br>Id vel hic voluptas repudiandae dignissimos quod, neque quo possimus mollitia veniam tenetur, atque maxime porro.<br>Id cum sapiente, commodi ad asperiores.</p>

## A Pré-formatação `<pre>`

Os navegadores ignoram a formatação do seu parágrafo quando você utiliza mais de um espaço em branco, ou suas quebras de linha.

Veja esse exemplo utilizando um poema de Mário Quintana.

```
<p>Eu, agora       -         que desfecho!
Já nem penso           mais em ti...
Mas será          que nunca deixo
De lembrar           que te esqueci?</p>
```
Resultado:
> <p>Eu, agora - que desfecho! Já nem penso mais em ti... Mas será que nunca deixo De lembrar que te esqueci?</p>

Agora, utilizando a tag `<pre>` que renderiza o conteúdo considerando a pré-formatação do texto:

```
<pre>
    Eu, agora       -         que desfecho!
    Já nem penso           mais em ti...
    Mas será          que nunca deixo
    De lembrar           que te esqueci?
</pre>
```
Resultado:
> <pre>
    Eu, agora       -         que desfecho!
    Já nem penso           mais em ti...
    Mas será          que nunca deixo
    De lembrar           que te esqueci?
</pre>

Percebeu a diferença? A tag `<pre>` considera todos os espaços e quebras de linha utilizados no conteúdo.

## Formatação de texto

Você pode querer utilizar alguma formatação diferente em seu texto.
Algumas regras de estilo deverão ser colocadas através de CSS, como veremos no próximo item desta aula.

Mas o HTML tem algumas tags próprias que formatam um texto que possua um significado especial.

As opções em HTML são:

### Negrito

O elemento `<b>` define um conteúdo em negrito, porém sem uma ênfase semântica.

```
<p>Lorem ipsum dolor sit amet, <b>consectetur adipisicing elit</b>. Unde, explicabo.</p>
```

> <p>Lorem ipsum dolor sit amet, <b>consectetur adipisicing elit</b>. Unde, explicabo.</p>

Porém, também temos o elemento `<strong>` que define um conteúdo em negrito. Mas este com uma ênfase ou importância semântica maior. Ou seja, se algum leitor de tela, ou um mecanismo de busca ler esse texto, entenderá que este conteúdo destacado tem uma relevância maior e não apenas um destaque meramente visual.

```
<p>Lorem ipsum dolor sit amet, <strong>consectetur adipisicing elit</strong>. Unde, explicabo.</p>
```

> <p>Lorem ipsum dolor sit amet, <strong>consectetur adipisicing elit</strong>. Unde, explicabo.</p>

### Itálico

O elemento `<i>` define um texto em itálico, porém sem uma ênfase semântica.

```
<p>Lorem ipsum dolor sit amet, <i>consectetur adipisicing elit</i>. Unde, explicabo.</p>
```

> <p>Lorem ipsum dolor sit amet, <i>consectetur adipisicing elit</i>. Unde, explicabo.</p>


Já o elemento `<em>`, assim como o `<strong>`, possui uma ênfase semântica e também define um conteúdo com formatação em itálico. O resultado visual é o mesmo, mas a importância semântica é maior.

```
<p>Lorem ipsum dolor sit amet, <em>consectetur adipisicing elit</em>. Unde, explicabo.</p>
```

> <p>Lorem ipsum dolor sit amet, <em>consectetur adipisicing elit</em>. Unde, explicabo.</p>

### O elemento Small

O elemento `<small>` define um conteúdo de texto visualmente menor que o normal. Muito utilizado para breves descrições ou subtítulos.

```
<h1>Meu Título<br><small>com um breve subtítulo</small></h1>
```

> <h1 class="no-nav">Meu Título<br><small>com um breve subtítulo</small></h1>

### Destacando um texto

O elemento `<mark>` define um conteúdo destacado. Veja:

```
<p>Lorem ipsum dolor sit amet, <mark>consectetur adipisicing elit</mark>. Laudantium, quasi.</p>
```

> <p>Lorem ipsum dolor sit amet, <mark>consectetur adipisicing elit</mark>. Laudantium, quasi.</p>

### Conteúdo deletado e inserido

O elemento `<del>` define um conteúdo que foi deletado, enquanto que o elemento `<ins>` define um conteúdo que foi inserido.

```
<p>Lorem ipsum dolor sit amet, <del>consectetur adipisicing elit.</del> <ins>laudantium quasi.</ins></p>
```

> <p>Lorem ipsum dolor sit amet, <del>consectetur adipisicing elit.</del> <ins>laudantium quasi.</ins>ins></p>

### Subscrito e Sobrescrito

O elemento `<sub>` define um conteúdo subscrito e o elemento `<sup>` um conteúdo sobrescrito.

```
<p>log<sub>b</sub> a = x    <=>    b<sup>x</sup> = a</p>
```

> <p>log<sub>b</sub> a = x <=> b<sup>x</sup> = a</p>

## Um pouco de estilos

Como eu disse antes, algumas regras de formatação que são visuais devem ser inseridas através de CSS. Que é uma linguagem de estilos e é mais apropriada para essa tarefa.
Um estilo em texto pode ser adicionado através do atributo `style=""` onde você determina uma regra de CSS.
Veremos muito mais sobre CSS mais tarde, mas o básico sobre textos é o que veremos agora:

### Cor de Background

A propriedade de CSS `background-color` define a cor de fundo de qualquer elemento HTML, e portanto, também pode ser usada em parágrafos.

```
<p style="background-color: #DDFFE9;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>
```

> <p style="background-color: #DDFFE9;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>

"#DDFFE9" é a cor hexadecimal que representa esse verde claro que você vê no parágrafo acima. Veremos mais sobre cores hexadecimais mais tarde.

### Cor de texto

Para definir a cor de um texto, utilize a propriedade `color` de CSS.

```
<p style="color: red;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>
```

> <p style="color: red;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>

### Fonte do texto

Caso você queira alterar a fonte do seu texto, utilize a propriedade `font-family`. Veja:

```
<p style="font-family: cursive;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>
<p style="font-family: Courier;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>
```

> <p style="font-family: cursive;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p><p style="font-family: Courier;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>

### Tamanho do Texto

Utilize a propriedade `font-size` para alterar o tamanho do seu texto.

```
<p style="font-size: 150%;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>
```

> <p style="font-size: 150%;">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, laudantium.</p>

### Alinhamento de Texto

Para alinha um texto, utilize a propriedade `text-align`.

```
<p style="text-align: right">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente porro facilis quasi delectus pariatur dolorum veritatis voluptatibus explicabo illo nemo.</p>
```

> <p style="text-align: right">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente porro facilis quasi delectus pariatur dolorum veritatis voluptatibus explicabo illo nemo.</p>

Teste as opções de valores da propriedade: `left`, `right`, `center` e `justify`.

### Mais regras

Para adicionar mais de uma propriedade CSS ao mesmo elemento, separe as declarações com ponto-e-vírgula.

```
<p style="text-align: center; font-size: 90%; color: blue; font-family: Courier;">Lorem ipsum dolor sit amet, <strong>consectetur adipisicing elit</strong>. Sapiente porro facilis quasi delectus pariatur <em>dolorum veritatis</em> voluptatibus explicabo illo nemo.</p>
```

> <p style="text-align: center; font-size: 90%; color: blue; font-family: Courier;">Lorem ipsum dolor sit amet, <strong>consectetur adipisicing elit</strong>. Sapiente porro facilis quasi delectus pariatur <em>dolorum veritatis</em> voluptatibus explicabo illo nemo.</p>

---

Bom pessoal, por enquanto é só o que temos sobre parágrafos.
Vamos ver muito mais regras de CSS e outras tags de HTML.

Acompanhe os próximos capítulos dessa série.

Qualquer dúvida, sugestão ou crítica, comente abaixo ok?

Abraço!