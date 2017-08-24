---
title: Spinner
introduction: |
  A spinner component is used to indicate that content is loading and is particularly useful for dynamically loaded content displaying an animated circle graphic.
  A spinner may be required when elements of a page are still loading, or following a user interaction whilst new content is loaded.
  Once the content has loaded the spinner fades and should be replaced by the loaded content.
source: sky-toolkit-ui/components/_spinner.scss
dependencies:
  - sky-toolkit-core
contributors:
  - danieljbryson
  - joebell93
  - skitson
  - welikeideas
template: component
---

# Spinner

## Base

### Spinner

Displays a single spinner component in the page.

```html
<strong class='c-spinner' role='progressbar'>Loading…</strong>
```

### Spinner Overlay

Used in tiles and displays a spinner with an opaque background over the top of
the content to be loaded.

```html
<article class="c-tile">
  <div class="c-tile__content">
    <div class="c-spinner-overlay c-spinner-overlay--light">
      <strong class="c-spinner" role="progressbar">Loading…</strong>
    </div>
    <img src="<url-to-image>" alt="Demo image"/>
  </div>
</article
```

## Modifiers

### Spinner

#### Small 

```html
<strong class="c-spinner c-spinner--small" role="progressbar">Loading…</strong>
```

#### Large

```html
<strong class="c-spinner c-spinner--large" role="progressbar">Loading…</strong>
```

### Spinner Overlay

#### Dark

Displays an Overlay Spinner using a dark background with a lighter, inverted
Spinner to contrast with the darker background.

```html
<article class="c-tile">
  <div class="c-tile__content">
    <div class="c-spinner-overlay c-spinner-overlay--dark">
      <strong class="c-spinner c-spinner--inverse" role="progressbar">Loading…</strong>
    </div>
    <img src="url-to-image" alt="Sample image"/>
  </div>
</article>
```

### Complete

Adding a class of `.is-complete` to the Spinner or Spinner Overlay will provide
a fade-out exit transition to indicate loading completion.

```html
<strong class="c-spinner is-complete" role="progressbar">Loading…</strong>
```