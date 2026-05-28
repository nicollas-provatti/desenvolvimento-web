## 📘 Aula 3: Semântica

--- 

### 🔵  Elementos Semânticos

Elementos semânticos ajudam a dar significado ao conteúdo da página, facilitando a organização, a acessibilidade e a indexação por buscadores.

---

#### 1. `<header>`

- Representa o cabeçalho da página ou de uma seção.
- Normalmente contém logo, título, menu de navegação ou informações introdutórias.

**Exemplo:**
```html
<header>
  <h1>Meu Site</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#sobre">Sobre</a>
  </nav>
</header>
```

---

#### 2. `<main>`

- Representa o conteúdo principal da página.
- Deve ser único por página (apenas um `<main>)`).
- O conteúdo principal é a parte que difere de uma página para outra.

**Exemplo:**
```html
<main>
  <section>
    <h2>Artigo Principal</h2>
    <p>Conteúdo importante da página.</p>
  </section>
</main>
```

---

#### 3. `<section>`
- Representa uma seção genérica do conteúdo, agrupando conteúdos relacionados.
- Pode ser usada para dividir o conteúdo em blocos temáticos.

**Exemplo:**
```html
<section>
  <h2>Sobre Nós</h2>
  <p>Informações sobre a empresa.</p>
</section>
```

---

#### 4. `<footer>`
- Representa o rodapé da página ou de uma seção.

- Geralmente contém informações de contato, direitos autorais e links adicionais.

**Exemplo:**
```html
<footer>
  <p>© 2025 Meu Site. Todos os direitos reservados.</p>
</footer>
```

---

#### 🔍 Por que usar elementos semânticos?
- Melhoram a acessibilidade para leitores de tela.
- Facilitam o SEO (otimização para buscadores).
- Tornam o código mais organizado e legível para desenvolvedores.

---

📝 **Resumo rápido:**

| Elemento | Função                                      | Exemplo de uso                    |
|----------|---------------------------------------------|----------------------------------|
| `<header>` | Cabeçalho da página ou seção               | Logo, menu, título                |
| `<main>`   | Conteúdo principal da página                | Artigos, informações principais  |
| `<section>`| Seção temática do conteúdo                   | Blocos com assuntos relacionados |
| `<footer>` | Rodapé da página ou seção                    | Contato, direitos autorais       |

---