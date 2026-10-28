# Ideation — Output, form di input e passaggi fra livelli

Data: 28 ottobre 2026.
Versione: **IO-0.1**.
Stato: documento di lavoro che raccoglie le definizioni e i campi concordati.

Destinazione: futuro motore di ideation e relativi form della dashboard. Il documento definisce contenuti e comportamenti attesi; non implementa interfacce, agenti o automazioni.

Il mandato e i parametri dello studio sono descritti in [Mandato dello studio](mandato-studio.md). Qui ne viene mantenuto il riferimento, senza duplicare le soglie economiche. La [dashboard futura](dashboard-configurazione-mandato.md) ne specifica i controlli; il [sistema operativo](ideation-sistema-operativo.md) collega questi campi alla conduzione della ricerca.

Ogni scheda potrà essere accompagnata dalla valutazione descritta in [Valutazione e scoring](ideation-valutazione-scoring.md), distinta dai suoi contenuti descrittivi e dalla validazione commerciale. La futura dashboard dovrà riportarla.

## 1. Finalità e principi

Il sistema deve ampliare la capacità dell'Head of Product Studio di scoprire opportunità di prodotto coerenti con il mandato, anche in settori e attività che non conosce. Deve poter esplorare e approfondire autonomamente, oltre a supportare la co-progettazione.

- Output selezionabile all'inizio: **spazi**, **opportunità** oppure **concept**.
- Ingressi combinabili: settori, professioni, imprese, attività, problemi, competitor, prodotti, trend e altri segnali.
- Richiesta formulabile in testo libero, tramite parametri o usando entrambe le modalità.
- Una scheda già prodotta può diventare input della ricerca successiva.
- La scelta di arrivare al concept autorizza l'approfondimento autonomo; non obbliga a produrre una proposta priva di presupposti credibili.
- La selezione manuale delle piste non è un passaggio sempre obbligatorio.
- I livelli descrivono gli oggetti prodotti, non il loro grado di validazione. Un concept può essere ancora ipotetico.
- Test ads, landing, creatività, budget sperimentali e piano di validazione appartengono alla fase successiva al concept.

La knowledge base fornirà contesto e ampiezza all'esplorazione. Le sue tassonomie, la struttura tecnica e le skill di ricerca saranno definite successivamente.

## 2. Richiesta comune ai tre form

| Campo | Tipo concettuale | Funzione |
| --- | --- | --- |
| Output desiderato | Selezione | Spazi, opportunità o concept. Determina il risultato richiesto, non il punto da cui è obbligatorio iniziare. |
| Mandato attivo | Riferimento alla versione | Tesi, pilastri e parametri da applicare. |
| Richiesta libera | Testo lungo facoltativo | Descrizione complessiva della ricerca, utilizzabile anche senza compilare i campi specifici. |
| Riferimenti iniziali | Elenco di riferimenti facoltativo | Competitor, prodotti, fonti, documenti o schede già disponibili. |
| Parametri della ricerca | Campi specifici facoltativi | Settori, clienti, attività, bisogni e altre informazioni del form scelto. |
| Ruolo di ciascun elemento | Flag «Vincolo» | Attivo: condizione da rispettare. Disattivo: spunto che può essere reinterpretato o ampliato. |
| Altri input e indicazioni | Testo lungo facoltativo, presente in tutti e tre i form | Informazioni particolari, eccezioni, esempi, osservazioni o istruzioni pertinenti che non trovano posto nei campi preimpostati. |

### Testo libero e parametri

«Richiesta libera» permette di esprimere l'intera domanda. «Altri input e indicazioni» permette di integrare anche una richiesta costruita principalmente attraverso campi e selettori. Non è necessario compilare entrambi.

Esempi di indicazioni aggiuntive, da interpretare nel contesto della singola ricerca:

- «Considera anche attività che si presentano soltanto in alcuni periodi dell'anno».
- «Usa questo prodotto estero come riferimento, ma esplora anche professioni differenti».
- «Concentrati sui passaggi che avvengono dopo la consegna del lavoro».

Regole per il futuro sistema:

