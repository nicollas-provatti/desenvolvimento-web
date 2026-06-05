# 📘 Aula 6 - CSS: Box Model, Unidades de Medida e Position

---

## 🔵 Box Model

O **Box Model** é um conceito fundamental do CSS que define como os elementos HTML são renderizados e ocupam espaço na página.

Cada elemento é considerado como uma "caixa" composta por 4 áreas:
- **Content**: conteúdo real do elemento (texto, imagem, etc.)
- **Padding**: espaço interno, entre o conteúdo e a borda
- **Border**: borda ao redor do padding e conteúdo
- **Margin**: espaço externo, fora da borda	

Veja a representação abaixo:

![](https://media.gcflearnfree.org/content/5ef2084faaf0ac46dc9c10be_06_23_2020/box_model.png)

<br>

**Importante:**
- O valor do tamanho total de um elemento normalmente é calculado assim:

```arduino
Largura Total = width + padding esquerdo + padding direito + border esquerdo + border direito + margin esquerdo + margin direito

```

- Para alterar esse comportamento, usamos:

```css
box-sizing: border-box;
```

Com isso, `padding` e `border` passam a ser incluídos dentro da largura definida (`width`).

---

## 🔵 Propriedades de Largura e Altura

As propriedades `width` e `height` definem a **largura e altura** dos elementos em CSS.


### 1. `width` (largura)

- Define a largura do elemento.

```css
width: 300px;
```

- Pode ser definida em:
  - **Pixels (px)**: valor fixo.
  - **Porcentagem (%)**: valor relativo ao elemento pai.
  - **Viewport (vw/vh)**: relativo ao tamanho da tela (1vw = 1% da largura da tela).

**Exemplos:**
```css
width: 500px;   /* Largura fixa */
width: 80%;     /* 80% da largura do elemento pai */
width: 50vw;    /* 50% da largura da janela (viewport) */
```

---

### 2. height (altura)
- Define a altura do elemento.

```css
height: 200px;
```

- Funciona com as mesmas unidades que width.

**Exemplos:**
```css
height: 300px;  /* Altura fixa */
height: 100vh;  /* 100% da altura da janela (viewport) */
```
---

### 3. max-width e min-width

- Define o tamanho máximo ou mínimo que um elemento pode ter, independentemente de seu conteúdo ou da tela:

```css
max-width: 100%;
min-width: 300px;
```

---

### 4. max-height e min-height

- Controla a altura máxima ou mínima de um elemento:

```css
max-height: 400px;
min-height: 100px;
```

---

## 🔵 Unidades de Medida
As unidades de medida definem o **tamanho dos elementos** na tela — como larguras, fontes, margens, etc. Entender as unidades ajuda a controlar o layout e a garantir que seu site fique bonito em diferentes dispositivos.

### 🔹 Tipos de Unidades

#### 1. Unidades Absolutas
Têm um valor **fixo**, que **não se adapta** ao tamanho da tela.

| Unidade | Significado             | Exemplo           |
|---------|-------------------------|-------------------|
| `px`      | Pixels                  | `font-size: 16px;` |
| `cm`      | Centímetros             | `width: 5cm;`      |
| `mm`      | Milímetros              | `width: 50mm;`     |
| `in`      | Polegadas               | `width: 2in;`      |
| `pt`      | Pontos (1/72 in)        | `font-size: 12pt;` |
| `pc`      | Picas (12 pt)           | `font-size: 1pc;`  |


A mais usada é o `px`. É boa boa para elementos fixos ou pequenos ajustes.

<br>

#### 2. Unidades Relativas
Se adaptam ao **contexto**, sendo melhores para layouts **responsivos**.

| Unidade | Base de cálculo                          | Exemplo             |
|---------|-------------------------------------------|---------------------|
| `%`       | Percentual do elemento pai                | `width: 50%;`       |
| `em`      | Relativo ao tamanho da fonte do elemento pai | `padding: 2em;`     |
| `rem`     | Relativo à fonte raiz (html)              | `font-size: 1.2rem;`|
| `vw`      | 1% da largura da janela (viewport width)  | `width: 50vw;`      |
| `vh`      | 1% da altura da janela (viewport height)  | `height: 80vh;`     |
| `vmin`    | 1% do menor lado da janela                | `font-size: 2vmin;` |
| `vmax`    | 1% do maior lado da janela                | `font-size: 2vmax;` |


As mais usadas são `%`, `em`, `rem`, `vw`, `vh`. São boas para fontes adaptáveis, containers fluidos e responsividade.

---

### 🔵 Position em CSS
A propriedade `position` define como um elemento é posicionado no layout e como interage com as coordenadas `top`, `right`, `bottom` e `left`. Os principais valores da propriedade `position` são:

| Valor        | Descrição                                                                                                  |
|-------------|-----------------------------------------------------------------------------------------------------------|
| ``static``  | **Padrão**. O elemento segue o fluxo normal da página. `top`, `left` não têm efeito.                           |
| ``relative``| Permite mover o elemento **em relação à posição original** sem tirá-lo do fluxo.                               |
| ``absolute``| O elemento é removido do fluxo e posicionado **em relação ao primeiro ancestral** com `position` diferente de `static`. |
| ``fixed``   | Fica **fixo na tela**, mesmo com rolagem. Posicionado em relação à janela do navegador.                        |
| ``sticky``  | Mistura `relative` e `fixed`: fica relativo até atingir um ponto, depois fixa na tela.                     |

<div style="height: 3px; width: 1px;"></div>

#### 🔹 Coordenadas
As propriedades `top`, `right`, `bottom` e `left` definem o deslocamento do elemento em relação ao seu ponto de referência, mas só funcionam quando o elemento tem um `position` **diferente** de `static` (ou seja: `relative`, `absolute`, `fixed` ou `sticky`).

<div style="height: 1px; width: 1px;"></div>

##### 🔍 Como funcionam?
- Elas movem o elemento **a partir do lado indicado**.
- O valor pode ser em `px`, `%`, `em`, `rem`, etc.
- O **ponto de referência** depende do tipo de `position`:

  <div style="height: 10px; width: 1px;"></div>

  - `relative` → Baseado na **posição original** do elemento.

  <div style="height: 10px; width: 1px;"></div>

  * `absolute` → Baseado no **primeiro ancestral** posicionado (ou `body` se não houver).

  <div style="height: 10px; width: 1px;"></div>

  - `fixed` → Baseado na **janela do navegador** (viewport).

  <div style="height: 10px; width: 1px;"></div>

  * `sticky` → Baseado no **container pai e comportamento de scroll**

<div style="height: 1px; width: 1px;"></div>

##### 🔍 O que significa cada uma ?
- `top` → Define a distância do **lado superior** do elemento até o **ponto de referência**.
* `bottom` → Define a distância do **lado inferior** do elemento até o **ponto de referência**.
- `left` → Define a distância do **lado esquerdo**.
* `right` → Define a distância do **lado direito**.

**Exemplo:**
```css
.box {
  position: absolute;
  top: 50px;
  left: 100px;
}
```
O elemento será deslocado **50px do topo e 100px da esquerda** em relação ao seu container posicionado.

<div style="height: 1px; width: 1px;"></div>

##### ▸ Valores negativos
Você pode usar valores negativos para **mover além da borda do container**:

```css
top: -10px; /* Sobe 10px além do topo */
```

<div style="height: 1px; width: 1px;"></div>

#### 🔹 Centralizando um elmento com `position`
Centralizar um elemento com CSS é uma necessidade frequente, mas quando usamos `position`, existem alguns conceitos importantes para entender. A técnica mais conhecida para centralização absoluta funciona da seguinte forma: primeiro, é necessário que o container onde o elemento será centralizado tenha a propriedade `position: relative`. Isso é essencial porque, por padrão, um elemento com `position: absolute` se posiciona em relação **ao primeiro ancestral com** `position` **diferente de** `static`, e queremos que esse ancestral seja nosso container.

Depois de definir o container como relativo, aplicamos `position: absolute` ao elemento que queremos centralizar. Agora, precisamos colocá-lo no centro do container. A forma mais simples de fazer isso é utilizar as coordenadas `top` e `left` com valor `50%`. Quando fazemos isso, o canto superior esquerdo do elemento ficará posicionado exatamente no centro do container. Porém, isso não é uma centralização perfeita, pois a posição é calculada a partir do canto do elemento, e não do seu centro. Ou seja, visualmente ele ficará deslocado.

Para corrigir isso, usamos a transformação `transform: translate(-50%, -50%)`. Essa propriedade move o elemento metade da sua própria largura para a esquerda e metade da sua altura para cima, fazendo com que o centro do elemento coincida exatamente com o centro do container. Essa técnica é muito popular porque funciona independentemente do tamanho do elemento, tornando-a ideal para layouts responsivos, onde as dimensões podem variar.

Em resumo, centralizar com `position` consiste em três passos: definir o container como `position: relative`, posicionar o elemento como `absolute` com `top` e `left` em 50%, e, por fim, usar `transform: translate(-50%, -50%)` para corrigir o deslocamento. Essa combinação garante uma centralização precisa tanto horizontal quanto verticalmente, sem a necessidade de cálculos manuais de largura ou altura.

**Exemplo:**
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centralização com Position</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    background-color: #f4f4f4;
    position: relative; /* Container para centralização */
  }

  .card {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 300px;
    padding: 20px;
    background: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    text-align: center;
    font-family: Arial, sans-serif;
  }
