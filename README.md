# udemy-html-css

## HTML - CSS udemy course

Header
article
aside

## HEAD

- Elementos no visibles dentro del sitio, tales como titulo, icono, etc.
- Se usa tambien para alojar metadatos.

existen elementos HTML (etiquetas)
y entidades HTML (caracteres especiales, como el signo copyright)

## Headings

son elementos gerarquicos para indicar titulos, existen H1 hasta H6

usar elemento _strong_ por su valor semantico para negrillas
usar _em_ (emphatize) para cursivas

es importante agregar el atributo "alt" y "desc" a cualquier imagenes (buenas practicas SEO)

los hipervinculos, a hacen referencia a "anchor" y si no se tiene un URL para especificar se utiliza el default "#"

Los ID de elementos HTML solo se pueden usar una vez, para reutilizar alguno se debe utilizar clases en su lugar.

la prioridad de HTML en cuanto a aplicacion de estilos es:
element > class > id > inline

CSS
Selectors

\# -> ID

. -> class

## Margins and paddings:

vertical margings collapse to the size of the greater one
Collapsing margins:The top and bottom margins of blocks are sometimes combined (collapsed) into a single margin whose size is the largest of the individual margins (or just one of them, if they are equal), a behavior known as margin collapsing. Note that the margins of floating and absolutely positioned elements never collapse.

margins are not inherited

space inside elements: Padding (IE: colored backgrounds and gat between text and borders)
space outside elements: Marging (IE: separation)

To any element that has an exact height defined, the real height of the element is:
height(80px) + padding-top(20px) + padding-botton(20px) total: 120px

margin doesnt work on certain small elements (IE: anchors)

## block level elements

Elements are Formatted visually as _blocks_

Elements occupy _100% of parents element's width_, no matter the content

elements are _stacked vertically_ by default one after another

the box-model _applies as showed_ earlier

default elements: `body, main, header, footer, section, nav, aside, div, h1-h6, p, ul, ol, li`, etc

with CSS:
`display: block`

## Inline elements

occupie only the space _neccesary for its content_

causes _no line-breaks_ after or before the element

box model applies in different way: _heigths and widths do not apply_

_paddings and margings_ are applied _only horizontally_ (left and right)

default elements: `a, img, strong, em, button`, etc.

with CSS: `display: inline`

## Absolute and relative position

absolute elements must be contained whiting a relative element and must have top, bottom, right and left properties.

## pseudo elements

Pseudo elements are similar to pseudo classes but this works for elements instead, IE: `h1::first-letter`

### adyacent Silbing elements

adyacent silbing element selector stands to select the after `h3+p::first-line` and before pseudo element `h3 - p::first-line`
example:

```
h2 {
background-color> orange;
position: relative;
}

h2::after {
content: "TOP";
background-color: "yellow";
font-size: 16px;
font-weight:bold;
display:inline-block;
padding: 5px 10px;
position: absolute;
top: 15px;
right: -25px;
}
```

## Layouts, Floats, Flexbox and Grids

### FLOATS

deprecated CSS Flow, do not use

## FLEX AND GRID

Flex and grid are meant to work together or be used withing their own use cases based on the developer design

both are modern and captable of great results

## FLEX

Items are automatically distributed along the FLEX container

Two axis, main axis (default one, left to right) and cross axis (top to bottom)

good practice: include all the configuration for layaout inside the flex container

use order to set order of items appearing on the flex container, default is 0, lower number (less than 0) goes first, higher items (more than 0) shows last

## GRID

similar to flex box, this case developer define rows amount, content acomodate to have as many columns needed to show all content within the grid container

grid items fill entire row size

## Site personality

Each site personalities have some characteristics that make the user feel different emotion, the goal here is to understand the business itself to pick a matching personality for the site, this is a combination from both, site and business goals.

## Units

- px
- %: percentage of screen
- rem: Root Element Size, default 60px, rem is used to keep relation between components and font size as relative relation

When using max-width it is inherited by child components of the container.
