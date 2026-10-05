# Appunti di Fondamenti di Ricerca Operativa (A.A. 2026/27)

Appunti in LaTeX del corso della Prof. Marta Pascoal (Politecnico di Milano).

**PDF aggiornato:** sezione *Releases* del repository (l'ultima release è sempre la versione corrente).

## Struttura
| File | Contenuto |
|---|---|
| `appunti_FRO.tex` | documento principale (preambolo, include i capitoli) |
| `cap0_info.tex` | informazioni su corso, esame e quesiti brevi |
| `cap1_intro.tex` | introduzione alla Ricerca Operativa |
| `cap2_modelli.tex` | modelli di Programmazione Lineare |
| `cap3_complessita.tex` | cenni di complessità computazionale |
| `cap3b_pl.tex` | PL: forme, geometria, teorema fondamentale |
| `cap4_esercitazione.tex` | Esercitazione 1 con soluzioni |
| `cap5_quiz.tex` | allenamento V/F per i quesiti brevi |
| `cap5_riepilogo.tex` | formulario |

## Compilare in locale
```
latexmk appunti_FRO.tex
```

## Release automatiche
A ogni push su `main` che modifica un `.tex`, la GitHub Action `.github/workflows/build-release.yml`
compila il PDF e crea una release con tag `vAAAA.MM.GG-N`, allegando il PDF e l'elenco dei commit inclusi.
Si può lanciare anche a mano da *Actions → Build e release appunti → Run workflow*.
