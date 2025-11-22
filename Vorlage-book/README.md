Vorlage-book/
```
├── bib/                 # Zentrale Literaturdatenbank (BibLaTeX)
│   └── literatur.bib
│
├── de/                  # Deutsche Version
│   ├── main.tex         # Hauptdatei (Deutsch)
│   ├── chapters/        # Kapitel
│   ├── appendix/        # Anhänge
│   ├── bilder/          # Abbildungen
│   └── cover/           # Cover-Elemente
│
├── en/                  # English version
│   ├── main.tex
│   ├── chapters/
│   ├── appendix/
│   ├── bilder/
│   └── cover/
│
└── styles/              # Globale Styles & Makros
    ├── print.de.sty     # Style für deutsche Ausgabe
    ├── print.en.sty     # Style für englische Ausgabe
```
cd de
pdflatex main.tex
