# Ideation — Sistema operativo documentale

Data: 28 ottobre 2026.
Versione: **IDEATION-0.1**.
Aggiornamento: 28 ottobre 2026, collegamento al modello condiviso di gate di ricerca GATE-0.1.
Stato: consolidamento delle strutture concordate, con prime regole operative qualitative proposte dall'assistente. Utilizzabile come procedura assistita in chat; affidabilità del modello e risultati commerciali ancora da verificare.

## 1. Scopo e confini

Aiutare l'Head of Product Studio a scoprire piste di prodotto anche in attività sconosciute, svilupparle e giudicarle rispetto al mandato. La macchina deve alternare esplorazione e approfondimento: può partire da un competitor, un settore, una professione, un'attività o una domanda aperta.

Spazio, opportunità e concept sono oggetti con granularità diversa. La scelta dell'output determina dove arrivare, senza imporre la produzione di tutte le schede intermedie. Le informazioni necessarie vanno comunque ricostruite.

Questa versione collega i documenti e fornisce istruzioni riusabili. La presenza dei file non configura un servizio, non addestra un modello e non esegue ricerche automaticamente. L'Excel ricevuto è stato esaminato: il suo uso come lente di selezione progressiva è descritto nei [gate di ricerca](ideation-gate-ricerca.md). Arricchimento della base, skill specialistiche, automazione e dashboard appartengono alle fasi successive. I test ads rimangono successivi al concept.

## 2. Documenti di riferimento

| Documento | Responsabilità | Riferimento iniziale |
| --- | --- | --- |
| [Mandato dello studio](mandato-studio.md) | Tesi, definizioni, pilastri, criteri economici e loro natura. | M-2026-10-28-01 |
| [Input e output](ideation-input-output.md) | Form, campi delle tre schede, flag e passaggi fra livelli. | IO-0.1 |
| [Valutazione e scoring](ideation-valutazione-scoring.md) | Scala, vincoli, supporto delle affermazioni e descrittori. | Spazio 0.2, opportunità 0.2, concept 0.2 |
| Questo documento | Conduzione della ricerca, priorità relative e prossime azioni. | IDEATION-0.1 |
| [Gate di ricerca](ideation-gate-ricerca.md) | Preselezione dei target, arricchimento progressivo e controllo dell'effort. | GATE-0.1 |
| [Istruzioni riusabili](ideation-istruzioni.md) | Avvio in chat e modelli di richiesta e restituzione. | ISTRUZIONI-0.1 |
| [Calibrazioni](calibrazione-concept.md) | Esempi sintetici per comprendere i giudizi, insieme ai casi di [spazio](calibrazione-spazio.md) e [opportunità](calibrazione-opportunita.md). | Revisioni indicate nei singoli file |
| [Dashboard futura](dashboard-configurazione-mandato.md) | Specifica dell'interfaccia e dei selettori, da conservare. | Nessuna interfaccia implementata |

Le fonti hanno responsabilità distinte: i casi simulati non definiscono soglie del mandato e le istruzioni brevi non sostituiscono le rubriche. Se due documenti sono incoerenti, segnalare il conflitto e non scegliere silenziosamente la formulazione più favorevole. Le versioni iniziali qui riportate non sostituiscono la scelta della versione attiva nella singola sessione.

## 3. Avvio di una sessione

Acquisire la richiesta libera, gli eventuali parametri e i riferimenti, secondo [Input e output](ideation-input-output.md). Conservare il testo originale ed esplicitare gli elementi estratti.

