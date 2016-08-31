# foundation-mail-reference

## Alignment classes

`.[small-]?text-[left, center, right]{1}`: align text to whichever position and optionally target only small breakpoint;

`<center>...</center>`: center images, buttons and menus;

`.float-[left, right]{1}`: float an image left or right;

`<columns></columns><columns [[small, large]{1}=...]*>...</columns><columns></columns>`: centering the middle column and optionally giving it a width;

`valign=[top, middle, bottom]{1}`: vertically align content;


## Button

`<button href="[#, ...]{1}"></button>`: creates a button, href attribute is mandatory;

`.[tiny, small, large]?`: sizes the button or can be omitted for default size;

`.[small-]?expanded`: expand the button to full width;


## Global Styles

`.[primary, secondary, success, warning, alert, white, black]{1}`: colors the element in (blue, grey, green, yellow, red, white, black, ...) respectively;

`$global-width`: width of the container;
`$global-gutter`: width of the grid gutter (between columns and the outside edge);
`$global-breakpoint`: $global-width + $global-gutter, width at which layout is changed;


## The Grid

`<container>...</container>`: main container for the email, it gives the email the full width that is available;

`<row>...</row>`: creates a new row to accept more columns;

`.[collapse]?`: removes gutters in all columns within;

`<columns [small="..."]? [large="..."]?>...</columns>`: creates a new column of the specified width/12 for both small and large screens;

`.[first, last]{1}`: adds an appropriate amount of padding from the container's edge;

`.[expander]?`: forces columns to take up max width in outlook;

`.[large-, small-]?offset-[...]`: offsets the column by the specified amount;

`$grid-column-count`: number of columns in the email;


## Spacer

`<spacer size="..."></spacer>`: vertically space out content by a pixel value;


## Wrapper

`<wrapper>...</wrapper>`: wraps a container to bind content to its width and allow background colors;


## Text

`<p>...</p>`: place text in a paragraph, use <strong> and <em> for bold and italics;

`<h[1, 2, 3, 4, 5, 6]?>...[<small>...</small>]...</h[]>`: text headers that go from largest to smallest, different presets for each screen size. use "small" tag to force smaller screen preset.
