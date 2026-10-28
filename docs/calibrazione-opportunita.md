# Calibrazione iniziale dell'opportunità — Casi di riferimento

Data: 28 ottobre 2026.
Rubrica: opportunità, revisione 0.2 di [Valutazione e scoring](ideation-valutazione-scoring.md).

Stato: applicazione manuale a venti casi simulati, con revisione concettuale dei descrittori. Non sono state eseguite venti valutazioni indipendenti di un modello, ricerche di mercato o prove commerciali. I profili sono riferimenti proposti dall'assistente; non sono etichette di riferimento già approvate dall'utente.

## 1. Metodo e perimetro

Tutte le informazioni e i numeri sono inventati per l'esercizio. Vengono assunti veri soltanto all'interno del caso; il supporto sul mercato reale rimane **ipotesi simulata**, senza fonti esterne.

La verifica combina lettura critica dei descrittori, assegnazione ragionata dei profili e confronto di varianti. Mantiene separati coerenza, supporto e vincoli. Non introduce pesi, medie, soglie di selezione o una probabilità di successo.

I profili sono nell'ordine **[O1, O2, O3, O4, O5]**. NV indica una base insufficiente per il giudizio, compresi dati contraddittori non ancora riconciliati; specificare sempre il motivo. Un processo sconosciuto non è un processo incompatibile.

Si valuta l'opportunità, non ancora un'offerta di prodotto. I riferimenti di prezzo e acquisizione sono ipotesi di scenario e non un concept definitivo o un piano di test ads. Il recupero di tutti i costi nel primo mese non viene dichiarato superato: manca una soluzione specifica con costi e calendario degli incassi.

L'utente ha condiviso in chat la distinzione illustrativa fra prodotto autonomo usato da un professionista (O4 = 3 nelle condizioni descritte), servizio con lavorazione interna personalizzata per pratica (O4 = 0 nel relativo perimetro) e processo sconosciuto (O4 = NV). Il riscontro non viene esteso automaticamente agli altri descrittori o ai venti profili.

## 2. Caso base P00

**Opportunità candidata: gestione del quadro documentale della formazione per consulenti italiani con partita IVA che assistono microimprese.**

Il perimetro riguarda raccogliere e associare informazioni, mantenere un quadro aggiornato e individuare elementi da gestire. Non implica che un software possa sostituire ogni valutazione professionale o erogare formazione.

Assunzioni del caso:

- Il consulente è utilizzatore e acquirente; sceglie autonomamente strumenti per questo lavoro.
- Il risultato ha conseguenze economiche e operative importanti; il beneficio è comprensibile e riconosciuto nel caso.
- Gli approcci attuali coprono parte del lavoro ma lasciano una difficoltà rilevante. Il cambiamento è plausibile, senza condizioni particolarmente favorevoli già dimostrate.
- Il processo è descritto: raccolta dei dati, associazione ai soggetti pertinenti, controllo e aggiornamento. Per ciascun passaggio sono identificati responsabile, input e output.
- Il consulente può continuare a svolgere il proprio lavoro professionale. Gli input necessari al perimetro autonomo sono ottenibili e standardizzabili; il futuro team del prodotto non deve verificare manualmente ogni pratica.
- Le ipotesi economiche sono quelle della sezione seguente. Non sono stime reali del numero di consulenti, dei prezzi accettabili o delle prestazioni degli annunci.

Profilo assegnato: **[3, 3, 2, 3, 2]**.

| Criterio | Motivazione |
| --- | --- |
| O1 = 3 | Utilizzo e decisione d'acquisto sono vicini, con autonomia esplicitata. |
| O2 = 3 | Il risultato ha peso ed è comprensibile; il giudizio non deriva dalla sola frequenza o dall'esistenza di obblighi. |
| O3 = 2 | È presente una ragione plausibile per cambiare, ma non una condizione particolarmente favorevole già descritta. |
| O4 = 3 | Il perimetro può essere gestito dal cliente senza lavorazione interna per pratica. Il lavoro professionale del cliente non equivale a un costo umano del nostro team. |
| O5 = 2 | Lo scenario è coerente nelle unità e nei calcoli, ma dipende da ipotesi su prezzo, volume dei lead, conversione e permanenza dei clienti. Non giustifica 3 né prova il pareggio. |

### Scenario economico base

