# Controllo delle lacune — storico del primo run,29 ottobre2026

**Stato aggiornato nel [secondo run](ricerca-2026-10-29-run2/RUN2-ESITO.md):50 redditi e7 conteggi ancora vuoti;1 unità operativa aggiunta;C391/J391/N391 invalidati per errata identificazione di AcquaViva. I numeri sotto sono lo storico del primo run.**

**L’Excel non è completo.** Il riesame ha coperto tutte le 339 lacune originariamente registrate, ma non equivale all’esaurimento di tutte le fonti possibili. In questo passaggio sono stati inseriti 32 conteggi prima vuoti, con fonti e perimetri espliciti; nessun nuovo reddito personale è stato verificato.

## Stato effettivo

| Campo | Celle fisicamente vuote | Interpretazione |
| --- | ---: | --- |
| Remunerazione lorda | 49 | Ricerca ancora incompleta; non sostituite con fatturato, stipendi dipendenti, risultati aziendali o media ISA generale. |
| Numerosità | 7 | Non trovato un conteggio verificato con perimetro pertinente. |
| Fonti remunerazione | 41 | Da associare a un reddito effettivamente verificato. Le altre cinque fonti contestuali aggiunte nel primo passaggio non risolvono quei redditi. |
| Unità di output | 177 | 168 vuoti ammessi nel modello a tempo indicato, senza prova di una tariffazione per output; 9 applicabilità ancora aperte. Non significa che le 168 attività non producano output operativi. |
| Note aggiuntive | 27 | Facoltative; non riempite con testo artificiale. |

Totale fisico: **301 celle vuote**. I campi sostanziali ancora privi di un numero sono **56**, suddivisi in 49 redditi e 7 numerosità. I conteggi numerici aggiunti rispetto alla sorgente v6 sono complessivamente 33, compreso il proxy Honey Cost del precedente passaggio. Non sono 33 popolazioni di titolari P.IVA tutte verificate: ogni numerosità conserva il suo perimetro.

## Nuovi conteggi inseriti in questo riesame

Le cifre Eurostat riguardano imprese statistiche `enterprise`, non persone, singole partite IVA, unità locali o sole microimprese. Le classi NACE Rev.2 non coincidono sempre con il titolo della riga: i perimetri più ampi sono indicati come proxy in E e I. Non sommare automaticamente le righe del database: popolazioni, periodi e livelli di aggregazione possono sovrapporsi.

Le cifre Unioncamere-InfoCamere riguardano **sole imprese artigiane registrate al 31 marzo 2025**, non tutte le imprese attive. È un perimetro specifico, non una popolazione di persone.

| Cella | Attività | Valore inserito | Fonte e periodo |
| --- | --- | ---: | --- |
| D408 | Macellaio | 19,589 | Eurostat; 2024 |
| D409 | Pescivendolo | 4,935 | Eurostat; 2024 |
| D410 | Pasticciere | 25,795 | Eurostat; 2024 |
| D412 | Pastaio (Pastificio Artigianale) | 3,585 | Eurostat; 2024 |
| D415 | Muratore | 227,988 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D416 | Impresa Edile / Costruttore Edile | 133,198 | Eurostat; 2024 |
| D417 | Idraulico | 49,492 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D418 | Elettricista | 57,072 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D419 | Imbianchino (Tinteggiatore) | 10,446 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D420 | Intonacatore | 7,241 | Eurostat; 2024 |
| D421 | Impresa di Coperture (Copritetti/Lattoniere) | 5,145 | Eurostat; 2024 |
| D422 | Vetraio | 2,118 | Eurostat; 2024 |
| D423 | Falegname (Mobili e Arredi su Misura) | 13,281 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D424 | Carpentiere Metallico (Strutture in Ferro) | 12,140 | Eurostat; 2024 |
| D425 | Sarto / Sartoria | 11,114 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D426 | Calzolaio | 2,775 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D435 | Tecnico Riparatore Elettrodomestici | 3,141 | Eurostat; 2024 |
| D436 | Orologiaio (Riparazione Orologi) | 1,569 | Eurostat; 2024 |
| D438 | Ceramista | 1,848 | Eurostat; 2024 |
| D440 | Tappezziere | 5,700 | Eurostat; 2024 |
| D442 | Lavanderia / Tintoria | 9,956 | Unioncamere e InfoCamere, elaborazione Movimprese su Registro delle Imprese; 2025-03-31 |
| D448 | Catering per Eventi | 2,169 | Eurostat; 2024 |
| D450 | B&B / Affittacamere | 43,180 | Eurostat; 2024 |
| D454 | Negozio di Abbigliamento | 53,483 | Eurostat; 2024 |
| D455 | Ferramenta | 24,831 | Eurostat; 2024 |
| D456 | Libreria | 3,074 | Eurostat; 2024 |
| D460 | Negozio di Articoli per la Casa / Casalinghi | 22,547 | Eurostat; 2024 |
| D461 | Profumeria | 10,518 | Eurostat; 2024 |
| D464 | Calzature (Negozio di Scarpe) | 10,720 | Eurostat; 2024 |
| D465 | Negozio di Giocattoli | 2,774 | Eurostat; 2024 |
| D467 | Negozio di Elettronica / Telefonia | 5,410 | Eurostat; 2024 |
| D472 | Impresa di Traslochi | 1,408 | Eurostat; 2024 |

