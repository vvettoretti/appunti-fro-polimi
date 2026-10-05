# Appunti di Fondamenti di Ricerca Operativa (A.A. 2026/27)

Appunti in LaTeX del corso della Prof. Marta Pascoal (Politecnico di Milano).

**PDF aggiornati:** sezione *Releases* del repository. L'ultima release contiene sempre la versione corrente di:
- `appunti_FRO.pdf`: la teoria delle lezioni;
- `esercitazioni_FRO.pdf`: le esercitazioni con le soluzioni.

## Struttura
```
preambolo.tex               preambolo comune (pacchetti, box, macro)
lezioni/
  appunti_FRO.tex           documento principale degli appunti
  cap0_info.tex             corso, esame, quesiti brevi
  cap1_intro.tex            introduzione alla Ricerca Operativa
  cap2_modelli.tex          modelli di Programmazione Lineare
  cap3_complessita.tex      cenni di complessità computazionale
  cap4_pl.tex               PL: forme, geometria, teorema fondamentale
  cap5_quiz.tex             allenamento V/F per i quesiti brevi
  cap6_riepilogo.tex        formulario
esercitazioni/
  esercitazioni_FRO.tex     documento principale delle esercitazioni
  es01_modelli.tex          Esercitazione 1: modelli
```

## Compilare in locale
```
cd lezioni && latexmk appunti_FRO.tex
cd esercitazioni && latexmk esercitazioni_FRO.tex
```

## Release automatiche
A ogni push su `main` che modifica un `.tex`, la GitHub Action `.github/workflows/build-release.yml`
compila entrambi i PDF e crea una release con tag `vAAAA.MM.GG-N`, allegando i PDF e l'elenco dei commit inclusi.
Si può lanciare anche a mano da *Actions → Build e release appunti → Run workflow*.
