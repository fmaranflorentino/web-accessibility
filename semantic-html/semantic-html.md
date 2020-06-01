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

#### Want to see more examples, follow the links bellow

1. [Menu](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/menu.md)
2. [Link](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/link.md)
3. [Tabs](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/tabs.md)
4. [Breadcrumb](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/breadcrumb.md)
5. [Buttons](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/buttons.md)
6. [Accordion](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/accordion.md)
7. [Dialog](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/dialog.md)
8. [Checkbox](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/checkbox.md)
9. [Autocomplete/combobox](https://github.com/fmaranflorentino/web-accessibility/blob/master/semantic-html/autocomplete-combobox.md)