| Elemento operativo | Comportamento |
| --- | --- |
| Risultato richiesto | Spazi, opportunità o concept. Se ambiguo, chiarire prima di sviluppare schede di granularità diversa; intanto si può ricostruire il contesto comune. |
| Mandato e rubriche | Dichiarare le versioni realmente disponibili e usate. Senza il mandato non dichiarare una valutazione conforme allo studio. |
| Vincoli e spunti | Usare il flag per ciascun elemento, compresi quelli ricavati dal testo libero. Un limite esplicito dell'utente prevale sulle ipotesi generate. Un conflitto con il mandato va evidenziato. |
| Numero di risultati | Seguire la richiesta. In sua assenza, proporre fino a tre risultati distinti: scelta operativa modificabile, non criterio del mandato o quota da riempire. |
| Shortlist dei target | Se prevista una preselezione dall'Excel, definire l'ampiezza e i limiti della ricerca. Il numero dei target è distinto dal numero di schede spazio, opportunità o concept; non eredita il riferimento ai tre risultati. |
| Conduzione | Proseguire autonomamente fino all'output richiesto. Se l'utente chiede confronto o selezione intermedia, lavorare in modo guidato. |
| Ampiezza e limiti | Dichiarare perimetro effettivo, fonti accessibili e limiti indicati dall'utente. Le parti non esplorate restano tali; nessuna promessa di copertura esaustiva. |
| Budget e azioni esterne | La richiesta di ideation non avvia campagne, acquisti o contatti con terzi. La ricerca usa gli strumenti e i materiali disponibili. |

Chiedere chiarimenti quando un'ambiguità cambia il mandato applicabile o impedisce una scelta sensata. Non trasformare tutti i campi mancanti in domande all'utente: molte informazioni sono precisamente ciò che la macchina deve cercare. Se non si può risolvere un conflitto, sospendere soltanto la parte dipendente e proseguire sulle parti indipendenti.

## 4. Un ciclo di ricerca

```mermaid
flowchart LR
    A[Richiesta e mandato] --> B[Ricostruisci il contesto necessario]
    B --> C[Esplora piste differenti]
    C --> D[Seleziona e approfondisci]
    D --> E[Valuta e cerca obiezioni]
    E --> F[Restituisci output e prossima azione]
    E -->|Lacuna decisiva risolvibile nel ciclo| D
```

### 4.1 Ricostruire il contesto e aprire piste

1. Riconoscere ciò che l'input descrive già e ciò che manca al livello richiesto. Da un prodotto osservato risalire a cliente, attività e risultato prima di ipotizzarne una versione migliore.
2. Esplorare piste che differiscono per cliente, attività, punto della value chain, risultato o apertura commerciale. Variazioni cosmetiche e slogan diversi non costituiscono nuove piste.
3. Collegare, quando disponibili, categorie di clienti, attività, strumenti, cambiamenti e bisogni. Cercare anche piste adiacenti meno evidenti, mantenendo i vincoli dell'utente.
4. Separare la lista iniziale delle piste dai risultati sviluppati. La prima aiuta a non fermarsi alla prima idea; non richiede una scheda completa o uno scoring per ogni voce.

Non servono tutti i settori mappati per avviare una sessione. Con materiali limitati dichiarare che cosa deriva dai documenti, che cosa è un'ipotesi e che cosa non si conosce. Non descrivere la memoria generale del modello come una ricerca aggiornata.

### 4.2 Selezionare e approfondire

Applicare prima il perimetro e i vincoli pertinenti. Tra le piste rimaste, scegliere dove investire ricerca usando le domande della sezione 6, senza inventare un totale numerico.

Approfondire soprattutto le informazioni che possono cambiare la scelta. Una ricerca a 360° non obbliga a compilare un rapporto completo su ogni settore: l'ampiezza iniziale serve a trovare piste, il dettaglio serve a decidere su quelle selezionate.

| Output | Domande minime da affrontare al relativo livello |
| --- | --- |
| Spazio | Di che contesto si tratta? Quali soggetti e 2–3 passaggi sono coinvolti? Quale risultato generale conta? Quali approcci esistono? Perché merita attenzione rispetto al mandato? |
| Opportunità | Quale cliente svolge quale attività? Quale risultato cerca? Come funziona il processo, con ruoli, input, output e dipendenze? Quanto pesa il bisogno? Come lo soddisfa oggi? Perché potrebbe pagare una soluzione diversa? |
| Concept | Per quale problema specifico? Con quale promessa e meccanismo? Che cosa copre e che cosa lascia fuori? Perché sceglierlo? A quale prezzo e con quale acquisizione? Lo scenario recupera i costi iniziali e rimane sostenibile? |

I dettagli delle schede restano quelli di [Input e output](ideation-input-output.md). Si può arrivare al concept senza pubblicare prima due rapporti intermedi, ma non senza aver motivato cliente, problema e contesto necessari.

### 4.3 Valutare e cercare obiezioni

