## 📘 Aula 1: Introdução à Web e ao Desenvolvimento

### 🔍 O que é Desenvolvimento Web?

O desenvolvimento web é a área da tecnologia responsável por criar sites, sistemas e aplicações que funcionam através da internet ou de redes locais. Esses sistemas geralmente são compostos por duas partes principais:

#### 🔹 Cliente (Client) x Servidor (Server)

- **Cliente (Client):**  
  O cliente é o computador ou dispositivo do usuário que faz uma requisição (pedido) para acessar uma página ou serviço na internet. Normalmente, esse papel é desempenhado pelo navegador web (Google Chrome, Firefox, Safari, etc.).

  Exemplo:  
  Quando você digita `https://www.google.com` no seu navegador e pressiona Enter, o navegador é o cliente que faz uma solicitação para o servidor do Google.

* **Servidor (Server):**  
  O servidor é uma máquina (computador) que armazena os arquivos e dados de um site ou sistema. Ele recebe as requisições do cliente, processa essas solicitações (se necessário) e envia uma resposta de volta.

  **Exemplo:**  
  O servidor do Google recebe o pedido do seu navegador e devolve a página de busca pronta para ser exibida.

#### 🔹 Front-end x Back-end

- **Front-end:**  
  É a parte do desenvolvimento que lida com o que o usuário vê e interage diretamente no navegador. O front-end é construído com tecnologias como:

  - HTML (estrutura da página)
  - CSS (estilo da página)
  - JavaScript (interatividade da página)

  **Exemplo:**  
  Botões, menus, animações e formulários de um site fazem parte do front-end.

* **Back-end:**  
  É a parte que funciona "por trás dos panos", no servidor. O back-end é responsável por processar dados, acessar bancos de dados, autenticar usuários, etc. As linguagens e tecnologias comuns no back-end incluem:

  - Node.js, Python, Java, PHP, Ruby, etc.
  - Banco de Dados: MySQL, PostgreSQL, MongoDB, etc.

  Exemplo:  
  Quando você faz login em um site, o back-end verifica seu usuário e senha no banco de dados antes de permitir o acesso.

---

📝 **Resumo rápido:**

| Conceito      | O que é?                                                | Exemplo                                  |
|--------------|---------------------------------------------------------|------------------------------------------|
| Cliente      | Dispositivo/navegador que faz uma requisição ao servidor | Seu navegador acessando um site          |
| Servidor     | Computador que armazena e envia os dados da aplicação    | Servidor do Google enviando a página     |
| Front-end    | Parte visível da aplicação que o usuário interage        | Botão, formulário, menu em um site       |
| Back-end     | Parte que processa dados e regras no servidor            | Verificação de login, acesso ao banco de dados |

---

### 🔍 Como funciona a Web: HTTP, URL, Navegador e Servidor

A internet funciona através da troca de informações entre dois pontos principais: **cliente** e **servidor**. Essa troca é realizada usando regras bem definidas chamadas de **protocolo**. O principal protocolo da web é o **HTTP**.

#### 🔹 HTTP – HyperText Transfer Protocol

- O **HTTP (Protocolo de Transferência de Hipertexto)** é o conjunto de regras que define como os dados são enviados e recebidos entre o cliente (navegador) e o servidor.
- Ele permite, por exemplo, que você abra páginas web, envie formulários e acesse APIs.

**Exemplo de requisição:**

- Cliente (Navegador) → faz um pedido HTTP → Servidor (Web)
- Servidor (Web) → envia uma resposta HTTP → Cliente (Navegador)


##### ▻ Principais métodos HTTP:
- **GET** – Requisitar (buscar) informações de um servidor.
- **POST** – Enviar dados para serem processados no servidor.
- **PUT** – Atualizar dados existentes no servidor.
- **DELETE** – Remover dados do servidor.

---

#### 🔹 URL – Uniform Resource Locator

