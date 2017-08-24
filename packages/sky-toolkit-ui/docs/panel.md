---
title: Panel
introduction: |
  A panel component is usually used alongside a tile component. When a tile has been clicked and has an `.is-selected` class, the panel component opens.
  Panels typically contain further information relating to the tile component that has triggered the panel.
  Panels span 100% width of the viewport and appear to split the document horizontally at page level.
source: sky-toolkit-ui/components/_panel.scss
dependencies:
  - sky-toolkit-core
contributors:
  - danieljbryson
  - aaronthomas
  - joebell93
  - mrdinsdale
  - skitson
template: component
---

# Panel

## Base

This is the panel component in it's basic default form. The default panel has a
white background with dark text. When a panel is visible, it also has a class of
`.is-open`.

You can put any content you like inside a panel. It is recommended that you nest
the content inside a wrapper with a class of `.o-container`.

```html
<article class="c-panel is-open">
  <div class="c-panel__content">
    <a class="c-panel__toggle" href="#1">Close</a>
    <div class="o-container">
      <h2 class="c-heading-bravo">This is a title</h2>
      <p class="c-text-body  u-text-constrain">
        This is a paragraph. Lorem ipsum dolor sit amet, consectetur adipisicing
        elit. Quos officiis atque ab esse eaque, facilis dolor. Culpa quidem
        officiis, ea. Debitis, delectus? Hic quam rem, accusamus officia libero
        quidem unde.
      </p>
    </div>
  </div>
</article>
```

## Modifiers

### Dark

A dark version of the panel with a black background and white text.

```html
<article class="c-panel c-panel--dark is-open">
  <div class="c-panel__content">
    <a class="c-panel__toggle" href="#1">Close</a>
    <div class="o-container">
      <h2 class="c-heading-bravo">This is a title</h2>
      <p class="c-text-body  u-text-constrain">
        This is a paragraph. Lorem ipsum dolor sit amet, consectetur adipisicing
        elit. Quos officiis atque ab esse eaque, facilis dolor. Culpa quidem
        officiis, ea. Debitis, delectus? Hic quam rem, accusamus officia libero
        quidem unde.
      </p>
    </div>
  </div>
</article>
```