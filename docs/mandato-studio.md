# Mandato dello studio — Fonte di riferimento

Data: 28 ottobre 2026.
Versione: **M-2026-10-28-01**.
Stato: consolidamento documentale dei criteri discussi. Il trasferimento dalla specifica della dashboard conserva testi, valori e condizioni; gli identificativi dei campi rimangono proposte organizzative.

## 1. Uso e natura dei criteri

Questo è il riferimento dei criteri dello studio per la [procedura di ideation](ideation-sistema-operativo.md), le [schede](ideation-input-output.md) e le [valutazioni](ideation-valutazione-scoring.md). La [dashboard futura](dashboard-configurazione-mandato.md) ne descrive la modifica e i selettori.

Distinguere definizioni del perimetro, vincoli, obiettivi orientativi, preferenze e riferimenti per i test. Una preferenza non diventa un requisito obbligatorio; una fascia orientativa non diventa una soglia di esclusione. «Da definire» non equivale a zero.

I filtri della sessione restringono questo mandato senza modificarlo. Una modifica deliberata dei criteri richiede una nuova versione identificabile, con data e differenze; le valutazioni precedenti conservano il riferimento alla versione usata. La versione qui indicata è la fotografia iniziale, non un valore da assumere attivo per sempre.

I parametri numerici sono mantenuti in questo documento. I casi di calibrazione usano invece valori fittizi e configurazioni di scenario, da non trasferire automaticamente al mandato.

## 2. Tesi e obiettivo dello studio

| Identificativo | Tipo | Valore iniziale concordato |
| --- | --- | --- |
| `tesi.testo` | Testo lungo | La tesi riportata sotto. |
| `tesi.obiettivo` | Testo lungo | Creare business software che generino cassa rapidamente, sostenibili con un piccolo team e interessanti anche a dimensioni contenute. |
| `tesi.ambizione_crescita` | Testo | Una crescita maggiore è benvenuta, ma non è necessaria per rendere il business interessante. |

Testo iniziale della tesi:

> Costruiamo prodotti software per professionisti e microimprese che operano in Italia, con possibilità di espansione internazionale.
>
> Risolviamo attività o processi circoscritti, aiutando i clienti a lavorare meglio o a far crescere il business attraverso prodotti semplici, acquistabili e utilizzabili prevalentemente in autonomia.
>
> Cerchiamo business sostenibili con un piccolo team, acquisibili attraverso pubblicità digitale e capaci di recuperare tutti i costi entro il primo mese dal lancio, generando successivamente cassa. Devono essere economicamente interessanti anche a dimensioni contenute; un potenziale maggiore rimane benvenuto.

## 3. Clienti e geografia

| Identificativo | Tipo | Valore iniziale / natura |
| --- | --- | --- |
| `clienti.professionisti.definizione` | Testo lungo | Persone con partita IVA che offrono sul mercato prestazioni basate prevalentemente sulle proprie competenze personali, tecniche, intellettuali o creative. Definizione del perimetro. |
| `clienti.professionisti.esempi` | Elenco di testi | Geometri, architetti, RSPP, legali, consulenti ambientali e sui rifiuti. Esempi non esaustivi, senza esclusione delle categorie non elencate. |
| `clienti.microimprese.definizione` | Testo lungo | Imprese con meno di 10 addetti e fatturato annuo oppure totale di bilancio annuo non superiore a 2 milioni di euro. Definizione del perimetro. |
| `clienti.microimprese.addetti_limite` | Intero, limite esclusivo | 10. |
| `clienti.microimprese.fatturato_limite_eur` | Importo, limite inclusivo | 2.000.000 €/anno. |
| `clienti.microimprese.bilancio_limite_eur` | Importo, limite inclusivo | 2.000.000 €. |
| `clienti.microimprese.esempi` | Elenco di testi | Ristoranti, centri estetici, aziende di consulenza. Esempi non esaustivi. |
| `clienti.note_perimetro` | Testo | Professionisti e microimprese possono sovrapporsi. La clientela B2B/B2C non è un filtro del mandato. Cluster da mappare successivamente. |
| `geografia.mercato_iniziale` | Selezione geografica | Italia: clienti che operano in Italia, senza requisito sulla nazionalità del titolare. Focus iniziale. |
| `geografia.espansione` | Selezione + testo | Facoltativa; possibilità di espansione internazionale in funzione del prodotto. |

La condizione microimpresa usa: addetti sotto soglia **e** almeno una delle due condizioni economiche rispettata. I valori economici non sono entrambi obbligatori.

## 4. Pilastri qualitativi

Per ogni pilastro: titolo modificabile, descrizione modificabile, segnali favorevoli, segnali critici ed esempi. I segnali sono indicazioni per il ragionamento, non prove automatiche.

