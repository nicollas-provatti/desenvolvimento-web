## 📘 Aula 2: Estrutura e Tags

### 🔵 Introdução ao HTML (Revisão)

O **HTML (HyperText Markup Language)** é a linguagem de marcação utilizada para estruturar o conteúdo de páginas na web. Ele define o que será exibido no navegador, como textos, imagens, vídeos, links e outros elementos.

---

#### 🔹 Principais Características do HTML:

- **Hipertexto:**  Permite criar links para outras páginas ou recursos.

- **Linguagem de Marcação:**  Utiliza "tags" (etiquetas) para marcar o início e o fim dos elementos da página.

---

##### 🔹 Estrutura de uma Tag HTML:

![](https://www.chiefofdesign.com.br/wp-content/uploads/2018/05/estrutura-de-um-elemento-html.jpg)

---

##### 🔹 Estrutura Mínima de um Documento HTML

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <title>Meu Primeiro Site</title>
  </head>
  <body>
    <h1>Olá, mundo!</h1>
    <p>Bem-vindo ao meu site.</p>
  </body>
</html>
```

**Explicando cada parte:**
| Parte                    | Função                                                             |
|-------------------------|--------------------------------------------------------------------|
| `<!DOCTYPE html>`        | Informa ao navegador que este é um documento HTML5                  |
| `<html>`                | Elemento raiz do documento                                          |
| `<head>`                | Contém informações da página (não visíveis), como título e metadados |
| `<meta charset="UTF-8">` | Define a codificação de caracteres (importante para acentuação)      |
| `<title>`               | Define o título que aparece na aba do navegador                     |
| `<body>`                | Contém o conteúdo visível da página                                  |

---

#### 🔍 Por que o HTML é importante?

- É a base de toda página web;
- Organiza o conteúdo de forma lógica e estruturada;
- Facilita o trabalho de outras tecnologias, como CSS (estilo) e JavaScript (interatividade).

---

📝 **Resumo rápido:**

| Termo       | O que é?                                                  |
|------------|-----------------------------------------------------------|
| HTML       | Linguagem de marcação usada para estruturar páginas web     |
| Tag        | Elemento que define partes do conteúdo (ex: `<p>`, `<h1>`) |
| Atributo   | Informações extras dentro das tags (ex: `lang="pt-br"`)    |
| Estrutura  | Documento deve ter sempre: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>` |

---

### 🔵 Elementos e Estrutura Básica 

Todo documento HTML possui uma estrutura básica obrigatória, que organiza o conteúdo da página de forma clara e compreensível para o navegador.

---

#### 🔹 Principais Elementos da Estrutura:

#### 1. `<html>`

- **Função:**  Elemento raiz do documento.  Todo o conteúdo da página deve estar dentro dessa tag.

##### Exemplo:
```html
<html lang="pt-br">
  <!-- Conteúdo da página aqui -->
</html>
```

---

#### 2. `<head>`
**Função:** Contém metadados (dados sobre a página) que não são exibidos diretamente ao usuário, mas são essenciais para o funcionamento da página e sua interpretação pelos navegadores e mecanismos de busca.

**Itens comuns no `<head>`:**

- `<meta charset="UTF-8">`: Define a codificação de caracteres.
- `<title>`: Define o título da aba do navegador.
- `<link>`: Importa arquivos externos (CSS, ícones).
- `<script>`: Inclui ou referencia arquivos JavaScript.

**Exemplo:**
```html
<head>
  <meta charset="UTF-8">
  <title>Minha Página</title>
</head>
```

---

#### 3. `<body>`
**Função:** Contém todo o conteúdo visível da página, como textos, imagens, links, listas, tabelas, vídeos e outros elementos interativos.

**Exemplo:**
```html
<body>
  <h1>Bem-vindo!</h1>
  <p>Esta é a minha primeira página HTML.</p>
</body>
```

---

**Exemplo Completo de Estrutura HTML Básica:**
```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <title>Página Exemplo</title>
  </head>
  <body>
    <h1>Olá, mundo!</h1>
    <p>Esta é uma página simples feita com HTML.</p>
  </body>
</html>

```

---

📝 **Resumo rápido:**

| Elemento  | Função                                             |
|-----------|---------------------------------------------------|
| `<html>`  | Elemento raiz; envolve todo o código da página     |
| `<head>`  | Contém metadados, título, links e scripts externos |
| `<body>`  | Contém o conteúdo visível da página (textos, imagens, etc.) |

---

#### 🔵 Tags Básicas

O HTML oferece diversas tags para estruturar o conteúdo de uma página. Vamos conhecer as mais utilizadas no dia a dia do desenvolvimento web.

---

#### 1. Títulos (`<h1>` a `<h6>`)

- Usados para definir títulos e subtítulos.
- Existem 6 níveis: `<h1>` (mais importante) até `<h6>` (menos importante).

**Exemplo:**
```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
```

---

#### 2. Parágrafos (`<p>`)
- Usados para escrever blocos de texto.

**Exemplo:**
```html
<p>Este é um parágrafo de texto.</p>
```

---

#### 3. Listas
**(a) Lista Não Ordenada (`<ul>`)**
- Utilizada para listas sem ordem específica (marcadores).

**Exemplo:**
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

**(b) Lista Ordenada (`<ol>`)**
- Utilizada para listas numeradas.

**Exemplo:**
```html
<ol>
    <li>Primeiro item</li>
    <li>Segundo item</li>
</ol>
```

A tag `<li>` é usado para definir os itens na lista.

---

#### 4. Links (`<a>`)
- Utilizados para criar hiperlinks para outras páginas, sites ou arquivos.

**Atributo importante:**
- `href`: Define o destino do link.

**Exemplo:**
```html
<a href="https://www.google.com" target="_blank">Ir para o Google</a>
```

---

#### 5. Imagens (<`img>`)
- Usada para exibir imagens na página.

**Atributos importantes:**
- `src`: Caminho da imagem.
- `alt`: Texto alternativo (acessibilidade).

**Exemplo:**
```html
<img src="imagem.jpg" alt="Descrição da imagem">
```

---

📝 **Resumo rápido:**

| Tag    | Função                                      | Exemplo                                  |
|--------|--------------------------------------------|-----------------------------------------|
| `<h1>` a `<h6>` | Títulos e subtítulos                  | `<h1>Olá</h1>`                          |
| `<p>`   | Parágrafos de texto                         | `<p>Texto aqui</p>`                      |
| `<ul>`, `<ol>`, `<li>` | Listas não ordenadas e ordenadas | `<ul><li>Item</li></ul>`               |
| `<a>`   | Links para outras páginas ou sites          | `<a href="url">Link</a>`                 |
| `<img>` | Inserção de imagens                         | `<img src="imagem.jpg" alt="descrição">` |

---
