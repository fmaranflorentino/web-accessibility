# Checkbox

A simple checkbox example

<b>BAD</b>

```html
<h3>
  Select your gender
</h3>

<div class="checkbox_content">
  <div>
    <div>
      <div class="checkbox">
        Male
      </div>
    </div>
    <div>
      <div class="checkbox">
        Female
      </div>
    </div>
    <div>
      <div class="checkbox">
        Others
      </div>
    </div>
  </div>
</div>
```

<b>GOOD</b>

```html
<h3 id="gender_selection">
  Select your gender
</h3>

<div role="group" aria-labelledby="gender_selection">
  <div class="checkbox_container" role="menubar">
    <div role="menuitem">
      <div role="checkbox" aria-checked="false" tabindex="0">
        Male
      </div>
    </div>
    <div role="menuitem">
      <div role="checkbox" aria-checked="false" tabindex="0">
        Female
      </div>
    </div>
    <div role="menuitem">
      <div role="checkbox" aria-checked="false" tabindex="0">
        Others
      </div>
    </div>
  </div>
</div>
```

<b>GREAT</b>

```html
<h3 id="gender_selection">
  Select your gender
</h3>

<div role="group" aria-labelledby="gender_selection">
  <ul>
    <li>
      <div role="checkbox" aria-checked="false" tabindex="0">
        Male
      </div>
    </li>
    <li>
      <div role="checkbox" aria-checked="false" tabindex="0">
        Female
      </div>
    </li>
    <li>
      <div role="checkbox" aria-checked="false" tabindex="0">
        Others
      </div>
    </li>
  </ul>
</div>
```
