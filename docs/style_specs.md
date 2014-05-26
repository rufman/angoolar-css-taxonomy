
* vertical-rhythm-text-styles
  * Todo: document
  * basicness: 2
  * customizability: 1
* appearance-none
  * Removes the element's default browser-provided appearance (such as a <select>)
  * basicness: 0
  * customizability: 0
* hardware-render
  * Gives the element an identity transform that causes the element to be processed by the browsers graphics processor more effectively; this helps with images in a scroll-overflow container or when changing opacity through CSS causes elements to shudder
  * basicness: 0
  * customizability: 0
* transitions
  * Causes all transitionable styles to be transitioned from one to another whenever they change
  * basicness: 0
  * customizability: 1
* no-transitions
  * Prevents any transitionable styles from being transitioned from one to another whenever they change
  * basicness: 0
  * customizability: 0
* not-selectable
  * When applied, prevents the text from being able to be selected with the cursor
  * basicness: 0
  * customizability: 0
* selectable
  * When applied, makes the text able to be selected with the cursor
  * basicness: 0
  * customizability: 0
* hoverable
  * When applied, all descendant elements with the hovered class will be opaque only when the hoverable element is hovered, and all descendant elements with the not-hovered class will be opaque only when the hoverable element is not hovered.
  * basicness: 2
  * customizability: 0
* gone
  * Makes the element completely gone (e.g. display:none)
  * basicness: 0
  * customizability: 0
* invisible
  * Makes the element invisible (e.g. visibility:hidden)
  * basicness: 0
  * customizability: 0
* target-opaque
  * Applies opaque to a descendant with the .target class
  * basicness: 2
  * customizability: 1
* definitely-opaque
  * Applies opaque with !important
  * basicness: 2
  * customizability: 0
* target-mostly-transparent
  *   * basicness: 2
  * customizability: 1
* transparent
  * Makes the element transparent
  * basicness: 0
  * customizability: 0
* mostly-transparent
  * Makes the element mostly transparent (e.g. opacity: .4)
  * basicness: 1
  * customizability: 1
* barely-transparent
  * Makes the element barely transparent (e.g. opacity: .9)
  * basicness: 1
  * customizability: 1
* opaque
  * Makes the element opaque
  * basicness: 0
  * customizability: 0
* mostly-opaque
  * Makes the element mostly opaque (e.g. opacity: .6)
  * basicness: 1
  * customizability: 1
* barely-opaque
  * Makes the element barely opaque (e.g. opacity: .1)
  * basicness: 1
  * customizability: 1
* inline
  * Makes the element an inline element (e.g. display:inline)
  * basicness: 0
  * customizability: 0
* inline-block
  * Makes the element an inline-block element (e.g. display:inline-block with cross-browser fallback)
  * basicness: 0
  * customizability: 0
* block
  * Makes the element a block element (e.g. display:block)
  * basicness: 0
  * customizability: 0
* floatfix
  * This is a real clearfix that works on ALL browsers (not just the typical clearfix that works by muddying the :after pseudo-element)
  * basicness: 0
  * customizability: 0
* no-overflow
  * This indicates that the element should hide all overflowing content
  * basicness: 0
  * customizability: 0
* show-overflow
  * This indicates that the element should show all overflowing content
  * basicness: 0
  * customizability: 0
* scroll-overflow
  * This indicates that the element should scroll all overflowing content (with touch scroll for mobile webkit)
  * basicness: 0
  * customizability: 0
* ellipsis-overflow
  * This indicates that the element should truncate any overflowing text with ellipses (this applies no-wrap and no-overflow for you)
  * basicness: 0
  * customizability: 0
* left
  * Floats the element to the left
  * basicness: 0
  * customizability: 0
* right
  * Floats the element to the right
  * basicness: 0
  * customizability: 0
* clear-left
  * Clears float to the left
  * basicness: 0
  * customizability: 0
* clear-right
  * Clears float to the right
  * basicness: 0
  * customizability: 0
* clear-both
  * Clears float to the left and right
  * basicness: 0
  * customizability: 0
* link
  * Treats element as an anchor tag, even if it's not an anchor tag
  * basicness: 0
  * customizability: 0
* non-link
  * Treats element as a non-anchor tag, even if it's an anchor tag
  * basicness: 0
  * customizability: 0
* text-left
  * Aligns text to the left
  * basicness: 0
  * customizability: 0
