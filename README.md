# Aula de HTML

## 1. Introdução

HTML (HyperText Markup Language) é a **linguagem de marcação** usada para estruturar o conteúdo de páginas da web.  
Ele funciona em conjunto com:

- **CSS**: para estilização.
- **JavaScript**: para interatividade.

O HTML foi criado no início da década de 90 e evoluiu até o HTML5, que trouxe novos elementos semânticos, suporte a áudio/vídeo e melhorias de acessibilidade.

---

## 2. Estrutura básica de um documento HTML

Todo documento HTML começa com uma estrutura base:

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Minha Página</title>
  </head>
  <body>
    <h1>Olá Mundo!</h1>
  </body>
</html>
```

- `<!DOCTYPE html>`: informa ao navegador que estamos usando HTML5.
- `<html>`: raiz do documento.
- `<head>`: contém metadados, título e links para scripts e CSS.
- `<body>`: contém todo o conteúdo visível.

---

## 3. Tags e elementos

- **Tag**: o código entre `<` e `>` (ex.: `<p>`).
- **Elemento**: o conjunto de tag de abertura + conteúdo + tag de fechamento.
- **Atributo**: informação adicional dentro da tag (ex.: `<a href="#">`).
- **Bloco** vs **Inline**:
  - Bloco: ocupa toda a largura disponível (`<div>`, `<p>`, `<h1>`...).
  - Inline: ocupa apenas o espaço do conteúdo (`<span>`, `<a>`...).

---

## 4. Principais elementos HTML

### Estruturais

```html
<header>Topo da página</header>
<main>Conteúdo principal</main>
<section>Seção de conteúdo</section>
<article>Artigo independente</article>
<footer>Rodapé</footer>
<nav>Menu de navegação</nav>
```

### Texto

```html
<h1>Título</h1>
<p>Parágrafo</p>
<strong>Negrito semântico</strong>
<em>Itálico semântico</em>
<span>Texto em linha</span>
```

### Listas

```html
<ul>
  <li>Item não ordenado</li>
</ul>

<ol>
  <li>Item ordenado</li>
</ol>

<dl>
  <dt>Termo</dt>
  <dd>Descrição</dd>
</dl>
```

### Links e imagens

```html
<a href="https://example.com">Clique aqui</a>
<img src="imagem.jpg" alt="Descrição da imagem" />
```

### Tabelas

```html
<table>
  <caption>
    Tabela de exemplo
  </caption>
  <tr>
    <th>Nome</th>
    <th>Idade</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>25</td>
  </tr>
</table>
```

### Formulários

```html
<form>
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" />
  <button type="submit">Enviar</button>
</form>
```

---

## 5. Atributos HTML

- **Globais**: `id`, `class`, `title`, `style`.
- **Específicos**: variam conforme a tag (`src` em `<img>`, `href` em `<a>`).
- **Boas práticas**: usar nomes descritivos e evitar atributos obsoletos.

---

## 6. HTML Semântico

Usar elementos que descrevem o propósito do conteúdo ajuda SEO e acessibilidade.
Exemplo:

```html
<header>
  <h1>Notícias de Tecnologia</h1>
</header>
<main>
  <article>
    <h2>Nova IA Lançada</h2>
    <p>Detalhes da notícia...</p>
  </article>
</main>
<footer>© 2025 Meu Site</footer>
```

---

## 7. Multimídia

```html
<img src="foto.jpg" alt="Descrição da foto" />

<audio controls>
  <source src="musica.mp3" type="audio/mpeg" />
</audio>

<video controls>
  <source src="video.mp4" type="video/mp4" />
</video>

<iframe src="https://example.com" width="600" height="400"></iframe>
```

---

## 8. Acessibilidade e boas práticas

- Sempre usar `alt` em imagens.
- Respeitar a hierarquia de títulos (`<h1>` → `<h2>` → `<h3>`).
- Associar `<label>` a campos de formulário.

---

## 9. Novidades do HTML5

- Novas tags: `<section>`, `<article>`, `<aside>`, `<figure>`, `<figcaption>`, `<main>`.
- Novos tipos de input: `email`, `date`, `number`, `range`, `color`.

```html
<input type="email" placeholder="Digite seu email" />
<input type="date" />
<input type="color" />
```

---

## 10. Ferramentas e dicas finais

- **Inspecionar elementos**: clique com o botão direito → "Inspecionar" no navegador.
- **Validar HTML**: [W3C Validator](https://validator.w3.org/).
