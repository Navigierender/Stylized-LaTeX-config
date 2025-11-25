# Notion Style:
| Type          | Command / Environment | Purpose                         | Style & Key Features |
|---------------|------------------------|---------------------------------|-----------------------|
| Environment   | `quoteB`               | Creates a block quote or definition box. | Features a light-gray vertical line on the left boundary (borderline west). Uses custom vertical spacing (`\Mvspace`) for clean paragraphs. |
| Environment   | `Nbox`                 | Creates a rounded, distinct container box. | Styled with rounded corners (`arc=2ex`), a light gray frame (`tintedwhite`), and centered text alignment. Useful for callouts or quick notes. |
| Command       | `\thinrule`            | Inserts a horizontal separator. | A very thin (0.2pt) horizontal rule in lightgray, surrounded by medium spacing (`\Mvspace`). |
| Length        | `\Svspace`             | Small Vertical Space            | A dedicated small space command (`\vspace{6pt}`) for fine-tuning vertical alignment. |
| Length        | `\Mvspace`             | Medium Vertical Space           | A medium space command (`\vspace{2ex}`) primarily used around `\thinrule` and within environments like `quoteB`. |
| Length        | `\Lvspace`             | Large Vertical Space            | A large space command (`\vspace{6ex}`) for significant manual section breaks. |
| Global Style  | Font & Typeface        | Sets the default font.          | Uses the Fira Sans typeface (`sfdefault`) in its light variant. Numbering uses old-style figures (`\oldstylenums`). |
| Global Style  | Page Geometry          | Sets the page margins.          | A4 paper with equal 20mm margins (left and top margins explicitly set). |
| Global Style  | Colors                 | Defines custom colors.          | Defines `black` (212529), `gray` (6C757D), `lightgray` (ADB5BD), and `tintedwhite` (F8F9FA). |
| Global Style  | Spacing                | Display math spacing.           | Reduces vertical space above and below displayed equations (`\abovedisplayskip`, `\belowdisplayskip`) for a tighter look. |
! Use Tabu rather than tabular since Tabular isnt changed using this Style !
