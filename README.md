# PISA: family, school and the score gap

An interactive project based on six PISA student studies (KSE), featuring a research dashboard and a 20-question school quiz.

## Open the project

- **[Open the PISA research website](https://vladyslavrak25-ship-it.github.io/PISA/)**
- **[Play the interactive school quiz](https://vladyslavrak25-ship-it.github.io/PISA/game.html)**

Both links open the live pages, not the source code.

## What is on the page

- **The Q4−Q1 gap** for Ukraine, Estonia, Czechia, Poland and Brazil, with the shares of students at levels 2 and 5+.
- **Two independent studies, the same result**: a comparison of Study 1.1 and the 11-country EU report for Estonia, Czechia and Poland.
- **What the gap is made of: family or school** (new). A calculation based on the coefficients of Study 1.1.
- **A desegregation simulator** that uses real coefficients instead of made-up weights.
- **What matters: education, occupation or possessions at home** (new). A country comparison of HISEI, PAREDINT and HOMEPOS.
- **Where Ukraine sits on the scale** (new). R² for 14 countries, with caveats about the data.
- What the studies have in common and where they disagree; a table of sources.

## Interactive school quiz

**What Kind of School Would You Attend?** is a 20-question game about family resources, school choice, and who you study with. Its scores and outcomes are illustrative, not predictions or empirical measurements for individuals.

## Sources

| Study | Data |
|---|---|
| 1.1 (Lynnyk Olha) | Estonia, Czechia, Poland, Brazil, PISA 2025, math |
| 1.2 (Polina Sakhno) | Student ambition, science (text only) |
| 1.3 | Ukraine, 7,105 students, cycle not confirmed |
| 1.4 (Katya) | Research plan for Ukraine, no results |
| 1.5 | Georgia, PISA 2022 |
| 11-country EU report | PISA 2025, science, academic selection |

## How the gap split is calculated

```
SD in points  = gap ÷ d
own part      = 2 × β_own × 1.271 × SD
school part   = 2 × β_school × 1.271 × √ICC(ESCS) × SD
remainder     = gap − own − school
```

This is the page's own calculation, not a result of the studies themselves. It assumes roughly normal ESCS and that the link to school composition is causal; in reality these are only associations.

## Publishing

Settings → Pages → Deploy from a branch → `main` / root.
