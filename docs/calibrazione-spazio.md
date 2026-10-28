# Calibrazione iniziale dello spazio — Casi di riferimento

Data: 28 ottobre 2026.
Rubrica di riferimento: spazio, revisione 0.2 di [Valutazione e scoring](ideation-valutazione-scoring.md).

Stato: prima applicazione manuale su casi simulati e revisione concettuale dei descrittori. Non è una verifica indipendente delle prestazioni di un modello, una ricerca di mercato o una calibrazione su giudizi già assegnati dall'utente.

## 1. Obiettivo e metodo

Verificare che la rubrica distingua caratteristiche favorevoli, deboli, incompatibili e sconosciute, rispettando il mandato. Individuare ambiguità prima di definire pesi o decisioni automatiche.

La revisione è stata svolta in due passaggi: lettura critica dei descrittori; assegnazione ragionata dei profili ai casi seguenti e confronto fra varianti. I profili sono riferimenti proposti dall'assistente, da confrontare successivamente con il giudizio dell'Head of Product Studio e con casi reali.

Tutti i fatti e i numeri del documento sono inventati per l'esercizio. Si assumono veri soltanto all'interno del caso; il supporto sul mercato reale rimane **ipotesi simulata**, senza fonti esterne. Non attribuire a questi esempi lo stato di evidenza diretta su un mercato.

Durante l'esercizio si utilizzano soltanto le informazioni del caso. Un agente di ricerca futuro potrà raccoglierne altre, ma dovrà dichiararle e produrre una nuova valutazione, senza inserirle implicitamente nel caso originale.

## 2. Convenzioni

Profilo: **[S1, S2, S3, S4, S5]**.

- S1: cliente e decisione d'acquisto.
- S2: valore potenziale delle attività.
- S3: apertura rispetto alle alternative.
- S4: possibilità di prodotti autonomi e leggeri.
- S5: compatibilità commerciale potenziale.

0–3 e NV mantengono i significati della rubrica. Il simbolo «—» nelle tabelle indica che lo scoring non è stato avviato perché il caso è già fuori dal perimetro obbligatorio; non è un nuovo punteggio né un sinonimo di NV.

Per gli spazi, il calcolo del recupero di tutti i costi nel primo mese è sempre **non applicabile a questo livello**, non «superato». Il vincolo continua a valere per i futuri concept.

## 3. Caso base C00

**Spazio Alfa: attività documentali per professionisti e microimprese italiane.**

Informazioni assunte nell'esercizio:

- I potenziali acquirenti sono professionisti e microimprese che operano in Italia. Il titolare utilizza o supervisiona direttamente gli strumenti e può acquistarli autonomamente.
- Le attività producono conseguenze economiche importanti e un beneficio comprensibile e riconosciuto dai soggetti coinvolti.
- Le alternative coprono parte del lavoro; rimane una difficoltà circoscritta. È motivabile un miglioramento, senza assumere che i clienti cambino automaticamente.
- Nel perimetro esistono passaggi autonomi con input standardizzabili, forniti dal cliente, e un risultato ottenibile senza lavorazioni manuali interne per ciascun output.
- Si ipotizzano 20.000 unità potenzialmente paganti e riferimenti di spesa pertinenti alle attività. Esiste una strada plausibile per raggiungere tali soggetti tramite ads. Prezzo del prodotto, conversione, CAC e costi non sono ancora definiti.

Profilo assegnato: **[3, 3, 2, 3, 2]**.

| Criterio | Motivazione |
| --- | --- |
| S1 = 3 | La struttura dell'acquisto è direttamente favorevole a self-service o demo breve. |
| S2 = 3 | Il caso specifica conseguenze importanti e beneficio riconosciuto; il giudizio non deriva dalla sola frequenza. |
| S3 = 2 | L'apertura è plausibile, ma non sono descritte condizioni particolarmente favorevoli rispetto al cambiamento. |
| S4 = 3 | Sono esplicitamente individuati passaggi delimitati, input standardizzabili e un risultato autonomo. |
| S5 = 2 | È motivabile una combinazione commerciale potenziale, senza dimostrare ancora conversioni, CAC o redditività. La numerosità, da sola, non giustifica 3. |

