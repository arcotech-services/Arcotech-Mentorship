# 🌐 Estrutura Básica de um Documento HTML

O **HTML (HyperText Markup Language)** é a linguagem padrão para a criação de páginas web. Ele define a estrutura do conteúdo, organizando textos, imagens, links e outros elementos.

---

## 🏗️ Estrutura Básica do HTML (Teoria + Prática)

Para entender a estrutura do HTML, vamos construir um exemplo passo a passo:

### 🔹 Passo 1: Criar um Arquivo HTML

Crie um arquivo chamado `index.html` e adicione o seguinte código básico:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página HTML</title>
</head>
<body>
    <h1>Olá, mundo!</h1>
    <p>Este é um documento HTML básico.</p>
</body>
</html>
```

📌 **Explicação**:

- `<!DOCTYPE html>` → Declara o tipo de documento como HTML5.
- `<html lang="pt-BR">` → Define o idioma da página para português do Brasil.
- `<head>` → Contém informações essenciais do documento (metadados, título, links para CSS, etc.).
- `<body>` → Contém o conteúdo visível da página, como textos, imagens e links.

---

## 🌟 Tags Semânticas e Boas Práticas

As **tags semânticas** são fundamentais para tornar o HTML mais organizado, acessível e otimizado para mecanismos de busca. Elas indicam o significado do conteúdo dentro da página.

### 🔹 Principais Tags Semânticas

| Tag         | Descrição                                                  |
| ----------- | ---------------------------------------------------------- |
| `<header>`  | Representa o cabeçalho de uma seção ou página              |
| `<nav>`     | Define a navegação do site                                 |
| `<main>`    | Contém o conteúdo principal da página                      |
| `<section>` | Define seções dentro do `<main>`                           |
| `<article>` | Indica um conteúdo independente, como um post de blog      |
| `<aside>`   | Representa um conteúdo relacionado, como uma barra lateral |
| `<footer>`  | Define o rodapé de uma página ou seção                     |

### 🔹 Exemplo Prático com Tags Semânticas

```html
<body>
    <header>
        <h1>Bem-vindo ao HTML!</h1>
        <nav>
            <ul>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="sobre">
            <h2>Sobre o HTML</h2>
            <p>O HTML é uma linguagem de marcação usada para estruturar páginas web.</p>
        </section>
        <aside>
            <h3>Dica de Acessibilidade</h3>
            <p>Use sempre textos alternativos em imagens para tornar sua página acessível.</p>
        </aside>
        <section id="contato">
            <h2>Contato</h2>
            <p>Envie um e-mail para contato@exemplo.com</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 - Todos os direitos reservados</p>
    </footer>
</body>
```

📌 **Boas práticas aplicadas**:

- Utilização de **tags semânticas** para melhorar a estrutura do HTML.
- Separação clara entre **conteúdo principal (**`**)**, **navegação (**`**)**, **cabeçalho (**`**)** e **rodapé (**`**)**.
- Inclusão da tag `<aside>` para conteúdos complementares.

---

## 🎯 Desafio de Fixação 🚀

Agora é a sua vez! Coloque em prática os conceitos aprendidos criando um site HTML utilizando **tags semânticas** e garantindo **acessibilidade**.

### 🔹 Requisitos do Projeto

1. **Criar três páginas HTML:**
   - `index.html` (Página Home)
   - `saiba-mais.html` (Página Saiba Mais)
   - `projetos.html` (Página Projetos)
2. **Utilizar tags semânticas**, como `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>` e `<footer>`.
3. **Criar um menu de navegação comum** para todas as páginas.
4. **Cada página deve conter:**
   - Um **cabeçalho (**\`\`**)** com um título adequado.
   - Um **menu de navegação (**\`\`**)** com links entre as páginas.
   - Um **conteúdo principal (**\`\`**)** com ao menos duas seções.
   - Um **rodapé (**\`\`**)** com informações de contato.
5. **Garantir acessibilidade**, incluindo:
   - **Texto alternativo** para imagens (`alt` em `<img>`).
   - **Hierarquia correta** de títulos (`<h1>` → `<h2>` → `<h3>`).
   - **Links descritivos** (`<a>` com textos claros).

### 🔹 Estrutura do Menu de Navegação

O menu deve estar presente em todas as páginas e pode ser criado assim:

```html
<nav>
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="saiba-mais.html">Saiba Mais</a></li>
        <li><a href="projetos.html">Projetos</a></li>
    </ul>
</nav>
```

🔎 **Desafio extra:** Na página "Projetos", adicione um `<article>` para cada projeto e um `<aside>` com links para referências.

---

## 🎯 Conclusão

O uso de **tags semânticas** melhora a organização, acessibilidade e SEO da página. Combinando **teoria** e **prática**, conseguimos construir páginas web estruturadas e fáceis de navegar. 🚀

## Links-uteis de referencia
- [Guide to Writing Semantic HTML](https://cs.fyi/guide/writing-semantic-html);
- [HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp);
- [Why & When to Use Semantic HTML Elements over Divs](https://www.youtube.com/watch?v=bOUhq46fd5g)
