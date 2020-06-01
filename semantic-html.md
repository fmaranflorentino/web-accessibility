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

Simple menu example

<b>BAD</b>

```html
<div class="menu">
  <div class="menu-content">
    <div class="menu-item">Home</div>
    <div class="menu-item">About</div>
  </div>
</div>
```

<b>GOOD</b>

```html
<div aria-label="Acessible menubar">
  <div class="menubar" role="menuBar" aria-label="Acessible menubar">
    <div class="menu-item" role="menuitem" aria-label="Home">Home</div>
    <div class="menu-item" role="menuitem" aria-label="About">About</div>
    <div class="menu-item" role="menuitem" aria-label="COntact">Contact</div>
  </div>
</div>
```

<b>GREAT</b>

```html
<nav aria-label="Acessible menubar">
  <ul id="acessibleMenu" role="menubar" aria-label="Acessible menubar">
    <li role="none">
      <a
        role="menuitem"
        aria-haspopup="false"
        aria-expanded="false"
        href="#"
        tabindex="0"
      >
        About
      </a>
    </li>
    <li role="none">
      <a
        role="menuitem"
        aria-haspopup="false"
        aria-expanded="false"
        href="#"
        tabindex="0"
      >
        Contact
      </a>
    </li>
  </ul>
</nav>
```
