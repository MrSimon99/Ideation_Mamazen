# Futura dashboard — Configurazione del mandato Mamazen

Stato: specifica di struttura e campi, da conservare per una futura realizzazione della dashboard.
Data: 27 ottobre 2026.
Aggiornamento: 28 ottobre 2026, separazione della fonte del mandato e collegamento al sistema operativo documentale.

Questo documento non implementa un'interfaccia o un sistema di agenti. Specifica come consultare e modificare il [mandato dello studio](mandato-studio.md) attraverso la futura dashboard. Il flusso di ideation è descritto nel [sistema operativo documentale](ideation-sistema-operativo.md). La mappatura dei settori e dei cluster di clienti sarà svolta successivamente.

## 1. Scopo e confini

Consentire all'Head of Product Studio di consultare e modificare la tesi d'investimento, le definizioni dei target, i pilastri e i parametri utilizzati per l'ideation e la prevalutazione delle opportunità.

La prima dashboard sarà dedicata alla configurazione del mandato e ai selettori per restringere il perimetro di una sessione di ideation o dei risultati mostrati. Knowledge base, ricerca, skill specialistiche, gestione delle opportunità e risultati dei test sono ambiti successivi.

I form di ricerca e le schede riutilizzabili di spazio, opportunità e concept sono descritti in [Ideation — Input e output](ideation-input-output.md). È previsto un campo facoltativo **«Altri input e indicazioni»** in tutti e tre i form, accanto ai parametri preimpostati. Questi contenuti appartengono alla singola richiesta e non modificano automaticamente il mandato.

La struttura delle future schede di valutazione e la loro restituzione nella dashboard sono descritte in [Valutazione e scoring](ideation-valutazione-scoring.md): profilo sui pilastri, vincoli, motivazioni, evidenze e lacune. La struttura generale è approvata. Sono documentate prime rubriche e calibrazioni concettuali manuali per [spazio, revisione 0.2](calibrazione-spazio.md), [opportunità, revisione 0.2](calibrazione-opportunita.md) e [concept](calibrazione-concept.md). La revisione 0.2 del concept aggiunge QP, QS e QV; i precedenti profili C1–C5 restano riferiti alla revisione 0.1. I riscontri dell'utente restano limitati agli esempi condivisi; verifiche reali e ripetibilità sono ancora da svolgere. Non sono definiti pesi o totali numerici.

Le sezioni e gli identificativi dei campi seguenti sono una proposta organizzativa. I valori indicati come concordati derivano dalla conversazione; gli elementi aperti non devono essere completati automaticamente.

## 2. Regole comuni dei campi

Ogni criterio dovrà poter esprimere:

| Campo | Tipo | Significato |
| --- | --- | --- |
| Identificativo | Testo tecnico stabile | Riferimento del criterio, indipendente dalla sua etichetta. Gli identificativi proposti qui non definiscono ancora un'API. |
| Etichetta e spiegazione | Testo | Significato leggibile per chi configura il mandato. |
| Valore | Testo, numero, intervallo o selezione | Contenuto effettivamente utilizzato nella valutazione. |
| Natura | Selezione | Definizione del perimetro, vincolo, obiettivo orientativo, preferenza o riferimento per i test. |
| Stato di definizione | Selezione | Definito oppure da definire. Un campo aperto non vale zero e non equivale a un'esclusione. |
| Unità e base di calcolo | Testo/selezione, ove pertinente | Euro, percentuale, mesi; per prodotto, per cliente, annuale, mensile, cumulato. |
| Eccezioni e note | Testo | Flessibilità consentita e condizioni da considerare. |

La dashboard dovrà distinguere uno stato di configurazione «da definire» da un dato «non verificato» relativo a una specifica opportunità.

I limiti di una fascia orientativa non diventano automaticamente soglie di esclusione. In particolare, una fascia di soglie massime CAC del 15–25% non implica che un CAC inferiore al 15% sia indesiderabile.

Distinguere due azioni: **modificare il mandato generale** cambia i criteri di riferimento; **applicare selettori** restringe il campo della ricerca o della visualizzazione mantenendo il mandato invariato. I filtri non possono ampliare implicitamente il mandato o disattivarne i vincoli.

## 3. Struttura e campi

### A. Campi del mandato

La fonte dei testi, dei valori iniziali, della natura dei parametri e degli identificativi è ora [Mandato dello studio](mandato-studio.md), versione **M-2026-10-28-01**. Le sezioni prima raccolte qui sono state trasferite senza modificarne i valori. La dashboard dovrà leggere la versione dichiarata attiva per la sessione; il riferimento qui identifica soltanto la fotografia iniziale.

