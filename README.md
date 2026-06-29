# Professional Resume Portfolio

This repository contains the professional resume source code for **Aaysha Ali**, formatted in LaTeX and automatically compiled to a publication-quality PDF via GitHub Actions.

---

## 📄 Download Latest PDF

The compiled, ATS-friendly resume PDF is automatically generated on every push to the `main` branch. 

* [**Download Compiled Resume (PDF)**](../../releases/latest/download/resume.pdf)

---

## 🛠️ Automated CI/CD Compilation

The repository utilizes a GitHub Actions workflow to build and publish the resume:
1. **Source Update:** Modify [`resume.tex`](./resume.tex) to update professional details.
2. **Auto-Compile:** Upon pushing commits to `main`, GitHub Actions triggers a build using the [Tectonic](https://tectonic-typesetting.github.io/) LaTeX engine.
3. **Release Publication:** The compiled PDF is uploaded as a build artifact and automatically published to the [latest repository release](../../releases/latest).

---

## 📁 Repository Structure

```
├── .github/
│   └── workflows/
│       └── build.yml      # CI/CD compilation pipeline
├── README.md
└── resume.tex             # LaTeX resume source file
```

---

## 🔧 Local Compilation (Optional)

To compile the LaTeX source code locally, execute one of the following commands in the root directory:

### Using Tectonic (Recommended)
```bash
tectonic resume.tex
```

### Using PDFLaTeX (TeX Live / MikTeX)
```bash
pdflatex resume.tex
```