| Pilastro | Contenuto iniziale concordato |
| --- | --- |
| Cliente definito e decisione corta | Identificare segmento, attività e contesto. Chi utilizza acquista o si confronta direttamente con chi decide. Percorso compatibile con self-service o demo breve. |
| Valore concreto e riconosciuto | Migliorare il lavoro o favorire la crescita. Considerare difficoltà percepite, obblighi e risultati desiderati. Valutare insieme peso del risultato e frequenza, senza frequenza minima universale. |
| Domanda e spazio competitivo | Spiegare perché un gruppo identificabile di clienti sceglierebbe il prodotto rispetto alle alternative attuali. Sono ammesse nicchie trascurate, debolezze di distribuzione e brand, soluzioni arretrate e attività oggi manuali. |
| Autonomia e leggerezza | Privilegiare autonomia lungo acquisto, attivazione e utilizzo. Sviluppo, assistenza e manutenzione sostenibili per un piccolo team. Interventi manuali ricorrenti e verifiche per singola pratica sono segnali di incompatibilità da esplicitare. |
| Bacino, ticket e acquisizione compatibili | Valutare insieme clienti plausibilmente acquisibili, ricavo per cliente, canali e costi. Il ticket emerge dal valore; i competitor sono un riferimento. Nessun bacino minimo o ticket universale fissato. |

Campi trasversali:

| Identificativo | Tipo | Valore iniziale |
| --- | --- | --- |
| `prodotto.perimetro` | Testo lungo | Attività o processi chiaramente delimitati. Ammessa una piattaforma completa quando il lavoro del target è sufficientemente circoscritto. |
| `valore.peso_frequenza` | Testo lungo | «Peso × frequenza» è un criterio di ragionamento qualitativo, non una formula di punteggio. Attività occasionali ad alto valore sono ammesse. |
| `competizione.alternative` | Elenco di testi | Software dedicati, strumenti generici, Excel, WhatsApp, attività manuali e servizi esterni. |
| `competizione.regola` | Testo lungo | Il numero di competitor da solo non determina l'attrattività. Esplicitare lo spazio disponibile e il vantaggio per il cliente. |

## 5. Modello commerciale e operatività

| Identificativo | Tipo | Valore iniziale / natura |
| --- | --- | --- |
| `commerciale.modello_preferito` | Selezione | Abbonamento. Preferenza. |
| `commerciale.modelli_ammessi` | Selezione multipla | Abbonamento e pagamento per singolo output, pratica o documento. |
| `commerciale.incasso_abbonamento` | Selezione multipla | Mensile e annuale anticipato, secondo prodotto e cliente. Nessuna formula universalmente obbligatoria. |
| `commerciale.self_service` | Selezione + testo | Modalità prevalente lungo comprensione, acquisto, attivazione e utilizzo continuativo. |
| `commerciale.assistenza` | Testo | Assistenza via WhatsApp. Deve restare sostenibile. |
| `commerciale.demo` | Selezione + testo | Ammessa prima dell'acquisto se breve e poco dispendiosa, soprattutto con ticket più alti. Nessuna soglia di ticket definita. |
| `operativita.sostenibilita` | Testo lungo | Effort e costi contenuti; piccolo team; evidenziare personalizzazioni, assistenza frequente e lavoro umano necessario per erogare ogni risultato. Nessun budget numerico iniziale fissato. |

## 6. Obiettivi economici

Tutti i valori si riferiscono al singolo prodotto. Le fasce descrivono una dimensione interessante, non il massimo potenziale ammissibile.

| Identificativo | Tipo | Valore iniziale / natura |
| --- | --- | --- |
| `economia.abbonamento.arr_eur` | Intervallo monetario | 150.000–500.000 € di ARR. Obiettivo orientativo. |
| `economia.output.ricavi_annui_eur` | Intervallo monetario | 150.000–300.000 € di ricavi annui effettivi. Obiettivo orientativo. |
| `economia.orizzonte_mesi` | Intero | 12 mesi dal lancio. Obiettivo. Per gli abbonamenti: ARR raggiunto entro il periodo; per output: ricavi effettivi del primo anno. |
| `economia.flessibilita_temporale` | Testo | Tempi maggiori valutabili quando manutenzione e impegno operativo sono contenuti. Per output oltre il primo anno, esplicitare periodo e ricavi annuali attesi senza confrontare ricavi cumulati pluriennali con la fascia annua. |
| `economia.flessibilita_fasce` | Testo | Valori superiori ammessi senza penalizzazione automatica; valori inferiori da valutare nel contesto. Nessuna percentuale di tolleranza fissata. |
| `economia.recupero_costi_mesi` | Intero | 1 mese dal lancio. Vincolo: almeno pareggio complessivo entro il primo mese, includendo i costi iniziali. |
| `economia.costi_da_considerare` | Elenco di testi | Sviluppo/preparazione, lancio/acquisizione, gestione ed erogazione sostenute fino al termine del primo mese. Dettaglio delle voci da esplicitare nelle stime. |
| `economia.obiettivo_cassa` | Testo | Recuperare tutti i costi e generare successivamente cassa; usare gli incassi effettivi per valutare il recupero. |
| `economia.margine_aspirato_percento` | Numero + nota | Superiore all'80%. Aspirazione, esclusa dai filtri e dai calcoli dettagliati richiesti in ideation. Definizione contabile del margine ancora aperta. |
| `economia.budget_sviluppo_eur` | Importo non valorizzato | Da definire. Non introdurre un tetto universale. Le singole ipotesi devono comunque esplicitare un ordine di grandezza dei costi per motivare il pareggio. |