* text-right
  * Aligns text to the right
  * basicness: 0
  * customizability: 0
* text-center
  * Aligns text to center
  * basicness: 0
  * customizability: 0
* text-justify
  * Justifies text alignment
  * basicness: 0
  * customizability: 0
* uppercase
  * Makes text uppercase
  * basicness: 0
  * customizability: 0
* capitalize
  * Capitalizes the first letter of each word of the text
  * basicness: 0
  * customizability: 0
* no-wrap
  * Prevents text from wrapping
  * basicness: 0
  * customizability: 0
* break-word
  * Ensures words break (useful in tables)
  * basicness: 0
  * customizability: 0
* wrap
  * Ensures that text wraps
  * basicness: 0
  * customizability: 0
* small-text
  * Makes font size smaller
  * basicness: 1
  * customizability: 1
* very-small-text
  * Makes font size much smaller
  * basicness: 1
  * customizability: 1
* large-text
  * Makes font size larger
  * basicness: 1
  * customizability: 1
* very-large-text
  * Makes font size much larger
  * basicness: 1
  * customizability: 1
* light-weight
  * Makes font weight light
  * basicness: 1
  * customizability: 0
* normal-weight
  * Makes font weight normal
  * basicness: 1
  * customizability: 0
* bold
  * Makes font weight bold
  * basicness: 0
  * customizability: 0
* italic
  * Makes font italic
  * basicness: 0
  * customizability: 0
* underline
  * Makes font underlined
  * basicness: 0
  * customizability: 0
* less-wide
  * Makes font spacing less wide
  * basicness: 2
  * customizability: 1
* wide
  * Makes font spacing wide
  * basicness: 2
  * customizability: 1
* more-wide
  * Makes font spacing more wide
  * basicness: 2
  * customizability: 1
* way-more-wide
  * Makes font spacing way more wide
  * basicness: 2
  * customizability: 1
* table
  * Makes the element a table even if it's not actually (e.g. a div or span)
  * basicness: 0
  * customizability: 0
* table-row
  * Makes the element a tr even if it's not actually (e.g. a div or span)
  * basicness: 0
  * customizability: 0
* table-cell
  * Makes the element a td even if it's not actually (e.g. a div or span)
  * basicness: 0
  * customizability: 0
* fixed-layout
  * Gives a table-styled element a fixed layout
  * basicness: 0
  * customizability: 0
* auto-layout
  * Gives a table-styled element an auto layout
  * basicness: 0
  * customizability: 0
* valign-center
  * Vertically aligns text or cell contents to the bottom of the center
  * basicness: 0
  * customizability: 0
* valign-bottom
  * Vertically aligns text or cell contents to the bottom of the container
  * basicness: 0
  * customizability: 0
* valign-top
  * Vertically aligns text or cell contents to the bottom of the top
  * basicness: 0
  * customizability: 0
* relative
  * Gives the element relative positioning
  * basicness: 0
  * customizability: 0
* absolute
  * Gives the element absolute positioning
  * basicness: 0
  * customizability: 0
* fixed
  * Gives the element fixed positioning
  * basicness: 0
  * customizability: 0
* target-above
  * Makes the z-index of any descendant element with the .target class be above any element without a z-index-related class
  * basicness: 2
  * customizability: 1
* above
  * Makes the z-index be above an element without a z-index-related class
  * basicness: 1
  * customizability: 1
* way-above
  * Makes the element's z-index be above an element with the above class
  * basicness: 2
  * customizability: 1
* way-way-above
  * Makes the element's z-index be above an element with the way-above class
  * basicness: 2
  * customizability: 1
* below
  * Makes the z-index be below an element without a z-index-related class
  * basicness: 1
  * customizability: 0
* tl
  * Positions the element at top:0;left:0
  * basicness: 0
  * customizability: 0
* tr
  * Positions the element at top:0;right:0
  * basicness: 0
  * customizability: 0
* br
  * Positions the element at bottom:0;right:0
  * basicness: 0
  * customizability: 0
* bl
  * Positions the element at bottom:0;left:0
  * basicness: 0
  * customizability: 0
* ratio-size
  * Sizes the element with the ratio given by the last two numbers in the class-name; e.g. width-ratio-1-2 is width: 50% and bottom-ratio-4-5 is bottom: 80%
  * basicness: 1
  * customizability: 0
