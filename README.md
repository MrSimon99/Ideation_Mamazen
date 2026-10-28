# Ideation Mamazen

Un metodo per scoprire e sviluppare piste di prodotti software coerenti con il mandato dello studio, anche in attività e mercati inizialmente sconosciuti.

**Stato: base documentale IDEATION-0.1, 28 ottobre 2026.** Il lavoro è raccolto in una procedura utilizzabile in chat. Comprende prime regole operative proposte e rubriche da verificare su casi reali; non è un'applicazione o un sistema di agenti già implementato.

## Da dove partire

- Per continuare l'arricchimento nella nuova chat: [Punto di ripresa](docs/RIPRESA-ARRICCHIMENTO.md), da leggere prima di ripetere operazioni sulla rete o sul database.
- Per capire il funzionamento: [Sistema operativo](docs/ideation-sistema-operativo.md).
- Per avviare una ricerca assistita: [Istruzioni e richiesta compilabile](docs/ideation-istruzioni.md). L'assistente deve poter leggere i documenti richiamati.
- Per conoscere tesi, criteri e valori: [Mandato dello studio](docs/mandato-studio.md).
- Per selezionare dove investire ricerca usando l'Excel: [Gate di ricerca](docs/ideation-gate-ricerca.md), modello progressivo condiviso.
- Per riprendere il completamento dell'Excel: [Registro di lavorazione](docs/arricchimento-database.md), con copia di lavoro, checkpoint e blocco di accesso alle fonti.
- Per trovare sorgente, copia di lavoro e registri: [Database e convenzioni](data/README.md).

La ricerca può partire da testo libero, parametri, competitor, prodotti, professioni, attività o settori. L'output richiesto è selezionabile fra **spazi, opportunità e concept**. Il sistema ricostruisce il contesto necessario e valuta al livello scelto, senza imporre tre rapporti intermedi.

## Mappa dei documenti

| Ambito | Documento di riferimento |
| --- | --- |
| Tesi, target, pilastri e parametri | [Mandato dello studio](docs/mandato-studio.md), M-2026-10-28-01 |
| Form, flag, schede e passaggi fra livelli | [Input e output](docs/ideation-input-output.md), IO-0.1 |
| Vincoli, punteggi, evidenze e qualità del concept | [Valutazione e scoring](docs/ideation-valutazione-scoring.md), rubriche 0.2 |
| Esplorazione, priorità e prossime azioni | [Sistema operativo](docs/ideation-sistema-operativo.md), IDEATION-0.1 |
| Preselezione dei target e approfondimenti progressivi | [Gate di ricerca](docs/ideation-gate-ricerca.md), GATE-0.1 |
| Completamento dati e successivo approfondimento delle attività | [Registro di lavorazione del database](docs/arricchimento-database.md) |
| Avvio e restituzione in chat | [Istruzioni riusabili](docs/ideation-istruzioni.md), ISTRUZIONI-0.1 |
| Esempi sintetici di calibrazione | [Spazio](docs/calibrazione-spazio.md), [opportunità](docs/calibrazione-opportunita.md), [concept](docs/calibrazione-concept.md) |
| Interfaccia da conservare per il futuro | [Configurazione della dashboard](docs/dashboard-configurazione-mandato.md) |

Vincoli, coerenza ed evidenze restano distinti. Per il concept si esplicitano anche **QP — problema, QS — soluzione, QV — value proposition**. Nessuna media o soglia automatica nasconde un ostacolo decisivo; l'esito riguarda la coerenza con il mandato, non una validazione commerciale.

## Confini della versione

Le calibrazioni sono applicazioni manuali a casi inventati. Accuratezza e ripetibilità del modello non sono state misurate. Le prime regole operative sono modificabili e distinte dai criteri già concordati.

L'Excel ricevuto è stato esaminato. È condiviso il modello di selezione progressiva: usare la base esistente e quattro arricchimenti leggeri per scegliere i target, poi approfondire soltanto le piste selezionate. L'utente ha autorizzato il completamento dei campi mancanti in piccoli batch, seguito da value chain e parametri Gate 1. Sono predisposti copia, registro e checkpoint; nessun nuovo numero è stato inserito. L'accesso pubblico è già abilitato e pubblicato secondo la conferma dell'utente, ma la sessione precedente continua a ricevere 403 dal proxy: verificare la nuova sessione senza chiedere di ripetere la configurazione. Definizione delle priorità del Gate 1, implementazione degli agenti, dashboard, integrazioni e test ads restano nelle fasi dedicate.
