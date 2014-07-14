# Sass Mixins, in production mode

## small little helpers


### 1. FS($font) - Font Size
for responsive and absolute sized Fonts

```sass
=FS($fontSize)
	@if $fontSize == h1 or $fontSize == h2 or $fontSize == h3 or $fontSize == h4
		#{$fontSize}
			// font-size: $FS-#{$fontSize}


	@if $fontSize == ps
		p
			font-size: $FS-ps-sm

	@if $fontSize == pl
		p
			font-size: $FS-pl-sm

	@if $fontSize == pi
		p
			font-size: $FS-pi-sm
			font-style: italic
```


### 2. CE - Clear Everything
	quick overwrite of margin and padding

```sass
	=CE
		margin: 0
		padding: 0
```