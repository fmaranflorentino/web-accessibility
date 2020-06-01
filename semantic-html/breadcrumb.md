# Breadcrumb

A breadcrumb simple example

<b>BAD</b>

```html
<div class="breadcrumb">
  <div class="breadcrumb-item">
    Services
  </div>
  <div class="breadcrumb-item last">
    Web Development
  </div>
</div>
```

<b>GOOD</b>

```html
<div role="menubar" aria-label="Breadcrumb" class="breadcrumb">
  <div role="menuitem" aria-label="Services" class="breadcrumb-item">
    Services
  </div>
  <div
    role="menuitem"
    aria-label="web development"
    class="breadcrumb-item last"
  >
    Web Development
  </div>
</div>
```

<b>GREAT</b>

```html
<nav aria-label="Breadcrumb" class="breadcrumb">
  <ol>
    <li>
      <a href="../../" title="Services">
        Services
      </a>
    </li>
    <li>
      <a href="../../#aria_ex" title="web development">
        Web Development
      </a>
    </li>
  </ol>
</nav>
```
