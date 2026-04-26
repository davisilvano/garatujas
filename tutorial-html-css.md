# ia26-webdesign  

Esta disciplina ensina o básico de criação de sites. Você vai aprender principalmente três coisas:  
- **HTML** → marcação (estrutura da página)
- **CSS** → aparência (cores, tamanhos, layout)  
- **JavaScript (básico)** → programação (comportamento/interação)

O objetivo é que você consiga criar páginas web simples e entender como sites funcionam. Mesmo sendo um curso introdutório, ele é muito importante para quem quer seguir na área de desenvolvimento web.

---

## Antes do início  

Antes de começar, é importante ter:  
- Um **editor de código** (vamos usar o Visual Studio Code)  
- Um **navegador atualizado** (vamos usar o Google Chrome)  

Essas ferramentas são gratuitas e muito usadas no mercado.

---

## HTML - Linguagem de Marcação  

O HTML **não é uma linguagem de programação**. Ele serve para **organizar o conteúdo da página**.

Pense assim:  
HTML = estrutura (tipo o esqueleto de um corpo)

Ele usa **tags** (etiquetas) para marcar cada parte do conteúdo.

Exemplos:  
- `<h1>` → título principal  
- `<p>` → parágrafo  
- `<a>` → link  

As tags geralmente têm **abertura e fechamento**:

```html
<p>Este é um parágrafo</p>
```

![Animação de seleção](docs/select.gif)

Na animação, é escrita a frase de exemplo `lorem ipsum dolor sit amet potentia` e, então, **muda a formatação de partes do texto**. Veja a seguir, passo a passo, o equivalente em HTML para cada uma delas.

Passo a passo

1. O usuário seleciona lorem ipsum e coloca em negrito.

- Em HTML, fica assim:

  ``` html
  <strong>lorem ipsum</strong> dolor sit amet potentia 
  ```

  A tag `<strong>` deixa o texto em negrito.
  Tudo que estiver entre `<strong> e </strong>` ficará em negrito.




---

2. O usuário seleciona sit amet e coloca em itálico.

- Em HTML, fica assim:

  ``` html
  <strong>lorem ipsum</strong> dolor <em>sit amet</em> potentia
  ```

  A tag `<em>` deixa o texto em itálico.
  Tudo entre `<em> e </em>` ficará em itálico.




---

3. O usuário seleciona ipsum dolor sit e muda a cor para vermelho.

- Em HTML, fica assim:

  ``` html
  <strong>lorem <span style="color: red;">ipsum dolor sit</span></strong> amet <em>sit amet</em> potentia
  ```

  A tag `<span>` serve para aplicar estilos específicos em partes do texto.
  O `style="color: red;"` muda a cor para vermelho.

> **⚠️ Nota:**
>
> > O HTML serve principalmente para organizar o conteúdo, não só para deixar bonito.



Existem outras tags como:

`<b>` → negrito

`<i>` → itálico


Mas o ideal é usar:

`<strong>` → indica importância

`<em>` → indica ênfase


Isso é melhor para acessibilidade (por exemplo, pessoas com deficiência entendem melhor).

Isso é só o básico do HTML, e existem **muitas** outras tags e atributos que podem ser usados para criar páginas web mais complexas e interativas. Uma boa forma de aprender HTML é começar desenhando uma página em um papel. Pense em cada parte da página (título, texto, imagem, link) e tente imaginar qual tag HTML você usaria para cada uma delas.
Depois disso, você pode começar a transformar esse desenho em código, usando as tags corretas para organizar o conteúdo.
Sempre se pergunte: “qual é a melhor tag para isso?”
> Lembre-se: praticar é essencial. Quanto mais você criar páginas diferentes, mais fácil vai ficar entender HTML e usar suas tags e atributos.
No final deste conteúdo, você vai fazer um exercício prático. Nele, você vai criar uma página web simples usando HTML.
O objetivo é:
- usar as tags corretamente
- organizar bem o conteúdo
- deixar a página clara e acessível

### Estrutura básica de um documento HTML

Outra parte muito importante do HTML é entender como um documento é organizado.

Todo arquivo HTML começa com:

`<!DOCTYPE html>`

Isso serve para avisar ao navegador que o arquivo é HTML5.


---

Depois disso, o documento é dividido em duas partes principais:

`<head>`

O `<head>` é onde ficam informações sobre a página, mas que não aparecem na tela.

Exemplos do que vai aqui:

- título da página

- links para arquivos CSS

- scripts (JavaScript)

- configurações (meta tags)


Mesmo não aparecendo, essa parte é muito importante para o funcionamento da página.

`<body>`

O `<body>` é a parte mais importante visualmente.

Tudo que o usuário vê fica aqui, como:

- textos

- títulos

- imagens

- links

Exemplo completo

