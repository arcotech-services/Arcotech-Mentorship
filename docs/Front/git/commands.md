# 🌍 Comandos Básicos de Git

O **Git** é um sistema de controle de versão que permite rastrear alterações no código-fonte de um projeto. Abaixo estão alguns dos principais comandos utilizados no dia a dia do desenvolvimento.



## 🛠️ Comandos Básicos

### 📌 `git init`

Inicializa um repositório Git em um diretório.

```sh
git init
```

### 📌 `git add`

Adiciona arquivos ao staging area.

```sh
git add nome_do_arquivo
```

### 📌 `git commit`

Registra as mudanças no repositório local.

```sh
git commit -m "Mensagem descritiva da alteração"
```

### 📌 `git branch`

Lista as branches disponíveis ou cria uma nova branch.

```sh
git branch  # Lista todas as branches
```

```sh
git branch nome-da-branch  # Cria uma nova branch
```

### 📌 `git checkout`

Muda para uma branch específica.

```sh
git checkout nome-da-branch
```

### 📌 `git merge`

Mescla alterações de uma branch para outra.

```sh
git merge nome-da-branch
```

### 📌 `git push`

Envia os commits para o repositório remoto.

```sh
git push origin nome-da-branch
```

### 📌 `git pull`

Atualiza o repositório local com as mudanças do repositório remoto.

```sh
git pull origin nome-da-branch
```



## 📝 Exemplo Prático do Início ao Fim

A seguir, um fluxo básico de uso do Git em um novo projeto:

1. Criar um diretório e inicializar um repositório Git:

   ```sh
   mkdir meu-projeto
   cd meu-projeto
   git init
   ```

2. Criar um novo arquivo e adicioná-lo ao Git:

   ```sh
   echo "# Meu Projeto" > README.md
   git add README.md
   ```

3. Realizar o primeiro commit:

   ```sh
   git commit -m "Adiciona README inicial"
   ```

4. Conectar ao repositório remoto no GitHub:

   ```sh
   git remote add origin https://github.com/seu-usuario/meu-projeto.git
   ```

5. Enviar as alterações para o repositório remoto:

   ```sh
   git push -u origin main
   ```

Agora o repositório está versionado e armazenado remotamente no GitHub!

## 🌍 Aprofundando mais no assunto

- [curso free com certificado](https://www.udemy.com/course/git-e-github-para-iniciantes/?srsltid=AfmBOorHch2xvjeVaxZCi7rRL3pWBok8L9A-bQyL7idBTwvYYJscH5ZF);
- [documentação completa](https://docs.github.com/pt)


## 🔍 Hora da prática

- Com suas palavras, descreva quais e qual a função dos principais comandos git?;
- Crie um repositorio na sua conta git;
   - Adicione um read-me;
   - Adicione a mudança;
   - Commite a mudança;
   - Realize o push da mudança.
- Realize alguma mudança no read-me da questao anterior, por dentro da propria interface do git
- Realize o pull request da mudança anterior dentro do repositorio local da sua maquina

## 🎯 Conclusão

Estes são os comandos essenciais para começar a utilizar o Git de forma eficiente. Com a prática, será possível gerenciar projetos de forma mais organizada e colaborativa. 🚀
