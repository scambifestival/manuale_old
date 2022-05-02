---
description: Guida all’utilizzo del software per la gestione dei dati
---

# Baserow

[Baserow](https://baserow.io) è il nome del software tramite la cui interfaccia è gestito _Pino_, il database di Scambi. Se le informazioni in questa pagina non fossero esaustive, prima di rivolgersi al povero team Silicon provare a cercare maggiori informazioni [spulciando il forum ufficiale](https://community.baserow.io).

### Accesso

Per la sola visualizzazione dei dati, fare riferimento alle istruzioni in [questo messaggio](https://t.me/c/1617977522/5), mentre per accedere e modificare i dati occorre andare su [pino.scambi.org](https://pino.scambi.org), utilizzando un account con un indirizzo email autorizzato.

### Utilizzo

Baserow è un Google Sheets con i superpoteri. Sono rimosse tutte le funzionalità di formattazione come i colorini, i font, eccetera, mentre sono aggiunte funzionalità che aiutano immensamente nella gestione di grosse quantità di dati, nonché la loro visualizzazione ed analisi.

Il video di seguito riassume le funzionalità essenziali

{% embed url="https://peertube.uno/w/rQx6eXZpXUhcjzHJZeZfjm" %}

### Contenuti

In Pino esistono diverse tabelle, ciascuna con un ruolo specifico. Nel tutorial sopra non sono specificati nel dettaglio i ruoli di ogni tabella ed i criteri di inserimento e catalogazione dei dati.

* in [_Relazioni_](https://baserow.io/database/22288/table/58822) sono raccolte tutte le interazioni che Scambi ha con persone o enti esterni.
  * ogni genere di relazione, anche se non andata a buon fine, va assolutamente inserita.
  * se una relazione si ripete per più di un’edizione, il campo **`stato`** si riferisce automaticamente all’**ultima edizione**.
* in _Programma `anno_edizione`_ (e.g. [_Programma 2022_](https://baserow.io/database/22288/table/58806)) sono raccolte tutte le attività **confermate** per una determinata edizione.
  * Che il nome non confonda: in Programma non devono essere presenti solo cose che fisicamente avverranno, ma **ogni sorta di collaborazione** relativa all’edizione in questione.
* in _Programma `anno_edizione`_ (e.g. [_Persone 2022_](https://baserow.io/database/22288/table/61708)) sono raccolte tutte le persone che, in qualunque ruolo, partecipano ad un’edizione
