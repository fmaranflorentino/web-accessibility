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

<hr>

Simple link example

<b>BAD</b>

```html
<a href="{yourLink}">See my link</a>
```

```html
<span onClick="{handleClick}">See My link</span>
```

<b>GREAT</b>

A link with `<a>`tag

```html
<span
  tabindex="0"
  role="link"
  aria-label="Link to your link"
  onclick="{...}"
  onkeydown="{...}"
>
  Your link
</span>
```

A link with a `<img />`tag

```html
<img
  tabindex="0"
  role="link"
  onclick="{...}"
  onkeydown="{...}"
  src="{imgSource}"
  alt="Img description"
/>
```

```html
<a
  href="{yourLink}"
  title="{linkTitle}"
  role="link"
  aria-label="See my link"
  tabindex="0"
  >See my link</a
>
```

Simple tabs example

<b>BAD</b>

```html
<div class="tabs">
  <div class="tabs-header">
    <div class="header-item" id="skills-tab">Skilss</div>
    <div class="header-item" id="experience-tab">Experience</div>
  </div>

  <div class="tabs-content">
    <div class="tabs-item-content" id="skills-tab-content">
      skills content
    </div>

    <div class="tabs-item-content" id="experience-tab-content">
      Experience content
    </div>
  </div>
</div>
```

<b>Great</b>

```html
<div class="tabs">
  <div role="tablist">
    <button
      role="tab"
      aria-selected="true"
      aria-controls="skills-tab"
      id="skills"
    >
      Skills
    </button>
  </div>

  <div tabindex="0" role="tabpanel" id="skills-tab" aria-labelledby="skills">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc sit amet
      euismod ex. Integer euismod, justo sed blandit aliquet, ex quam porta
      ligula, eu hendrerit diam purus nec sem. Mauris a sagittis dolor. Donec
      pellentesque elit sit amet urna rutrum sollicitudin. Ut eu elit laoreet,
      dapibus sem et, ultrices lacus. Maecenas fermentum purus porttitor,
      facilisis lectus nec, molestie lorem. Morbi elementum ligula est, eu
      dignissim ex faucibus sed. Maecenas consequat et quam id tempus. Aliquam
      elementum leo id vehicula semper. Vivamus in eleifend neque. Donec finibus
      iaculis enim, sed sodales nunc. Curabitur vel dapibus risus. Donec ut
      neque sodales ligula malesuada accumsan. Nullam aliquet diam in elit
      facilisis, quis accumsan sapien volutpat.
    </p>
  </div>
</div>
```
