# Notion Style:
| **Type** | **Command / Environment** | **Purpose** | **Style & Value** |
|-----------|----------------------------|--------------|-------------------|
| **Environment** | `quoteB` | Creates the main definition or quote block. | Features a left vertical sidebar (using lightgray) and custom paragraph spacing. |
| **Command** | `\thinrule` | Inserts the standard horizontal separator. | Thin (0.2pt) line using the gray color, preceded and followed by `\mvspace`. |
| **Length** | `\svspace` | Small Vertical Space (S) | Defined as 3pt. Used for paragraph separation within `quoteB` and manual small gaps. |
| **Length** | `\mvspace` | Medium Vertical Space (M) | Defined as 2ex. Used around the `\thinrule`. |
| **Length** | `\lvspace` | Large Vertical Space (L) | Defined as 6ex. Available for larger manual section breaks. |
