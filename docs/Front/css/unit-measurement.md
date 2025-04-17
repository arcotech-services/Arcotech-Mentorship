# 📏 CSS: Unidades de Medida

As **unidades de medida** em CSS definem tamanhos de elementos como altura, largura, margens, padding, fontes e muito mais. Elas se dividem em dois grupos principais:

- **Absolutas:** `px`, `cm`, `mm`, `in`...
- **Relativas:** `em`, `rem`, `vw`, `vh`, `%`

---

## 🔹 Unidades Absolutas

### `px` (pixels)

- Medida fixa baseada na resolução da tela.
- Exemplo: `width: 200px;`

Uso comum para tamanhos precisos.

---

## 🔸 Unidades Relativas

### `em`

- Relativa ao tamanho da fonte do elemento **pai**.
- Exemplo: `font-size: 2em; // o dobro da fonte do pai`

### `rem`

- Relativa ao tamanho da fonte do **elemento raiz** (`html`).
- Exemplo: `font-size: 1.5rem;`

### `%`

- Relativa ao tamanho do **elemento pai**.
- Exemplo: `width: 50%; // metade da largura do pai`

### `vw` e `vh`

- `vw` = 1% da largura da janela
- `vh` = 1% da altura da janela

Exemplo:

```css
.container {
  width: 80vw;   /* 80% da largura da tela */
  height: 50vh;  /* 50% da altura da tela */
}
```

---

## 💡 Comparativo Prático

```html
<!-- index.html -->
<div class="box-px">Pixels</div>
<div class="box-rem">Rem</div>
<div class="box-em">Em</div>
<div class="box-pct">Percentual</div>
<div class="box-vw">VW</div>
```

```css
/* styles.css */
body {
  font-size: 16px; /* base para rem e em */
}

.box-px {
  width: 200px;
  height: 100px;
  background-color: lightblue;
}

.box-rem {
  width: 15rem;
  height: 5rem;
  background-color: lightgreen;
}

.box-em {
  font-size: 2em; /* 2 x 16px = 32px */
  width: 10em;
  height: 4em;
  background-color: lightsalmon;
}

.box-pct {
  width: 50%;
  height: 100px;
  background-color: lightpink;
}

.box-vw {
  width: 80vw;
  height: 10vh;
  background-color: lightgoldenrodyellow;
}
```

---

## 🚀 Desafio de Fixação

Crie um layout simples que contenha:

1. Um cabeçalho com altura em `vh`
2. Um container principal com largura em `vw` e altura fixa em `px`
3. Três caixas com tamanhos diferentes utilizando `em`, `rem`, `%`

💡 Lembre-se de usar `body { font-size: 16px; }` como base para medir `em` e `rem`.

