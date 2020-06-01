# Tabs

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

<b>GOOD</b>

```html
<div class="tabs" role="tablist">
  <div class="tabs-header">
    <div
      class="item-title"
      id="skills-tab"
      role="tab"
      aria-selected="true"
      aria-controls="skills-tab"
    >
      Skilss
    </div>
    <div
      class="item-title"
      id="experience-tab"
      role="tab"
      aria-selected="true"
      aria-controls="experience-tab"
    >
      Experience
    </div>
  </div>

  <div class="tabs-content">
    <div
      class="tabs-item-content"
      id="skills-tab-content"
      tabindex="0"
      role="tabpanel"
      id="skills-tab"
      aria-labelledby="skills"
    >
      skills content
    </div>

    <div
      class="tabs-item-content"
      id="experience-tab-content"
      tabindex="0"
      role="tabpanel"
      id="experience-tab"
      aria-labelledby="experience"
    >
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