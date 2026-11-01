# Statistica Economica con R, Python e SAS (VERSIONE IN BOZZA DI PROVA)

Edizione online, bilingue (italiano/inglese), del volume *Statistica Economica con R* di Erasmo Vassallo, con gli esempi in **R**, **Python** e **SAS**.

Sito: https://erasmovassallo.github.io/statistica-economica/

## Struttura

```
_quarto.yml                 configurazione del sito (menu, lingue, stile)
index.qmd                   home (inglese)
preface.qmd                 prefazione (inglese)
chapters/                   capitoli in inglese
it/                         versione italiana (home, prefazione, capitoli/)
data/                       file di dati usati nel testo
images/                     figure statiche
assets/sas.xml              evidenziazione della sintassi SAS
styles.css                  stile
.github/workflows/          pubblicazione automatica su GitHub Pages
```

## Aggiungere un capitolo (solo per analisi interna... da rimuovere...)

1. Creare `it/capitoli/02-....qmd` e `chapters/02-....qmd` (copiare la struttura del capitolo 1).
2. Aggiungerli alle due barre laterali in `_quarto.yml`.
3. Ogni esempio va in un blocco a schede:

   ````markdown
   ::: {.panel-tabset group="language"}
   ### R
   ```{r}
   ...
   ```
   ### Python
   ```{python}
   ...
   ```
   ### SAS
   ```sas
   ...
   ```
   :::
   ````

   Il codice R e Python (blocchi `{r}` e `{python}`) viene eseguito; il codice SAS (blocchi `sas`, senza graffe) viene solo mostrato.

