# NoStyle
---
*Notion-Style is now deprecated since it does not use the same Enviroments*

Custom clean LaTeX style package with a Notion-inspired aesthetic. Built on Fira Sans and Fira Mono.

---

## Commands

| Command | Description |
|---|---|
| `\thinrule` | Thin horizontal divider line |
| `\Svspace` | Small vertical space (6pt) |
| `\Mvspace` | Medium vertical space (2ex) |
| `\Lvspace` | Large vertical space (6ex) |
| `\used{text}` | Inline badge in a tinted box |

---

## Environments

### `Ncode` — Code Block

Properly Stylized Syntax-highlighted code block (listing would work but will not be stylized by default)

```latex
\begin{Ncode}{Rust}
fn main() {
    println!("hello");
}
\end{Ncode}
```


---

### `Nquote` — Block Quote

a Left bordered quote block (useful for way more than just quotes)

```latex
\begin{Nquote}
This is a quoted passage
\end{Nquote}
```

---

### `Nbox` — Centered Box

a Stylized callout Box

```latex
\begin{Nbox}
Important note here.
\end{Nbox}
```

---

## Tables

Tables use `tabu` with globally changed spacing (do me a favor and use tabu even if its not sustained anymore)

```latex
\begin{tabu}{|X|X|X|}
    \hline
    Header 1 & Header 2 & Header 3 \\
    \hline
    Cell A & Cell B & Cell C \\
    \hline
\end{tabu}
```

`X` columns stretch to fill available width automatically. Prefer `tabu` over `tabular` throughout.

---

## Math

`|` is redefined as a relation symbol in math mode, so you can write:

```latex
\[ A | B \]
```

instead of `\mid`. Display spacing is also tightened globally (`abovedisplayskip`, `belowdisplayskip`).

---

## Typography & Layout

- **Font:** Fira Sans Light (`sfdefault`) for body text, Fira Mono for code
- **Layout:** A4, 20mm left and top margin, `\raggedright` globally
- **Subsections** as well as **sections** are stylized globally
- **Section spacing** is tightened via `\titlespacing`

---

## Colors

### UI

| Name | Hex | Usage |
|---|---|---|
| `black` | `#212529` | Default text |
| `gray` | `#6C757D` | Subsection headings, accents |
| `lightgray` | `#ADB5BD` | Rules, borders, line numbers |
| `tintedwhite` | `#F8F9FA` | Badge backgrounds, box borders |

### Code

| Name | Hex | Usage |
|---|---|---|
| `codeDark` | `#252422` | Default code text |
| `codeSemidark` | `#403D39` | Identifiers |
| `codeSemilight` | `#CCC5B9` | Comments |
| `codeLight` | `#FFFCF2` | not in use for now ._. |
| `codeAccent` | `#EB5E28` | Keywords |
| `codeSemiaccent` | `#D98E71` | Strings |
