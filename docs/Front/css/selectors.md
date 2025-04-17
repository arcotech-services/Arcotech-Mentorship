# 🎨 CSS: Seletores, Especificidade e Herança

O CSS (Cascading Style Sheets) permite aplicar estilos aos elementos HTML. Compreender **seletores**, **especificidade** e **herança** é essencial para criar estilos eficientes e organizados.

---

## 🏏r Seletores CSS

Os **seletores** são usados para apontar para os elementos HTML que queremos estilizar.

### 🔹 Exemplos de Seletores

#### 1. Seletor de Tag

```css
/* styles.css */
p {
  color: blue;
}
```

```html
<!-- index.html -->
<p>Este parágrafo ficará azul.</p>
```

#### 2. Seletor de Classe

```css
/* styles.css */
.alerta {
  background-color: yellow;
}
```

```html
<!-- index.html -->
<p class="alerta">Mensagem de alerta!</p>
```

#### 3. Seletor de ID

```css
/* styles.css */
#destaque {
  font-weight: bold;
}
```

```html
<!-- index.html -->
<p id="destaque">Texto em destaque.</p>
```

#### 4. Seletor Descendente

```css
/* styles.css */
article p {
  font-size: 18px;
}
```

```html
<!-- index.html -->
<article>
  <p>Esse parágrafo está dentro de um article.</p>
</article>
```

#### 5. Seletor de Atributo

```css
/* styles.css */
input[type="text"] {
  border: 2px solid green;
}
```

```html
<!-- index.html -->
<input type="text" placeholder="Digite algo">
```

---

## 🮮 Especificidade

A **especificidade** define qual estilo tem prioridade quando múltiplos seletores afetam o mesmo elemento.

### 📊 Hierarquia de Especificidade (do menos para o mais específico)

1. Seletores universais (`*`), de tag (`div`, `p`, etc.)
2. Seletores de classe (`.classe`), atributos (`[type="text"]`) e pseudoclasses (`:hover`)
3. Seletores de ID (`#id`)
4. Estilos inline (`style="..."`)

### 🔍 Exemplo Prático

```css
/* styles.css */
p {
  color: black;
}
.avisar {
  color: red;
}
#principal {
  color: blue;
}
```

```html
<!-- index.html -->
<p id="principal" class="avisar">Qual cor será aplicada?</p>
```

➡️ A cor azul será aplicada, pois o seletor `#principal` tem maior especificidade.

---

## 🌱 Herança

Algumas propriedades CSS são **herdadas** pelos elementos filhos automaticamente, como `color` e `font-family`.

### 🔹 Exemplo

```css
/* styles.css */
body {
  font-family: Arial;
  color: darkgray;
}
```

```html
<!-- index.html -->
<body>
  <section>
    <p>Este texto herdará a fonte e a cor do body.</p>
  </section>
</body>
```

➡️ O parágrafo usará `Arial` e `darkgray` mesmo sem ter essas propriedades definidas diretamente.

---

## 💡 Boas Práticas

- Use classes para reutilizar estilos.
- Evite IDs em CSS para estilização, prefira classes.
- Agrupe seletores quando possível:

```css
/* styles.css */
h1, h2, h3 {
  font-weight: bold;
}
```

---

## 🚀 Desafio de Fixação

Crie um pequeno projeto HTML + CSS com os seguintes requisitos:

### 🧱 Estrutura HTML (arquivo `index.html`)

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Desafio CSS</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1 class="titulo-principal">Bem-vindo ao Estilo CSS</h1>
  </header>
  <main>
    <section class="conteudo">
      <p id="introducao">Este parágrafo apresenta a introdução.</p>
      <p class="destaque">Este texto deve estar em destaque.</p>
    </section>
    <aside>
      <p>Texto lateral com menos destaque.</p>
    </aside>
  </main>
  <footer>
    <p>&copy; 2025 Mentoria Frontend</p>
  </footer>
</body>
</html>
```



