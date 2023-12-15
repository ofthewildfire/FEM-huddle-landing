# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the
[Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0).
Frontend Mentor challenges help you improve your coding skills by building
realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

Pretty fun; this is just a single page challenge with a background image, some
socials at the bottom.

### Screenshot

![](./desktop.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

### Built with

- HTML
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I learned how to make the hover state when you hover over an svg nested in an
anchor tag change both the border of the link and the svg fill property. Before
I had an issue with this, it would change one at a time, for example, if I moved
my mouse into the border (the `a` tag in this case) the `svg` would change
colour but the border might not and vice versa, which was not a good look, but,
with the CSS below, now that isn't the case.

```css
.social-link:hover,
.social-link:active,
.social-link:focus,
:is(
		.social-link:hover > svg,
		.social-link:active > svg,
		.social-link:focus > svg
	) {
	border-color: var(--soft_magenta-clr);
	fill: var(--soft_magenta-clr);
}
```

Its very messy, but, it does what I want it to do and I will continue to
refactor and learn. :)

### Continued development

Improving use of Grid and Flexbox along with Media Queries to make responsive
layouts.

## Author

- Frontend Mentor -
  [@ofthewildfire](https://www.frontendmentor.io/profile/ofthewildfire)
- Twitter - [@km_fsdev](https://www.twitter.com/km_fsdev)
