## 📝 Exercícios 

---

### 🔹 Exercício 1 – Agrupando Conteúdo com Divs
**Descrição:** Você recebeu o código de um site simples (veja o arquivo fornecido). Seu desafio é **organizar melhor o conteúdo utilizando a tag `<div>`** para criar uma estrutura mais clara.

A página está divida da seguinte forma:

1. **Cabeçalho** (título principal e navegação).
2. **Conteúdo principal** (seções, artigos e artigos relacionados).
3. **Conteúdo tangencial** (a dica rápida).
4. **Rodapé** (último parágrafo).

Insira **linhas horizontais (`<hr>`)** para separar visualmente cada uma dessas seções.

> 💡 **Dica**: Embora a tag `<div>` não produza efeito visual, ela é essencial para organizar o código e preparar o layout para futuros estilos com CSS.

**`index.html`**
```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
  <meta charset="UTF-8" />
  <title>Blog Simples</title>
</head>

<body>

  <h1>Blog do Estudante</h1>
  <p>Bem-vindo ao blog com dicas e curiosidades sobre programação e tecnologia.</p>

  <a href="#">Início</a> |
  <a href="#">Artigos</a> |
  <a href="#">Contato</a>

  <h2>Último Artigo: Por que aprender HTML?</h2>
  <h3>Vantagens de aprender HTML</h3>
  <p>HTML é a base da construção de sites. Aprender HTML é o primeiro passo para se tornar um desenvolvedor web.</p>
  <ul>
    <li>Fácil de aprender</li>
    <li>Usado em todos os sites</li>
    <li>Essencial para o front-end</li>
  </ul>

  <h2>Artigos Relacionados</h2>
  <h3>Leituras recomendadas para iniciantes</h3>
  <ul>
    <li><a href="#">Como o CSS funciona</a></li>
    <li><a href="#">Primeiros passos com JavaScript</a></li>
    <li><a href="#">O que é a Web?</a></li>
  </ul>

  <p>Blog do Estudante - Todos os direitos reservados © 2025</p>

</body>

</html>
```

---

### 🔹 Exercício 2 – Tags Semânticas
**Descrição:** Agora que você já organizou o conteúdo do site utilizando a tag `<div>`, chegou o momento de dar mais **significado semântico** à sua estrutura HTML.

Sua tarefa é **editar o exercício anterior** (Agrupando Conteúdo com Divs) e substituir as `<div>`s por **tags semânticas do HTML5**, `<header>`, `<main>`, `<footer>`, `<nav>`, `<section>`, `<article>`.

---