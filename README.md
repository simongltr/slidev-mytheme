# slidev-mytheme

My custom [Slidev](https://sli.dev) theme, forked from the default theme.

## Summary

Compared to the default Slidev theme, this fork adds:
- custom content components in `components/`
- different default fonts
- refined heading and spacing rules in `styles/layouts.css`
- improved spacing for the built-in `two-columns` layout

The layouts in `layouts/` are inherited from the default theme and currently remain structurally unchanged.

## New Components

These components were added on top of the base theme:

When a component accepts a `color` prop, the available colors are:
- `red`
- `orange`
- `amber`
- `yellow`
- `lime`
- `green`
- `emerald`
- `teal`
- `cyan`
- `sky`
- `blue`
- `indigo`
- `violet`
- `purple`
- `fuchsia`
- `pink`
- `rose`

### `Callout`

Purpose:
- highlight a key point
- provide a lightweight colored emphasis block

Behavior:
- accepts a `color` prop
- defaults to `blue`
- renders a left border with a tinted background

### `Box`

Purpose:
- group related content
- frame supporting content with a border and a soft background

Behavior:
- accepts a `color` prop
- defaults to `blue`
- renders a bordered block with rounded corners

### `Keyword`

Purpose:
- emphasize an inline term
- provide a small colored label inside running text

Behavior:
- accepts a `color` prop
- defaults to `blue`
- renders an inline badge-like highlight

### `Caption`

Purpose:
- render secondary text
- support muted notes, captions, or source lines

Behavior:
- no props
- uses smaller text and reduced opacity
- renders as a `div` so it can safely wrap arbitrary Slidev slot content

## Typography Changes

Compared to the default theme font stack:
- `sans` changed from `Avenir Next,Nunito Sans` to `IBM Plex Sans`
- `mono` changed from `Fira Code` to `JetBrains Mono`
- `serif` was added as `Fraunces`
- `local` changed from `Avenir Next` to `IBM Plex Sans`

This shifts the theme away from the default Slidev look toward a more editorial tone, especially through serif headings.

## Global Layout Styling Changes

These changes affect the existing default-theme layouts without changing their Vue structure.

### Heading Typography

All headings now use the serif font:
- `h1`
- `h2`
- `h3`
- `h4`
- `h5`
- `h6`

This is the main visual departure from the base theme.

### Section Spacing

Spacing before subsection headings was broadened:
- `h2` now gets top margin after `p`, `ul`, `ol`, `table`, `blockquote`, `pre`, and `h6`
- `h3` now gets top margin after the same set of preceding elements

This makes long-form slides read more consistently than the default theme.

### `h1 + p` Behavior

The default theme applied reduced opacity and negative top margin to paragraphs directly following `h1`.

This fork removes that global `h1 + p` styling. As a result:
- subtitles and first paragraphs are less forced into the default hero/subtitle pattern
- content slides get more neutral paragraph styling

## Built-in Layout Adjustments

No layout Vue file in `layouts/` has been structurally changed relative to the base theme.

The only layout-specific adjustment in this fork is:

### `two-columns`

Added:
- extra gap via `@apply gap-8`

Effect:
- gives the built-in two-column layout more breathing room than the default theme

## What Remains Unchanged From The Base Theme

These layouts still come from the default Slidev theme structure:
- `cover`
- `intro`
- `section`
- `statement`
- `fact`
- `quote`

That matters because this fork is currently more of a styling and component extension than a layout rewrite.

## Practical Positioning

Relative to the base theme, the current theme identity is:
- same default layout structure
- stronger editorial typography
- better content spacing
- more useful authoring primitives through custom components
