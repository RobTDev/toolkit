---
title: Tile
introduction: |
  Tiles are made of a glass edge with a shine on hover, they contain our content and allow any colour beneath to show though.
  Tiles open panels or link to new pages.
  **Note**: Do not feel that all your content must fit within a tile and panel format.
source: sky-toolkit-ui/components/_tile.scss
dependencies:
  - sky-toolkit-core
  - sky-toolkit-ui/components/shine
contributors:
  - danieljbryson
  - joebell93
  - aaronthomas
  - csswizardry
  - mrdinsdale
template: component
---

# Tile

## Default Tile

This is the Tile component in its most simple form.

```html
<article class="c-tile">
  <div class="c-tile__content">
    <div class="c-tile__body">
      <p class="c-tile__title c-heading-delta u-margin-bottom-none">Tile Title</p>
      <p class="c-text-body">Tile Content</p>
    </div>
  </div>
</article>
```

## Split Media Tile

The split media tile allows for an image to be placed in the top half of the
tile and title to be placed below.

```html
<article class="c-tile c-tile--square">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img alt="Demo Image" class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Tile Title</p>
      </div>
    </div>
  </a>
</article>
```

## Full Tile

The full tile allows for an image to be placed as a background for the tile and
title to be placed at the bottom.

```html
<article class="c-tile c-tile--square c-tile--full">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img alt="Demo image" class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body">
        <div class="c-tile__overlay">
          <p class="c-tile__title c-heading-delta">Tile Title</p>
        </div>
      </div>
    </div>
  </a>
</article>
```


## Modifiers

### Square

The square modifier sets a fixed ratio for equal tile height and width. To
remove this forced ratio on mobile see `.c-tile--collapsible`.

**Note**: square tiles can cause issues with scaling typography.

```html
<article class="c-tile c-tile--square">
  <div class="c-tile__content">
    <div class="c-tile__body">
      <p class="c-tile__title c-heading-delta">Tile Title</p>
      <p class="c-text-body">Tile Content</p>
    </div>
  </div>
</article>
```

### Collapsible

The collapsible tile is used in conjuncture with the `.c-tile--square` to remove
the height constraint for mobile breakpoints and allow the tile to inherit
height from its content. If used on a tile featuring the `.c-tile__media`
element it will reposition this to the left.

```html
<article class="c-tile c-tile--square c-tile--collapsible">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Tile Title</p>
      </div>
    </div>
  </a>
</article>
```

### Channel Themes

For tiles requiring branded hover states, simply include the name of the channel
in the format of the gradient names defined in `sky-toolkit-core`; such as 
`.c-tile--sky-atlantic`.

```html
<article class="c-tile c-tile--square c-tile--sky-atlantic">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Sky Atlantic</p>
      </div>
    </div>
  </a>
</article>
```

## States

### Focus

We can programmatically apply a has focus class to Tiles by adding the
`.has-focus` state. This is a requirement for accessibility.

```html
<article class="c-tile c-tile--square has-focus">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img alt="Demo Image" class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Tile Title</p>
      </div>
    </div>
  </a>
</article>
```

### Selected

The `.is-selected` class is used to signify that a tile is selected and its
corresponding panel is open and display the indicator. It should only be used
in combination with a panel.

```html
<article class="c-tile c-tile--square is-selected">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img alt="Demo Image" class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Tile Title</p>
      </div>
    </div>
  </a>
</article>
<article class="c-panel is-open">
  <div class="o-container">
      <p class="c-text-body u-text-constrain">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos officiis
        atque ab esse eaque, facilis dolor. Culpa quidem officiis, ea. Debitis,
        delectus? Hic quam rem, accusamus officia libero quidem unde.
      </p>
  </div>
</article>
```

### Selected (Dark)

As the indicator arrow to show that the corresponding panel is open is part of
the tile we can use the .c-tile--dark class to match the tile indicator to the panel.

```html
<article class="c-tile c-tile--square c-tile--dark is-selected">
  <a class="c-tile__link" href="#">
    <div class="c-tile__content">
      <div class="c-tile__media">
        <img alt="Demo Image" class="c-tile__poster" src="<url-to-image>" />
      </div>
      <div class="c-tile__body c-tile__caption">
        <p class="c-tile__title c-heading-delta">Tile Title</p>
      </div>
    </div>
  </a>
</article>
<article class="c-panel c-panel--dark is-open">
  <div class="o-container">
      <p class="c-text-body u-text-constrain">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos officiis
        atque ab esse eaque, facilis dolor. Culpa quidem officiis, ea. Debitis,
        delectus? Hic quam rem, accusamus officia libero quidem unde.
      </p>
  </div>
</article>
```