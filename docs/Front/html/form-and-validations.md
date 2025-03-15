# 📝 Formulários e Validação em HTML

Os **formulários** são elementos essenciais para interatividade em sites, permitindo que os usuários enviem dados. O HTML oferece diversas tags e atributos para criar e validar formulários sem necessidade de JavaScript.

---

## 📌 Estrutura Básica de um Formulário HTML

Um formulário é definido pela tag `<form>`, que pode conter diferentes tipos de campos para entrada de dados.

```html
<form action="/enviar" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" required>
    
    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" required>
    
    <label for="idade">Idade:</label>
    <input type="number" id="idade" name="idade" min="18" max="100" required>
    
    <label for="mensagem">Mensagem:</label>
    <textarea id="mensagem" name="mensagem" rows="4" required></textarea>
    
    <button type="submit">Enviar</button>
</form>
```

### 🔹 Explicação

- `<form action="/enviar" method="post">` → Define o formulário e o local para onde os dados serão enviados.
- `<label>` → Associa uma descrição a um campo de entrada.
- `<input>` → Campo de entrada de dados com diferentes tipos (`text`, `email`, `number`).
- `<textarea>` → Campo para texto longo.
- `required` → Torna o campo obrigatório.
- `min` e `max` → Definem limites numéricos.
- `<button type="submit">` → Botão que envia os dados.

---

## ✅ Validação Nativa no HTML

O HTML permite adicionar regras de validação para evitar entradas inválidas.

### 🔹 Tipos de Validação

| Tipo            | Exemplo de Uso | Descrição |
|----------------|---------------|-------------|
| **Obrigatório** | `required` | O campo não pode ficar vazio |
| **Tamanho mínimo/máximo** | `minlength="3" maxlength="10"` | Define a quantidade de caracteres |
| **Padrão (Regex)** | `pattern="[A-Za-z]+"` | Define um padrão para entrada |
| **Tipo de dado** | `type="email"` | Garante que o usuário digite um e-mail válido |

### 🔹 Exemplo de Formulário com Validação

```html
<form>
    <label for="username">Usuário:</label>
    <input type="text" id="username" name="username" required minlength="3" maxlength="15">
    
    <label for="senha">Senha:</label>
    <input type="password" id="senha" name="senha" required minlength="6">
    
    <label for="telefone">Telefone:</label>
    <input type="tel" id="telefone" name="telefone" pattern="\d{10,11}" title="Digite um número de telefone válido">
    
    <button type="submit">Registrar</button>
</form>
```

---

## 🎯 Desafio de Fixação 🚀

Crie um **formulário de cadastro** para um site de eventos, seguindo as regras abaixo:

### 🔹 Requisitos

1. O formulário deve conter os seguintes campos:
   - Nome completo (Obrigatório, mínimo 5 caracteres)
   - E-mail (Obrigatório, formato de e-mail)
   - Telefone (Opcional, deve aceitar apenas números)
   - Data de nascimento (Obrigatório, deve ser maior de 18 anos)
   - Tipo de ingresso (Escolha entre "Padrão", "VIP" e "Backstage")
   - Comentário (Opcional, máximo 300 caracteres)

2. O formulário deve garantir a **validação dos dados** usando apenas HTML.
3. Deve conter um botão para envio das informações.

---

## 🎯 Conclusão

Os formulários em HTML são poderosos e podem ser validados sem JavaScript. Com os atributos corretos, é possível garantir que os usuários preencham corretamente os campos, melhorando a experiência e a integridade dos dados enviados. 🚀

## 🎯 Saiba-mais
- [Client-side form validation](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Form_validation);