* whole-size
  * Sizes the element at 100% of the property given by the first term in the class-name; e.g. whole-width is width: 100% and whole-top is top: 100%
  * basicness: 1
  * customizability: 0
* no-size
  * Sizes the element at 0% (by default, or 0em/0px/etc depending on the unit property of the no-size spec in the theme's style-specs) of the property given by the first term in the class-name; e.g. no-top is top:0%, no-width is width: 0%
  * basicness: 1
  * customizability: 0
* specific-value
  * Gives the element a specific size on the property given by the key with the specific size spec in the specific-size property of the theme's style-specs
  * basicness: 2
  * customizability: 2
* target-specific-value
  * Gives the descendant target element the specific size on the property given by the key with the specific size spec in the target-specific-size property of the theme's style-specs
  * basicness: 2
  * customizability: 2
* table-padded
  * Makes the table padded between cells (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* no-background
  * Ensures the element has no background (color, image, whatever)
  * basicness: 1
  * customizability: 0
* whole-rounded
  * Gives the element completely rounded corners (i.e. the element will be an ellipse)
  * basicness: 1
  * customizability: 0
* no-rounding
  * Gives the element squared corners
  * basicness: 1
  * customizability: 0
* border-box
  * Makes the element's box model border-box
  * basicness: 0
  * customizability: 0
* not-bordered
  * Takes away the element's border
  * basicness: 0
  * customizability: 0
* no-padding
  * Removes the element's padding (if any)
  * basicness: 0
  * customizability: 0
* no-margin
  * Removes the element's padding (if any)
  * basicness: 0
  * customizability: 0
* lr-auto-margin
  * This makes the element's left and right margin auto, so if the element has a defined width, it will be centered in its container.
  * basicness: 0
  * customizability: 0
* rounded
  * Gives the element rounded corners
  * basicness: 1
  * customizability: 1
* t-rounded
  * Gives the element rounded corners on the top two corners
  * basicness: 1
  * customizability: 1
* r-rounded
  * Gives the element rounded corners on the right two corners
  * basicness: 1
  * customizability: 1
* b-rounded
  * Gives the element rounded corners on the bottom two corners
  * basicness: 1
  * customizability: 1
* l-rounded
  * Gives the element rounded corners on the left two corners
  * basicness: 1
  * customizability: 1
* tl-rounded
  * Gives the element a rounded top-left corner
  * basicness: 1
  * customizability: 1
* tr-rounded
  * Gives the element a rounded top-right corner
  * basicness: 1
  * customizability: 1
* bl-rounded
  * Gives the element a rounded bottom-left corner
  * basicness: 1
  * customizability: 1
* br-rounded
  * Gives the element a rounded bottom-right corner
  * basicness: 1
  * customizability: 1
* padded
  * Makes the element padded (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* t-padded
  * Makes the element padded on top (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* r-padded
  * Makes the element padded on the right (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* b-padded
  * Makes the element padded on the bottom (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* l-padded
  * Makes the element padded on the left (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* lr-padded
  * Makes the element padded on the left and right (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* tb-padded
  * Makes the element padded on the top and bottom (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* margin
  * Gives the element a margin (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* t-margin
  * Gives the element a margin on top (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* r-margin
  * Gives the element a margin on the right (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* b-margin
  * Gives the element a margin on the bottom (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* l-margin
  * Gives the element a margin on the left (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* lr-margin
  * Gives the element a margin on the left and right (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* tb-margin
  * Gives the element a margin on the top and bottom (or less or more or way more or way, way more depending on the modifier classes also present on the element)
  * basicness: 1
  * customizability: 1
* negative-t-margin
  * Gives the element a margin on top (or less or more or way more or way, way more depending on the modifier classes also present on the element) negative
  * basicness: 1
  * customizability: 1
* negative-r-margin
  * Gives the element a margin on the right (or less or more or way more or way, way more depending on the modifier classes also present on the element) negative
  * basicness: 1
  * customizability: 1
* negative-b-margin
  * Gives the element a margin on the bottom (or less or more or way more or way, way more depending on the modifier classes also present on the element) negative
  * basicness: 1
  * customizability: 1
* negative-l-margin
  * Gives the element a margin on the left (or less or more or way more or way, way more depending on the modifier classes also present on the element) negative
  * basicness: 1
  * customizability: 1
* inset-shadow
  * Gives the element an inset shadow
  * basicness: 1
  * customizability: 1
* deep-inset-shadow
  * Gives the element a deep inset shadow
  * basicness: 1
  * customizability: 1
* shadow
  * Gives the element a shadow
  * basicness: 1
  * customizability: 1
* deep-shadow
  * Gives the element a deep shadow
  * basicness: 1
  * customizability: 1
* no-shadow
  * Removes the element's shadow
  * basicness: 1
  * customizability: 1
* text-shadowed
  * Makes the element's text shadowed
  * basicness: 1
  * customizability: 1
* bordered
  * Makes the element bordered
  * basicness: 1
  * customizability: 2
* t-bordered
  * Makes the element bordered on top
  * basicness: 1
  * customizability: 2
* r-bordered
  * Makes the element bordered on the right
  * basicness: 1
  * customizability: 2
* b-bordered
  * Makes the element bordered on the bottom
  * basicness: 1
  * customizability: 2
* l-bordered
  * Makes the element bordered on the left
  * basicness: 1
  * customizability: 2
* lr-bordered
  * Makes the element bordered on the left and right
  * basicness: 1
  * customizability: 2
* tb-bordered
  * Makes the element bordered on the top and bottom
  * basicness: 1
  * customizability: 2
* ltr-bordered
  * Makes the element bordered on top, left, and right
  * basicness: 1
  * customizability: 2
* lbr-bordered
  * Makes the element bordered on left, bottom, and right
  * basicness: 1
  * customizability: 2
* trb-bordered
  * Makes the element bordered on top, right, and bottom
  * basicness: 1
  * customizability: 2
* blt-bordered
  * Makes the element bordered on bottom, left, and top
  * basicness: 1
  * customizability: 2
* transparent-border
  * Makes the element's border transparent (if it is bordered)
  * basicness: 1
  * customizability: 0
* text-input
  * Makes the element appear as a text-input
  * basicness: 1
  * customizability: 2
* select
  * Makes the element appear as a select
  * basicness: 1
  * customizability: 2
* button
  * This is the convex, shaded button featuring the theme's light secondary color that's no longer deemed hip in the current fad of "flat design"
  * basicness: 1
  * customizability: 2
* shallow-button
  * Is the shallower cousin to the convex, shaded button featuring the theme's light secondary color that's no longer deemed hip in the current fad of "flat design"
  * basicness: 1
  * customizability: 2
* flat-button
  * This is like button and shallow-button, but without any of the shading that would make the button feel convex
  * basicness: 1
  * customizability: 2
* raised-flat-button
  * This is a raised variant of flat-button, where the element starts out a little raised off the page, and when hovered or focused is more shadowed than the flat-button when it is hovered or focused.
  * basicness: 1
  * customizability: 2
* hybrid-button
  * Is the combination of flat-button and button, where when not hovered or focused, it's a flat-button, but then when hovered, it's the convex button that's hovered
  * basicness: 1
  * customizability: 2
* button-shading
  * This is just the shading behavior or the button (with convexness)
  * basicness: 1
  * customizability: 2
* button-shadow
  * This is just the shadow behavior or the button (with convexness)
  * basicness: 1
  * customizability: 2
* text-coloring
  * Makes the element's color that of the theme's light secondary color (regardless of the element's background color - be careful)
  * basicness: 1
  * customizability: 2
* link-coloring
  * Makes the color of all anchor tags and elements with the .link class that of the theme's light secondary color (regardless of the element's background color - be careful)
  * basicness: 1
  * customizability: 2
* coloring
  * Makes the element's background that of the theme's light secondary color, and makes the color whichever of the theme's light and dark primary colors that provides the highest contrast with the background
  * basicness: 1
  * customizability: 2
* sheer-coloring
  * Makes the element's background a mostly opaque version of the theme's light secondary color, and makes the color whichever of the theme's light and dark primary colors that provides the highest contrast with the background
  * basicness: 1
  * customizability: 2
* barely-sheer-coloring
  * Makes the element's background a barely transparent version of the theme's light secondary color, and makes the color whichever of the theme's light and dark primary colors that provides the highest contrast with the background
  * basicness: 1
  * customizability: 2
* mostly-sheer-coloring
  * Makes the element's background a mostly transparent version of the theme's light secondary color, and makes the color whichever of the theme's light and dark primary colors that provides the highest contrast with the background
  * basicness: 1
  * customizability: 2