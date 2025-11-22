# Vorlagen – LaTeX Project



## 📂 Projektstruktur

```
Vorlage-book/
├── bib/                 # Zentrale Bibliographie (DE/EN)
│   └── literatur.bib
│
├── de/                  # Deutsche Version
│   ├── main.tex
│   ├── chapters/
│   ├── appendix/
│   ├── bilder/
│   └── cover/
│
├── en/                  # Englische Version
│   ├── main.tex
│   ├── chapters/
│   ├── appendix/
│   ├── bilder/
│   └── cover/
│
└── styles/              # Globale Styles & Makros
    ├── print.de.sty
    ├── print.en.sty

Vorlage-paper/
├── bib/
│   └── literatur.bib
│
├── de/                  # Deutsche Version
│   ├── main.tex
│   ├── captures/
│   └── figures/
│
├── en/                  # Englische Version
│   ├── compton_en.tex
│   ├── captures/
│   └── figures/
│
└── styles/
    ├── paper-style-de.sty
    └── paper-style-en.sty

```

## 📖 Kompilieren

### 1. Deutsche Version
```
cd de
pdflatex main.tex


```
### 2. Englische Version
```
cd en
main_eng.tex
```

👉 In **TeXstudio** reicht es, `main.tex` zu kompilieren, wenn folgende Einstellungen aktiv sind:
- Bibliographie-Tool: **Biber**
- Index-Tool: **MakeIndex** oder **Xindy** (empfohlen für Umlaute)
- "Erzeugen & Ansicht" → Standard: `pdflatex → biber → makeindex → pdflatex ×2`

## 📚 Literatur
```
bib/literatur.bib


```
## 🔤 Index

```
\printindex[myindex]

```
- Ignoriere temporäre Index-Dateien in `.gitignore`:
  ```
 *.aux
*.log
*.bbl
*.blg
*.toc
*.idx
*.ind
*.ilg
*.out
*.pdf

  ```

## 🗂️ GitHub-Hinweise

- Temporäre LaTeX-Dateien (aux, log, bbl, blg, toc, pdf …) sind in `.gitignore`.
- Im Repo liegen nur die **Quellen** (Tex, Bib, Bilder, Styles).
- PDFs werden lokal erzeugt, nicht im Repo gespeichert.

---

✍️ **Autor:** Christian Weilharter, Dipl.-Ing. (FH)  
📅 Stand: Oktober 2025

- 🌐 Website: [https://mathandphysics.de](https://mathandphysics.de)
