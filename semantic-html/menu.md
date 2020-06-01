# Menu

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