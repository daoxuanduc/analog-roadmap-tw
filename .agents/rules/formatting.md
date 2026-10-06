# Formatting & Style Guidelines

## 1. No LaTeX Math Syntax
- DO NOT use LaTeX math delimiters (such as `$formula$` or `$$formula$$`) in chat responses or markdown notes.
- The IDE chat interface does not render MathJax/KaTeX, resulting in raw unparsed LaTeX text like `$I_D \propto (V_{GS}-V_{th})^2$`.

## 2. Preferred Notation Styles
- **Formulas & Multi-line Equations:** Use fenced code blocks (` ```text `) with standard ASCII and Unicode characters (e.g. `μ_n`, `C_ox`, `(W/L)`, `²`, `√`, `||`).
  ```text
  I_D = (1/2) * μ_n * C_ox * (W/L) * (V_GS - V_th)²
  Av  = -G_m * R_out = -g_m * (r_oN || r_oP)
  ```
- **Inline Variables & Parameters:** Use inline backticks (e.g. `V_GS`, `V_th`, `V_DS`, `I_D`, `g_m`, `r_o`, `C_L`, `PM ≥ 60°`, `I_SS = 100 μA`).
- **Comparisons & Summaries:** Use clean Markdown tables.
