---
id: Make Files
aliases: []
tags: []
---


Make files control the order a project is compiled, and defines the dependencies of each file

# Comprises:
- Targets
    - The files to be "created" 
- Dependencies
    - The files that each target depends on
- Process
    - How to "create" each target and bring it up to date

E.G.:

```lang-makefile
test1:test2
    echo "Creating test1"
    touch test1

test2:
    echo "Creating test2"
    touch test2

filename=INFO1111_Group_Project_CC99-01
bibfile=main.bib

pdf:${filename}.pdf
    echo
    echo "PDF files now up to date"

${filename}.pdf: ${filename}.tex ${bibfile}
    pdflatex ${filename}
    bibtex ${filename}
    pdflatex ${filename}
    pdflatex ${filename}
    echo
    echo ${filename} "has been updated"

${filename}.bib:

${filename}.tex:

clean:
    rm -rf ${filename}.*
```