Usare il protocollo e i descrittori di [Valutazione e scoring](ideation-valutazione-scoring.md). Separare stato dei vincoli, profilo 0–3/NV e solidità del supporto alle singole affermazioni. Per i concept esplicitare anche **QP, QS, QV**.

Riesaminare la pista cercando una ragione concreta per cui potrebbe non funzionare: bisogno debole, alternative sufficienti, attrito di adozione, dati indisponibili, lavoro interno ricorrente, ads poco plausibili o conti fragili. Non basta riformulare in positivo la descrizione generata.

Per le ipotesi decisive dichiarare quale informazione contraria farebbe cambiare il giudizio. Un controllo critico svolto dallo stesso assistente non è una verifica indipendente né una prova sul mercato.

### 4.4 Chiudere il ciclo

Restituire il numero di risultati sostenibili entro i limiti della sessione, anche inferiore a quello richiesto. Per ciascuno distinguere contenuto, valutazione e prossima azione.

Se mancano i presupposti per l'output richiesto, consegnare gli elementi utili già ricostruiti e indicare la lacuna che impedisce di completarlo. Un abbozzo non va presentato come concept completo; un'ipotesi credibile può invece essere un concept, senza essere validata.

Chiudere quando l'output e il controllo critico sono completati, quando si esauriscono i limiti concordati oppure quando le lacune decisive richiedono fonti non disponibili. Non ripetere ricerche equivalenti senza una nuova domanda o fonte. Registrare dove riprendere, evitando una catena indefinita di approfondimenti.

## 5. Esito e prossima azione sono due cose distinte

Gli esiti del mandato rimangono quelli già previsti. Questa versione ne rende esplicita l'interpretazione operativa, senza introdurre soglie numeriche.

| Esito | Quando usarlo |
| --- | --- |
| Coerente | Esiste una spiegazione plausibile di compatibilità al livello valutato e non emergono incompatibilità obbligatorie. Esplicitare le assunzioni da cui dipende; se un vincolo applicabile resta decisivo e non valutabile, usare «da approfondire». |
| Da approfondire | Una lacuna o contraddizione impedisce di concludere, oppure la pista richiede una revisione sostanziale per diventare plausibile. Non equivale a un rifiuto. |
| Fuori mandato | È identificata un'incompatibilità con una definizione del perimetro o un vincolo obbligatorio, non soltanto un punteggio basso. Precisare segmento, offerta o scenario interessato. |

Per «coerente» il supporto può ancora essere ipotetico: riguarda la logica dello scenario, non la sua dimostrazione. Un vincolo non applicabile al livello non risulta superato.

La prossima azione descrive che cosa conviene fare con quella specifica versione della pista:

| Azione proposta | Condizione e contenuto da restituire |
| --- | --- |
| Proseguire al livello richiesto | I presupposti sono sufficienti per costruire un'ipotesi motivata e il livello non è ancora raggiunto. Procedere senza chiedere selezioni manuali a ogni passaggio, salvo richiesta dell'utente. |
| Approfondire una domanda decisiva | Specificare la domanda, perché potrebbe cambiare la scelta e quale informazione servirebbe. L'incertezza non diventa zero. |
| Riformulare | Un ostacolo riguarda problema scelto, segmento, perimetro, promessa, prezzo o scenario. Indicare una modifica plausibile da riesaminare; non assumerne automaticamente la riuscita. |
| Non proseguire nella formulazione corrente | Esiste un'incompatibilità motivata oppure la formulazione è debole senza una correzione plausibile entro i limiti attuali. Conservare il motivo; non estendere il giudizio ai genitori. Una formulazione debole ma interna al mandato non diventa per questo «fuori mandato». |
| Proporre il concept alla successiva fase di validazione | È un'offerta formulata, valutata anche su QP/QS/QV, con ipotesi commerciali ed economiche credibili e principali fragilità esplicite. Nessun ostacolo decisivo noto viene nascosto. È una raccomandazione, non una campagna avviata o una previsione di successo. |

Un basso punteggio QS o QV può portare a riformulare il concept conservando un problema interessante. Un concept scartato non scarta automaticamente opportunità o spazio. La fase di test definirà separatamente esperimenti e criteri di decisione.

## 6. Priorità relativa e scelta della prossima ricerca