| Gruppo di campi | Controlli futuri |
| --- | --- |
| Tesi e obiettivo dello studio | Testi modificabili, descrizione dell'ambizione e dell'obiettivo di cassa. |
| Clienti e geografia | Definizioni, esempi, soglie e relazioni logiche del perimetro. |
| Pilastri qualitativi | Titoli, descrizioni, segnali, esempi e regole trasversali. |
| Modello commerciale e operatività | Modelli ammessi, incasso, autonomia, supporto e condizioni operative. |
| Obiettivi economici | Importi, intervalli, orizzonti, natura dei criteri e condizioni di flessibilità. |
| Canali e acquisizione | Canali, riferimenti CAC/CPL, assunzioni e base di calcolo. |

Gli identificativi sono proposte documentali, non un'API già implementata. I campi ancora aperti rimangono tali: l'interfaccia non deve introdurre valori impliciti.

### B. Selettori per restringere il perimetro

Requisito concordato: poter scegliere quali parti del perimetro esplorare o visualizzare, per esempio solo professionisti, solo microimprese oppure entrambi. Il mandato generale resta il riferimento; la selezione serve a concentrare una specifica sessione o vista.

Campi e comportamenti proposti:

| Identificativo | Controllo previsto | Opzioni e comportamento iniziale |
| --- | --- | --- |
| `filtri.tipologie_clienti` | Selettore multiplo, per esempio caselle di selezione | Professionisti / Microimprese. Entrambi selezionati come impostazione iniziale; possibilità di selezionarne uno solo. «Imprese» indica qui le microimprese definite nel mandato. |
| `filtri.cluster_clienti` | Selettore multiplo gerarchico | Cluster pertinenti alle tipologie selezionate, quando saranno mappati. Inizialmente nessuna restrizione aggiuntiva; opzioni ancora da definire. |
| `filtri.settori_segmenti` | Selettore multiplo | Settori o segmenti da includere, disponibili dopo la mappatura. Inizialmente tutti quelli ammessi dal mandato, senza restrizioni aggiuntive. |
| `filtri.attivita_processi` | Selettore multiplo | Attività o processi su cui concentrare l'esplorazione, quando presenti nella mappatura. Inizialmente nessuna restrizione aggiuntiva. |
| `filtri.modelli_ricavo` | Selettore multiplo | Abbonamento / Pagamento per output. Inizialmente entrambi, in coerenza con i modelli ammessi. Selezionare solo output non cambia la preferenza generale per l'abbonamento. |
| `filtri.intervallo_economico` | Intervallo numerico facoltativo con unità e metrica visibili | Possibile restrizione su ARR per abbonamento o ricavi annui per output. Nessun filtro iniziale. Le due metriche restano separate e un limite esplicito della vista non modifica le fasce orientative del mandato. |

Regole di funzionamento proposte:

- Le selezioni all'interno dello stesso campo si sommano: «professionisti + microimprese» include chi appartiene ad almeno una categoria. I filtri di campi diversi si applicano insieme.
- Un professionista che è anche microimpresa resta incluso selezionando una qualsiasi delle categorie pertinenti; con entrambe selezionate non viene duplicato.
- Il selettore delle tipologie richiede almeno una categoria; per gli altri campi, l'assenza di una restrizione significa «tutti quelli ammessi». La dicitura deve essere esplicita.
- Mostrare un riepilogo dei filtri attivi e un comando per tornare all'intero perimetro del mandato.
- Le opzioni dei selettori dipendenti devono essere coerenti con le selezioni superiori. Un eventuale filtro diventato incompatibile va segnalato prima dell'applicazione, senza azzerarlo silenziosamente.
- Conservare, insieme alla valutazione, la versione del mandato e i filtri applicati, così da spiegare il perimetro effettivamente esplorato.
- Distinguere «nessun risultato corrispondente» da «informazioni insufficienti per applicare il filtro». Un dato sconosciuto non va presentato come esclusione certa.
- La disponibilità iniziale del selettore professionisti/microimprese non dipende dalla futura mappatura dei cluster. I selettori senza opzioni mappate devono risultare non ancora disponibili, senza inventare tassonomie.

Esempio: mandato generale rivolto a professionisti e microimprese; sessione limitata a «professionisti» e «abbonamento». Restano validi ads obbligatorie, criteri economici e condizioni operative. Per tornare a includere le microimprese basta modificare la selezione, senza riscrivere la tesi.

## 4. Uso del mandato nelle valutazioni future

Questa sezione descrive il risultato atteso dall'uso della configurazione, non una schermata da implementare ora.

Ogni valutazione dovrebbe riportare:

1. Cliente, attività e risultato desiderato.
2. Ragione concreta dell'opportunità e alternative attuali.
3. Coerenza con i criteri ed eventuali incompatibilità.
4. Scenario economico essenziale, assunzioni e principali fragilità.
5. Informazioni mancanti e ipotesi prioritarie da validare.