</style>
</head>
<body>
  <div class="card">
    <h2>Centralizado!</h2>
    <p>Este card está no centro da tela usando <strong>position</strong>.</p>
  </div>
</body>
</html>
```

---

### 🔵 O que é `z-index` no CSS?


O `z-index` é uma propriedade do CSS usada para **controlar a ordem de empilhamento (stacking order)** dos elementos em uma página. Quando dois ou mais elementos ocupam a mesma área, o `z-index` determina qual ficará **por cima** e qual ficará **por baixo**.

**Por padrão**, os elementos em HTML são exibidos na ordem em que aparecem no código. O último elemento no DOM tende a ficar por cima, **a não ser que usemos** `z-index` **para mudar isso**.

Para que o `z-index` funcione o elemento precisa ter um contexto de empilhamento, ou seja, possuir um `position` diferente de `static` (`relative`, `absolute`, `fixed` ou `sticky`). Se você aplicar `z-index` em um elemento com `position: static`, ele não terá efeito.

A propriedade `z-index` aceita valores inteiros (positivo, negativo ou zero):

- **Maior número** → fica por cima.
- **Menor número** → fica atrás.
- **Padrão** é auto (igual a zero).

Os valores negativos fazem com que o elemento fica ainda mais atrás.

Quando um elemento com `position` e `z-index` é definido, ele cria um novo **contexto de empilhamento** para seus filhos. Isso significa que elementos dentro dele só se comparam entre si, e não com elementos de fora. Esse é um detalhe que costuma confundir iniciantes.

**Exemplo:**
```css
<style>
  .box {
    position: absolute;
    width: 150px;
    height: 150px;
    color: white;
    font-size: 18px;
    text-align: center;
    line-height: 150px;
  }

  .red {
    background: crimson;
    top: 50px;
    left: 50px;
    z-index: 1;
  }

  .blue {
    background: steelblue;
    top: 100px;
    left: 100px;
    z-index: 2; /* Este ficará por cima */
  }
</style>

<div class="box red">Red</div>
<div class="box blue">Blue</div>
```

---