``` html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Título da Página</title>
   <!-- Aqui vão configurações, CSS e scripts -->
</head>
<body>
   <!-- Aqui vai tudo que aparece na tela -->
</body>
</html>
```

Resumindo:

`<head>` = configurações (não visível)

`<body>` = conteúdo visível

> **⚠️ Nota:**
>
> Todo o código HTML deve ficar dentro da tag <html>, que é a base de toda a página.
>
> O atributo lang="pt-BR" serve para dizer que o idioma da página é português do Brasil.
> Isso ajuda:
>
> - leitores auditivos de tela (acessibilidade)
>
> - mecanismos de busca (como o Google)
>
> A tag:
>
>`<meta charset="UTF-8">`
>
> serve para garantir que acentos e símbolos apareçam corretamente (como: ã, ç, é).
>
>Já a tag:
>
>`<title>Título da Página</title>`
> 
> define o nome que aparece:
> 
> - na aba do navegador
> 
> - nos resultados de busca

### Atributos HTML

Os atributos são informações extras que colocamos dentro das tags.

Eles sempre ficam na abertura da tag e seguem esse formato:

nome="valor"

Os atributos servem para:

- mudar o comportamento do elemento

- adicionar funções

- personalizar o conteúdo

#### Exemplos

Link:

`<a href="https://www.google.com">Visite o Google</a>`

Aqui:

`<a>` cria um link

`href="link"` define para onde o link vai.

Imagem:

`<img src="imagem.jpg">`

`src="imagem"` diz onde está a imagem.

Os atributos são muito importantes porque deixam sua página mais completa e interativa.

Quando você clica aqui:

