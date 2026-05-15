# Programma di rilevamento sporcizia su telecamera

## Obiettivi formativi

Progettazione, implementazione e sperimentazione di un sistema di computer vision per il monitoraggio dello stato di pulizia dell'ottica di una telecamera, attraverso:

- definizione di metriche e/o caratteristiche visive correlate allo sporco
- costruzione di dataset di immagini e pipeline di pre-processing
- sviluppo di un algoritmo (classico e/o con modelli ML leggeri) che produca un indice numerico robusto e ripetibile
- validazione sperimentale, analisi delle prestazioni e documentazione tecnica

1. Analisi del problema e requisiti
   - Comprensione dello scenario (telecamera, condizioni ambientali, illuminazione, tipologia di sporco)
   - Definizione dei requisiti funzionali: range indice, frequenza calcolo, soglie allarme, vincoli HW/SW
2. Raccolta dati e definizione dataset
   - Acquisizione e catalogazione immagini (ottica pulita / sporca / livelli intermedi)
   - Definizione etichette qualitative, classi, oppure riferimento da ispezione manuale
   - Gestione variabili confondenti: variazioni luce, esposizione, scene diverse, vibrazioni
3. Pre-processing e normalizzazione
   - Correzioni fotometriche (es. normalizzazione luminosità/contrasto)
   - Filtri e maschere ROI (es. area più informativa, esclusione elementi di scena non utili)
4. Studio e implementazione
   - Implementazione di metriche di base
   - Eventuale proposta di un indice composito
   - Approccio ML (opzionale): addestramento di un classificatore o regressore per stimare livello di sporco
5. Validazione sperimentale
   - Test condizioni reali
   - Taratura dell'indice e definizione soglie (warning/alarm)
   - Analisi robustezza: luce diversa, scene diverse, rumore, compressione
6. Prototipazione software
   - Realizzazione modulo eseguibile o libreria in C#
   - Eventuale piccola UI o tool di analisi per visualizzare indice e debug
7. Documentazione
   - Documentazione tecnica (architettura, scelte algoritmiche, parametri, limiti noti)
   - Report finale con risultati e raccomandazioni per industrializzazione.


# Informazioni sul THUD: THesis at UniUD

THUD è un formato LaTeX per le tesi di laurea in Informatica ed affini presso il Dipartimento di Scienze Matematiche, Informatiche e Fisiche dell'Università degli Studi di Udine.

Si assume che sappiate scrivere in LaTeX; altrimenti, [sappiatelo](https://www.learnlatex.org/en/).

## Procedura per laurearsi

1. Clonare o forkare questo repository.
2. Rinominare thesis.tex in thesis_*cognome*.tex (con il vostro cognome), che sarà il file principale della tesi. 
3. Editare il file thesis_*cognome*.tex.  È sufficiente riempire i campi necessari e aggiungere tutto il materiale che serve. Il codice dovrebbe essere auto-esplicativo.
4. Compilare thesis_*cognome*.tex con pdflatex.
5. Se si usa bibtex (fortemente consigliato!): riempire il file thud.bib, passare bibtex, poi pdflatex e pdflatex.
6. Caricare thesis_*cognome*.pdf su Esse3 entro la scadenza.
7. Preparare le slide, eventualmente con il formato ufficiale del dipartimento.
8. Esporre slide.pptx.
9. Ubriacarsi con amici e parenti.
