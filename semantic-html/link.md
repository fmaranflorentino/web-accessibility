# Link

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