- A **URL** é o endereço de um recurso (como uma página ou imagem) na internet.
* Estrutura de uma URL:
![text](https://cwbm.com.br/wp-content/uploads/2019/07/estrutura-de-urls-1024x427.png)


#### Exemplos de URLs:
- `https://www.google.com`
- `https://meusite.com/contato`
- `http://api.exemplo.com/v1/usuarios`

---

#### 🔹 Navegador (Browser)

- O navegador é o programa que interpreta e exibe os arquivos HTML, CSS e JavaScript vindos do servidor.
* Principais navegadores: **Google Chrome, Mozilla Firefox, Safari, Microsoft Edge**.
- O navegador também faz requisições HTTP e renderiza (exibe) o resultado visual para o usuário.

---

#### 🔹 Servidor

- O servidor é responsável por armazenar os arquivos de um site e responder às requisições dos clientes.
* Tipos de servidores:
  - **Servidor Web:** Apache, Nginx
  - **Servidor de Aplicação:** Node.js, Express, Django

---

📝 **Resumo rápido:**

| Termo     | O que é?                                          | Exemplo                                 |
|-----------|---------------------------------------------------|-----------------------------------------|
| HTTP      | Protocolo de comunicação entre cliente e servidor | Carregar uma página web                 |
| URL       | Endereço de um recurso na web                     | https://www.exemplo.com/pagina          |
| Navegador | Programa que interpreta HTML/CSS/JS               | Google Chrome, Firefox                  |
| Servidor  | Computador que armazena e envia os dados          | Servidor do Google, API de um sistema   |

---

### 🔵 Ferramentas Básicas: Editores, Navegadores e DevTools

Para desenvolver sites e aplicações web, utilizamos algumas ferramentas essenciais que facilitam o trabalho do programador.

---

#### 🔹 Editores de Código

O editor de código é o programa onde você escreve seus arquivos HTML, CSS e JavaScript.

##### ▻ Principais editores:
- **Visual Studio Code (VS Code):**  
  Gratuito, leve e com milhares de extensões para facilitar o desenvolvimento web.
- **Sublime Text:**  
  Leve e rápido, mas algumas funções avançadas são pagas.
- **Atom (descontinuado):**  
  Ainda usado por algumas pessoas, mas o suporte foi encerrado.

##### ▻ Por que usar o VS Code?
- Suporte a várias linguagens (HTML, CSS, JS, etc.).
- Extensões úteis: Live Server, Prettier, ESLint.
- Interface amigável.
- Gratuito.

---

#### 🔹 Navegadores

São os programas que abrem e exibem os sites.

##### ▻ Principais navegadores:
- **Google Chrome (recomendado para desenvolvimento)**
- Mozilla Firefox
- Microsoft Edge
- Safari

Cada navegador possui ferramentas internas que ajudam no desenvolvimento (as DevTools).

---

#### 🔹 DevTools (Ferramentas de Desenvolvedor)

As **DevTools** são um conjunto de ferramentas integradas no navegador que permitem:

- Visualizar o HTML gerado da página.
- Alterar o CSS em tempo real.
- Verificar erros de JavaScript.
- Analisar o desempenho e tempo de carregamento.
- Simular tamanhos de tela (responsividade).

##### ▻ Acessando as DevTools:
- Atalho: `F12` ou `Ctrl + Shift + I` (Windows) | `Cmd + Option + I` (Mac)
- Clique com o botão direito na página → **"Inspecionar"**

---

📝 **Resumo rápido:**

| Ferramenta     | Função                                        | Exemplo                         |
|----------------|---------------------------------------------|---------------------------------|
| Editor de Código | Onde você escreve o código do seu site       | VS Code, Sublime Text           |
| Navegador      | Exibe o resultado visual do seu site         | Google Chrome, Firefox          |
| DevTools       | Permite inspecionar e testar o site no navegador | Inspecionar elementos, console JS |

---

### 🔵 Estrutura de um Site

Um site moderno geralmente é composto por **três tipos de arquivos principais**: **HTML, CSS e JavaScript**. Cada um tem um papel específico no funcionamento da página.

---

#### 🔍 Qual o objetivo de cada linguagem?

##### 🔹 1. HTML (HyperText Markup Language)

**Função:**   Responsável pela **estrutura e conteúdo** da página.   O HTML define os elementos visíveis como textos, títulos, imagens, links, listas, formulários, etc.

**Exemplo de código HTML:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Meu Primeiro Site</title>
</head>
<body>
    <h1>Bem-vindo ao meu site!</h1>
    <p>Este é um parágrafo de texto.</p>
</body>
</html>
```

##### 🔹 2. CSS (Cascading Style Sheets)
**Função:** Responsável pelo **estilo e aparência visual** da página. Com o CSS, você define cores, tamanhos de fonte, espaçamento, bordas, posicionamento de elementos e muito mais.

**Exemplo de código CSS:**
```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: blue;
}
```

##### 🔹 3. JavaScript
**Função:** Responsável pela **interatividade e comportamento** da página. O JavaScript permite criar ações dinâmicas, como responder a cliques de botões, validar formulários, carregar dados de APIs, entre outros.

**Exemplo de código JavaScript:**
```js
function mostrarMensagem() {
  alert('Olá, bem-vindo ao meu site!');
}
```

📝 **Resumo rápido:**

| Linguagem   | Função                          | Exemplo de uso                        |
|------------|---------------------------------|--------------------------------------|
| HTML       | Estrutura e conteúdo da página   | Títulos, parágrafos, imagens, links   |
| CSS        | Estilo e aparência visual        | Cores, fontes, tamanhos, layout       |
| JavaScript | Interatividade e comportamento   | Cliques, validação de dados, animações |

---

### 🔵 GitHub
O GitHub é uma plataforma de **hospedagem de código-fonte** que permite salvar, compartilhar e colaborar em projetos.

**Criar uma conta:**
- Acesse: https://github.com
- Clique em **Sign Up** e preencha os dados.

**Criar um repositório:**
- Após fazer login, clique em **New Repository**
- Dê o nome: C - OxeTech Lab
- Clique em **Create repository**

**Adicionar arquivos manualmente**
- Dentro do repositório, clique em **Add file** > **Upload files**
- Escolha o arquivo `.c` ou pasta do seu computador
- Clique em **Commit changes**

**Estrutura do Repositório:**
```scss
📁 desenvolvimento-web
├── 📁 Aula 01
│   └── (Exercícios da Aula 01)
├── 📁 Aula 02
│   └── (Exercícios da Aula 02)
├── 📁 Aula 03
│   └── (Exercícios da Aula 03)
├── 📁 Aula 04
│   └── (Exercícios da Aula 04)
├── 📁 Aula 05
│   └── (Exercícios da Aula 05)
├── 📁 Aula 06
│   └── (Exercícios da Aula 06)
├── 📁 Aula 07
│   └── (Exercícios da Aula 07)
├── 📁 Aula 08
│   └── (Exercícios da Aula 08)
├── 📁 Aula 09
│   └── (Exercícios da Aula 09)
├── 📁 Aula 10
│   └── (Exercícios da Aula 10)
├── 📁 Aula 11
│   └── (Exercícios da Aula 11)
├── 📁 Aula 12
│   └── (Exercícios da Aula 12)
├── 📁 Aula 13
│   └── (Exercícios da Aula 13)
├── 📁 Aula 14
│   └── (Exercícios da Aula 14)
├── 📁 Aula 15
│   └── (Exercícios da Aula 15)
├── 📁 Aula 16
│   └── (Exercícios da Aula 16)
├── 📁 Aula 17
│   └── (Exercícios da Aula 17)
├── 📁 Aula 18
│   └── (Exercícios da Aula 18)
├── 📁 Aula 19
│   └── (Exercícios da Aula 19)
├── 📁 Aula 20
│   └── (Exercícios da Aula 20)
```

---
