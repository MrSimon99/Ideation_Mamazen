# Ripresa dell'arricchimento Excel

## Richiesta autorizzata da continuare

L'utente vuole completare il database con profondità e costanza, **una riga e una colonna alla volta, in piccoli batch**. Qualità del dato prioritaria. Non occorre richiedere nuovamente approvazione per i batch.

1. Primo giro: ricercare e completare i campi mancanti con fonti effettivamente consultate e tracciabili.
2. Secondo giro: approfondire attività e processi come una value chain, soprattutto commercianti e microimprese; aggiungere cluster, attività circoscritte candidate, leve di valore e metadati economici del Gate 1.

## Stato al passaggio di chat — 28 ottobre 2026

- Fonte originale ora disponibile anche nel repository: `data/sorgenti/professioni_con_piva_italia_v6_output.xlsx`.
- Copia di lavorazione: `data/lavorazione/professioni_con_piva_italia_v7_lavorazione.xlsx`.
- Stato macchina: `data/lavorazione/checkpoint.json`.
- Coda: `data/lavorazione/batch-primo-giro.json` e `registro-lacune.json`.
- Documento operativo: `docs/arricchimento-database.md`.
- **Nessun nuovo numero inserito; nessuna nuova fonte esterna verificata.** I sette fogli originari conservano tutti i valori originali. Il file sorgente è invariato.
- 473 voci: 399 professioni/ruoli e 74 attività artigianali/commerciali.
- Da ricercare: 49 remunerazioni e 40 numerosità, in 62 righe. Ci sono inoltre 46 fonti remunerazione vuote.
- 177 unità di output vuote: 168 compensi a tempo, 8 non determinabili e un caso misto M244 (Enotecari). Verificare applicabilità, non inventare output per eliminare un vuoto.
- 27 Note generali vuote sono facoltative.
- Sono preparati 13 batch di massimo cinque target, non ancora svolti. I soli metadati delle righe 402–406 sono stati estratti dalle note esistenti, con verifica esterna esplicitamente non eseguita.
- Secondo giro non avviato. Nessuna classifica dei target o scoring numerico del Gate 1 da assumere già definito.

## Punto preciso da cui riprendere

**P1-B01, C402: remunerazione annua dell'Agricoltore / Coltivatore Diretto.** Poi C403 Viticoltore, C404 Floricoltore, C405 Allevatore, C406 Apicoltore e D406 numerosità Apicoltore; completare le relative fonti con ciascun dato. Seguire la coda e salvare il checkpoint dopo ogni batch verificato.

Per ciascun numero: fonte, URL, estratto/tabella/pagina, editore, anno del fenomeno, data di pubblicazione e accesso, unità e popolazione. Distinguere reddito personale lordo/netto, fatturato, RAL dipendente, imprese/persone/iscritti/licenze. Reddito convenzionale contributivo non equivale a reddito effettivo. Un proxy o una stima restano riconoscibili; un dato non reperibile non diventa zero.

## Blocco della sessione precedente

L'utente ha **già abilitato e pubblicato l'accesso a tutto Internet pubblico** e ha fornito uno screenshot dell'interruttore attivo. La lettura della configurazione modificabile conferma `network_type: unrestricted`, revisione 3. La vecchia sessione continua invece a riportare rete `restricted`, revisione runtime 1, e ISTAT/CREA restituiscono 403 dal proxy. È un disallineamento di configurazione/sessione osservato, non una mancanza di credenziali dei siti.

**Non far ripetere all'utente l'abilitazione o la pubblicazione.** Nella nuova sessione verificare prima l'accesso effettivo alle fonti; se funziona, procedere subito con C402. Non rigenerare la preparazione già salvata e non rimpiazzare l'accesso pubblico con una nuova lista limitata di domini. Se il blocco permane, riportare la limitazione tecnica con evidenza, senza attribuirla a impostazioni che l'utente non avrebbe applicato.

## Contesto di prodotto

Leggere `AGENTS.md`, `README.md`, `docs/mandato-studio.md` e `docs/ideation-gate-ricerca.md`. La base guida la ricerca top-down e supporta ideation da competitor, attività o intuizioni. Gate = decisioni su dove investire ricerca; spazio/opportunità/concept = oggetti valutati. Mandato, rubriche e valutazioni restano distinti. Non implementare dashboard o agenti e non avviare test ads in questa attività.

## Portabilità

Sorgente, copia di lavorazione, checkpoint e documenti fanno parte dello stesso repository. Nella nuova chat verificare che il checkout contenga questi file e leggere prima `AGENTS.md` e questo documento. Non ricreare il database dal solo nome della repo o da una versione precedente del file.

`consegna_mamazen.zip` è un export locale derivato, escluso da Git per evitare duplicati e copie obsolete. È una soluzione alternativa per il trasferimento manuale se fornito come allegato; il riferimento ordinario resta il contenuto versionato del repository. Non dichiarare avvenuto ripristino o aggiornamento del checkout prima di verificarli.
