+++
title = "Markdown examples"
date = 2023-01-31
updated = 2023-07-08
description = "This post showcases some examples of Markdown formatting, including a table, code blocks and tags, quotes, tables, and footnotes."

[taxonomies]
tags = ["markdown", "showcase"]

[extra]
katex = true
+++

## $\KaTeX$

[$\KaTeX$](https://katex.org/) is a fast and easy-to-use library that enables the rendering of mathematical notation, using LaTeX syntax.

You can use $\KaTeX$ **inline** by wrapping the expression between `$` or between `\\(` and `\\)`.

For example, `$ \sin(x) = \sum_{n=0}^{\infty} \frac{(-1)^n}{(2n + 1)!} x^{2n + 1} $` would render: $ \sin(x) = \sum_{n=0}^{\infty} \frac{(-1)^n}{(2n + 1)!} x^{2n + 1} $

To display the expression **on its own line and centered**, wrap it around `$$` or between `\\[` and `\\]`.

For example, `\\[ r = \frac{\sum_{i=1}^{n}(x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum_{i=1}^{n}(x_i - \bar{x})^2}\sqrt{\sum_{i=1}^{n}(y_i - \bar{y})^2}} \\]` renders: \\[ r = \frac{\sum_{i=1}^{n}(x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum_{i=1}^{n}(x_i - \bar{x})^2}\sqrt{\sum_{i=1}^{n}(y_i - \bar{y})^2}} \\]

To activate $\KaTeX$ for a post, include `katex = true` within the `[extra]` section of the post's front matter. For exemple:

```toml,hl_lines=5-6
+++
title = "Testing KaTeX"
date = 2002-11-30

[extra]
katex = true
+++
```

For enhanced performance and security, the $\KaTeX$ JavaScript, CSS, and fonts are hosted locally.

**Note**: After enabling $\KaTeX$, if you want to use \$ without rendering a mathematical expression, escape it with a single backslash: `\$`.

## Table

Here's an example of a table[^1]. Its colours change depending on the current theme.

| Symbol  | Element | Atomic Number |
|---------|---------|---------------|
| H       | Hydrogen| 1             |
| C       | Carbon  | 6             |
| Fe      | Iron    | 26            |
| Au      | Gold    | 79            |

## Code Block

```rust
fn main() {
    println!("Hello, world!") -> ();
}
```

## Code tags

Lorem ipsum `dolor` sit amet, `consectetur adipiscing` elit.
`Lorem ipsum dolor sit amet, consectetur adipiscing elit.`

## Quote

> "We're all hurtling towards death. Yet here we are, for the moment, alive. Each of us knowing we're going to die. Each of us secretly believing we won't."
>
> — Charlie Kaufman, Synecdoche, New York


[^1]: And here's an example of a footnote!