## 7. Canali e acquisizione

| Identificativo | Tipo | Valore iniziale / natura |
| --- | --- | --- |
| `acquisizione.ads` | Stato di requisito | Obbligatorie come canale plausibile di acquisizione. |
| `acquisizione.email` | Stato di requisito | Facoltativo, ammesso. |
| `acquisizione.altri_canali` | Testo | Ammessi per contribuire alla crescita; non compensano l'assenza di una strada credibile attraverso ads. |
| `acquisizione.cac_soglia_percento` | Intervallo percentuale | 15–25% come fascia indicativa della soglia massima ipotizzata. Non è una fascia minima/massima del CAC desiderato. |
| `acquisizione.cac_base` | Testo | Quanto il cliente paga in un anno. Per output, esplicitare numero di acquisti annuali ipotizzato. Nessun LTV pluriennale. |
| `acquisizione.cpl_riferimento_eur` | Intervallo monetario | 0,80–5 € per lead: riferimento indicato per i test, non soglia universale di esclusione. |
| `acquisizione.conversione_lead_cliente` | Percentuale non valorizzata | Da ipotizzare per opportunità e poi verificare. Nessun valore predefinito concordato. |
| `acquisizione.altri_costi` | Importi di scenario, da definire | Demo, attività commerciali o altri costi di acquisizione se presenti, con periodo e base di allocazione dichiarati. Nessuno zero automatico. |
| `acquisizione.evidenza_richiesta` | Testo | In ideation: ipotesi credibili. Successivamente: test ads e lead generation senza prodotto per le proposte selezionate. |

Relazioni da spiegare nella dashboard, senza imporre un simulatore nella prima versione:

- ARR = clienti paganti attivi × ricavo ricorrente annuo medio per cliente.
- Ricavi per output = output pagati nel periodo × ricavo medio per output.
- CAC massimo ipotizzato = pagamento annuale del cliente × percentuale massima ipotizzata.
- CAC delle sole ads = CPL ÷ tasso di conversione lead → cliente, usando la percentuale come frazione e unità/coorti coerenti.
- CAC complessivo = (spesa ads + altri costi di acquisizione pertinenti) ÷ nuovi clienti paganti acquisiti. È questo costo complessivo a essere confrontato con il limite.
- CPL massimo ipotizzato = (CAC massimo ipotizzato − altri costi di acquisizione per cliente) × tasso di conversione lead → cliente, quando gli altri costi sono già stimati per lo stesso scenario. Se cambiano volumi o conversioni, riallocare gli eventuali costi fissi. Senza altri costi la formula si riduce a CAC massimo × conversione.

Un'acquisizione entro il rapporto CAC/ricavo annuo non dimostra da sola il pareggio nel primo mese. Incassi mensili e annuali anticipati producono disponibilità di cassa diverse. ARR, ricavi effettivi, incassi e profitto devono mantenere significati distinti.

## 8. Applicazione alle ricerche

- Per ciascuna sessione dichiarare la versione del mandato, i filtri e i vincoli specifici. La richiesta può combinare testo libero e parametri.
- Applicare i criteri al livello richiesto. Uno spazio ampio non deve già dimostrare il recupero dei costi di un prodotto; il relativo scenario appartiene al concept.
- Esplicitare fatti supportati, assunzioni e dati mancanti. In ideation sono ammesse ipotesi credibili; il risultato resta una prevalutazione.
- Leggere la fascia CAC come riferimento per un massimale da motivare, senza scegliere silenziosamente un unico limite o trattare il suo estremo inferiore come minimo desiderato. Un vincolo numerico esplicito della sessione va invece rispettato.
- Il margine aspirato, il numero di competitor e la numerosità del target non introducono soglie universali aggiuntive.
- Per interpretazioni, formule e giudizi usare la [rubrica di valutazione](ideation-valutazione-scoring.md); per scegliere il passo successivo usare la [procedura operativa](ideation-sistema-operativo.md).

## 9. Elementi aperti

Restano aperti la mappatura dei clienti, il dettaglio contabile degli scenari e i limiti quantitativi non concordati per effort, demo e assistenza. Dichiarare le ipotesi del singolo scenario senza attribuirle allo studio.

La scelta di un budget universale di sviluppo o di pesi e totali non è necessaria per usare la versione documentale. Knowledge base, skill specialistiche, automazione, dashboard e criteri dei test commerciali saranno affrontati nelle fasi dedicate.