1. Testo libero e campi strutturati alimentano la stessa richiesta. Le indicazioni aggiuntive non sono note decorative: devono essere considerate nella ricerca.
2. Conservare il testo originale e rendere visibili gli elementi ricavati e i relativi flag modificabili.
3. Una frase può contenere più elementi con ruoli differenti. Il flag riguarda l'elemento, non necessariamente tutto il campo di testo.
4. Se un'indicazione non corrisponde a un campo esistente, conservarla come informazione aggiuntiva; non perderla o forzarla in una categoria impropria.
5. Rendere espliciti conflitti fra testo, parametri e mandato. Il testo libero non modifica silenziosamente il mandato né disattiva i suoi vincoli.
6. Distinguere elementi indicati dall'utente, deduzioni del sistema e informazioni provenienti da fonti.

## 3. Form di input

I campi specifici seguenti sono facoltativi. Non è necessario conoscere già tutto ciò che il sistema deve scoprire. I campi mancanti restano sconosciuti oppure vengono approfonditi durante la ricerca; non valgono zero.

### A. Trovare spazi

| Campo preimpostato | Contenuto |
| --- | --- |
| Settore o ambito | Area economica o di lavoro da cui partire. |
| Tipologia di cliente | Professionisti, microimprese o cluster disponibili. |
| Attività o area di lavoro | Per esempio gestione della cassa, approvvigionamenti o adempimenti. |
| Bisogno o risultato generale | Direzione di valore da esplorare. |
| Prodotti o competitor di riferimento | Esempi che orientano la ricerca. |
| Segnali o cambiamenti | Trend, osservazioni, nuove esigenze o altri indizi. |
| Condizioni aggiuntive | Per esempio una numerosità desiderata del target o una caratteristica delle attività. |
| Altri input e indicazioni | Campo comune di testo libero per ulteriori elementi. |

È ammessa anche un'esplorazione aperta dentro il mandato, senza uno specifico punto di partenza.

### B. Trovare opportunità

| Campo preimpostato | Contenuto |
| --- | --- |
| Spazio di partenza | Scheda esistente oppure descrizione libera, quando disponibile. |
| Contesto e value chain | Attori, attività e collegamenti già individuati. |
| Clienti coinvolti | Categorie presenti nello spazio ed eventuali segmenti su cui concentrarsi. |
| Bisogno/JTBD generale | Direzione da cui cercare bisogni più circoscritti. |
| Soluzioni presenti | Approcci, servizi e prodotti già individuati. |
| Dati ed evidenze | Fonti, dimensioni indicative e segnali disponibili. |
| Restrizioni aggiuntive | Parti da includere, escludere o privilegiare. |
| Altri input e indicazioni | Campo comune di testo libero per ulteriori elementi. |

Se viene selezionata una scheda spazio, i suoi contenuti sono recuperabili senza ricopiarli. Uno spazio completo non è un prerequisito: si può partire anche da un competitor, un'attività o un altro riferimento e ricostruire il contesto necessario.

### C. Trovare concept

| Campo preimpostato | Contenuto |
| --- | --- |
| Opportunità di partenza | Scheda esistente oppure descrizione libera, quando disponibile. |
| Cliente e contesto | Segmenti, ruoli e situazioni individuati. |
| Attività e processo | Passaggi, scambi, strumenti e dipendenze. |
| Risultato desiderato | Il lavoro che il cliente vuole portare a termine. |
| Bisogno, peso e frequenza | Difficoltà, conseguenze e ricorrenza. |
| Alternative e apertura commerciale | Come risolve oggi e dove potrebbe esserci spazio. |
| Riferimenti economici | Bacino, spesa e prezzi osservabili, quando disponibili. |
| Evidenze e incertezze | Informazioni supportate e ipotesi ancora aperte. |
| Indicazioni di prodotto | Idee iniziali, confini o condizioni, ciascuna come spunto o vincolo. |
| Altri input e indicazioni | Campo comune di testo libero per ulteriori elementi. |

Una richiesta di concept può partire anche da input incompleti. Il sistema ricostruisce gli elementi necessari, dichiarando le lacune e le assunzioni; non impone la compilazione manuale di tutte le schede intermedie.

## 4. Schede di output riutilizzabili

### A. Spazio