[Visite o Google] (https://google.com/)

o navegador usa o `href` para te levar ao site.

### Lista de todas as tags HTML

Nestes links, tem todas as tags HTML, descrições e exemplos: [MDN Web Docs - Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element) ou [W3Schools - HTML Tags](https://www.w3schools.com/TAGS/default.asp).

## CSS - Cascading Style Sheets (Folhas de Estilo em Cascata)

O CSS é uma linguagem usada para mudar a aparência de uma página web. Com ele, você pode definir cores, fontes, espaçamentos, tamanhos e o layout dos elementos.

Uma ideia importante:
HTML = estrutura (o que é cada coisa)
CSS = aparência (como fica)

Isso ajuda a deixar o código mais organizado e fácil de mexer depois.

O CSS funciona com:

Seletores → escolhem quais elementos serão estilizados

Declarações → definem como esses elementos vão ficar


Veja o exemplo:

Código HTML:

``` html
<!DOCTYPE html>  
<html lang="pt-BR">  
<head>  
   <meta charset="UTF-8">  
   <title>Exemplo de CSS</title>  
   <link rel="stylesheet" href="styles.css">  
</head>  
<body>  
   <h1>Olá, Mundo!</h1>  
   <p>Este é um exemplo de CSS.</p>  
</body>  
</html>
```

Código CSS:
```css
/* styles.css */  
body {  
  background-color: #f0f0f0;  
  font-family: Arial, sans-serif;  
}  

h1 {  
  color: #333333;  
  text-align: center;  
}  

p {  
  color: #666666;  
  font-size: 18px;  
  margin: 20px;  
}
```

Aqui, o CSS:

- muda a cor de fundo

- centraliza o título

- muda tamanho e cor do texto


> ⚠️ Nota:
> CSS está funcionando porque o arquivo foi conectado no HTML com <link>.
>Sem isso, o estilo não seria aplicado.
>
>Sem CSS, a página fica com o estilo padrão do navegador (chamado de user agent stylesheet), que geralmente é simples e sem graça.

#### Sintaxe do CSS

O CSS segue um padrão simples:

seletor {  
  propriedade: valor;  
}

Exemplo:

`p {
  color: blue;
}
`

Isso significa: “todos os parágrafos serão azuis”.

> ⚠️ Nota:
>
>Cada linha termina com ;
>
>Tudo fica dentro de { }
>
>As propriedades dizem o que mudar (cor, tamanho, etc.)

#### Seletores CSS

Os seletores dizem quais elementos do HTML vão receber estilo.

Exemplo de HTML:

```html
<h1 class="titulo">Título Principal</h1>  
<p id="paragrafo1">Este é o primeiro parágrafo.</p>  
<p id="paragrafo2">Este é o segundo parágrafo.</p>  
<a href="#" class="link">Este é um link</a>
```

Agora veja os principais seletores:

1. Seletor de tipo



`h1 { color: blue; }`

Aplica a todos os `<h1>`

2. Seletor de classe



`.titulo { font-size: 24px; }`

Aplica a tudo que tem class="titulo"

3. Seletor de ID



`#paragrafo1 { color: red; }`

Aplica só naquele elemento específico

4. Seletor de atributo



`a[href="#"] { text-decoration: none; }`

Aplica a links com `href="#"`

5. Pseudo-classes



`p:first-child { font-weight: bold; }`

Aplica ao primeiro parágrafo dentro de um elemento

#### Hierarquia (muito importante)

O CSS segue a estrutura do HTML (tipo uma árvore).

Exemplo:

```html
<main>  
  <section>  
   <p>Este é um parágrafo dentro de uma seção...</p>  
  </section>  
</main>
```
CSS:

`main section p { color: green; }`

Isso significa:
“Todo `<p>` dentro de `<section>` dentro de `<main>` fica verde”.

Se tiver outro `<p>` fora da `<section>`, ele não será afetado.

> ⚠️ Nota:
> O espaço entre os seletores significa “dentro de”.


Se, no HTML que usamos de exemplo, tivéssemos um parágrafo fora das tags `<section>` e `</section>`, como:

```html
<main>
  <section>
   <p>Este é um parágrafo dentro de uma seção...</p>
  </section>
  <p>Este é um parágrafo fora da seção...</p>
</main>
```

O seletor `main section p` aplicaria a cor verde apenas ao parágrafo dentro das tags `<section>` e `</section>`, enquanto o parágrafo fora delas não. Ou seja, os seletores CSS permitem que você aplique estilos com base na hierarquia dos elementos HTML, Assim, só os elementos desejados são estilizados de acordo com as regras definidas.

Resultando em algo como:

![Seletores CSS](docs/image-css-selectors.png)

### Tipos de Seletores CSS

Existem vários tipos de seletores CSS que permitem selecionar elementos HTML de diferentes maneiras. Abaixo está uma tabela com alguns dos tipos de seletores mais comuns. Esta tabela tem o intuito de servir como um guia rápido para entender os diferentes tipos de seletores CSS e como eles funcionam. No entanto, existem muitos outros tipos de seletores CSS; abordaremos esses outros tipos em conteúdos futuros. Por enquanto, foque em entender os tipos de seletores mais comuns listados abaixo, pois eles são os mais utilizados e fundamentais para o aprendizado do CSS.

| Tipo de Seletor               | Exemplo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Descrição |
|------------------------------ | -------------------------------- | --------- |
| Seletor de Tipo               | `nome_elemento { }`              | Seleciona todos os elementos de um determinado tipo. Exemplo: `p { color: blue; }` seleciona todos os parágrafos e aplica a cor azul. |
| Seletor de Classe             | `.nome_classe { }`               | Seleciona elementos com uma classe específica. Exemplo: `.titulo { font-size: 24px; }` seleciona todos os elementos com a classe "titulo" e aplica um tamanho de fonte de 24 pixels. |
| Seletor de ID                 | `#nome_id { }`                   | Seleciona um elemento com um ID específico. Exemplo: `#paragrafo1 { color: red; }` seleciona o elemento com o ID "paragrafo1" e aplica a cor vermelha. |
| Seletor de Atributo           | `elemento[atributo="valor"] { }` | Seleciona elementos com um atributo específico ou um valor de atributo específico. Exemplo: `a[href="#"] { text-decoration: none; }` seleciona todos os links que têm um atributo `href` com o valor "#" e remove o sublinhado. |
| Pseudo-classes                | `elemento:pseudo-classe { }`     | Seleciona elementos com base em seu estado ou posição na hierarquia do documento. Exemplo: `p:first-child { font-weight: bold; }` seleciona o primeiro parágrafo dentro de seu elemento pai e aplica negrito. |

Seletores de descendentes, filhos e irmãos:

| Tipo de Seletor               | Exemplo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Descrição |
|------------------------------ | -------------------------------- | --------- |
| Seletor de Descendente        | `elemento1 elemento2 { }`        | Seleciona elementos que são descendentes de um elemento específico. Exemplo: `main section p { color: green; }` seleciona todos os parágrafos que estão dentro de uma seção, que por sua vez está dentro do elemento principal `<main>`, e aplica a cor verde. |
| Seletor de Filho              | `elemento1 > elemento2 { }`      | Seleciona elementos que são filhos diretos de um elemento específico. Exemplo: `main > section { background-color: lightgray; }` seleciona todas as seções que são filhos diretos do elemento principal `<main>` e aplica um fundo cinza claro. |
| Seletor de Irmão Adjacente    | `elemento1 + elemento2 { }`      | Seleciona um elemento que é imediatamente precedido por outro elemento específico. Exemplo: `h1 + p { margin-top: 0; }` seleciona o parágrafo que vem imediatamente após um título `<h1>` e remove a margem superior. |
| Seletor de Irmão Generalizado | `elemento1 ~ elemento2 { }`      | Seleciona elementos que são irmãos de um elemento específico, independentemente de sua posição. Exemplo: `h1 ~ p { color: gray; }` seleciona todos os parágrafos que são irmãos de um título `<h1>` e aplica a cor cinza. |