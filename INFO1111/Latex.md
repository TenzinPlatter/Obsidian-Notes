---
id: Latex
aliases: []
tags: []
---

- LaTeX is a typesetting program based on TeX
- Uses "high level" macros based on TeX functionality
- Uses markup tags to apply formatting (same as in markdown files)

Created by Donald Knuth so that anyone could produce high quality text from anything and so that any system could give the exact same results.

LaTeX can be considered a case study of software development because of its:
- Well documented changes
- Version Control
- Collaboration with the public
    - Paid anyone who could find a bug

Used extensively in academic writings, but not in industry due to its steep learning curve, and in
industry it is not worth making all employees learn it. Although it is sometimes used professionally 
by mathematicians, physicists and computer scientists.

- Forces writer to focus on content, rather than presentation
- Is very good at equations, layout, bibliographies
- Encapsulates a number of key computing concepts
    - Requires Compilation
    - Separation of concerns
- Free and open source


Latex can be compiled to pdf using the following commands:
$ pdflatex yourfile.tex
$ bibtex yourfile.tex
$ pdflatex yourfile.tex
$ pdflatex yourfile.tex