Una direzione di ricerca ampia e motivata. Esempi di perimetro: sicurezza nel cantiere, gestione della cassa in edilizia, gestione dei fornitori in edilizia.

| Campo | Contenuto atteso |
| --- | --- |
| Nome dello spazio | Denominazione comprensibile dell'ambito. |
| Contesto e value chain | Poche righe sul contesto, i soggetti e 2–3 attività o passaggi interessati. |
| Bisogno/JTBD generale | Risultato desiderato e possibile difficoltà a livello ampio, anche come ipotesi. |
| Soluzioni presenti | 2–3 tipologie di soluzioni o approcci esistenti; esempi concreti quando disponibili. Non sono ancora concept proposti dallo studio. |
| Perché esplorarlo | Ragioni di interesse rispetto al mandato, distinguendo segnali e ipotesi. |
| Priorità | Posizione relativa motivata fra le piste della sessione, con lo scopo della priorità, secondo la prima proposta qualitativa nel [sistema operativo](ideation-sistema-operativo.md). Non è un punteggio assoluto di settore. |
| Evidenze disponibili | Fonti, dati di mercato, soggetti potenzialmente coinvolti e segnali del bisogno, quando reperibili. |

Il valore di mercato dà contesto e non equivale al potenziale economico di un futuro prodotto. I soggetti coinvolti non coincidono automaticamente con gli acquirenti: indicare se si contano persone, professionisti, studi o imprese.

La scheda può esistere senza numeri, rendendo visibile ciò che resta da verificare. Non richiede un'analisi completa del settore.

### B. Opportunità

Un'ipotesi commerciale circoscritta: un cliente identificabile, un'attività e un risultato desiderato per cui potrebbe esserci spazio per un nuovo prodotto.

| Campo | Contenuto atteso |
| --- | --- |
| Cliente | Segmento specifico; utilizzatore e acquirente, quando identificabili. |
| Attività e contesto | Che cosa svolge e in quale situazione. |
| Risultato desiderato | Il JTBD preciso. |
| Bisogno e peso | Difficoltà, obbligo o opportunità di miglioramento; conseguenze e frequenza. |
| Processo e value chain pertinente | Approfondimento dei passaggi, ruoli, scambi di informazioni, strumenti e difficoltà. |
| Alternative attuali | Come ottiene oggi il risultato. |
| Apertura commerciale | Perché potrebbe scegliere e pagare una nuova soluzione. |
| Compatibilità iniziale con il mandato | Ragioni per ipotizzare un prodotto leggero, acquisibile tramite ads ed economicamente interessante. |
| Riferimenti economici | Bacino pertinente, spesa e ticket plausibile, quando motivabili. |
| Evidenze e incertezze | Fonti, assunzioni e domande decisive ancora aperte. |

La value chain è più approfondita rispetto allo spazio. Per ciascun passaggio rilevante: chi lo svolge, chi dipende dal risultato, quali informazioni entrano ed escono, quali strumenti intervengono e dove emergono difficoltà.

I passaggi del processo non diventano automaticamente nuove opportunità. Il confine esatto del prodotto resta da scegliere nel concept. Gestire la formazione sicurezza e predisporre DVR sono esempi di opportunità differenti dentro lo stesso spazio; i nomi sintetici vanno accompagnati dal contenuto della scheda.

### C. Concept

Una proposta concreta di prodotto per un cliente specifico, con promessa di valore, perimetro di soluzione e ipotesi commerciale ed economica da verificare.

