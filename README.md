# Modello LaTeX per il Research Project

## Benvenuti ai contributi

Ogni modifica e miglioramento è benvenuto. Sentitevi liberi di fare un fork
del repository, apportare le vostre modifiche e aprire una pull request (PR).

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

## Images

Lasciare tutte le immagini usate dal documento nella cartella
[`images/`](images/). Non spostare o rinominare il logo senza aggiornare il
percorso nel modello.

Il logo attualmente usato nell'intestazione è
[`images/logounict.png`](images/logounict.png). Anche eventuali nuove
immagini devono essere referenziate con il percorso relativo corretto, ad
esempio:

```latex
\includegraphics[width=0.8\textwidth]{images/nome-immagine.png}
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
- [`images/`](images/): immagini del documento;
- [`main.pdf`](main.pdf): versione PDF del modello.

## English instructions

This repository contains a **template** for the PhD research project. The
official call for applications always takes precedence over this template.

### Important: follow the official call

Before submitting the document, carefully check the current official call for
applications and comply with all its requirements, including the requested
sections, order, character limits, content, formatting, deadlines, and
submission procedures.

### Using the template

Replace the placeholders in [`main.tex`](main.tex), such as
`Firstname Lastname`, `NNNN`, and `Insert text...`. Replace the example
bibliographic entries with relevant and verifiable sources.

Before submitting the final document, remove all user guidance and the
corresponding commands:

- `\limit{...}` and the text inside the parentheses;
- `\instruction{...}` and the explanatory text shown in red.

These elements are only editing instructions and must not appear in the final
version.

### Images

Keep all images used by the document inside the
[`images/`](images/) folder. Do not move or rename the logo without
updating its relative path in the template.

The current header logo is
[`images/logounict.png`](images/logounict.png). Any additional image should
also be referenced using a relative path, for example:

```latex
\includegraphics[width=0.8\textwidth]{images/image-name.png}
```

### Bibliography

The bibliography is stored in [`bibfileTemplate.bib`](bibfileTemplate.bib).
Replace the example entries with relevant and verifiable references and cite
them in the text using:

```latex
\cite{entry-key}
```

The final bibliography must comply with the limits and requirements specified
in the official call.