## Sette conteggi ancora aperti

- D407, pescatore professionale: il rapporto di settore reperito conta imbarcati, anche dipendenti, e distingue headcount/FTE; non prova il numero di pescatori indipendenti con P.IVA.
- D431, elettrauto: il dato della riparazione autoveicoli non isola la figura; la successiva riunificazione meccatronica richiede attenzione al perimetro storico.
- D432, meccanico moto: il dato vendita+riparazione moto non isola le officine; “meccanici” generici non equivale a meccanici moto.
- D441, liutaio: la fabbricazione di tutti gli strumenti musicali non isola liutai e riparatori.
- D462, ottica: la classe residuale di commercio non isola i centri ottici; unità locali e imprese non sono intercambiabili.
- D466, cartoleria: la classe Eurostat comprende anche edicole; la pagina pubblica Federcartolai è in aggiornamento e i manuali richiedono registrazione. Nessun account o contatto eseguito.
- D471, corriere ultimo miglio: la classe postale/corrieri non isola padroncini e ultimo miglio.

## Redditi: ricerca aperta, non prova di inesistenza

Sono state consultate fonti settoriali, risultati RICA/Honey Cost e pubblicazioni fiscali MEF. La [sintesi ISA relativa all’anno d’imposta2024](https://www1.finanze.gov.it/finanze/analisi_stat/public/v_4_0_0/contenuti/sintesi_analisi_dati_2024_irpef_isa.pdf) pubblica 56.100 euro per soggetto come media generale di attività e forme giuridiche differenti: non è trasferibile alle 49 righe. La pagina ufficiale delle tavole dettagliate ISA ha restituito HTTP403. L’applicazione IRPEF raggiunta permette le sezioni economiche, non la granularità necessaria ai target.

La definizione fiscale pertinente del reddito di spettanza dell’imprenditore è RF101 + RG36; il reddito fiscale, anche per gli effetti del concordato preventivo biennale dal2024, non è automaticamente reddito effettivo. Occorre verificare separatamente attività, persone fisiche, regime, anno e popolazione. Le fonti aziendali o fiscali aggregate già trovate rimangono evidenze contestuali; non sono state convertite arbitrariamente in remunerazioni personali.

## Errori corretti nelle note

- Ottica: la nota originaria indicava come2025 un codice precedente; aggiunto il riferimento Federottica a 47.74.01 per occhiali/lenti, distinguendolo dall’attività fotografica.
- Cartoleria: corretta l’affermazione secondo cui non esiste un’associazione dedicata. Federcartolai aderisce a Confcommercio; questo non fornisce da solo il numero nazionale di cartolerie.

## Tracciabilità e ripresa

Nel workbook, `Registro nuove evidenze` registra i riscontri distinguendo fonte consultata da campo risolto. Il foglio `Controllo completezza` riporta tutti i 339 record storici di lacuna e lo stato corrente. `controllo-completezza-2026-10-29.json` conserva la stessa verifica in formato leggibile da programmi. La cartella `ricerca-2026-10-29` conserva ricerche settoriali, limiti, link e decisioni di inserimento; contiene anche la risposta ufficiale Eurostat2024 e il PDF InfoCamere2025. Alcuni log riportano percorsi temporanei di estrazione, che non sono necessari alla ripresa: usare gli URL canonici e i due documenti conservati.

Tutti i tredici batch restano **parziali**, dato che contengono campi sostanziali irrisolti. Il secondo giro di value chain/Gate1 non è stato avviato. Riprendere da C402 oppure dalla specifica lacuna indicata nel checkpoint, senza ripetere i conteggi già salvati e senza dichiarare il file interamente compilato.
