# AI-PENTEST

**Inteligentný systém na automatizované testovanie bezpečnosti webových aplikácií pomocou veľkých jazykových modelov**

Tímový projekt v predmete *Metódy inžinierskej práce*, FIIT STU, ak. rok 2026/27.

Tím: Kyrylo Bukhanets, Artur Toba, Maksym Tomkevych, Andrii Tsybulskyi

## Štruktúra repozitára

```
.
├── zameranie/            Zameranie projektu (názov, akronym, anotácia)
│   ├── zameranie.tex
│   └── zameranie.pdf
├── clanok/               Prehľadový článok
│   ├── clanok.tex
│   ├── clanok.pdf
│   ├── literatura.bib    Bibliografia (BibTeX), spoločná aj pre formulár VV-F
│   └── obrazky/          Diagramy – zdroj (.dot, .uxf) aj export (.pdf)
├── formulare/            Žiadosť pre aplikovaný výskum (podľa vzoru APVV VV 2024)
│   ├── vv-a-e.tex/.pdf   Formulár VV-A až VV-E
│   └── vv-f.tex/.pdf     Formulár VV-F – vecný zámer projektu
├── jira/                 Export z Jira (úlohy, snímky backlogu a boardu)
└── git_log.txt           História commitov (git log)
```

## Odovzdania

| Časť | Termín | Súbory |
|---|---|---|
| Zameranie projektu | 4. 10. 2026 | `zameranie/` |
| Predbežná verzia projektu | 1. 11. 2026 | `formulare/`, `clanok/` |
| Slajdy prezentácie | najneskôr 29. 11. 2026 | – |
| Projekt a jeho súčasti | 12. 12. 2026 | – |

## Preklad do PDF

Potrebná je distribúcia LaTeX (MiKTeX alebo TeX Live) s nástrojom `latexmk`.

```bash
cd clanok && latexmk -pdf clanok.tex
cd formulare && latexmk -pdf vv-a-e.tex && latexmk -pdf vv-f.tex
cd zameranie && latexmk -pdf zameranie.tex
```

## Riadenie projektu

Úlohy sa evidujú v Jira (projekt `MIP`, Scrum). Každý commit začína kľúčom úlohy, napr.
`MIP-3 Prehlad tradicnych nastrojov automatizovaneho testovania`. Podrobnosti sú v [`jira/README.md`](jira/README.md).
