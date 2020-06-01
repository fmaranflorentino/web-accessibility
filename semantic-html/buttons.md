# Buttons

A simple buttons example

<b>BAD</b>

```html
<div class="button button-primary">
  Login
</div>
```

```html
<a class="button button-primary">
  Login
</a>
```

<b>GOOD</b>

A example using a `<div></div>`

```html
<div tabindex="0" role="button" id="login">
  Login
</div>
```

A example using a `<a></a>`

```html
<a tabindex="0" role="button" id="loginAction" aria-pressed="false">
  Login
  <svg>
    <use xlink:href="images/login.svg#login-icon"></use>
  </svg>
</a>
```

<b>GREAT</b>

```html
<button tabindex="0" aria-pressed="false" id="loginAction">Login</button>
```