La priorità riguarda le piste della sessione e il tipo di lavoro richiesto. Non è una proprietà assoluta di un settore o una probabilità di successo.

Per ordinare poche piste, motivare il confronto su:

1. **Valore e apertura:** importanza del risultato e ragione concreta per scegliere una nuova offerta.
2. **Compatibilità operativa e commerciale:** autonomia, raggiungibilità tramite ads ed equilibrio economico, valutabili al livello corrente.
3. **Fragilità decisive:** da quali assunzioni dipende l'interesse e quanto sono supportate, comprese le informazioni contrarie.
4. **Utilità del prossimo approfondimento:** se una domanda accessibile può cambiare la scelta e quale impegno richiede.

Questo elenco è una guida al confronto, non un ordine di pesi o una formula. Una pista nuova con poco supporto può meritare ricerca; una pista già approfondita può essere più pronta a diventare concept. Dichiarare se la priorità è **di esplorazione**, **di approfondimento** oppure **di sviluppo del concept**. La candidatura ai test è una raccomandazione separata.

Restituire posizione relativa e una breve ragione del confronto. Se due piste non sono confrontabili, dichiararlo o mantenerle a pari priorità. Niente somma dei punteggi, media con QP/QS/QV, graduatoria a decimali o soglia automatica di Proceed/Drop.

## 7. Informazioni da conservare

In una sessione documentale gli identificativi sono etichette leggibili, non un formato tecnico definitivo.

| Registrazione | Contenuti minimi |
| --- | --- |
| Sessione | Identificativo/data, richiesta originale, output, mandato e rubriche, filtri, vincoli/spunti, limiti e materiali effettivamente utilizzati. |
| Oggetto | Identificativo, revisione, livello, perimetro e collegamenti alle schede di origine eventualmente presenti. |
| Affermazione e supporto | Contenuto, fonte effettivamente consultata o ipotesi con ragionamento, geografia/periodo/unità se quantitativa, limiti di pertinenza ed elementi contrari. |
| Valutazione | Versioni, stati dei vincoli, punteggi e motivazioni per criterio, QP/QS/QV per concept, assunzioni e lacune. |
| Decisione | Esito, prossima azione, priorità relativa quando utile, ragione e condizione per riesaminare la pista. |
| Chiusura | Risultati consegnati, piste accantonate con motivo, copertura effettiva, questioni aperte e punto da cui riprendere. |

Non basta fornire un elenco di link: collegare ogni fonte alla specifica affermazione sostenuta. Se non si sono consultate fonti esterne, dirlo. Una ricerca senza risultati non dimostra l'assenza di concorrenti o di bisogno.

Quando una scheda diventa input, trasferire contenuti e provenienza, non voti, vincoli inventati o bacini non pertinenti. Nuove informazioni producono una revisione riconoscibile con ciò che è cambiato.

La lettura del repository e l'ideation in chat non implicano il salvataggio automatico di tutte le future ricerche: dichiarare che cosa è stato effettivamente registrato. Le regole di persistenza tecnica saranno definite con l'automazione.

## 8. Chiusura della fase e passaggio alla KB

La base documentale comprende mandato, input, oggetti, valutazioni, procedura, istruzioni e calibrazioni sintetiche. È sufficiente per impostare una prima sessione assistita; il comportamento stabile del modello deve ancora essere verificato con casi reali.

Le nuove scelte operative di questa versione sono: fino a tre risultati in assenza di un numero richiesto, un ciclo con chiusura esplicita, priorità comparative motivate e azioni separate dagli esiti del mandato. Sono impostazioni proposte e modificabili, non nuovi vincoli economici approvati.

L'Excel è stato letto e il modello di selezione progressiva è stato condiviso con l'utente: una lente per decidere dove spendere ricerca e approfondire soltanto le piste selezionate. I [gate di ricerca](ideation-gate-ricerca.md) raccolgono struttura e arricchimenti leggeri concordati; il prossimo passo è definire operativamente il Gate 1. Eventuali tassonomie descriveranno il contesto: non proveranno automaticamente bisogni, clienti paganti o attrattività di una pista.

Restano fuori da questa chiusura l'implementazione di agenti e servizi, la verifica ripetuta del modello, l'integrazione delle fonti, il design della dashboard e l'esecuzione dei test commerciali.
