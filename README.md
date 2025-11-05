# Hebrew LaTeX Template

A minimal LaTeX setup for writing Hebrew (RTL) documents with proper directionality, modern fonts, and compatibility with both Hebrew and English text.

---

## Overview

This template provides a clean and stable baseline for Hebrew LaTeX projects — articles, reports, or coursework — that mix Hebrew and English text.  
It is based on a modern toolchain supporting OpenType fonts, proper punctuation mirroring, and Unicode input.

It uses:

- [`babel`](https://ctan.org/pkg/babel) for Hebrew language support and bidirectional typesetting  
- [`fontspec`](https://ctan.org/pkg/fontspec) for OpenType fonts  
- [`polyglossia`](https://ctan.org/pkg/polyglossia) as an alternative for XeLaTeX users  

---

### Compile using

```bash
xelatex -interaction=nonstopmode "EX00.tex"
```

---

## Key Packages
babel

babel provides full Hebrew support including right-to-left directionality, punctuation mirroring, and localized captions.

For short English text inside Hebrew paragraphs, use:

```
\textenglish{This text is left-to-right.}
```

Note that it is also recommended to wrap Tikz illustrations and Algorithm environments with these commands for consistency across documents.