| Grandezza | Assunzione dell'esercizio |
| --- | --- |
| Bacino pertinente N | 50.000 unità potenzialmente paganti nel perimetro e periodo considerati. Non è una soglia minima del mandato. |
| Lead L | 10.000 unità distinte e pertinenti nei primi dodici mesi, normalizzate alla stessa unità d'acquisto di N. Disponibilità e raggiungibilità sono ipotesi da verificare. |
| Conversione q | 5% dei lead diventa cliente. |
| Ricavo ricorrente annuo per cliente P | 300 €, ipotizzato con un riferimento di spesa pertinente ma non validato. |
| CPL | 2 €. |
| Altri costi di acquisizione | Assunti pari a zero soltanto per isolare il caso base e le varianti che non li modificano. Non è un valore predefinito per ricerche reali. |
| Permanenza | Nell'esercizio tutti i clienti acquisiti sono ancora attivi al dodicesimo mese. |
| Soglia CAC di scenario | 20% di P, scelta per l'esercizio dentro la fascia orientativa del mandato. Non viene salvata come nuova soglia globale. |

Calcoli:

- Clienti attivi al dodicesimo mese = 10.000 × 5% = **500**.
- ARR al dodicesimo mese = 500 × 300 € = **150.000 €**. Non sono gli incassi effettivi del primo anno.
- Spesa di acquisizione ipotizzata = 10.000 × 2 € = **20.000 €**.
- CAC delle sole ads = 2 € / 5% = **40 €**. Nel caso base coincide con il CAC complessivo perché gli altri costi di acquisizione sono assunti nulli; vale il **13,33%** del ricavo annuo per cliente.
- CAC massimo dello scenario = 300 € × 20% = **60 €**.
- CPL massimo coerente con quel limite e quella conversione = 60 € × 5% = **3 €**.

Il CAC inferiore al 15% non è una penalità. Il limite dipende dalla percentuale massima scelta nello scenario; il 15–25% non è una fascia dentro cui il CAC debba necessariamente cadere.

La previsione di 10.000 lead non è dimostrata da N = 50.000. Richiede una successiva verifica di raggiungibilità, domanda, qualità dei contatti e costi. La coerenza aritmetica è necessaria, ma non dimostra la fattibilità commerciale.

## 3. Varianti applicate

Ogni variante mantiene le condizioni di P00 salvo le sostituzioni esplicitate. In un caso reale una nuova informazione può modificare più criteri: non assumere che siano indipendenti soltanto perché qui vengono confrontati in modo controllato.