Vincoli: target e geografia compatibili **nel caso simulato**; ads plausibili, con fattibilità economica ancora da verificare; pareggio al primo mese non applicabile come calcolo dello spazio. Non dichiarare validazione o autorizzazione automatica al lancio.

## 4. Varianti applicate

Ogni variante conserva le informazioni di C00 salvo le sostituzioni esplicitate. Le differenze nei profili devono essere giustificate dalle nuove caratteristiche, non dal nome del settore o dal tono della descrizione.

| Caso | Informazione sostituita o aggiunta | Profilo assegnato | Interpretazione |
| --- | --- | --- | --- |
| C01 — Solo un nome | È disponibile soltanto il titolo «Spazio Alfa»; nessun'altra informazione. | [NV, NV, NV, NV, NV] | Non inventare caratteristiche. Anche target e ads sono da verificare; assenza di dati non significa incompatibilità. |
| C02 — Alternative sconosciute | Sono rimosse tutte le informazioni sulle alternative e sulla difficoltà residua. | [3, 3, NV, 3, 2] | Non conoscere competitor e alternative non significa mercato libero né assenza di domanda. |
| C03 — Più competitor | Le alternative dedicate passano da poche a molte; difficoltà residua, segmenti e condizioni di cambiamento restano identici. | [3, 3, 2, 3, 2] | Il numero dei competitor da solo non cambia S3. |
| C04 — Apertura favorevole | Il segmento pertinente ha un bisogno importante non coperto dalle alternative; il vantaggio è rilevante e il cambiamento non richiede migrazioni o dipendenze onerose. | [3, 3, 3, 3, 2] | S3 cresce per caratteristiche favorevoli del vantaggio e del cambiamento, non per quantità delle fonti. |
| C05 — Apertura debole | Il miglioramento possibile è modesto e il cliente dovrebbe sostenere un cambiamento oneroso. Rimane un vantaggio, ma fragile. | [3, 3, 1, 3, 2] | Un problema reale non basta a rendere forte la ragione di acquisto. |
| C06 — Nessuna ragione di cambiamento nel perimetro | Nel perimetro delimitato le alternative soddisfano il risultato; le differenze possibili non producono beneficio utile e gli ostacoli al cambiamento sono sostanziali. | [3, 3, 0, 3, 2] | S3 = 0 deriva dalle condizioni dichiarate, non dalla mancata scoperta di un'apertura. Non estendere il giudizio ad altri perimetri non analizzati. |
| C07 — Attività rara ma importante | L'attività si presenta una volta l'anno; conseguenze, beneficio e riconoscibilità rimangono importanti. | [3, 3, 2, 3, 2] | Non esiste una frequenza minima universale. Non dedurre da S2 la scelta obbligatoria dell'abbonamento. |
| C08 — Valore fragile | Il beneficio esiste ma ha conseguenze limitate ed è poco rilevante per il cliente, anche considerando la frequenza. | [3, 1, 2, 3, 2] | S2 diminuisce per il valore del risultato; non per assenza di una fonte. |
| C09 — Valore marginale | I benefici sono marginali anche considerando il loro accumulo nel tempo e gli effetti su costi, rischi operativi e ricavi. | [3, 0, 2, 3, 2] | Non usare la frequenza per rendere attraente un'attività priva di valore sufficiente nel caso. |
| C10 — Decisione complessa | L'acquisto richiede coordinamento sostanziale fra più soggetti; i percorsi brevi sono eccezioni difficili, ma non impossibili. | [1, 3, 2, 3, 2] | S1 è debole per gli effetti del coordinamento, non per un numero arbitrario di interlocutori. |
| C11 — Core umano, passaggi autonomi | L'attività centrale richiede lavoro professionale personalizzato, ma sono esplicitamente presenti passaggi adiacenti separabili, autonomi e di valore. La loro gestione richiede alcune eccezioni. | [3, 3, 2, 2, 2] | Non assegnare 0 a tutto lo spazio perché il core è umano. Valutare i perimetri software individuati. |
| C12 — Valore inseparabile dal lavoro umano | Nel sotto-perimetro specificamente valutato ogni risultato di valore richiede lavorazione manuale interna personalizzata; non si tratta della sola attività centrale di uno spazio più ampio. | [3, 3, 2, 0, 2] | La struttura commerciale può essere favorevole mentre l'autonomia è incompatibile. Non nasconderlo in una media. Il giudizio vale per questo sotto-perimetro. |
| C13 — Ads incompatibili | È esplicitamente stabilito nel caso che il canale paid digitale non può raggiungere gli acquirenti pertinenti nel perimetro considerato. | [3, 3, 2, 3, 0] | Il vincolo ads è incompatibile nel caso e non può essere compensato. Non confondere questa premessa con «non abbiamo trovato annunci». |
| C14 — Target fuori mandato | Gli unici possibili acquirenti del perimetro sono consumatori privati, senza segmenti professionisti o microimprese. | [—, —, —, —, —] | Fuori mandato per target: i benefici eventualmente elevati non compensano il vincolo. |
| C15 — Nicchia piccola, spesa maggiore | Il bacino è di 1.000 unità paganti potenziali, con riferimenti di spesa pertinente di circa 2.000 €/anno. Rimane una strada plausibile tramite ads. | [3, 3, 2, 3, 2] | Nessuna penalità automatica per essere sotto 50.000 soggetti. Il riferimento di spesa non diventa prezzo garantito del futuro prodotto. |
| C16 — Contesto misto | Lo spazio contiene microimprese con il profilo C00 e grandi imprese con processi d'acquisto differenti. Il mandato permette di concentrarsi sulle prime. | [3, 3, 2, 3, 2], solo per la porzione microimprese | Dichiarare il sottoinsieme valutato; non attribuire il profilo all'intero contesto e non scartare tutto per la presenza di altri soggetti. |
| C17 — Dato macro aggiunto | Si parte da C02 e si aggiunge soltanto un dato sul valore complessivo del settore, senza informazioni sulle alternative o sul bisogno specifico. | [3, 3, NV, 3, 2] | Il dato macro non risolve S3 e non dimostra spesa pertinente, clienti conquistabili o CAC. |
| C18 — Struttura commerciale favorevole | I soggetti paganti sono individuabili, una spesa consistente è già rivolta alla stessa classe di attività e il contesto presenta acquisti di strumenti autonomi attraverso canali digitali compatibili. Non si assume un CAC verificato. | [3, 3, 2, 3, 3] | S5 cresce per l'incastro commerciale favorevole. Rimane una valutazione dello spazio, non del pareggio di un prodotto. |
| C19 — Combinazione commerciale fragile | Il bacino pertinente è ristretto, la spesa disponibile per quelle attività è limitata e raggiungerlo tramite ads presenta difficoltà concrete. Il canale non è impossibile. | [3, 3, 2, 3, 1] | La combinazione è debole, ma non è introdotta una soglia minima universale né un'esclusione automatica. |

