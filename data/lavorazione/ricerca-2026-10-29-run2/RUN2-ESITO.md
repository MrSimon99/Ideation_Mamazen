# Secondo run di ricerca —29 ottobre2026

**Nessun nuovo reddito o conteggio numerico sufficientemente affidabile e pertinente.** I campi restano bianchi con note specifiche. La ricerca ha riesaminato i56 campi numerici ancora aperti (49 redditi e7 conteggi) e le9 unità di output con applicabilità incerta, seguendo nuove piste e distinguendo conferme da nuove fonti. Questo esito non dimostra che i dati non esistano.

## Risultato concreto

- Nessun nuovo importo o conteggio inserito: nessun proxy numerico aggiuntivo, zero fittizio o valore medio generale assegnato alle professioni.
- Compilata M391 con `servizio/uscita di accompagnamento guidato in acqua viva`, derivata dalla definizione professionale AIPRAV. È una **unità operativa descrittiva**, non una tariffa, una durata standard, un prezzo o una modalità di pagamento verificata. L391 rimane `Non determinabile`.
- Corretta la identificazione del target391: AIPRAV rappresenta guide in contesto fluviale, non operatori di watsu/naturopatia. C391(16.000€), J391(riferimenti al benessere) e N391(10% automatizzabile basato sul profilo errato) sono stati invalidati e lasciati bianchi, con storico in `invalidazioni.json` e fonte v6 immutata. La numerosità450 era e resta una stima interna preesistente, non un nuovo dato verificato.
- Inseriti commenti sulle celle bianche e motivazioni in K/E e nei registri, senza trasformare le celle quantitative in segnaposto testuali. I vuoti facoltativi e quelli ammessi nel modello a tempo restano riconoscibili.

## Stato corrente

| Campo | Vuoti fisici | Motivo/stato |
| --- | ---: | --- |
| Remunerazione lorda | 50 |49 erano già aperti;1 stima invalidata perché riferita al mestiere sbagliato. |
| Numerosità |7 |Pescatore, elettrauto, meccanico moto, liutaio, ottica, cartoleria e corriere ultimo miglio: nessun nuovo totale coerente con il target. |
| Fonti remunerazione |42 |41 già vuote;1 riferimento non pertinente invalidato. Le fonti di contesto non provano un reddito personale. |
| Unità di output |176 |168 vuoti ammessi nel modello a tempo documentato;8 ancora da chiarire. |
| Quota automatizzabile |1 |N391: non trasferito il10% del precedente profilo errato; nuova valutazione non effettuata. |
| Note aggiuntive |27 |Facoltative, lasciate bianche senza testo artificiale. |

Sono303 vuoti fisici. Il registro conserva tutte le339 lacune originarie più3 campi invalidati nel secondo run:342 record, distinti per provenienza. I precedenti33 conteggi numerici aggiunti restano immutati, con i loro limiti di perimetro. Non sono tutte popolazioni di titolari P.IVA verificate e non sono nuovi risultati di questo run.

## Nuove piste effettivamente esaminate

- **Catalogo nazionale dati.gov.it/AgID:** interrogazioni e metadati non hanno individuato un dataset con redditi personali per queste attività dettagliate. I risultati fiscali comunali o societari non coprono il bisogno; non è prova di inesistenza di tavole altrove.
- **INPS:** applicazione statistica e metadati pubblici artigiani/commercianti contengono iscritti e media annua iscritti, senza reddito o filtro per mestiere. I professionisti non sono scorporati per professione; le fasce agricole sono convenzionali. Questi campi non sostituiscono reddito personale effettivo.
- **MEF, definizioni IRPEF2024:** reddito agrario basato sul valore catastale, non rilevazione del reddito personale agricolo effettivo. Le sintesi ISA già note restano aggregati non attribuibili ai singoli target; conferme di vecchie fonti non vengono presentate come nuovi dati.
- **Pesca/STECF:** il rapporto sociale distingue salari dipendenti e redditi autonomi e avverte che utile diviso proprietari dà solo stime grossolane, potenzialmente sovrastimate se le imprese sono persone giuridiche. Non ricavati reddito personale o imprenditori dai dati su navi, FTE, contributi o lavoratori totali.
- **Ottica/ANFAO:** il dato814 aziende del report2024 riguarda produttori, non negozi di ottica; escluso dal campoD462. Commercio/cartolerie: ulteriori problemi di accesso o granularità, senza ricorrere agli aggregati già scartati.
- **Liuteria/CERSI:** nuovi rapporti accademici analizzano produzione, canali e prezzi, senza reddito personale annuo. I margini ipotizzati dei rivenditori non vengono attribuiti ai liutai; botteghe locali non trasformate in totale nazionale.
- **Ospitalità/ISMEA/FIPE/FAITA/Federalberghi:** produzione, fatturato, spesa turistica, prezzi e norme fiscali non equivalgono a redditi personali. Limiti di accesso a documenti e report su richiesta sono registrati, senza creare account o contattare soggetti.
- **Corrieri/AGCOM/ASSOESPRESSI:** imprese associate, operatori postali e volumi di mercato non sono un censimento nazionale dei corrieri indipendenti dell’ultimo miglio. L’associazione specifica esiste, ma non fornisce il conteggio richiesto nelle fonti consultate.
- **Profili non ordinistici:** pagine primarie di AMPIT, PA Social e ANPICOF non definiscono una prestazione remunerata unica per tutti gli associati. La pagina AEPI non è risultata consultabile. Non inferite unità di tariffazione dal nome della professione o da proxy salariali.

## Come leggere e riprendere il lavoro

`RUN2-ESITO.json` contiene un esito per ciascun campo riesaminato, fonti, limiti e azione. I file settoriali conservano estratti, anno, perimetro e motivazione; `evidenze-run2.json` distingue le fonti consultate dal fatto che il campo sia stato risolto. `invalidazioni.json` conserva i valori rimossi e la prova della correzione. `manifest-sha256.json` registra l’integrità dei documenti conservati.

Nel workbook, `Controllo completezza` e `Registro lacune` includono342 record. Commenti e note distinguono reddito non reperito, numero di iscritti, reddito convenzionale, fonte inaccessibile, aggregato troppo ampio e unità soltanto descrittiva. Non leggere “bianco” come zero, assenza del mercato o prova che il dato non esista. Tutti i13 batch restano parziali; value chain e scoring Gate1 non sono avviati.

Non è stata modificata né pubblicata la configurazione dell’ambiente. Non occorre ripetere i passaggi di pubblicazione già effettuati dall’utente.