| Caso | Variazione | Profilo assegnato | Ragione del giudizio |
| --- | --- | --- | --- |
| P01 — Responsabile ignoto | Non è noto chi debba svolgere i passaggi necessari al risultato; le altre informazioni rimangono disponibili. | [3, 3, 2, NV, 2] | O4 non può essere dedotto dal solo nome dell'attività. Non attribuire automaticamente il lavoro al cliente o al nostro team. |
| P02 — Lavorazione interna per pratica | Il risultato richiesto nel perimetro impone una verifica personalizzata del nostro team per ciascuna pratica, inseparabile dal servizio. | [3, 3, 2, 0, 2] | Il contesto può essere commercialmente interessante ma il perimetro contrasta con l'autonomia. Non compensare O4 con una media. |
| P03 — Eccezioni frequenti | Una parte è standardizzabile, ma eccezioni note e frequenti richiedono interventi interni. | [3, 3, 2, 1, 2] | La fragilità deriva dal processo descritto, non dalla mancanza di una fonte. |
| P04 — Dipendenze residue | È individuabile un risultato autonomo di valore, ma alcuni input o dipendenze possono richiedere eccezioni da risolvere nel perimetro del futuro prodotto. | [3, 3, 2, 2, 2] | Esiste una strada plausibile, con condizioni ancora da approfondire. Non dichiarare autonomia particolarmente favorevole. |
| P05 — Attività occasionale | L'attività è annuale, mantenendo conseguenze importanti, beneficio comprensibile e motivo per intervenire. | [3, 3, 2, 3, 2] | Nessuna frequenza minima; il modello di pagamento resta da scegliere. |
| P06 — Frequente ma marginale | L'attività è frequente ma i benefici sono marginali anche considerando l'accumulo nel tempo; il vantaggio e il ticket prima motivati da quel beneficio perdono la loro base. | [3, 0, 1, 3, 1] | La frequenza non sostituisce il valore. La nuova informazione indebolisce anche apertura e incastro commerciale: non modificare meccanicamente un solo criterio. |
| P07 — Acquisto difficile | Coordinamento e approvazioni rendono difficile una decisione breve, anche se esistono percorsi compatibili. | [1, 3, 2, 3, 2] | Si valutano gli effetti sul percorso, non il numero di ruoli in sé. |
| P08 — Percorso incompatibile | L'acquisto richiede obbligatoriamente diversi incontri personalizzati e trattative lunghe, senza percorso autonomo o demo breve. Sono stimati inoltre 90 € di attività commerciale per nuovo cliente, oltre alle ads; il numero di clienti è mantenuto invariato nell'esercizio. | [0, 3, 2, 3, 1] | O1 è incompatibile per il percorso. Il CAC complessivo diventa 130 €, il 43,33% di P: anche O5 si indebolisce. Il solo CAC ads di 40 € non rappresenta tutti i costi di acquisizione. |
| P09 — Alternative sconosciute | Mancano tutte le informazioni sulle alternative e sull'apertura commerciale. | [3, 3, NV, 3, 2] | Assenza di analisi non equivale a mercato libero. |
| P10 — Più competitor | Aumenta il numero dei competitor, senza cambiare vantaggio per il segmento o condizioni del cambiamento. | [3, 3, 2, 3, 2] | Nessuna penalità automatica per affollamento. |
| P11 — Apertura favorevole | Il vantaggio per il segmento è rilevante e il cliente può ottenerlo senza migrazioni o altri ostacoli sproporzionati. | [3, 3, 3, 3, 2] | O3 cresce per il vantaggio e il cambiamento favorevole, non per il numero di concorrenti o fonti. |
| P12 — Conversione più bassa | q passa dal 5% al 2%; CPL, prezzo e lead rimangono quelli del caso base. | [3, 3, 2, 3, 1] | Il CAC diventa 100 €, il 33,33% di P, e l'ARR ipotizzato scende a 60.000 €. Lo scenario richiede una revisione; non dimostra che ogni possibile prodotto nell'opportunità sia impossibile. |
| P13 — Nicchia e ticket maggiore | N = 1.000, P = 2.000 €/anno, q = 10%, CPL = 5 €, L = 750. La spesa pertinente e il valore sono assunti compatibili con P. | [3, 3, 2, 3, 2] | 75 clienti sostengono 150.000 € ARR e CAC = 50 €. Il volume di lead ipotizzato copre il 75% del bacino: non è dimostrato né motivo per assegnare 3. Nessun minimo universale di 50.000 soggetti. |
| P14 — Bacino grande, ticket basso | N = 250.000, P = 120 €/anno, q = 5%, CPL = 2 €, L = 25.000. | [3, 3, 2, 3, 1] | L'ARR ipotizzato raggiunge 150.000 €, ma CAC = 40 € assorbe il 33,33% di P. Il bacino maggiore non corregge l'incastro dell'acquisizione. |
| P15 — Ads inutilizzabili | È esplicitamente stabilito che gli acquirenti pertinenti non sono raggiungibili tramite ads nel perimetro considerato; il funnel ads del caso base cessa quindi di essere applicabile. | [3, 3, 2, 3, 0] | Il vincolo ads è incompatibile. Email, partnership o vendite organiche non lo sostituiscono. Non dedurre questa condizione dalla semplice assenza di annunci trovati. |
| P16 — Pagamento per output | N = 50.000, prezzo = 50 €/output, quattro acquisti per cliente nell'anno considerato, L = 15.000, q = 5%, CPL = 2 €. | [3, 3, 2, 3, 2] | 750 clienti × quattro output × 50 € = 150.000 € di ricavi annui; CAC = 40 €, pari al 20% dei 200 € pagati annualmente dal cliente. Non chiamare il risultato ARR né imporre l'abbonamento. |
| P17 — Unità incoerenti | N = 5.000 unità paganti, ma sono dichiarati 10.000 lead distinti pertinenti, definiti come unità d'acquisto dello stesso bacino, periodo e geografia. Nessuna spiegazione riconcilia i dati. | [3, 3, 2, 3, NV] | Lo scenario è incoerente e va riconciliato. Non usarlo per assegnare 2 o 3 e non trasformarlo automaticamente in esclusione dell'opportunità. |
| P18 — Non cerca software | Il cliente non sta cercando attivamente software, ma comprende facilmente il beneficio e riconosce il motivo per intervenire quando il risultato viene spiegato. | [3, 3, 2, 3, 2] | Ricerca attiva e valore riconoscibile sono diversi. L'ipotesi sul beneficio non dimostra una vendita o una conversione ads. |
| P19 — Acquirente da chiarire | Il segmento è noto ma non è noto chi possa autorizzare la spesa o quale percorso debba seguire; il conteggio delle unità paganti è assunto corretto nell'esercizio. | [NV, 3, 2, 3, 2] | Non assegnare 1 perché la scheda è incompleta né 3 perché il target è un professionista. |

## 4. Controlli dei numeri e della sensibilità

