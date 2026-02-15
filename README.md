# Kaushik Goswami — Resume (LaTeX)

📄 **[View Resume (PDF)](./Kaushik-Goswami-Resume.pdf)**

This repository contains my **latest professional resume**, authored in **LaTeX** and compiled to PDF.  
The resume is **ATS-friendly**, machine-readable, and optimized for **Frontend / Full-Stack Engineering roles**.

LaTeX dependencies are managed at the **system level via TeX Live**.  
This project does **not** use npm, Node.js, or any JavaScript-based tooling.

---

# Kaushik Goswami — LaTeX Resume

This repository contains the source code for my ATS-optimized resume built using LaTeX.
The resume is written in a `.tex` file and compiled into a PDF using the LaTeX typesetting engine.

## Tech Stack

- LaTeX (Article class)
- TeX Live distribution
- `pdflatex` (compiler)
- `latexmk` (build automation)

## Prerequisites (Linux / Ubuntu)

Install required dependencies:

```bash
sudo apt update
sudo apt install latexmk texlive-latex-extra texlive-fonts-extra texlive-extra-utils
```

## Development (Live Preview Mode)

Start continuous compilation (watch mode):

```bash
latexmk -pdf -pvc Kaushik-Goswami-Resume.tex
```

This will automatically recompile the PDF every time the `.tex` file is saved.

Open the generated PDF:

```bash
xdg-open Kaushik-Goswami-Resume.pdf
```

Now any edit to the resume will immediately reflect in the PDF after saving.

## Production Build (Generate Final PDF)

To generate the final resume:

```bash
latexmk -pdf Kaushik-Goswami-Resume.tex
```

Output file:

```
Kaushik-Goswami-Resume.pdf
```

## Cleaning Build Files

Remove temporary compilation files (keeps the PDF):

```bash
latexmk -c
```

Remove all generated files including the PDF:

```bash
latexmk -C
```

## How It Works

1. The `.tex` file is the source code of the resume.
2. The LaTeX engine (`pdflatex`) compiles it into a PDF.
3. `latexmk` automatically runs multiple compilation passes required for:
   - hyperlinks
   - bookmarks
   - page references

This ensures consistent layout and ATS-readable output across different systems.

## Editing

All resume content is located in:

```
Kaushik-Goswami-Resume.tex
```

Edit the file, save, and the PDF will regenerate automatically in development mode.
