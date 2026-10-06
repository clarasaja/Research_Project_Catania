# Research Project LaTeX Template

Modello LaTeX per il progetto di ricerca del PhD. Il documento principale è
[`main.tex`](main.tex), mentre la grafica comune è contenuta nella classe di
supporto [`researchproject.sty`](researchproject.sty).

## Requisiti

È necessario avere una distribuzione LaTeX installata, ad esempio:

- MacTeX su macOS;
- TeX Live su Linux;
- MiKTeX su Windows.

Il progetto usa `pdflatex` e `bibtex`.

## Compilazione da Terminale

Aprire il Terminale nella cartella del progetto ed eseguire:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
bibtex main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

Il risultato è il file [`main.pdf`](main.pdf).

La sequenza va ripetuta quando si modificano le citazioni, il testo o il file
[`bibfileTemplate.bib`](bibfileTemplate.bib).

## Compilazione in Visual Studio Code

Aprire `main.tex` in Visual Studio Code con l'estensione **LaTeX Workshop** e
avviare la ricetta di compilazione `pdflatex -> bibtex -> pdflatex -> pdflatex`.

## Struttura del progetto

- [`main.tex`](main.tex): testo e struttura del documento;
- [`researchproject.sty`](researchproject.sty): margini, font, intestazione,
  logo e stile del frontespizio;
- [`bibfileTemplate.bib`](bibfileTemplate.bib): riferimenti bibliografici;
- [`Immagini/logounict.png`](Immagini/logounict.png): logo ripetuto
  nell'intestazione;
- `main.pdf`: PDF compilato.

Per aggiungere una fonte bibliografica, inserire una nuova voce nel file `.bib`
e citarla nel testo con `\cite{chiave}`.

## Pulizia dei file temporanei

I file `.aux`, `.bbl`, `.blg`, `.log` e `.out` sono generati durante la
compilazione e non devono essere modificati manualmente. Per rimuoverli:

```bash
rm -f main.aux main.bbl main.blg main.log main.out
```
