# garatujas

# HTML & CSS — Resumão / Cola Rápida

## O que é HTML?

HTML (*HyperText Markup Language*) é a estrutura do site.  
Ele organiza os elementos da página: textos, imagens, botões, links, vídeos etc.

## Estrutura básica

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Meu Site</title>
</head>
<body>

    <h1>Título</h1>
    <p>Parágrafo</p>

</body>
</html>
```

---

# Tags HTML principais

## Títulos

```html
<h1>Maior título</h1>
<h6>Menor título</h6>
```

## Texto

```html
<p>Parágrafo</p>
<strong>Negrito</strong>
<em>Itálico</em>
```

## Links

```html
<a href="https://google.com">Google</a>
```

## Imagens

```html
<img src="imagem.jpg" alt="Descrição">
```

## Listas

### Não ordenada

```html
<ul>
    <li>Item</li>
</ul>
```

### Ordenada

```html
<ol>
    <li>Item</li>
</ol>
```

## Divs e containers

```html
<div></div>
<section></section>
<header></header>
<footer></footer>
```

---

# O que é CSS?

CSS (*Cascading Style Sheets*) é o visual do site.  
Ele muda:

- cores
- tamanhos
- fontes
- espaçamento
- posição
- animações

---

# Como ligar CSS ao HTML

```html
<link rel="stylesheet" href="style.css">
```

---

# Sintaxe CSS

```css
seletor {
    propriedade: valor;
}
```

## Exemplo

```css
h1 {
    color: red;
    font-size: 40px;
}
```

---

# Propriedades CSS mais usadas

## Cores

```css
color: blue;
background-color: black;
```

## Texto

```css
font-size: 20px;
font-family: Arial;
font-weight: bold;
text-align: center;
```

## Espaçamento

```css
margin: 20px;   /* espaço externo */
padding: 20px;  /* espaço interno */
```

## Bordas

```css
border: 2px solid white;
border-radius: 10px;
```

## Tamanho

```css
width: 300px;
height: 200px;
```

---

# Box Model

Todo elemento HTML é uma caixa:

```plain text
Margin -> Border -> Padding -> Conteúdo
```

---

# Display

## Block

Ocupa linha inteira:

```css
display: block;
```

## Inline

Fica na mesma linha:

```css
display: inline;
```

## Flex

```css
display: flex;
```

Muito usado para alinhar elementos.

---

# Flexbox

## Centralizar tudo

```css
display: flex;
justify-content: center;
align-items: center;
```

## Direção

```css
flex-direction: row;
flex-direction: column;
```

---

# Responsividade

## Unidade relativa

```css
width: 100%;
height: 100vh;
```

## Media Query

```css
@media (max-width: 768px) {
    body {
        background: black;
    }
}
```

---

# Classes e IDs

## Classe

Pode repetir:

```html
<div class="card"></div>
```

```css
.card {
    background: gray;
}
```

## ID

Único:

```html
<div id="menu"></div>
```

```css
#menu {
    background: black;
}
```

---

# Position

## Relative

```css
position: relative;
```

## Absolute

```css
position: absolute;
top: 0;
left: 0;
```

## Fixed

Fica parado na tela:

```css
position: fixed;
```

---

# Hover

Muda algo quando passa o mouse:

```css
button:hover {
    background: red;
}
```

---

# Transição

```css
transition: 0.3s;
```

---

# Dicas importantes

## Ordem do CSS

Quanto mais específico, maior prioridade:

```css
#id > .classe > tag
```

## Reset básico

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

---

# Estrutura comum de projeto

```plain text
projeto/
│
├── index.html
├── style.css
└── script.js
```

---

# HTML + CSS exemplo completo

## HTML

```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="card">
        <h1>Olá</h1>
        <p>Meu site</p>
    </div>

</body>
</html>
```

## CSS

```css
body {
    background: #111;
    color: white;
    font-family: Arial;
}

.card {
    width: 300px;
    padding: 20px;
    background: #222;
    border-radius: 10px;
}
```

---

# Atalhos mentais úteis

| HTML | CSS |
|---|---|
| Estrutura | Aparência |
| Esqueleto | Pintura |
| Conteúdo | Estilo |

---

# Coisas que vale estudar depois

- Flexbox
- Grid
- Animações
- Responsividade
- JavaScript
- DOM
- APIs
- Frameworks (React, Vue)

---

# Resumo final

## HTML

Cria os elementos.

## CSS

Deixa bonito.

## Fluxo

```plain text
HTML: estrutura
CSS: estilo
JavaScript: interação
```
