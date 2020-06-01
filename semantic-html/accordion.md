# Accordion

A simple accordion example

<b>BAD</b>

```html
<div class="tabs-container">
  <div id="accordionContent" class="accordion">
    <h3>
      <button class="accordion-header" id="personalInfoid">
        <span class="accordion-title">
          My personal info
          <span class="accordion-icon"></span>
        </span>
      </button>
    </h3>
    <div id="personalInfo" class="accordion-panel">
      <div>
        Personal info content
      </div>
    </div>

    <h3>
      <button class="accordion-header" id="professionalInfoid">
        <span class="accordion-title">
          My personal info
          <span class="accordion-icon"></span>
        </span>
      </button>
    </h3>

    <div id="professionalInfo" class="accordion-panel">
      <div>
        professional info content
      </div>
    </div>
  </div>
</div>
```

<b>GREAT</b>

```html
<div class="tabs-container">
  <div data-allow-toggle id="accordionContent" class="accordion">
    <h3>
      <button
        aria-expanded="true"
        class="accordion-header"
        aria-controls="personalInfo"
        id="personalInfoid"
      >
        <span class="accordion-title">
          My personal info
          <span class="accordion-icon"></span>
        </span>
      </button>
    </h3>
    <div
      id="personalInfo"
      role="region"
      aria-labelledby="personalInfoid"
      class="accordion-panel"
    >
      <div>
        Personal info content
      </div>
    </div>

    <h3>
      <button
        aria-expanded="false"
        class="accordion-header"
        aria-controls="professionalInfo"
        id="professionalInfoid"
      >
        <span class="accordion-title">
          My personal info
          <span class="accordion-icon"></span>
        </span>
      </button>
    </h3>

    <div
      id="professionalInfo"
      role="region"
      aria-labelledby="professionalInfoid"
      class="accordion-panel"
    >
      <div>
        professional info content
      </div>
    </div>
  </div>
</div>
```
