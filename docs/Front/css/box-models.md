# 📦 CSS: Box Model

O **Box Model** (modelo de caixa) é um dos conceitos mais fundamentais do CSS. Ele define como os elementos HTML são renderizados no navegador: cada elemento é representado como uma **caixa retangular**, composta por quatro camadas:

```
+-----------------------------+
|        margin              |
|  +----------------------+  |
|  |      border          |  |
|  |  +---------------+   |  |
|  |  |   padding     |   |  |
|  |  | +----------+  |   |  |
|  |  | | content  |  |   |  |
|  |  | +----------+  |   |  |
|  |  +---------------+   |  |
|  +----------------------+  |
+-----------------------------+
```

---

## 🔍 Camadas do Box Model

### 1. `content`

É onde o conteúdo do elemento aparece: texto, imagem, etc.

### 2. `padding`

Espaço entre o conteúdo e a borda. Expande a área clicável.

### 3. `border`

A borda ao redor do `padding` e `content`. Pode ter largura, cor e estilo.

### 4. `margin`

Espaço externo entre o elemento e os elementos vizinhos.

---

## 🧪 Exemplo prático

### HTML (`index.html`)

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Box Model</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="caixa">Sou uma caixa</div>
</body>
</html>
```

### CSS (`styles.css`)

```css
.caixa {
  width: 300px;
  padding: 20px;
  border: 5px solid teal;
  margin: 40px;
  background-color: lightyellow;
}
```

➡️ Resultado: uma caixa amarela com espaçamento interno (padding), borda verde e distância de outros elementos (margin).

---

## 🧠 Dica importante: `box-sizing`

Por padrão, a largura total de um elemento é a soma de:

- `width + padding + border`

Mas com:

```css
* {
  box-sizing: border-box;
}
```

A largura total passa a ser **apenas** `width`, e o `padding` + `border` ficam contidos dentro dela.

---

## ✅ Boas práticas

- Sempre usar `box-sizing: border-box` para facilitar layouts.
- Use `padding` para afastar o conteúdo da borda.
- Use `margin` para espaçar elementos entre si.

---

## 🚀 Desafio de Fixação: Cartão de Perfil

### Objetivo

Criar uma estrutura de cartão que utilize todos os conceitos de box model.

### Requisitos

1. Criar um `div` com classe `.cartao` que contenha:
   - Uma imagem de perfil (`img`)
   - Um `h2` com nome fictício
   - Um `p` com descrição

2. Estilizar o cartão com:
   - `padding`, `margin`, `border`
   - Cor de fundo e espaçamento entre elementos
   - `box-sizing: border-box`

### Estrutura sugerida

```html
<div class="cartao">
  <img src="perfil.jpg" alt="Foto de Perfil">
  <h2>Maria Front</h2>
  <p>Desenvolvedora frontend apaixonada por interfaces acessíveis e bem estilizadas.</p>
</div>
```

### CSS sugerido

```css
.cartao {
  width: 300px;
  padding: 20px;
  border: 2px solid #999;
  margin: 30px auto;
  background-color: #f5f5f5;
  text-align: center;
  box-sizing: border-box;
}

.cartao img {
  width: 100px;
  border-radius: 50%;
  margin-bottom: 15px;
}
```

---

Se quiser, posso gerar um gabarito com HTML + CSS completos para esse desafio. Deseja isso?