Esiti: **coerente**, **da approfondire**, **fuori mandato**, sempre motivati, con le regole e le azioni successive distinte nel [sistema operativo documentale](ideation-sistema-operativo.md).

Separare fatti supportati da evidenze, assunzioni e dati mancanti. Un dato mancante non dimostra un'incompatibilità. «Coerente» significa coerente con il mandato sulla base delle informazioni disponibili, non validato commercialmente.

Le skill specialistiche forniranno successivamente evidenze su competitor, clienti, domanda, trend, pubblicità e altri aspetti. La lead generation misura interesse e costo del contatto: non dimostra automaticamente vendite, CAC o disponibilità a pagare.

## 5. Comportamenti proposti per la futura dashboard

Questi sono requisiti proposti per l'interfaccia futura, non funzionalità già presenti.

- Consultare e modificare testi, numeri, intervalli, natura dei criteri e relative note.
- Applicare i selettori della sezione 3.B per restringere il campo, mantenendo distinta questa operazione dalla modifica del mandato.
- Nei futuri form di ideation, permettere richieste libere, compilazione tramite parametri e uso combinato. Includere sempre «Altri input e indicazioni», conservando il testo e distinguendo spunti e vincoli anche al suo interno, come descritto nel documento collegato.
- Mostrare definizioni, unità e periodi vicino ai valori; consentire lo stato «da definire».
- Mantenere un'unica configurazione effettivamente letta dagli agenti e una sintesi leggibile del mandato.
- Segnalare incoerenze fra tesi testuale, definizioni e parametri prima di salvare; nessuna riscrittura silenziosa dei testi.
- Salvare versioni identificabili con data e riepilogo delle modifiche; mostrare la versione attiva.
- Associare le valutazioni alla versione usata e agli eventuali filtri applicati. Una modifica non riscrive gli esiti precedenti; un'eventuale rivalutazione deve essere esplicita.
- Restituire le valutazioni dei tre livelli secondo il documento collegato: punteggi 0–3, NV, vincoli separati, motivazioni, fonti e solidità delle evidenze. Mostrare lacune e stato di bozza delle rubriche senza presentare un totale non ancora definito.
- Mostrare la revisione della rubrica e distinguere valutazioni su casi simulati, ipotesi di mercato ed evidenze reali. Rendere consultabili i casi di calibrazione pertinenti e il motivo dei cambiamenti tra valutazioni.
- Per i concept rendere visibili bontà del problema (QP), adeguatezza della soluzione (QS) e forza della value proposition (QV), ciascuna con voto 0–3/NV, motivazione e supporto. Presentare questa qualità dell'offerta insieme ai pilastri e ai conti, senza un totale che nasconda una debolezza o trasferisca automaticamente i vecchi voti ai nuovi giudizi.
- Per i concept mostrare separatamente incassi e calendario, costi iniziali/operativi/acquisizione, saldo di recupero nel primo mese, saldo di cassa, costi del servizio venduto e dimensione annuale. Mantenere visibili natura dei parametri e scenari di sensibilità; un saldo positivo non implica da solo profitto sostenibile.
- Evitare punteggi e pesi numerici non concordati. La natura di un criterio e le sue eccezioni devono essere visibili.

Controlli di coerenza proposti:

- Intervalli con estremi ordinati, importi non negativi, percentuali entro 0–100 e periodi positivi.
- Differenza visibile fra limite esclusivo degli addetti e limiti inclusivi economici della microimpresa.
- Differenza visibile fra fascia desiderata di ricavo e potenziale massimo del mercato.
- Segnalazione dei conflitti tra ipotesi di acquisizione, calendario degli incassi e recupero dei costi; i dati mancanti producono una richiesta di approfondimento, non un calcolo inventato.
- Le scelte oggi obbligatorie, come ads e recupero dei costi nel primo mese, potranno essere cambiate deliberatamente in una nuova versione del mandato, senza essere trattate come codice immutabile.

## 6. Punti volutamente aperti

- Mappatura e clusterizzazione di professionisti e microimprese.
- Budget universale di sviluppo: non definito e non richiesto come filtro in ideation.
- Definizione contabile e verifica dettagliata del margine superiore all'80%.
- Base fiscale degli importi e allocazione puntuale dei costi interni: non specificate; da dichiarare quando si costruiscono scenari economici, senza attribuire scelte già approvate allo studio.
- Percentuali di tolleranza sulle fasce e limiti quantitativi per demo, manutenzione e assistenza.
- Metodo e soglie dettagliate per passare dai test alla costruzione.
- Architettura tecnica, persistenza, integrazioni, layout e design visivo della dashboard.

Questi punti non vanno compilati automaticamente con valori presentati come decisioni di Mamazen.
