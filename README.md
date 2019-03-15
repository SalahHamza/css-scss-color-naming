# CSS/SCSS Color Naming Convention:

## First suggestion

### Overview

```
$color-alpha
$color-beta
$color-gamma
$color-psi
$color-omega
```

### Dark & Light Variants

Most of the time there'll be **dark** and **light** variants of each color, in that case we can apply a `--dark` or `--light` modifiers. **e.g**:

```
$color-alpha
$color-alpha--dark
$color-alpha--light
```

### Multiple Dark and Light Variants

In case there are more than one **light** or **dark** variants a number system can be applied, for example:

```
$color-alpha
$color-alpha--dark-1
$color-alpha--dark-2
//...
$color-alpha--dark-n

$color-alpha--light-1
$color-alpha--light-2
//...
$color-alpha--dark-n
```

`dark-1` & `light-1` being closest to the main color.

### Resources

- [**ALPHA**, **BETA**, **GAMMA** naming convention](https://www.silvestarbistrovic.from.hr/articles/alpha-beta-gamma-naming-convention/)
- [What do you name color variables?](https://css-tricks.com/what-do-you-name-color-variables/)

## Second suggestion

### Overview

```
$color-primary
$color-secondary
$color-accent
$color-semantic
$color-neutral
```

As mentioned in the [first seggestion](#first-suggestion) we can apply `--dark` and `--light` variants to each color and in case we have multiple variants we can use a numbering system, except for [**Semantic Colors**](#semantic-colors) & [**Neutral Colors**](#neutral-colors).

### Semantic Colors

Semantic colors should be described _semantically_:

```
$color-semantic--success
$color-semantic--error
$color-semantic--warning
$color-semantic--info
```

### Neutral Colors

> These colors are usually made for text and/over background. To do that, Material design has a good hack. Instead of defining specific code for black or grey, they use the opacity of black to apply typography value. In other words, no need to define grey color code, they adjust the opacity of black to 54% or 81% or so. Pretty smart, huh?
> — Anna Molly - [Basic UI color guide](https://blog.prototypr.io/basic-ui-color-guide-7612075cc71a)

For neutral colors, since they are usually White, black or gray schemes, we can apply a numbering system "similar" to [Material Design's color system](https://material.io/design/color/the-color-system.html), with **1** given to the lightest color in the neutral set:

```
$color-neutral--1
$color-neutral--2
//...
$color-neutral--n
```

### Resources

- [Basic UI color guide](https://blog.prototypr.io/basic-ui-color-guide-7612075cc71a)
- [The color system ](https://material.io/design/color/#)

## Other Resources:

- [BEM — Block Element Modifier](https://blog.prototypr.io/basic-ui-color-guide-7612075cc71a)
- [Design System Sprint 2: One Color Palette to Rule them All](https://medium.com/@ethersystem/speccing-colors-in-design-systems-f06e91ed9ca0)
