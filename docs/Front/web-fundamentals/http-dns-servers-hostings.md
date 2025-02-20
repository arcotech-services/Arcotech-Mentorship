# ✨ Como a Web Funciona?

A web é um vasto sistema interconectado onde navegadores, servidores e protocolos trabalham juntos para entregar conteúdo aos usuários. Este documento explora em profundidade os principais conceitos envolvidos. Além disso, recomendo fortemente o <b>[video](https://www.youtube.com/watch?v=7_LPdttKXPc&ab_channel=Aaron)</b> .



## 🔍 1. Fluxo de Requisições na Web

Quando você acessa um site digitando uma URL no navegador, vários processos acontecem em frações de segundos:

1. **Conversão do Domínio para IP (DNS Lookup)** → O navegador consulta um servidor DNS para descobrir o endereço IP do site.
2. **Envio da Requisição HTTP** → O navegador faz uma requisição HTTP para o servidor.
3. **Processamento pelo Servidor** → O servidor interpreta a requisição e retorna a resposta.
4. **Renderização da Página** → O navegador recebe os arquivos e exibe a página para o usuário.

## 🌐 2. O que é DNS?

O **DNS (Domain Name System)** é como a "agenda de contatos" da internet. Ele traduz nomes de domínio (ex: `www.google.com`) em endereços IP (ex: `142.250.217.78`).

### 👁️ Etapas de uma consulta DNS

1. **Navegador verifica o cache local** → Se o IP já foi resolvido antes, ele não precisa consultar o DNS.
2. **Consulta ao servidor DNS recursivo** → Se o cache não tiver a informação, o navegador consulta um servidor DNS recursivo.
3. **Busca no DNS raiz** → Caso necessário, o servidor recursivo pergunta ao servidor raiz onde encontrar o domínio.
4. **Resposta final** → O servidor retorna o endereço IP ao navegador.

### 🔄 Servidores DNS populares

- **Google DNS** 
- **Cloudflare DNS** 
- **OpenDNS** 

Caso após a leitura acima sobre DNS, ainda tenha duvidas recomendo:

- [What Is a Domain Name | Domain Names Explained](https://www.youtube.com/watch?v=lMHzpBwPuG8&ab_channel=HostingerAcademy)

## 🔗 3. HTTP e HTTPS

O **HTTP (Hypertext Transfer Protocol)** é o protocolo usado para transferir dados entre o navegador e o servidor.

### 🛡️ Diferença entre HTTP e HTTPS

- **HTTP** → Envia os dados sem criptografia.
- **HTTPS** → Usa criptografia SSL/TLS, protegendo os dados transmitidos.

### 🌍 Principais Métodos HTTP

| Método | Descrição |
|---------|------------|
| `GET` | Busca informações no servidor |
| `POST` | Envia dados para o servidor |
| `PUT` | Atualiza um recurso no servidor |
| `DELETE` | Remove um recurso |

Exemplo de uma requisição `GET` com o comando `curl`:

```bash
curl -X GET "https://api.exemplo.com/usuarios"
```
Além disso, recomendo para um maior aprofudamento os links

- [Everything you need to know about HTTP](https://cs.fyi/guide/http-in-depth)
- [why-do-we-need-https](https://howhttps.works/why-do-we-need-https/)
- [http-status-code](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status)

## 🛠️ 4. Servidores Web e Como Funcionam

Os **servidores web** são responsáveis por armazenar e entregar os arquivos do site quando requisitados pelos navegadores.

### 📂 Tipos de Servidores

- **Apache** → Popular em hospedagens tradicionais.
- **NGINX** → Alta performance e escalabilidade.
- **Node.js** → Para aplicações em tempo real.
- **LiteSpeed** → Otimizado para velocidade.

### 💻 O que é um servidor estático e dinâmico?

- **Servidor Estático** → Apenas entrega arquivos (ex: HTML, CSS, JS). Exemplo: GitHub Pages.
- **Servidor Dinâmico** → Processa dados antes de enviar ao cliente. Exemplo: Aplicativos com Node.js ou PHP.



## 💡 5. Hospedagem e Deploy

Para tornar um site acessível, ele precisa ser **hospedado** em um servidor.

### 🏢 Tipos de Hospedagem

- **Hospedagem Compartilhada** → Sites pequenos, barato.
- **VPS (Servidor Virtual Privado)** → Mais controle e recursos.
- **Cloud Hosting** → Escalabilidade (AWS, Google Cloud, Azure).
- **Serverless** → O servidor é gerenciado automaticamente pelo provedor (Vercel, Firebase Hosting).

### 🛠️ Onde hospedar um site gratuitamente?

- **GitHub Pages** → Para sites estáticos.
- **Netlify / Vercel** → Para aplicações frontend modernas.
- **Firebase Hosting** → Integração fácil com backend serverless.


## 🔍 Hora da prática
- Com suas palavras, descreva tudo que acabou de entender definindo e dizendo para
que ser HTTP, HTTPS, DNS, Fluxo de Requisições na Web?;
- Onde uma aplicação frontend se encaixa dentro do Fluxo de Requisições na Web?;
- Qual a principal diferença entre HTTP e HTTPS?;
- Quais os principais métodos HTTP e para que serve cada um deles?;
- Quais os principais grupos de codigos de resposta HTTP?

## 🎯 Conclusão

Compreender como a web funciona é essencial para qualquer desenvolvedor frontend. Saber como o navegador se comunica com servidores, como funcionam os protocolos de rede e os tipos de hospedagem ajuda na criação de aplicações mais rápidas, seguras e escaláveis.
