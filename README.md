# maturana scss

a small scss boiler for minimal needs

## file structure

```
main.scss
├── abstracts file(s)
│   └── config file with many variables
├── base files
│   ├── reset file based on v8.0.1 | MIT License | github.com/necolas/normalize.css; sort some things out into the module files
│   ├── fonts file | choose your favorite fonts
│   └── typography - sizes based on the config file
├── layouts
│   └── layout composition here
├── modules
│   ├── links
│   ├── button
│   ├── lists
│   ├── forms
│   ├── hamburger
│   ├── navigation
│   ├── hero
│   ├── cards
│   ├── screenreader
│   ├── osano-cookie
│   └── helpers
└── shame
    └── vendors - for bootstrap or something like that
```

## config file

### font sizes
```
$sizes: (
	base-size: 16px,
	h1: 3rem,
	h2: 2.5rem,
	h3: 2rem,
	h4: 1.75rem,
	h5: 1.5rem,
	h6: 1.3rem,
	p: 1rem
);

// use it like this: font-size: sizes(base-size);
// base size is used for html; use REM in body
```

### colors
```
$colors: (
	// base colors
	dark: #444444,
	light: #eeeeee,
	colored: #f39c12,
	colored-contrast: #ecf0f1,
	body-background: #ffffff,
	font: #444444,
	
	// navigation-bar
	h-bg: transparent,			// hamburger background
	o-color: #37474f,			// open color
	c-color: #37474f,			// close color
	
	nav-bg: #ffffff,			// navigation-bar background
	nav-link: #444444,			// navigation link color
	nav-hover: #000000,			// navigation link hover color
	
	nav-mobile-bg: #37474f,		// mobile navigation background color
	nav-mobile-link: #ffffff,	// mobile navigation link color
	nav-mobile-hover: #eeeeee,	// mobile navigation hover color
	
	// link colors
	link-color: blue,			// link color
	link-hover: green,			// hover color
);

// use it like this: color: colors(dark);
```

### breakpoints
```
$breakpoints: (
	'small':	(max-width: 320px),
	'medium':	(min-width: 768px),
	'large':	(min-width: 992px),
	'xlarge':	(min-width: 1200px),
);
// use it like this: @include respond-to('medium') {};
```


