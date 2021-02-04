---
layout: page
title: "Formattazione testo"
permalink: /istruzioni
redirect_from: ["/markdown", "/sintassi", "/formattazione", "/guida-formattazione", "/guida-sintassi"]
---
[Markdown: Guida Completa 2019](https://informaticabrutta.it/markdown-guida/)

## Guida Markdown

Ti dico subito come è strutturata questa guida. Questo argomento è abbastanza semplice e tecnico, non si presta a divagazioni varie e robe teoriche, quindi può essere tranquillamente espresso in modo rapido e asciutto.

Quello che troverai ora sarà una serie di sezioni in cui vedremo come fare cosa. In alcuni punti lascio aperte delle questioni per incoraggiare prove da parte tua.

### Ritorni a capo

In Markdown un ritorno a capo è dato lasciando una **riga vuota**.

Questo è il primo paragrafo. Questa linea non è un ritorno a capo. Questo, invece, è un altro paragrafo; quindi il ritorno c'è

### Intestazioni

Con intestazioni mi riferisco a quelli che in HTML sarebbero i vari tag `H`, quindi `H1-H7`.

In Markdown creiamo le intestazioni aggiungendo il carattere `#`.

    # H1
    ## H2
    ### H3
    #### H4
    ##### H5
    ###### H6

In alternativa, per gli `H1` e `H2` possiamo usare quest'altro formato:

    H1
    ===
    H2
    ---


### Enfasi

Possiamo formattare il testo usando i soli caratteri {`*`, `_`, `~`}.

    *Corsivo* e sempre _corsivo_.
    **Grassetto** e sempre __grassetto__.
    **Grassetto e pure _corsivo_**.
    Infine ~sbarrato~


### Liste

Scrivere liste con Markdown è tanto intuitivo quanto potente.

#### Liste non ordinate (ul)

    - Elemento 1
    - Elemento 2
    * Notato la seperazione?
    * Altro elemento
    + Notato l'altra separazione?


#### Liste ordinate (ol)

    1. Uno
    2. Due
    3. Tre
    4. Quattro
    8. <-- la numerazione è cambiata?

Possiamo anche avere **liste miste**. Prova a ficcare una lista non ordinata in una ordinata (o viceversa) e osserva che succede.

#### Link

Il modo di creare link in Markdown ricorda un po' quello usato da MediaWiki.

    [Link](https://www.google.it/)
    [Link con titolo](https://www.google.it/ "Google")
    [Riferimento][chiave del riferimento]
    Ora metto un [altro riferimento] [chiave del riferimento]: http://qualcosa
    [altro riferimento]: http://altro-qualcosa

Qui possiamo aggiungere qualche parola:

-   Possiamo usare **numeri come chiave** di riferimento;
-   URL da soli, o circondati da `<>` vengono **automaticamente** tradotti in link.

#### Immagini

Simile ai link, con l'aggiunta del **punto esclamativo**.

    ![alt-text](url/immagine.png "Titolo")


Possiamo usare i riferimenti anche per le immagini.

#### Tabelle

Molto semplice, basta anche qui usare qualche carattere.

    Prodotto|Q.tà
    --------|----
    Legno|10
    Staffa|20
    Vite|10
    Stop|10

#### Citazioni

Basta usare il carattere `> `.

    > Questa è una citazione

#### Linea orizzontale (hr)

A volte può essere utile dare una separazione netta al testo. Con Markdown possiamo usare:

    Separatore 1:
    ---
    Separatore 2:
    ***
    Separatore 3:
    ___


Basta avere almeno tre caratteri.