Questi profili costituiscono una prima applicazione manuale della rubrica. Non sono il risultato di venti esecuzioni indipendenti di un modello; non è stata misurata una percentuale di accuratezza o ripetibilità.

## 5. Controlli trasversali

### T01. Fonte più pertinente, caratteristiche uguali

Se le caratteristiche valutate non cambiano, aggiungere fonti pertinenti può rafforzare il supporto senza aumentare il punteggio di coerenza. Se la fonte introduce fatti nuovi, invece, il punteggio può cambiare: dichiarare quali fatti hanno modificato il giudizio.

Parafrasare lo stesso input, aggiungere parole come «enorme opportunità» o duplicare una fonte non giustifica cambiamenti del profilo.

### T02. Incassi mensili e annuali: controllo per il futuro concept

Esempio soltanto contabile, non calibrazione della rubrica concept: 100 nuovi clienti, ricavo annuale per cliente di 240 €, CAC di 48 €, sviluppo iniziale di 2.000 € e altri costi del primo mese di 1.000 €. Tutti i costi di acquisizione sono sostenuti nel primo mese; nessun altro incasso o costo è presente nell'esercizio.

- CAC/ricavo annuale = 20% in entrambe le formule.
- Costi complessivi sostenuti entro il primo mese = 4.800 + 2.000 + 1.000 = 7.800 €.
- Incasso annuale anticipato: 24.000 €; saldo di cassa dell'esercizio = +16.200 €.
- Incasso mensile: 2.000 €; saldo di cassa dell'esercizio = −5.800 €.

