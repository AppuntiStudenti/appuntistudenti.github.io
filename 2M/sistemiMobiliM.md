orale ottobre 2012
 
- domanda su quali tecnologie avrei usato per uno scenario ipotetico da lui inventato (non mi ricordo nel dettaglio)- vita/morte/miracoli (intendo davvero nel dettaglio) di UPNP- descrizione del D-GPS- domanda su un'esercitazione (che io ammisi candidamente di non ricordarmi)- descrizione di un protocollo di routing (non ricordo quale) 
 
 
altro orale 1
 
- Come realizzeresti un'applicazione per il pagamento del parcheggio (struttura e interazioni)
- GPRS (manet)
- GPS
- pattern proxy (esempio mail in push per applicazioni mobili su cellulare)
 
 
altro orale 2
 
- struttura e architettura Android
- ICMP V4 e V6
- Manet e dense Manet
 
 
orale 4/6/13
 
- Android: vitamorteemiracoli di Intent e NotificationBrodcaster
- UPnP: assegnamento IP (AUTO-IP) e discovery device (primi 2 passi con broadcast e response del device e composizione del response: file.xml)
- Handoff tra foreign network di un mobile host in mobile IP. (non tra base station come avevo capito io....), differenza tra triangolar e quadrilateral routing.
- Bluetooth: protocollo enquiry-page per creazione piconet e comunicazione nella piconet (time-slices / no comunicazione diretta tra slave)
 
altro orale 3
 
- intent e intent filters, broadcast receiver, bluetooth (perchè usato nel progetto)
-mobile ip, come funziona il location update ed handover in generale
-d-gps, come funziona e perchè funziona bene
-il modello di sicurezza in j2me, 2 fasi + sandbox
-upnp
 
17/06
 
- Android: Intent + Broadcaster
- Handoff in GSM
- Jini
- GPSR
 
- SIP: descrizione protocollo + esempio d'uso;
- Handoff: classificazione delle varie tipologie di handoff con esempi reali;
- Android Multimedia API: parlare in generale, anche riguardo all'esercitazione svolta;
- UPnP: le due possibilità di discovery del protocollo (ssdp:discover, ssdp:alive).
 
- DSR: cosa succede in caso di fault (nei casi con e senza cache sui nodi) e quali informazioni ha senso salvare sui nodi se si vuole fare cache
- Come funzionano gli eventi in UPnP
- Android: esempio di codice di una Activity che passa il controllo a un'altra Activity o a un Intent
- Come si possono propagare le sottoscrizioni nei sistemi a eventi (simple routing, identity-based, covering-based, merging-based)
 
02/07/2013
 
J2ME
Ciclo di vita applicazione (callback, risorse, thread);  
Protezione (Sandbox runtime, verifiche offline e on-device)
Handover Mobile IP 
Cosa succede quando passo da un Foreign Agent ad un altro Foreign agent? Messaggi che si scambiano le entità.
Perdita pacchetti, come la evito?
UPnP
Come fa un device ad inoltrare la richiesta di un servizio?
Tutti gli step con relativi protocolli e diagramma di scambio di messaggi.
SOAP in UPnP è over HTTP?
Client Initiated connection
Che pattern è? A cosa serve? Esempi.
Altro orale di giorno 2 Luglio
Intent ed Intent Filter
Cosa sono, esempi di intent
AODV 
Cosa succede in caso di caduta di link
Ekahau
in generale, cosa fa.
Jini
cosa serve il Lease
FB Photo Zoom (off)
23/07/13
 
- Handoff in GSM
- Android: come si fa a fare partire un Service da una Activity e modello di programmazione android
- miglioramenti di Mobile Ipv6 rispetto a Mobile Ipv4
- Pattern Client Initiated Connection e esempi
 
 
26/07/2013
 
