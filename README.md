# Modello LaTeX per il Research Project

Questo repository contiene un **modello** per il progetto di ricerca del PhD.
Il file da compilare e modificare è [`main.tex`](main.tex), mentre
[`researchproject.sty`](researchproject.sty) contiene le impostazioni grafiche
comuni.

## IMPORTANTE: attenersi al bando

Questo è soltanto un modello tipografico e organizzativo. Il testo finale deve
rispettare integralmente il **bando ufficiale**: sezioni richieste, ordine,
limiti di caratteri, contenuti, formato, scadenze e modalità di presentazione.

Prima di consegnare il documento, verificare sempre il bando aggiornato e non
considerare il modello come sostitutivo delle istruzioni ufficiali.

## Come usare il modello

Sostituire in [`main.tex`](main.tex) i campi segnaposto, ad esempio:

- `Firstname Lastname`;
- `NNNN`;
- `Insert text...`;
- le citazioni bibliografiche di esempio.

Quando il testo è completo, cancellare dal file tutte le istruzioni destinate
all'utente e i relativi comandi:

- `\limit{...}` e il testo contenuto tra parentesi;
- `\instruction{...}` e il testo esplicativo in rosso.

Questi elementi servono solo come guida durante la compilazione del progetto e
non devono comparire nella versione finale.

## Immagini

Lasciare tutte le immagini usate dal documento nella cartella
[`Immagini/`](Immagini/). Non spostare o rinominare il logo senza aggiornare il
percorso nel modello.

Il logo attualmente usato nell'intestazione è
[`Immagini/logounict.png`](Immagini/logounict.png). Anche eventuali nuove
immagini devono essere referenziate con il percorso relativo corretto, ad
esempio:

```latex
\includegraphics[width=0.8\textwidth]{Immagini/nome-immagine.png}
```

## Bibliografia

Le voci bibliografiche sono contenute in
[`bibfileTemplate.bib`](bibfileTemplate.bib). Sostituire gli esempi con
riferimenti pertinenti e verificabili, quindi usare nel testo:

```latex
\cite{chiave-della-voce}
```

La bibliografia finale deve rispettare i limiti e i requisiti indicati dal
bando.

## File principali

- [`main.tex`](main.tex): testo e struttura del progetto;
- [`researchproject.sty`](researchproject.sty): stile, margini, intestazione e
  frontespizio;
- [`bibfileTemplate.bib`](bibfileTemplate.bib): bibliografia;
- [`Immagini/`](Immagini/): immagini del documento;
- [`main.pdf`](main.pdf): versione PDF del modello.
