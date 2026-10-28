# Bike Sharing — notebooks revisionati per Scientific Data Visualization

**Questa è una copia revisionata dei tuoi otto notebook.** Non sovrascrive i tuoi file originali.

## Esecuzione

1. Copia i notebook nella tua cartella `SCI-VIZ-PROG/notebooks/` (conserva una copia dei vecchi notebook prima di sostituirli).
2. Nello ZIP sono inclusi i due CSV originali in `data/raw/` e i CSV elaborati in `data/processed/` per comodità; puoi mantenere i file che possiedi già.
3. Puoi rieseguire `01_DataCleaning.ipynb` per verificare e rigenerare i due file `data/processed/bike_*_clean.csv`.
4. I notebook 02–08 sono indipendenti e producono grafici PNG in `output/figures/`.

## Interventi principali

- Titoli che riportano la scoperta anziché il solo nome delle variabili.
- Colori consistenti: registered = blu, casual = arancione, ripetuti dove usiamo queste categorie.
- Sorgente, periodo, unità e limiti visualizzati nelle figure.
- In RQ1, piccoli multipli con scale Y non condivise per rendere visibili anche gli occasionali (è dichiarato).
- In RQ3, legenda associata ai giusti colori; nessuna conclusione causale.
- In RQ4, il picco dell'intervallo non viene presentato come temperatura ottimale dimostrata.
- In RQ5, confronto stagionale 2011 vs 2012, senza confondere crescita temporale e stagionalità.
- In RQ7/RQ8 originale (ora `07_MobilityPatterns`), silhouette, stabilità delle assegnazioni e interpretazione dei cluster; dichiarata esclusione dei giorni incompleti.
- In RQ9, rimossa l'API deprecata Pandas `.dt.weekday`.

## Concetti appresi dai materiali del corso

- Data source reliability (UCI, Capital Bikeshare, paper 2013).
- Question → computation → visual encoding → implementation, senza grafici superflui.
- Titoli esplicativi, legende minime, colori coerenti, confronto di grandezze omogenee.
- Collegamento alle presentazioni dei colleghi: K-means è unsupervised, e i cluster vanno *spiegati* con variabili che non hanno fatto parte del clustering.

## Limitazioni generali

- Dati storici di Washington D.C., 2011–2012.
- La fonte è una serie aggregata di noleggi, **non i viaggi dei singoli utenti**.
- `workingday=0` comprende festività e weekend.
- Alcune combinazioni data/ora non hanno osservazioni; non devono essere equiparate automaticamente a zero.
- Analisi meteo e eventi sono descrittive; mancano controlli sperimentali per inferenze causali.

**Fonte dataset:** https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset

**Paper:** Fanaee-T, H. & Gama, J. (2013), *Event labeling combining ensemble detectors and background knowledge*, Progress in Artificial Intelligence. https://doi.org/10.1007/s13748-013-0040-3
