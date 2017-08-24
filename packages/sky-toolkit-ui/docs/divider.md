---
title: Divider
introduction: |
  Dividers are used to dictate a thematic break in content or a shift in topic.
  The Toolkit provides two components to create horizontal rules; `.c-divider` for prominent breaks in content, and `.c-keyline` for simple border boundaries.
source: sky-toolkit-ui/components/_divider.scss
dependencies:
  - sky-toolkit-core
contributors:
  - danieljbryson
  - joebell93
template: component
---

# Divider

## Base

The divider in its basic form uses a gradient keyline and provides a prominent
shadow on the bottom edge. By utilising `<hr>` we can easily place content above
and below without disrupting the flow of the document.

```html
<hr class="c-divider" />
```

## Modifiers

### Top

Provides a horizontal divider with a prominent shadow on the top edge.

```html
<hr class="c-divider c-divider--top" />
```

### Left and Right

Provides vertical dividers with a prominent shadow on the left and right edges.

**Note**: Unlike horizontal dividers, these should be applied to a block element
and wrapped around content.

```html
<div class="c-divider c-divider--left">
  Divider on the left.
</div>
<div class="c-divider c-divider--right">
  Divider on the right.
</div>
```

## Spacing

Extra spacing can be applied on any edge with the spacing utility classes.