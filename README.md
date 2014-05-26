# angoolar-css-taxonomy

A CSS framework for styling at least 80% of literally any site without actually writing a single
line of CSS.

## What is a Theme?

* defined by a map

* that defines a common set of constants (colors, dimensions)

* and a collection of styles

### The Theme Config Map

So for instance, to declare a theme, you first declare a SASS map that defines the colors and
dimensions for your theme. There is a helper function for making this map, which is make-theme:

```scss
$black-theme: make-theme((
	name            : 'black',
	primary-colors  : $black-primary-colors,
	secondary-colors: $black-secondary-colors,
	style-specs     : (
		coloring             : $default-style-spec-coloring,
		mostly-sheer-coloring: $default-style-spec-mostly-sheer-coloring,
	),
)) !global;
```

Above, you can see I'm configuring a black theme, by passing into the make-theme function a map with
all the fields of the theme I need to override in order to make the theme.

So, I specified `name`, `primary-colors`, `secondary-colors`, and `style-specs`; these are typically
the only theme fields you'll need to specify in order to create a theme that simply has differently
colored styles.

There are however, currently 14 map fields that can be overridden; they are as follows:

* _**name**_
* _**extends**_
* **style-specs**
* **theme-spec**
* primary-colors
* secondary-colors
* opacity-modifiers
* text-styles
* shadows
* colorings
* buttons
* borders
* spacing
* transitions

### The Theme Config Map - `name`, `extends`

I bolded `name`, `extends`, `style-specs`, and `theme-spec` because these four fields are very
different from the rest. Largely, the theme config map is a collection of constants that are colors
and whatnot, e.g. `primary-colors` and `opacity-modifiers` and so on. However, these four fields
determine what the theme _**is**_ and what the theme is **made up of**, respectively.

So, a `black` theme would have a _**name**_ of `'black'`. This means, if the `black` theme has a
button style declared, you would be able to style an element with the black button style either by
adding the class `.black-button` to the element or by adding the classes `.black.button` to the
element, or by having an ancestor element with the class `.black` and the class `.button` on the
element. Like so:

```html
<a class="black-button">A Black Button</a>

<a class="black button">A Black Button</a>

<div class="black">
	<a class="button">A Black Button</a>
</div>
```

`extends` is like name in that it defines how you can specify the theme of the style you're applying
to an element. But instead of like with name, where you specify the theme of the style you're
applying with a CSS class of the `name` of the theme, with `extends`, you can simply say that
everything under the `extends` selector, such as `extends: body`, should use this theme's styles.
For instance, if the black and blue themes, instead of using names to define where their respective
styles are used, used `extends` like so:

```scss
$black-theme: make-theme((
	extends         : body,
	secondary-colors: $black-colors,
	style-specs     : (
		button: make-style-spec()
	)
));

$blue-theme: make-theme((
	extends         : article,
	secondary-colors: $blue-colors,
	style-specs     : (
		button: make-style-spec()
	)
));
```

Then if you had HTML like so:

```html
<body>

	<a class="button">Black Button</a>

	<article>
		<a class="button">Blue Button</a>
	</article>

</body>
```

### The Theme Config Map - `theme-spec`

As mentioned, a theme is made up of a collection of styles, as well as any theme-level modifiers.
E.g. a `black` theme may have a `button` style, but a `grey` theme may not and instead have a
`coloring` style. What styles make up a theme is defined by the `style-specs` field. What modifiers
a theme has is defined by the `theme-spec` field.

Let's say we want two themes, `black`, and `blue`, and we want the `black` theme to be default and
the `blue` theme to be applied when the user hovers an element. We could define our themes as
follows:

```scss
$black-theme: make-theme((
	name            : 'black',
	secondary-colors: $black-colors,
	style-specs     : ( button: make-style-spec() ),
	theme-spec      : make-theme-spec(( with-when-hovered: true ))
));

$blue-theme: make-theme((
	name            : 'blue',
	secondary-colors: $blue-colors,
	style-specs     : ( button: make-style-spec() ),
	theme-spec      : make-theme-spec(( with-when-hovered: true ))
));
```

So, we could do this:

```html
<a class="black button blue-when-hovered">I'm Black and Blue</a>
```

### The Theme Config Map - `style-specs`

'style-specs is what defines which styles are rendered for each theme. So, if you want a theme with
'a `button` style, and a `sheer-coloring` style, youre going to have to define a spec for each of
'those styles in your themes `style-specs` field. Like so:

```scss
$blue-theme: make-theme((
	name            : 'blue',
	secondary-colors: $blue-colors,
	theme-spec      : make-theme-spec(( with-when-hovered: true )),
	style-specs     : (
		button            : make-style-spec(),
		sheer-coloring    : make-style-spec(),
		coloring          : make-style-spec(( with-when-hovered: true )),
		mostly-transparent: make-style-spec(),
		opaque            : make-style-spec(( with-when-hovered: true, only-with-whens: true )),
	),
));
```

Notice that in this theme, you will be able to use the following CSS styles:

```html
<body class="blue">
	<div class="sheer-coloring coloring-when-hovered">

		Transclucent blue background, but blue background when hovered.

		<a class="button">A Blue Button</a>

		<div class="coloring mostly-transparent opaque-when-hovered">
			Always solid blue background here, but semi-transparent until hovered.
		</div>

	</div>
</body>
```

And the nice thing is, you won't be bloating your CSS with the `.opaque` class because it's only being
rendered with the -when-hovered modifier.

### The Theme Config Map - Defaults

An important concept to configuring your Taxonomy themes efficiently and effectively is that of
defaults. For every Taxonomical style, there is a `default-style-spec-...`. For instance:

```scss
...
$default-style-spec-text-coloring        : make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
$default-style-spec-link-coloring        : make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
$default-style-spec-coloring             : make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
$default-style-spec-sheer-coloring       : make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
$default-style-spec-barely-sheer-coloring: make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
$default-style-spec-mostly-sheer-coloring: make-style-spec(( with-fully-qualified: true, with-inverse: true, with-secondary: true )) !global !default;
...
```

These are the default style specs for `text-coloring`, `link-coloring`, `coloring`, `sheer-
coloring`, `barely-sheer-coloring`, and `mostly-sheer-coloring`. Notice that for each of these, I
default their `with-fully-qualified` to true. There are for all Taxonomy styles, at least 15 possible spec fields:

* class-name
* only-with-whens
* with-inverse
* with-secondary
* with-this
* with-fully-qualified
* with-when-hovered
* with-when-active
* with-when-touching
* with-when-retina
* with-when-first
* with-when-last
* with-when-ff
* with-when-ie
* with-when-mobile

These allow you to *specify* how each style of the Taxonomy is rendered. For instance, what's its
`class-name`? By default, the class used to specify each style is given by the style's key in the
`style-specs` field of the theme config map. Currently, there are 150 possible styles you can define
in the style-specs field: [Taxonomy style-specs](docs/style_specs.md)



