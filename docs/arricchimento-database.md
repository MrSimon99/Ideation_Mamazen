# Arricchimento del database — Registro di lavorazione

Data: 28 ottobre 2026.
Stato: **preparazione completata; ricerca esterna bloccata nella sessione precedente**. L'utente ha già abilitato e pubblicato l'accesso pubblico, ma il runtime precedente continua a usare la rete limitata. Nessun nuovo dato numerico inserito e nessuna nuova fonte esterna verificata. Il lavoro autorizzato rimane aperto.

## 1. Mandato dell'attività

L'utente ha autorizzato due giri, con una riga e una colonna alla volta in piccoli batch:

1. Completare i campi mancanti, cercando dati di qualità e documentando ogni evidenza.
2. Approfondire attività e processi come una value chain, con particolare attenzione a commercianti e microimprese, e compilare i quattro arricchimenti del [Gate 1](ideation-gate-ricerca.md).

Non è necessario chiedere un nuovo consenso per ogni batch. La dimensione iniziale scelta per la lavorazione è di cinque target; è una scelta operativa modificabile. All'interno del batch ogni campo va chiuso con un dato documentato o un esito motivato prima di passare al successivo.

## 2. File e checkpoint

- [Excel di lavorazione](../data/lavorazione/professioni_con_piva_italia_v7_lavorazione.xlsx): conserva i sette fogli originari e aggiunge avanzamento, lacune, coda dei batch, metadati iniziali e strutture per evidenze e secondo giro.
- [Checkpoint](../data/lavorazione/checkpoint.json): fase corrente, conteggi, blocco e punto di ripresa.
- [Registro delle lacune](../data/lavorazione/registro-lacune.json): una voce per cella vuota, con categoria e stato.
- [Coda dei batch](../data/lavorazione/batch-primo-giro.json): tredici batch per le 62 righe con almeno un dato quantitativo mancante.

Sorgente: [professioni_con_piva_italia_v6_output.xlsx](../data/sorgenti/professioni_con_piva_italia_v6_output.xlsx), fornito dall'utente. SHA-256: `aacbdfcbfae9e78e4be29d44161f9e6898b1f3f6e9e6000dfd8fb4acd287aed4`. Gli identificativi `V6-R0402` e simili indicano una riga di questa precisa versione, non un identificativo universale della professione.

Il salvataggio con openpyxl normalizza le dimensioni dichiarate di alcuni fogli, eliminando dalle dimensioni le righe finali senza celle. Il controllo di conservazione confronta coordinate e valori di tutte le celle valorizzate, incluse eventuali formule; il file originale rimane invariato.

## 3. Ricognizione delle lacune

| Campo | Vuoti | Trattamento |
| --- | ---: | --- |
| Remunerazione | 49 | Ricerca sostanziale; distinguere reddito del titolare, RAL, netto e fatturato. |
| Numerosità | 40 | Ricerca sostanziale; dichiarare popolazione, unità, territorio e periodo. |
| Fonti remunerazione | 46 | Da completare insieme alla ricerca sul relativo dato economico. |
| Unità di output | 177 | Verificare applicabilità: 168 compensi a tempo, 8 non determinabili e 1 misto. |
| Note generali | 27 | Campo facoltativo; non riempire con informazioni artificiali per eliminare un vuoto. |

Totale: **339 celle vuote registrate**, di cui **89 quantitative** distribuite su **62 target**. Le celle quantitative mancanti appartengono alle attività artigianali/commerciali. Il registro non equivale a 339 ricerche già eseguite.

L'unica unità di output vuota con remunerazione classificata come mista è `M244`, Enotecari Professionisti Italiani: va controllata individualmente. Le fonti già presenti in righe con reddito vuoto non provano che quel dato sia disponibile: casi `431 Elettrauto`, `432 Meccanico Moto`, `466 Cartoleria`.

## 4. Primo batch e lavoro eseguito

Batch **P1-B01**:

| Riga originaria | Target | Primo campo quantitativo |
| --- | --- | --- |
| 402 | Agricoltore / Coltivatore Diretto | C402, remunerazione |
| 403 | Viticoltore / Produttore Vinicolo (Cantina) | C403, remunerazione |
| 404 | Floricoltore / Vivaista | C404, remunerazione |
| 405 | Allevatore di Bestiame (Bovini, Ovicaprini, Suini) | C405, remunerazione |
| 406 | Apicoltore | C406, poi D406 |

Sono stati estratti e controllati sulle note già presenti i metadati di queste cinque righe: unità della numerosità, perimetro, anno dichiarato e limiti. Il foglio `Metadati batch 01` li indica esplicitamente come **non verificati su nuove fonti**. Questo non completa le lacune quantitative del batch.

Per esempio, il numero dei coltivatori diretti conta persone con una qualifica specifica, quello dei viticoltori aziende con vite e quello degli allevatori include gruppi più ampi del titolo della riga. I redditi convenzionali contributivi non vanno usati come redditi effettivi del titolare.

Il secondo giro non è avviato. I fogli destinati a value chain e Gate 1 sono predisposti, senza classificazioni o analisi di attività già dichiarate concluse.

## 5. Regole di qualità per ogni campo

- Consultare la fonte effettiva: un riferimento già scritto nel file o il risultato di un motore di ricerca non è una nuova verifica.
- Conservare URL, editore, titolo, estratto/tabella/pagina, anno del fenomeno, data di pubblicazione e accesso.
- Dichiarare natura del dato e pertinenza al target: diretto, proxy, stima pubblicata, stima interna preesistente, fonte inaccessibile, ricerca incompleta o dato non reperito.
- Documentare unità, Italia/altro territorio, inclusioni ed esclusioni. Per gli importi distinguere lordo/netto, reddito/fatturato, titolare/dipendente, impresa/persona e FTE quando rilevante.
- Non mediare automaticamente fonti con anni, unità o popolazioni diversi. Non trasformare i vuoti in zero, una RAL in reddito del titolare o il fatturato in remunerazione.
- Un campo può rimanere senza numero se la ricerca non produce un dato adeguato; deve avere un esito e un punto da cui riprendere. Un blocco tecnico non dimostra che il dato non esista.
- Salvare dopo il controllo di ogni batch, aggiornando conteggi, registro delle modifiche e prossima cella. Conservare le vecchie stime come riconoscibili.

## 6. Blocco tecnico e ripresa

La sessione precedente permette soltanto le destinazioni del preset per strumenti di sviluppo. Le richieste a `https://www.istat.it/` e `https://www.crea.gov.it/` tramite il proxy previsto dall'ambiente hanno restituito **Tunnel connection failed: 403 Forbidden**. Non è una ricerca infruttuosa sulla remunerazione: è una verifica di accesso alle fonti.

Inizialmente è stata predisposta una bozza con fonti statistiche e settoriali. L'utente ha successivamente **abilitato tutto l'accesso pubblico e confermato la pubblicazione**. La configurazione modificabile risulta `unrestricted`, revisione 3; il runtime precedente continua invece a riportare rete `restricted`, revisione 1. Questo disallineamento è registrato nel checkpoint. Non sostituire la configurazione senza restrizioni con la vecchia bozza a domini limitati.

Per riprendere: usare il [punto di ripresa della nuova sessione](RIPRESA-ARRICCHIMENTO.md), verificare l'accesso effettivo e, se disponibile, iniziare da **C402**. Non far ripetere all'utente l'abilitazione o la pubblicazione già confermate, né la preparazione del database. Se il blocco permane, riportare la limitazione tecnica con evidenza senza attribuirla a una configurazione che l'utente non avrebbe applicato.

## 7. Verifiche prima di dichiarare il completamento

Controllare che l'originale conservi il suo hash; le celle originarie non interessate restino uguali; ogni nuovo numero abbia evidenza e perimetro; i riferimenti del registro corrispondano alle celle; le lacune aperte restino distinte da quelle risolte. Il completamento del primo giro va dichiarato soltanto dopo aver riesaminato ogni lacuna sostanziale ed esplicitato gli esiti ancora senza un numero utilizzabile.