| Scenario | Clienti | Grandezza economica | Spesa acquisizione complessiva | CAC complessivo | CAC / pagamento annuo per cliente |
| --- | --- | --- | --- | --- | --- |
| P00 | 500 | 150.000 € ARR | 20.000 € | 40 € | 13,33% |
| P08 | 500 | 150.000 € ARR | 65.000 € | 130 € | 43,33% |
| P12 | 200 | 60.000 € ARR | 20.000 € | 100 € | 33,33% |
| P13 | 75 | 150.000 € ARR | 3.750 € | 50 € | 2,50% |
| P14 | 1.250 | 150.000 € ARR | 50.000 € | 40 € | 33,33% |
| P16 | 750 | 150.000 € ricavi annui effettivi, nell'esercizio | 30.000 € | 40 € | 20,00% |

La variazione P00 → P12 mostra perché uno scenario favorevole non è una conclusione robusta. Al prezzo di 300 € e con massimale CAC del 20%, il CAC massimo è 60 €; con CPL di 2 €, serve una conversione almeno pari a **3,33%**. Questo è un limite aritmetico condizionato alle ipotesi, non una previsione o un benchmark universale.

Il limite del 3,33% assume gli altri costi di acquisizione nulli. P08 mostra perché la formula CPL / conversione, da sola, non misura il CAC complessivo quando sono presenti attività commerciali, demo o altri costi. Contare ogni costo una sola volta nello scenario economico completo.

L'ARR sotto la fascia orientativa non comporta da solo esclusione. In P12 e P14 il voto debole deriva dall'incastro complessivo, compreso il costo di acquisizione, non da una soglia minima rigida introdotta nell'esercizio.

In P17, il limite L ≤ N vale perché sono espressamente definiti lead distinti normalizzati alla stessa unità economica, nello stesso bacino e periodo. Non vale automaticamente per contatti grezzi: una stessa impresa può generare più contatti. In quel caso occorre esplicitare deduplicazione e conversione fra contatto e cliente, senza confrontare grandezze diverse.

## 5. Correzioni introdotte nella revisione 0.2

- **Ruolo umano:** il lavoro professionale del cliente non è una lavorazione interna del team. Verificare responsabilità e dipendenze per passaggio prima di giudicare O4.
- **Valore riconoscibile:** non richiedere ricerca attiva di software o un acquisto già avvenuto per riconoscere un bisogno. Separare comprensibilità del beneficio, disponibilità a pagare e comportamento osservato.
- **Unità economiche:** conteggi di persone, contatti, imprese e clienti non sono intercambiabili. Specificare l'unità e il periodo delle conversioni.
- **Scenari fragili:** una combinazione che funziona soltanto sotto un'ipotesi favorevole non giustifica un voto particolarmente alto senza dichiararne la dipendenza. Controllare almeno una variazione dell'assunzione decisiva quando è disponibile uno scenario numerico.
- **Dati contraddittori:** segnalare il conflitto; se impedisce il giudizio, usare NV con il motivo. Non scegliere silenziosamente i dati favorevoli e non attribuire l'errore del modello economico al mercato.
- **CAC massimo:** la percentuale va dichiarata nello scenario o riferita al parametro attivo. La fascia del mandato non rappresenta un costo minimo da sostenere.
- **CAC completo:** distinguere costo delle ads e altri costi di acquisizione. CPL / conversione è soltanto la componente media quando sono presenti costi ulteriori; la soglia del mandato va confrontata con il costo complessivo dichiarato.
- **Effetti fra criteri:** una nuova informazione può indebolire più giudizi. Per esempio un beneficio marginale può rendere meno motivati anche vantaggio e prezzo; non mantenere automaticamente i voti precedenti.
- **Output e abbonamenti:** per il CAC usare quanto il cliente paga nell'anno, con frequenza dichiarata. Ricavi per output e ARR rimangono distinti.

## 6. Risultato e verifiche successive

Sono documentati venti profili manuali e i calcoli di sei scenari economici. Non sono misurate accuratezza, ripetibilità o efficacia di acquisizione; la copertura non esaurisce tutte le combinazioni possibili dei descrittori.

L'agente futuro dovrà ricevere la rubrica, il mandato e i riferimenti pertinenti, applicando il protocollo della sezione 8 del documento di scoring. La presenza dei file non configura o addestra automaticamente un modello.

Restano confronto dei profili con l'utente, casi reali con fonti e valutazioni ripetute. Il livello concept ha ora una [prima rubrica e calibrazione concettuale](calibrazione-concept.md), che tratta offerta specifica, costi iniziali e correnti, calendario degli incassi, CAC e recupero di tutti i costi nel primo mese. I test ads operativi rimangono successivi all'ideation.