Il rapporto CAC può essere compatibile mentre il recupero dei costi nel primo mese non lo è. Il saldo positivo dell'incasso annuale non è una misura dell'utile maturato né elimina i costi futuri necessari a servire gli abbonati. Non trasferire questo calcolo al livello spazio.

### T03. Fasce di ricavo e preferenze

Un futuro scenario con potenziale superiore alla fascia orientativa non viene escluso. Un pagamento per output rimane ammesso; un'attività rara può sostenerlo. L'aspirazione di margine superiore all'80% non diventa un filtro di ideation.

Questi controlli confermano il significato dei parametri del mandato; non assegnano punteggi a concept non ancora valutati.

## 6. Correzioni introdotte nella revisione 0.2

| Ambiguità della revisione iniziale | Correzione |
| --- | --- |
| S4 poteva essere letto come giudizio sull'attività centrale dell'intero settore. | Valutare il perimetro e i passaggi pertinenti; considerare componenti adiacenti autonome, quando esplicitamente individuate. |
| La presenza di più decisori poteva diventare una penalità numerica automatica. | Considerare conseguenze su coordinamento, dipendenze e percorso d'acquisto. Nessuna soglia sul numero di persone. |
| Un 3 poteva essere confuso con molta documentazione. | Separare caratteristiche favorevoli e supporto delle evidenze. |
| Un vincolo non verificato poteva essere trattato come incompatibile. | Conservare lo stato «da verificare», senza trasformarlo in esclusione. |
| Il mercato macro poteva sostituire la pertinenza commerciale. | Distinguere spesa di settore, bacino pertinente e possibilità concreta di acquisizione. |
| Il pareggio poteva essere implicitamente dichiarato superato in uno spazio promettente. | Indicare esplicitamente «non applicabile a questo livello» come calcolo. |

## 7. Uso futuro e limiti

Il protocollo operativo è nella sezione 8 del documento di scoring. Un futuro agente valutatore dovrà ricevere il mandato, la rubrica pertinente e questi casi come riferimenti; la sola presenza dei file non aggiorna, addestra o configura automaticamente un modello.

Prossime verifiche: confronto dei profili con l'Head of Product Studio, applicazione a schede reali con fonti e verifica delle differenze fra valutazioni ripetute. Sono ora disponibili anche prime rubriche e calibrazioni concettuali per [opportunità](calibrazione-opportunita.md) e [concept](calibrazione-concept.md). La revisione 0.2 è un riferimento iniziale calibrato concettualmente, non una versione di produzione già validata.

Riscontro dell'utente, 28 ottobre 2026: condivisi i tre esempi presentati in chat, relativi a C07 (attività annuale ad alto valore, S2 = 3), C11 (core umano con passaggi adiacenti autonomi e alcune eccezioni, S4 = 2) e C03 (più competitor con apertura invariata, S3 = 2). Questo riscontro non viene esteso automaticamente a tutti i venti profili o ai singoli descrittori non discussi.
