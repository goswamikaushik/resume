# 📄 LaTeX Resume Template

📄 **[View Resume (PDF)](./Kaushik-Goswami-Resume.pdf)**

A clean, professional resume template built using LaTeX. This repository is designed to help developers manage their resumes with version control, separation of content and styling, and automated builds.

This is the repository I use to manage my own resume, and it's structured so that **any developer can fork, customize, and compile their own version in minutes**.

---

## ✨ Features

- **Machine-Readable:** Uses standard fonts and mappings (`glyphtounicode`) so text can be copied and parsed easily. You can verify your output using checkers like the [FAANG Tech Leads Resume Review](https://www.faangtechleads.com/resume/review).
- **Live Preview (Watch Mode):** Recompiles automatically on save so you can see your changes instantly.
- **Version Controlled:** Treat your resume like code—track changes, create branches, and maintain a history of your career growth.
- **Separation of Concerns:** Content is managed via clean LaTeX markup, letting the engine handle page margins, alignment, and formatting automatically.

---

## 📁 File Structure & Output Naming

When you compile the LaTeX source, the output PDF automatically matches the filename of your `.tex` source file:
- **Source File:** `Your-Name-Resume.tex` ➡️ **Output PDF:** `Your-Name-Resume.pdf`

To customize this template for yourself:
1. **Rename** the source file from `Kaushik-Goswami-Resume.tex` to your preferred filename (e.g., `Jane-Smith-Resume.tex`).
2. Run the compile command targeting your new file name.
3. The generated PDF will automatically match the name of your `.tex` file.

---

## 🚀 Getting Started

### 1. Prerequisites

You need a LaTeX distribution installed on your system.

#### **Linux (Ubuntu/Debian)**
Install the required TeX Live packages:
```bash
sudo apt update
sudo apt install latexmk texlive-latex-extra texlive-fonts-extra texlive-extra-utils
```

#### **macOS**
Install MacTeX using Homebrew:
```bash
brew install --cask mactex-no-gui
# Or for the full suite: brew install --cask mactex
```

#### **Windows**
Install [MiKTeX](https://miktex.org/) or use [WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install) to run the Linux commands.

---

### 2. Live Development (Watch Mode)

To start continuous compilation where the PDF regenerates instantly whenever you save the `.tex` file, run:

```bash
latexmk -pdf -pvc <your-filename>.tex
```
*(For example: `latexmk -pdf -pvc Kaushik-Goswami-Resume.tex`)*

This starts a file watcher. Keep this terminal open while you edit!

---

### 3. Production Build

To compile a final, optimized production PDF without starting a file watcher:

```bash
latexmk -pdf <your-filename>.tex
```

---

### 4. Cleaning Build Artifacts

LaTeX compilation generates several auxiliary tracking files (`.aux`, `.log`, `.fls`, etc.). You can clean them up easily:

- **Remove temp files (keeps the PDF):**
  ```bash
  latexmk -c
  ```
- **Remove all generated files (including the PDF):**
  ```bash
  latexmk -C
  ```

---

## 🛠️ Customizing the Template

1. Open your renamed `.tex` file in any code editor (e.g., VS Code with the *LaTeX Workshop* extension).
2. Customize the contact details in the `\begin{header}` block.
3. Update your experience, education, and skills sections by modifying the corresponding `\section` blocks.
4. Save the file, and your new PDF will be generated immediately.

---

## 📬 Connect With Me

If you have any questions or want to connect, feel free to reach out!

- 💼 **LinkedIn:** [linkedin.com/in/goswamikaushik](https://www.linkedin.com/in/goswamikaushik/)
- 🌐 **Portfolio:** [goswamikaushik.dev](https://goswamikaushik.dev/)
- 🐙 **GitHub:** [github.com/goswamikaushik](https://github.com/goswamikaushik)

---
