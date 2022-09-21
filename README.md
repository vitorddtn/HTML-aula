# Aula HTML

## Básico

```<!doctype html>
<!-- Este é o comentário -->
<html>
<head>
    <title>Aula HTML</title>
    <meta name="description" content="Nossa primeira página">
    <meta name="keywords" content="aprender html">
</head>
<body>
    <!-- Conteúdo vai aqui -->
</body>
</html>
```

## TAGS

**<!doctype html>** - Esta é uma tag especial que vai no topo do documento e identifica que tipo de código está sendo usado.

**\<html>** - As tags html abrem e fecham o documento HTML. Tudo o que está contido nele faz parte do documento.

**\<head>** - As tags head definem o cabeçalho do documento. Os itens aqui são dados extras que acompanham o documento.

**\<title>** - A title tag define o título do documento. Você notará que ele aparece na parte superior da janela do navegador.

**\<meta>** - As meta tags são usadas para descrever o documento.

**\<body>** - As tags body incluem o conteúdo real que é o documento.

### **TITLE**

A title tag nos permite dar um título ao documento. Isso é usado em vários lugares:

- O navegador irá incluí-lo na parte superior da janela.
- Se você salvar a página como favorita, o título será usado aqui.
- Os mecanismos de pesquisa usam o título quando listam sua página em seus resultados de pesquisa.

Os mecanismos de pesquisa geralmente mostram apenas os primeiros 65 caracteres do título (mais ou menos alguns caracteres). Você deve tentar manter seu título abaixo desse valor.

### **META**

Em seguida, na head, temos as duas metatags para descrição e palavras-chave. Eles são usados ​​por mecanismos de pesquisa (em graus variados) e também podem ser usados ​​por outros sistemas (como quando sua página está vinculada a mídias sociais e outros sites de compartilhamento).

A descrição é usada para fornecer um resumo do assunto da página. Os mecanismos de pesquisa normalmente colocam isso sob seu título em suas páginas de resultados.

Os mecanismos de pesquisa geralmente mostram apenas os primeiros 155 caracteres da descrição (mais ou menos alguns caracteres). Você deve tentar manter sua descrição abaixo desse valor.

A metatag de keywords é usada para fornecer uma série de palavras que correspondem ao assunto da página. Os mecanismos de pesquisa costumavam dar peso a esse aspecto da sua página, mas foi abusado a ponto de ter muito pouco peso hoje em dia. Você ainda deve incluí-lo no entanto para ser completo e também porque estima-se que alguns mecanismos de pesquisa o marcarão por não tê-lo.

Uma meta tag viewport faz com que a página fique bem em todos os tamanhos de tela (laptop, mobile):

### **BODY**

É aqui que o conteúdo real da sua página vai. Todo esse conteúdo estará contido em tags para explicar que tipo de conteúdo é. A seguir, começaremos a ver que tipo de tags podem ser usadas.

### **RESUMO**

**<!doctype html>** - Especifica que este é um documento HTML.

**\<html> \</html>** - Define o documento HTML real.

**\<head> \</head>** - Tag para colocar informações auxiliares que acompanham o documento.

**\<title> \</title>** - Tag para definir o título do documento.

**\<meta>** - Define as informações que descrevem o documento.

**\<body> \</body>** - Tag para armazenar o conteúdo do documento.

## VS Code

No VS Code podemos utilizar um atalho para criar toda a estrutura básica de um arquivo HTML.
Para isso digitamos uma ! e em seguida enter.


## Títulos

\<h1> até \<h6> - Podemos ter até 6 níveis de títulos. Um título de nível 1 \<h1> é o título principal do documento. Então os títulos de nível 2 \<h2> são subtítulos. O nível 3 é um subtítulo e assim por diante.

## Parágrafos

\<p> - Os parágrafos são criados em HTML usando uma tag \<p>. Você provavelmente está começando a ver um padrão aqui. A maioria das tags é uma abreviação da palavra que elas representam. Isso torna mais fácil lembrá-los.

## Formatação

O navegador sempre reformatará o conteúdo para fluir pelo tamanho da tela. Ele irá ignorar espaços em branco extras e novas linhas em nosso código.

\<b> - Se quisermos deixar o texto em negrito , usamos a tag \<b>texto\</b>.

Existe uma outra tag \<strong> que se destina a dar importância ao texto. A maioria dos navegadores renderizará texto strong em negrito, mas é mais seguro usar a tag b.

\<i> - Se quisermos deixar o texto em itálico , usamos a tag \<i>texto\</i>.

Existe uma outra tag \<em> que se destina a dar ênfase ao texto. A maioria dos navegadores renderiza o texto em itálico, mas é mais seguro usar a tag \<i>.

\<u>texto\</u> - Sublinhado.

\<sup>texto\</sup> - Sobrescrito.

\<sub>texto\</sub> - Subscrito.

Às vezes, queremos separar o texto e uma boa maneira de fazer isso é criar uma linha entre eles. Isso pode ser feito com uma régua horizontal que é criada com uma tag \<hr>.

Essa tag não é um contêiner, portanto, não precisa de uma tag de fechamento.

## Aninhamento

Agora podemos introduzir um conceito chamado aninhamento (nesting). Aninhamento é quando um contêiner fica inteiramente dentro de outro contêiner. No exemplo abaixo, a primeira frase está aninhada corretamente. A segunda não.


```
<body>
    <p>His mouth started to speak, <b><u>but his brain</u></b>
	decided it hadn't got anything to say yet and shut it again.</p>
   
    <p>His brain then <b><u>started to contend</b></u> with the
problem of what his eyes told it they were looking at, but in
doing so relinquished control of the mouth which promptly fell
open again.</p>
</body>
```

Se você fizer isso da maneira errada, praticamente todos os navegadores serão capazes de resolver o problema, mas não é considerado um HTML correto e elegante.

A exceção a isso é se os dois contêineres não se sobrepuserem totalmente.

```
<p>Once more gathering up the jaw, <b>his brain <u>lost control</b>
of his left hand</u> which then wandered around in an aimless fashion.</p>
```

## Caracteres Especiais

Às vezes, gostaríamos de incluir caracteres em nosso texto que normalmente fazem parte do código HTML (por exemplo, < e >). Ou gostaríamos de usar caracteres que não estão em nosso teclado (por exemplo, † ou ♣). Nós os incluímos por meio de códigos de caracteres

```
<p>Clubs is the character code for a clubs symbol - &clubs; or &#9827;</p>

<p>Dagger is the character code for a dagger symbol - &dagger; or &#8224;</p>
```

## Links

Os links são uma parte importante da world wide web. Eles nos permitem pular facilmente de uma página para outra e navegar pela montanha absoluta de informações que existe por aí. A vinculação eficaz entre as páginas do seu próprio site e outros sites é uma coisa importante a ser considerada como desenvolvedor de sites.