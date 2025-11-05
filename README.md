## Overview

This template provides a minimal but robust setup for right-to-left (RTL) Hebrew slides, while remaining compatible with English text, math, and standard Beamer features.

It uses:

- [`babel`](https://ctan.org/pkg/babel) for proper Hebrew language and bidirectional (bidi) text support  
- [`fontspec`](https://ctan.org/pkg/fontspec) for OpenType font selection  
- [`beamer`](https://ctan.org/pkg/beamer) as the base presentation class  
- A separate `config.tex` for easy customization (fonts, colors, and theme settings)  
- Optional `logo.png` for institutional branding  

---

## Files

| File | Description |
|------|--------------|
| `EX00.tex` | Main presentation source file (acts as entry point) |
| `EX00D.tex` | Example deck or Hebrew/English variant |
| `config.tex` | Contains theme configuration, color setup, and font definitions |
| `logo.png` | Logo used in the title slide (optional) |

---

## Key Packages

### `babel`
Handles bidirectional Hebrew text, punctuation mirroring, and RTL alignment automatically.  
It replaces older `bidi` and `polyglossia` stacks and works seamlessly with `luatex` and `xelatex`.

Example usage:
```latex
\usepackage[hebrew,english]{babel}
\selectlanguage{hebrew}