| Campo | Contenuto atteso |
| --- | --- |
| Opportunità di origine | Attività e bisogno cui risponde, con riferimento alla scheda disponibile. |
| Cliente iniziale | Segmento scelto, utilizzatore e acquirente. |
| Problema/JTBD scelto | Situazione specifica, risultato desiderato, conseguenze, peso/frequenza e motivo per intervenire per il cliente iniziale. |
| Promessa di valore / value proposition | Per chi e in quale situazione il risultato offerto è importante, perché è credibile e quale ragione dà per scegliere l'offerta rispetto alle alternative. |
| Soluzione essenziale | Meccanismo con cui affronta il problema scelto; legame fra funzioni essenziali, passaggi e risultato ottenibile. |
| Perimetro | Passaggi coperti, esclusioni, dipendenze ed eventuali interventi umani. |
| Vantaggio sulle alternative | Perché il cliente dovrebbe scegliere il prodotto. |
| Offerta commerciale | Prezzo ipotizzato, abbonamento/output e modalità di pagamento. |
| Plausibilità dell'acquisizione | Ipotesi sulla raggiungibilità tramite ads e sul percorso verso l'acquisto. |
| Scenario economico | Assunzioni essenziali su clienti/coorti, ricavi, incassi, CAC complessivo, costi iniziali e operativi, recupero nel primo mese e sostenibilità del servizio venduto. Dichiarare periodi e costi mancanti; distinguere cassa e profitto. |
| Evidenze e incognite | Elementi a sostegno e assunzioni che potrebbero invalidare la proposta. |

Il concept non è una specifica tecnica di sviluppo né un piano di test ads. Una promessa pubblicitaria diversa, da sola, non costituisce necessariamente un concept distinto.

La sua valutazione deve riportare esplicitamente QP (bontà del problema), QS (adeguatezza della soluzione) e QV (forza della value proposition), con motivazioni, evidenze e incertezze. Questi giudizi accompagnano il profilo sui pilastri e non vengono ricavati automaticamente dai conti economici.

## 5. Input → output → input

1. Uno spazio può alimentare la ricerca di più opportunità; ciascuna opportunità può alimentare più concept.
2. Conservare il collegamento alle schede di origine e alla versione del mandato utilizzata, oltre ai filtri e ai vincoli della sessione.
3. Riutilizzare i campi mantenendone il significato. Il JTBD generale dello spazio rimane contesto; il JTBD dell'opportunità lo approfondisce senza sovrascriverlo.
4. Mantenere evidenze, fonti e assunzioni collegate alle affermazioni cui si riferiscono. Per dati quantitativi: unità, periodo, geografia e distinzione fra dato riportato e stima.
5. Non trasferire automaticamente al sottoinsieme i numeri dell'intero spazio. Bacino, concorrenti e prezzi devono essere riferiti al nuovo perimetro.
6. Le ipotesi generate dall'AI non diventano vincoli per il passaggio successivo. Un prezzo stimato rimane modificabile, salvo una scelta deliberata dell'utente.
7. Conservare anche il testo libero aggiuntivo e il suo ambito di applicazione. Se era riferito soltanto a una fase, non trasformarlo in un vincolo globale.
8. Non inventare dati per completare una scheda. Un'informazione mancante richiede un approfondimento o un'assunzione dichiarata, non un'esclusione automatica.
9. Una soluzione scartata non elimina automaticamente l'opportunità o lo spazio da cui deriva.

Esempio di concatenazione, soltanto illustrativo: **sicurezza nel cantiere → gestione della formazione sicurezza → prodotto self-service per raccogliere attestati e controllare scadenze per un segmento di imprese edili**. Il collegamento fra livelli non costituisce evidenza della fattibilità commerciale del concept.

## 6. Collegamento operativo e fase successiva

La struttura generale e prime rubriche dei tre livelli, con calibrazioni concettuali manuali su casi simulati, sono definite nei documenti collegati. Il [sistema operativo IDEATION-0.1](ideation-sistema-operativo.md) aggiunge una prima proposta qualitativa per scegliere approfondimenti, confrontare le priorità, chiudere il ciclo e proporre la prossima azione. Le [istruzioni riusabili](ideation-istruzioni.md) consentono di avviare una sessione assistita con questi riferimenti.

Restano il confronto dei nuovi profili con l'utente, la calibrazione su casi reali e la ripetibilità. Le nuove regole operative non sono soglie di validazione o giudizi già verificati su un modello.

L'Excel ricevuto è stato esaminato. Il modello condiviso nei [gate di ricerca](ideation-gate-ricerca.md) usa i dati disponibili per selezionare target e aggiungere informazioni soltanto sulle piste che proseguono. I gate regolano l'impiego della ricerca; le schede spazio, opportunità e concept mantengono i campi qui definiti. La prossima definizione riguarda il Gate 1. Struttura tecnica della KB, skill specialistiche, persistenza e automazioni saranno affrontate nelle fasi dedicate.
