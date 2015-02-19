-	Contesto di persistenza e sua gestione in caso di transazioni (tipo transaction_scoped e extended).
-	JMX
-	Invocazione di un'operazione su un MBean
-	Connettori e adattatori di protocollo, differenza tra Dynamic MBean e Open MBean
-	JNDI
-	Servizi aggiuntivi per i sistemi di directory
-	Perché è importante usare JNDI in app jee
-	@resource e momento di iniezione delle dipendenze (by need o all'inizializzazione con svantaggi e vantaggi).
-	Annotazioni
-	Definizione di una nuova annotazione
-	Retention policy con esempi di utilizzo di ciascuna.

Molto tranquillo e lascia il tempo per rispondere comunque abbastanza specifico, anche metodi da invocare, signature, ecc.


21.12.2012

-	Ereditarietà tra entity jpa, le 3 possibilità di mapping sul db della gerarchia e vantaggi e svantaggi di ognuna, cos'è una query polimorfica.
-	Scrivere codice jms di un session bean che invia un messaggio su un topic, parlare dell'architettura jms, perché esiste la classe session separata dalla connection, reliability. 
-	Descrivere cos'è un dynamic mbean e dire se i clienti si accorgono di quale tipo di mbean stanno interrogando. Cosa sono i connettori e gli adattatori jmx e qual è il connettore obbligatorio da specifica. 
-	Come sarebbe possibile fare un meccanismo a eventi in ejb, come funziona il meccanismo di notifiche in spring e in jmx.
 
 
31.1.2013
 
-	Confronto caching in jpa (da specifica) e in hybernate(coerenza cache a carico del programmatore, API evict() )
-	Garanzie di qualità in jms (a livello di header del msg e dei metodi del publisher). è preservato l'ordine dei msg nelle sessioni? come? (numerazione in sequenza, anche in sessioni non transacted)
-	Dynamic mbean con codice, MbeanInfo, vantaggi rispetto standard mbean.
-	Spring e proxy (codice) vs ejb e interceptor. Microcontainer vs container pesante.
-	Ho dovuto realizzare un applicazione con EJB (ha voluto schema e parte del codice del cliente, mi ha dato quasi mezz'ora di tempo) per gestire gli ordini provenienti da due clienti diversi e quali scelte avrei fatto per gestire il merge degli ordini. bastano i session bean? ovviamente no, ci sarebbero diverse soluzioni. Si è addentrato particolarmente nei dettagli delle mie scelte, ad es. come avrei gestito la concorrenza nell'accesso alla stessa tupla (in teoria basterebbe l'annotazione @transacionManagemente (CONTAINER) oppure marcare un methodo come Synchronized )

 
28/03/13
 
-	Hibernate caching: i 2 livelli, protocollo di invalidazione, molto nello specifico (avevo fatto il piccolo progetto opzionale su questo)
-	Spring: un pò di tutto, codice per la dep.inj (message renderer e provider delle slide, in particolare i file di configurazione xml), come fare dep.inj in spring, core (beanFactory, come fa a trovare un componente, come fa a sapere se un componente è libero -> NON LO SA, quindi restituisce lo stesso riferimento al cliente, gestione degli stateful -activation/passivation- codice del ProxyFactory e analogie con intercettori, e altre cose piu generali)
-	Clustering: un pò tutto quello scritto sulle slide, , codice del file xml di configurazione di apache mod cluster
-	JPA: @mappedSuperclass e Inheritance
 
un consiglio: imparate bene il codice, praticamente in ogni domanda ho dovuto scrivere un pezzo di codice. prof molto tranquillo e calmo
 
 
29/03/13
 
-	Progettare l'architettura di un'applicazione "tipo" EJB 3.0, stile esercitazione EJB del corso. Lascia 10-15 min per descrivere le classi (senza codice) e i componenti usati. Poi mi ha chiesto di spiegare le scelte fatte (SLSB, MDB, etc)
-	JPA: @mappedSuperclass a cosa serve.
-	JMX: differenza tra static MBean e DynamicMBean, sistema di notifiche in JMX.
-	Clustering e HA-JNDI
 
A differenza del collega sopra, non ho dovuto scrivere una linea di codice.
Confermo prof molto tranquillo.

 
28/05/2013

-	Spiegare il funzionamento a basso livello dei un RESTFul web service (progettino)
-	Clustering: cosa sono e come sono realizzati da jboss i fat client. Esempio con stub RMI. Quali politiche di load balancing e cosa succede se provo a contattare un nodo che è caduto sul server. 
-	MDB + JMS
-	Codice di un mdb in ascolto su un topic. + architettura e funzionamento JMS + come recuperare un topic all'interno di un mdb (@resource)
-	Qualità in JMS (tutte le proprietà e quali a livello di messaggio e quale a livello di sessione.)
-	Ack con e senza transazione. Modalità e discorso sui messaggi duplicati. (nella modalità client dove viene effettuato il .ack() )
-	@mappedSuperclass con esempio
-	JMX generale + connector e adapter (differenze e esempio)
-	spring parlare dei proxy
 
il prof è tranquillo e ti lascia tutto il tempo per ragionare

  
04/06/2013

-	Spring e Proxy, perchè vengono usati e differenze con intercettori in EJB
-	Componenti EJB e web Service: deployment Clienti -> WS -> AppServer EJB , codice e caratteristiche sia di EJB che della servlet in WS.
-	Jboss, Ha partition, HAjndi, configurazione Fat vs Thin, replicazione e failover.
-	JPA, entity e entity manager.

prof tranquillo, ti da un foglio sul quale poter fare uno schema di quello che devi dire. Nel mio caso, se sbagli qualcosa non ti corregge mentre parli ma te lo dice solo alla fine dell'esame


26/07/2013

-	EJB 3.0 modellare un caso proposto dal prof elencando i componenti e il modo di farli interagire. Si trattava di una chat con diverse room 
-	Cluster HA-PARTITION descrizione dicendo le principali caratteristiche
-	Dep. Inj. in Hibernate e differenze con quella di EJB 3.0 con tanto di codice per farla (diciamo le api principali e grosso modo come è fatto l'xml di configurazione)

confermo quanto detto dagli altri ovvero prof. tranquillissimo che ti lascia tutto il tempo per pensare e per scrivere, ma non ti corregge mai quando parli tranne che a fine esame. Quindi consiglio di sfruttare bene il tempo a disposizione per pensare a come formulare la risposta. Se dimenticate di dire qualcosa considerate che non ve lo farà sapere, ma sarà contato come errore. Ad esempio io con l'HA PARTITION pur sapendoli molto bene, non ho fatto il discorso sul fat e thin client e me lo ha fatto notare solo dopo avermi dato il voto.

 
26/09/13

-	Componenti EJB. MessageDrivenBean e JMS. se un mdbean è registrato a una coda e arriva un messaggio, il messaggio viene consumato da una sola istanza, o da tutte le istanze di quella classe di componente? Risposta: da una sola istanza. (quindi i topic hanno poco senso coi MDbean, a meno che non ci siano classi di MDbean differenti nella applicazione...)
-	Annotation, meta annotation e retention policy.
-	Dependency injection in Sping (codice delle slide)