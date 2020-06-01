# Dialog

A simple dialog example

<b>BAD</b>

```html
<div onclick="openDialogProfile(this)">
  Open profile info
</div>

<div id="dialogProfileInfo">
  <div class="dialog_content">
    <h2 id="personal_information">
      Your profile information
    </h2>

    <div class="dialog_actions">
      <button onclick="closeDialog()">
        Cancel
      </button>
    </div>
  </div>
</div>
```

<b>GREAT</b>

```html
<button onclick="openDialogProfile(this)">
  Open profile info
</button>

<div
  role="dialog"
  id="dialogProfileInfo"
  aria-labelledby="personal_information"
  aria-modal="true"
>
  <div class="dialog_content">
    <h2 id="personal_information">
      Your profile information
    </h2>

    <div class="dialog_actions">
      <button onclick="closeDialog()">
        Cancel
      </button>
    </div>
  </div>
</div>
```
