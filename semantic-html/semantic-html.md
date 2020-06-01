# Semantic HTML

Simple structure example

<b>BAD</b>

```html
<div id="header">
  <div class="menu">{...}</div>
</div>

<div class="content">
  <div class="title"></div>
  <div class="article-content"></div>
</div>

<div id="footer">{...}</div>
```

<b>GOOD</b>

```html
<div id="header" role="banner">
  <div class="menu" role="navigation">{...}</div>
</div>

<div class="content" role="main">
  <div class="title" role=""></div>
  <div class="article-content" role="contentinfo"></div>
</div>

<div id="footer">{...}</div>
```

<b>GREAT</b>

```html
<header>
  <nav>
    <ul>
      <li></li>
      <li></li>
      <li></li>
    </ul>
  </nav>
</header>

<main>
  <section>
    <article>
      <header></header>
    </article>
  </section>

  <aside>
    <section>
      <article></article>
    </section>
  </aside>
</main>

<footer>{...}</footer>
```

<hr>



<hr>




