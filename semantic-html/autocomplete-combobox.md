# Autocomplete / Combobox

A simple example of autocomplete / combox

<b>BAD</b>

```html
<label id="autocomplete_label">
  Select your city
</label>

<div class="wrapper">
  <div id="autocomplete_combobox">
    <input type="text" id="autocomplete_input" />
  </div>
  <ul id="autocomplete_listbox" class="listbox hidden"></ul>
</div>
```

<b>GREAT</b>

```html
<label for="autocomplete_input" id="autocomplete_label">
  Select your city
</label>

<div class="wrapper">
  <div
    role="combobox"
    aria-expanded="false"
    aria-owns="autocomplete_listbox"
    aria-haspopup="listbox"
    id="autocomplete_combobox"
  >
    <input
      type="text"
      aria-autocomplete="list"
      aria-controls="autocomplete_listbox"
      id="autocomplete_input"
    />
  </div>
  <ul
    aria-labelledby="autocomplete_label"
    role="listbox"
    id="autocomplete_listbox"
    class="listbox hidden"
  ></ul>
</div>
```