j2me
- codice di una midlet funzionante (voleva della logica all'interno, bottoni, display ecc.)
- diagramma degli stati midlet
- sicurezza
 
qualche domanda sull'attività progettuale
 
location API (metodi più importanti e perchè l'ho usata nel progetto)
 
handoff GSM nel dettaglio (single MSC, multi MSC) + varie tipologie di handoff
 
AODV
- funzionamento
- meccanismi di failure detection
 
orale tranquillo, durata 1.20h
 
 
26/07/2013
 
(1) ANDROID
avendo fatto attività progettuale extra su App Android l'orale è iniziato parlando, appunto di questo argomento. Le domande:
- tutti i modi possibili per scambiare messaggi (io avevo usato gli Handler nel progetto);
- come è possibile ottenere i dati provenienti dai sensori con focus particolare sull'accelerometro.
 
Per entrambe le domande mi è stato chiesto di scrivere del codice di esempio.
 
(2) HANDOFF in Mobile IP nel dettaglio, in ordine di tempo cosa avviene e perché, cosa succede in vari casi di esempio (standard).
 
(3) JINI: domande generiche con focus in particolare sul meccanismo di lease.
 
(4) EKAHAU: tutto quello che sapevo e confronto con RADAR.
 
26/09/2013(1) GSMhandoff, specificando tutti i messaggi che vengono scambiati, parlare della tipologia di handoff (orizzontale, proattivo, attivato dal sistema)(2)ANDROID
esempio pratico, sviluppo di una piccola applicazione che mostrasse l'utilizzo di almeno un'activity e di un broadcast reciever, mostrando possibilmente codice. (Ho realizzato una piccola applicazione che in broadcast riceveva delle stringhe di testo per poi trasferirle tramite un intent implicito a tutte le applicazioni di messaggistica, in alternativa avevo realizzato una piccola interfaccia grafica costituita da un edittext e un bottone che alla pressione del bottone faceva sì che a venire data in pasto alle applicazioni di messaggistica fosse invece la stringa dell'edit text. Altra piccola activity collegata da un bottone per far vedere l'utilizzo degli intent espliciti. In questo modo sono riuscito a coprire circa tutti gli argomenti del corso di android ed evitare domande scomde ;) ) Domanda su i thread che gestiscono le activity e il broadcast reciever, e sulla tipologia di eventi a cui doveva registrarsi il broadcast reciever.(3) EKAUH: vita morte e miracoli(4) GSPR: descrizione dell'algoritmo con piccola introduzione sul tipo di algoritmo (routing Geografico)Durata: 1h 45m, ma stava facendo in contemporanea un altro orale. Confermo prof. tranquillissimo come al solito che lascia tutto il tempo di riflettere. A mio avviso vi consiglio vivamente di fare pratica con android perchè sono cose che apprezza molto.  
 
 
23/13/2013
- WP vs Android: confronto su threading/scheduling app e su Location API, a seguire domada al volo su GPS e D-GPS (avevo l'attività progettuale su WP)
- JINI con focus particolare sul meccanismo di lease
- Mobile IP: come gestisce handoff tra du FN diverse
- Hidden Node e Exposed node, cosa sono e come si possono limitare.
 
 09/01/2014
- BroadcastReceiver (e cosa lo rende diverso da un Service o una Activity)
- Domanda molto specifica sull'attività progettuale
- Motivi della lentezza del discovery e connessione WiFi direct (era centrale nella mia attività progettuale)
- AODV in particolare cosa succede quando cade un link
- JINI e il meccanismo di lease- Mobile IP, handoff e quali sono i due tipi di COA (ultimo dettaglio a cui non ho saputo rispondere)
 
 
 
11/02/2013
-Pub/Sub in generale, Subscriptions (i 4 tipi di routing, esempio di Covered-based routing[??] , vari tipi di filtraggio delle subscription[su canale ecc] )-Android: esempio di codice di Service [ma l'ha fatto in aula?] service in generale, broadcaster receiver in generale
-Handoff in mobile ip tra due Foreign Network diverse, chi lo inizia? è handoff verticale o orizzontale, reattivo o proattivo? (client initiated, orizzontale, reattivo)
-UPnP: gestione eventi nel dettaglio la comunicazione, i tipi di messaggi scambiati, Gena (messaggi multicast o unicast? -> multicast solo nel discover)
 
14/2/2013
-Handoff in mobile ip, illustrare i messaggi scambiati quando un nodo residente su una foreign network si sposta verso un'altra foreign network: semplicemente, va spiegato che il NM deve ottenere un nuovo COA dal nuovo FA e deve aggiornare la entry nella mobility binding list del HA (eventualmente anche del CN se in MIPv6). Domanda correlata: ci sono momenti in cui il nodo è disconnesso? Cosa succede se arriva un messaggio? Il NM resta disconnesso finchè non ottiene un COA e lo aggiorna presso l'HA, fino ad allora HA continua ad inoltrare i messaggi verso il vecchio COA (prova a trasmettere facendo ritrasmissioni, quando NM aggiorna il COA vengono inoltrati correttamente);
-JINI e lease: in generale come lavorano le tre entità (broker, provider e client), come funziona il lease, quali sono i vantaggi di usare un lease con timeout rispetto ad una de-registrazione del provider (affidabilità, il provider se cade non riuscirebbe a deregistrarsi, e minore impegno di banda per i messaggi scambiati), broker in comunità, come farlo (broker si registra come provider presso un altro broker), come "togliere" al client il proxy object alla scadenza del lease (mi ha messo un po' in difficoltà: il proxy object può avere un timeout interno che alla scadenza del lease non consente di effettuare più richieste)
-Android: buttare giù del codice di esempio per illustrare intent e intent filter (banalmente, le 4 righe che ci sono sulle slide, su come definirlo nel manifest e come usarlo nell'activity). Cosa succede quando viene lanciato un intent (viene avviata una nuova activity, portata in cima allo stack della conversazione corrente), cosa succede all'activity che lo lancia (va in stato paused), nel caso di più activity con intent filter compatibile quale viene lanciata (se c'è, activity di default,altrimenti scelta dell'utente). In caso volessimo far partire più activity? uso sendBroadcast() invece di startActivity() e definisco BroadcastReceiver con intent filter compatibile.
-DSR, propagazione di errori: default-> se un nodo non riesce a trasmettere invia un messaggio RERR indietro verso il nodo sorgente (come?-> source routing, nell'header è specificato l'intero percorso, segue il percorso inverso). Il nodo sorgente fa una nuova discovery (di nuovo flooding di RREQ). Se c'è caching, la propagazione di RERR invalida le cache, può essere bloccata da un nodo che ha un path alternativo.
 
 
 
 
Orale 20/02/2014
 
- GSM: ha voluto sapere solo l'handoff (non tutta la struttura con BSC, BTS, ecc..), con tutti i messaggi scambiati nel caso di MSC comune (chi lo inizia e perchè, perchè si fa preallocazione di risorse) e poi per quello tra diversi MSC ha voluto sapere, oltre a come funziona, perchè si tiene un MSC anchor e non si fa tutto senza un punto centralizzato (perchè lì ci tengo delle informazioni sulla chiamata, soprattutto quelle per il charging, che non posso o sono troppo "scomode" da trasferire ad ogni cambio di MSC).
 
- Android: esempio di codice di un BroadcastReceiver.
Io gli ho scritto la parte di dichiarazione che va fatta nel manifest (con assegnazione di intent-filter), gli ho scritto che il mio receiver deve estendere la classe BroadcastReceiver e implmentare la logica dentro al metodo on Receive() e infine gli ho fatto uno spezzone di codice su come va richiamato il receiver da un'altra activity (creazione dell'oggetto intent e sendBroadcast(intent) ). Gli è bastato, e poi mi ha chiesto come mai si chiama proprio sendBroadcast la funzione (perchè vengono risvegliati TUTTI i broadcast receiver che si sono registrati sotto quella categoria e azione, non è un sistema 1-a-1 come per le activity, dove invece se ne seleziona sempre e comunque una tra quelle che fanno match).
 
- J2ME: cosa cambia rispetto a J2SE.
Divisione in configurazioni e profili, modello di protezione (mi ha chiesto soprattutto come funziona il sandbox).
Ha voluto sapere quali tipi di classi NON ci sono rispetto a J2SE e quali invece possono essere utilizzate.
 
- UPnP: scambio dei messaggi nel caso di un device che vuole notificare i control point di una variazione di stato.
Gli ho messo tutto lo scambio di messaggi tra device e control point, ha voluto in più che gli dicessi per ogni messaggio quale protocollo si usa, quali sono fatti in multicast (solo discover e alive) e di GENA ha voluto sapere cosa invia in risposta il device al control point (l'intera tabella di stato attuale) e se la Notify è fatta in multicast ai control point registrati o in unicast (io non lo sapevo e gli ho risposto che avrebbe senso farlo in multicast, lui ha detto "in effetti sì, ma in gena non viene fatto!", non ci sono ottimizzazioni in merito perchè bisognerebbe gestire il gruppo di sottoscrittori e quindi vengono mandate in unicast).
 
- AODV: ha voluto sapere tutto il funzionamento, specialmente la differenza tra i timeout del link avanti e dei link indietro e a chi vengono mandati i messaggi di RERR (solo ai nodi "attivi", e lui "ok, attivi in base a quale timeout?". Risposta: quello dei link avanti, configurati dal passaggio di RREP).
 
20/02/2014
 
1) JINI: meccanismo di lease in particolare più varie domande (solite cose, quando in multicast, quando in unicast, come fare a non far propagare richieste dal PO quando lease scade, perché lease, chi programma PO, come avviene discovery e come Client trova Broker, piccolo parallelismo con UPNP)
2) Mobile-IP: handoff tra due FA, tutto standard come sopra
3) D-GPS
4) RADAR vs Ekahau
 
Altre domande che sentivo dall'altro ragazzo che faceva l'orale da me:
1) Android (mi pare meccanismo intent con "codice"), se si avviano Activity di app differenti si avviano nuove DVM? Come avviene comunicazione tra di loro (Binder IPC in sostanza)
 
03/03/2014
1) Domanda legata all'attività progettuale: AsyncTask vs Service perchè usare il primo invece del secondo? (interazione con il thread di UI), la seconda è troppo specifica dell'attività.
 
2) AODV: cosa succede in caso di link broken? Quali sono i timeout per RREQ/RREP? Come sono fatte le tabelle sui nodi?
 
3) JINI: meccanismo di lease e funzionamento su entrambi i lati (service provider,client), chi programma il proxy object (service provider) e chi incorpora il lease (service broker), come ? (campo durata all'interno di una struttura che controllo prima di ogni chiamata). Come fa il client a "scoprire" il broker? (multicast ad indirizzo fisso o broadcast).
 
4) Wi-Fi 802.11: Hidden/Exposed node, descrizione delle problematiche.