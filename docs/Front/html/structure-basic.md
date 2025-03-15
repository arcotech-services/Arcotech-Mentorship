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

### 🔹 Passo 2: Adicionar Estrutura Semântica

Agora, vamos melhorar o código organizando melhor os elementos da página:

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

📌 **Explicação**:

- `<header>` → Define o cabeçalho da página.
- `<nav>` → Cria uma barra de navegação com links.
- `<main>` → Define o conteúdo principal.
- `<section>` → Separa conteúdos por temas.
- `<footer>` → Representa o rodapé da página.

---

## ♿ Acessibilidade no HTML

### 🔹 Melhores Práticas de Acessibilidade

#### ✅ Adicionar Texto Alternativo às Imagens

Se houver imagens, adicione o atributo `alt` para descrever seu conteúdo:

```html
<img src="logo.png" alt="Logotipo da empresa XYZ">
```

#### ✅ Garantir Hierarquia de Títulos

Use `<h1>`, `<h2>`, `<h3>` corretamente para estruturar bem a página.

```html
<h1>Página Principal</h1>
<h2>Seção Importante</h2>
<h3>Subtópico</h3>
```

#### ✅ Criar Links Acessíveis

Evite links genéricos como "clique aqui". Use descrições mais claras:

```html
<a href="produtos.html">Veja nossos produtos</a>
```

---

## 🎯 Desafio de Fixação 🚀

Agora é a sua vez! Coloque em prática os conceitos aprendidos criando um projeto HTML com múltiplas páginas interligadas.

### 🔹 Requisitos do Projeto

1. **Criar três páginas HTML:**
   - `index.html` (Página Home)
   - `saiba-mais.html` (Página Saiba Mais)
   - `projetos.html` (Página Projetos)
2. **Criar um menu de navegação comum** a todas as páginas, permitindo a navegação entre elas.
3. **Cada página deve conter:**
   - Um cabeçalho (`<header>`) com um título adequado.
   - Uma seção principal (`<main>`) com conteúdos relevantes ao tema da página.
   - Um rodapé (`<footer>`) com informações de contato.
4. **Garantir acessibilidade**, incluindo:
   - Texto alternativo para imagens (`alt` em `<img>`).
   - Hierarquia correta de títulos (`<h1>` → `<h2>` → `<h3>`).
   - Links descritivos (`<a>` com textos claros).

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

---

## 🎯 Conclusão

A estrutura HTML é a base de toda página web. Ao combinar **teoria** com **prática** e seguir boas práticas de acessibilidade, garantimos uma experiência melhor para todos os usuários. 🚀
