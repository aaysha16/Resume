# Resume

A professional resume written in LaTeX, auto-compiled to PDF via GitHub Actions.

## 📄 Download Latest PDF

The compiled PDF is automatically generated on every push to `main` and is available under [**Releases → Latest Resume**](../../releases/latest).

## 🛠️ How It Works

1. Edit [`resume.tex`](./resume.tex) with your details.
2. Commit and push to `main`.
3. GitHub Actions automatically compiles the `.tex` file using [Tectonic](https://tectonic-typesetting.github.io/) and:
   - Uploads the PDF as a **build artifact** (retained for 90 days).
   - Publishes the PDF to the **latest GitHub Release**.

## 📁 Repository Structure

```
Resume/
├── .github/
│   └── workflows/
│       └── build.yml      # GitHub Actions workflow (LaTeX → PDF)
├── resume.tex             # LaTeX source file
└── README.md
```

## 🔧 Local Build (Optional)

If you have a LaTeX distribution installed locally (e.g., TeX Live or MiKTeX):

```bash
pdflatex resume.tex
```

Or using Tectonic:

```bash
tectonic resume.tex
```

## 📝 Template

This resume uses the **Jake's Resume** LaTeX template style — ATS-friendly, clean, and professional.

---

> Built with ❤️ using LaTeX + GitHub Actions
