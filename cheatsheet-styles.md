---
title: Cheatsheet styles
layout: 2017/sheet
tags: [WIP]
intro: |
  This is a reference of styles that you can use on Devhints cheatsheets. How
  meta! You can refer to this when contributing your own cheatsheets to the [GitHub repo](https://github.com/rstacruz/cheatsheets/).
---

Sections
--------
{: .-three-column}

### Adding variants
{: .-prime}

```
## Section
{: .-two-column}
```

Devhints uses Kramdown, and supports adding classes via Kramdown's syntax.

### H2 sections

| `-one-column` | 1 column |
| `-two-column` | _(default)_ 2 columns |
| `-three-column` | 3 columns |
| `-left-reference` | 3 columns<br>_(short first column)_ |

See: [H2 sections](#two-columns)

### H3 sections

| `-prime` | Adds highlight |

See: [H3 sections](#h3-sections-1)

### Tables

| `-shortcuts` | For shortcut keys |
| `-left-align` | Don't right align last column |
| `-headers` | Show headers |

See: [Tables](#tables-1)

### Code

| `-setup` | Gray background |
| `-box-chars` | Less line height<br>_for box drawing chars_ |

See: [Code](#code-1)

### Paragraphs

| `-setup` | Gray background |
| `-crosslink` | Has arrow on the link |
{: .-gray}

Paragraphs are automatically gray, unless they're the first elements in an H3 section.

See: [Paragraphs](#paragraphs-1)

### Lists

| `-also-see` | Lighter background |
| `-four-column` | 4 columns |
| `-six-column` | 6 columns |

See: [Lists](#lists-1)

H3 sections
-----------
{: .-three-column}

### Supported

Each section can have the following children:

#### White

- `pre`
- `ul`
- `table`

#### Gray

- `p`
- `h4`

### Prime section
{: .-prime}

This is a section with `{: .-prime}`. Notice the fancy highlight! Great for "getting started" kind of snippets.

### H3 section

Every box is an H3 section. The box will encompass everything inside the body of the H3.

This is a basic section with paragraphs in it.

Code
----
{: .-three-column}

### Basic code

```js
here.is(() => {
  some.code()
})
```

```js
here.is.some.more()
```

Code blocks can be placed one after the other.

See: [Cheatsheets](/)

### Code with headings

#### index.js
{: .-file}

```js
here.is(() => {
  some.code()
})
```

#### other.js
{: .-file}

```js
here.is.some.more()
```

Code blocks can have headings.

### Highlighted lines

```js
app.start(() => {
  const port = app.server.port
  console.log(`Started at ${port}`)
})
```
{: data-line="3"}

Add `{: data-line="3"}` to add line highlights.

### Multiple highlights

```js
app.start(() => {
  const port = app.server.port
  console.log(`Started at ${port}`)
})
```
{: data-line="2,3"}

Add `{: data-line="2,3"}` to add multiple line highlights.

### Setup blocks

```js
import React from 'react'
```
{: .-setup}

```js
class Hello extends React.Component {
  render () {
    return <span>Hello</span>
  }
}
```

Add `{: .-setup}` to a `pre` or `table` or `ul`.

### Long lines

```js
function createNode(nodeName: string, options: { key: string }) {
  return true
}
```

Long lines will have scrollbars.

## Lists
{: .-three-column}

### Lists

- This is
- a list
- with a few items

Here's an extra paragraph after the list.

### Lists with headings

#### Part 1

- `createElement()`
- `componentDidMount()`
- `componentWillUnmount()`

#### Part 2

- `shouldComponentUpdate()`
- `componentWillReceiveProps()`


Here's an extra paragraph after the list.

## List columns
{: .-one-column}

### Six columns

- One
- Two
- Three
- Four
- Five
- Six
- Seven
- Eight
- Nine
- Ten
- Eleven
{: .-six-column}

Add `{: .-six-column}` to make large lists.

### Four columns

- One
- Two
- Three
- Four
- Five
- Six
- Seven
- Eight
- Nine
- Ten
- Eleven
{: .-four-column}

Add `{: .-four-column}` to make large lists.

### Also see

- One
- Two
- Three
- Four
- Five
- Six
- Seven
- Eight
- Nine
- Ten
{: .-also-see}

Add `{: .-also-see}`.

## Paragraphs
{: .-three-column}

### Basic paragraphs

This is a basic section with paragraphs in it. When paragraphs are the first elements in an H3 section's body, they appear as white.

### Basic paragraphs

```
···
```

When paragraphs appear after `pre`/`table`/`ul`, they appear with a gray background.

### Preludes

Here's a prelude paragraph. Add `{: .-setup}` to make paragraphs appear with a gray background.
{: .-setup}

```
···
```

### Crosslink

Add `{: .-crosslink}` to make big loud external links:

```
···
```

[Home](/)
{: .-crosslink}

## Tables
{: .-three-column}

### Basic table

#### Date

| Example         | Output                 |
| ---             | ---                    |
| `%m/%d/%Y`      | `06/05/2013`           |
| `%A, %B %e, %Y` | `Sunday, June 5, 2013` |
| `%b %e %a`      | `Jun 5 Sun`            |

#### Time

| Example         | Output                 |
| ---             | ---                    |
| `%H:%M`         | `23:05`                |
| `%I:%M %p`      | `11:05 PM`             |

This is a basic table with h4's.

### Shortcuts

| `V` | Vector |
| `P` | Pencil |
| `T` | Text |
| `L` | Line |
| `R` | Rectangle |
| `O` | Oval |
| `U` | Rounded |
{: .-shortcuts}

Add `{: .-shortcuts}` to tables.

### With headers

| Prefix | Example               | What     |
| ---    | ---                   | ---      |
| `//`   | `//hr[@class='edge']` | Anywhere |
| `./`   | `./a`                 | Relative |
| `/`    | `/html/body/div`      | Root     |
{: .-headers}

Add `{: .-headers}` to add headers.

## Two columns

### One

```
···
```

### Two

```
···
```

## Left reference
{: .-left-reference}

### One

```
···
···
···
···
···
···
···
···
```

### Two

```
···
```

### Three

```
···
```

## One column
{: .-one-column}

### One

```
···
```