# Arricchimento del database — Registro di lavorazione

Data di aggiornamento: 29 ottobre 2026.
Stato: **secondo run concluso con esiti motivati, compilazione ancora incompleta**. Nessun nuovo reddito o conteggio affidabile inserito nelRUN2;1 unità operativa descrittiva aggiunta inM391. Corretto il profilo “AcquaViva” da benessere a guida fluviale: invalidati C391,J391,N391 e conservati i precedenti valori. Restano50 redditi,7 numerosità,42 fonti e1 quota automatizzabile vuoti;176 unità di output vuote(168 modello a tempo,8 da chiarire),27 note facoltative. Vedere [esitoRUN2](../data/lavorazione/ricerca-2026-10-29-run2/RUN2-ESITO.md).

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


## 8. Ricerca del 29 ottobre 2026 — P1-B01 parziale

La rete è stata verificata con richieste HTTPS riuscite, non soltanto dalla configurazione. Il vecchio blocco è conservato nello storico del checkpoint; nessuna modifica o nuova pubblicazione dell’ambiente è stata eseguita.

Fonti consultate:

- [CREA, Le aziende agricole in Italia nel 2024, Rapporto RICA 2026](https://rica.crea.gov.it/download.php?id=2027), pubblicazione annunciata l’11 settembre 2026. Campo di osservazione PS almeno 8.000 euro (p.8). Reddito netto medio Italia 38.177 euro/azienda (p.16 e tab.4 p.119); RN per UL totale 25.158 euro (tab.6b p.122). Sono remunerazioni dei fattori dell’imprenditore e della famiglia e del rischio, non redditi personali dei soli coltivatori diretti.
- Nella stessa tab.6b: Vite 23.195 euro/UL; Ortaggi e fiori 24.456; Bovini da latte 53.167; Altri erbivori 30.713; Granivori 59.622. Nessun dato è stato convertito in stipendio personale, nessuna media fra allevamenti. I comparti non isolano cantine con vino proprio, vivaisti o sole specie richieste.
- [CREA/ONM, Honey Cost, Fact Sheet 20 maggio 2025](https://honeycost.crea.gov.it/download.php?id=269): tab.1 p.5, universo 2024 composto da 4.581 aziende nomadi e 1.496 stanziali, somma 6.077. Il numero inserito in D406 è soltanto questo universo. Tab.2 p.6: margine operativo medio 18.018 euro/azienda nomade e 6.270 stanziale nel 2024; non reddito personale. Il [rapporto metodologico 2023](https://honeycost.crea.gov.it/download.php?id=263), p.10, definiva PS superiore a 8.000 euro e circa 120 alveari minimi; il Fact Sheet più recente non ripete la soglia, pertanto la sua invarianza non è accertata.
- [ONM, Report annuale stagione 2025](https://www.informamiele.it/wp-content/uploads/2026/10/Report-annuale-Monitoraggio-produzione-e-mercato-del-miele-stagione-2025.pdf), p.14: 78.017 apicoltori totali BDN (censimento nov-dic 2024, aggiornamento giugno 2025), inclusi allevamenti familiari. La quota commerciale è 27% nel grafico e 26% nel testo p.11: non si è ricavato un conteggio esatto da percentuali arrotondate e discordanti. Questo universo non coincide con Honey Cost né con tutti i titolari di P.IVA.

Nel foglio principale sono aggiornate J402:J406 e aggiunte note in K402:K406, oltre a D406/E406/H406/I406. Le vecchie note sono conservate. Il Registro nuove evidenze e il file `data/lavorazione/evidenze-2026-10-29-b01.json` contengono URL, data di accesso, estratto/riferimento, natura, trasformazioni e limiti. Registro lacune, coda e checkpoint sono allineati.

Restano 49 remunerazioni vuote, 39 numerosità vuote; cinque celle Fonti prima vuote hanno adesso riferimenti contestuali, ma **non cinque redditi risolti**. D406 riduce un vuoto numerico senza risolvere il conteggio completo delle imprese P.IVA. Il batch rimane parziale. Prossimo approfondimento: C402, reddito personale effettivo; le C403:C406 restano da approfondire a loro volta.


## 9. Riesame completo dopo la richiesta di verifica

Riesaminate tutte le339 lacune originarie. Inseriti32 nuovi conteggi; sommando D406 del primo passaggio sono33 numeri aggiunti alla sorgente, con natura/perimetro espliciti. Nessun nuovo reddito personale verificato. Le numerosità ancora vuote sono D407,D431,D432,D441,D462,D466,D471. Dettaglio delle32 nuove cifre, delle fonti e delle limitazioni nel [rapporto di completezza](../data/lavorazione/CONTROLLO-COMPLETEZZA-2026-10-29.md).

Restano49 remunerazioni,7 numerosità,41 fonti fisicamente vuote,177 unità di output e27 note facoltative. Dei177 output,168 restano vuoti ammessi nel modello a tempo già indicato (non prova dell’assenza di output operativi);9 richiedono ulteriori elementi. Le5 fonti contestuali già compilate non risolvono i redditi corrispondenti. Nessun reddito mancante trasformato in zero o riempito con la media ISA generale.

Aggiunto al workbook il foglio `Controllo completezza`; registro lacune, coda e checkpoint allineati. Tutti i batch sono ancora parziali. Corretti due errori nelle note (ATECO ottica e associazione Federcartolai), conservando la sorgente originale. Nessuna configurazione dell’ambiente o pubblicazione modificata.


## 10. Secondo run — criterio affidabilità e celle bianche

L’utente ha richiesto un ulteriore tentativo, lasciando bianchi i dati non accurati o non affidabili con nota/motivazione. Riesaminati56 campi numerici inizialmente aperti e9 unità di output incerte. Nuove piste nei cataloghi pubblici, metadati INPS, rapporti settoriali/accademici e definizioni fiscali non hanno prodotto nuovi redditi o conteggi sufficientemente pertinenti.

La fonte primaria AIPRAV ha invece permesso di correggere il mestiere391 e definire un servizio di accompagnamento guidato come unità operativa, senza dedurre tariffa o remunerazione. Eliminati il16.000€ basato su naturopatia, i relativi riferimenti e il10% di automazione motivato sul profilo errato, conservando lo storico. La fonte v6 resta immutata. Il registro ha ora342 record:339 lacune originarie+3invalidazioni. I numeri di completezza dei paragrafi precedenti sono storici; stato vigente in alto e nel rapportoRUN2.
