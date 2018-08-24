# DOS e BOT

## Diniego di Servizio

E’ impedire volutamente il funzionamento dei sistemi o delle reti della vittima.

Si distingue in:

* **Denial of Service** (_DOS_) da parte di un singolo attaccante
* **Distributed Denial of Service** (_DDOS_) da parte di molti attaccanti simultaneamente

Gli attacchi DOS coinvolgono spesso anche computer o reti non della vittima designata: danni collaterali. Questo è dovuto alla interconnessione complessa in Internet, e anche a connessioni esistenti ma non documentate.

### Scopi del DOS

* **Attacco di Cyberwarfare**
  * Nazionale o terroristico. Può avvenire per:
    * Parte di guerra calda vera
    * Pressione e intimidazione sul nemico
    * Vendetta limitata a torti subiti
* **Diversivo**
  * Per nascondere delle azioni offensive nei confronti di computer terzi
  * Occorre considerare quali relazioni di fiducia hanno i computer attaccati nei confronti degli altri
* **Degradazione del Servizio**
  * Per favorire la concorrenza a scopo di lucro
  * Per screditare politicamente l’ente vittima (Hackerism)
  * Per richiedere riscatto (**Ransomware**)

Il DOS vuole distruggere. Nè gli hacker nè i criminali di solito vogliono distruggere i computer, ma conquistarli e usarli, e di solito a scopo di lucro diretto o indiretto.

Il primo e storico motivo di DOS è da parte di uno hacker di dimostrare come è “bravo”. Ma è passato di moda.

Il secondo motivo è di arrecare danno al nemico, nazionale, politico, commerciale o religioso. Questo tipo di DOS è in forte espansione.

### Detezione e Responso

La detezione è probabilmente rapida, visto il degrado repentino delle performance.

Occorre comunque dichiarare ufficialmente lo **stato di attacco**:

* Si rende attiva la **Squadra di Responso**
* Potrebbe essere un malfunzionamento naturale dovuto a condizioni transienti

Occorre determinare l’ambito ed estensione dell’attacco:

* Un sistema
* Un’intera rete
* Tutte le nostre reti
* Il nostro _Access Provider_
* Una parte più vasta dell’Internet

Il responso immediato implica l’isolamento dei componenti attaccati dal resto della rete: **air gap**.

Air Gap - spazio d’aria - è lo slang per staccare il cavo di rete: c’è dell’aria tra la spina e la presa.

I componenti attaccanti, se identificati, sono subito spenti.

I DOS sono per forza sostenuti nel tempo, ma non possono avere durate troppo lunghe. Sono di solito dai pochi minuti ai giorni, con qualche ora come media. Più tempo durano e più l’attaccato ha modo di organizzarsi e far intervenire le Squadre di Responso aziendali o nazionali.

Se un mero PC individuale è coinvolto in un DOS di vasta portata non può praticamente farci niente e deve attendere l’intevento di altri. Si consiglia di staccarsi dalla rete e lavorare temporaneamente in locale.

La Squadra di Responso ad un DOS ha il difficile problema di identificare i veri responsabili, al più presto, in particolare la locazione fisica da cui parte l’attacco. Se sono hackers o criminali interviene la polizia.

Se l’attacco è condotto da una potenza straniera e si scopre quale, può essere in futuro un “casus belli”.

Se è condotto da un **BotNet** (vedi oltre) con mandante non identificabile, non si può forse praticamente fare niente, se non aspettare che smetta.

## BOTs

**BOT** è l’abbreviazione di **Robot**, ed originariamente era un programma autonomo per lo svolgimento di operazioni ripetitive con comunicazioni in rete.

Si possono distinguere tre tipologie:

* **Bot Benevoli**
  * Compiono azioni vantaggiose per più attori ed eque (_fair_)
  * Si adeguano alle specifiche del file di controllo `robot.txt`
* **Bot Malevoli**
  * Compiono azioni vantaggiose per un attore ma inique (_unfair_) o svantaggiose per altri
  * Ignorano il file `robots.txt`
* **Bot Malefici**
  * Concepiti per compiere azioni dannose per una o più vittime

Un BOT veniva anche chiamato un Agente Intelligente

### BOT Benevoli

Un Bot Benevolo è di vantaggio a chi lo usa e a chi viene usato. Esempi possono essere:

* Ricerca orari di treni o aerei
* Ricerca di un prodotto o servizio ottimale, fornito da più mercanti
* Ricerche bibliografiche o testuali da vari siti offerenti
* Indicizzazione di siti web
  * Detti _Web Spiders_ o _Web Crawlers_
* Giochi di ruolo online e strumenti di Chat

I siti che servono i Bot Benevoli hanno di solito un **Application Programming Interface** (_API_) standard e documentata, ed una **Policy d’Uso Accettabile** (_AUP_).

### Bot Malevoli

Un Bot Malevolo compie operazioni in emulazione o sostituzione di un essere umano, che sarebbe troppo lento. La sua velocità operativa va a discapito degli altri esseri umani veri con cui concorre.

Esempi possono essere:

* Aumento degli “I Like” di siti per incrementarne il rating
* Aumento del traffico per gli _Analytics_ e il SEO (_Search Engine Optimization_)
* Acquisto di biglietti e token a favore di bagarini
* Commercio elettronico automatico per creazione di scarsità o domanda
* _Fake accounts_ su siti social per influenzare politicamente i veri partecipanti

I Bot Malevoli spesso sfruttano la presenza di **algoritmi di ranking**, o la **presunzione implicita di reale esistenza**.

Un BOT malevolo non è criminale, ma è “unfair”: compie operazioni di rete troppo velocemente rispetto ad un essere umano.

L’uso di Bot malevoli è molto comune nella giungla Internet da parte di grossi enti.

Istituti Finanziari della City sono alla continua ricerca di piccoli vantaggi finanziari nel trading mondiale e compiono migliaia di transazioni al secondo, da ciascuna delle quali guadagnano pochi pennies.

In alcuni social è noto che metà degli accounts e tre quarti del traffico sono fake.

Se gli algoritmi di ranking sono noti è possibile inventare Bot che modificano le preferenze per certi siti o servizi. Dato che i siti web tracciano la provenienza delle richieste e registrano le preferenze, un Bot malevolo che ha contraffatto l’indirizzo di provenienza può facilmente compromettere la reputazione di un cittadino onesto.

La maggior parte dei progettisti di siti web presume che verranno visitati da umani, non da Bots, e non ha previso quanto veloci siano i Bot.

### Bot Malefici

I Bot Malefici sono programmi inavvertitamente installati e sotto il controllo di un criminale remoto.

Il computer infettato con un tale Bot viene detto **zombie**.

Lo zombie compie operazioni malefiche con traffico illegale in uscita.

Il criminale lentamente infetta con lo stesso Bot un numero elevato di computer che poi può controllare: una **BotNet**.

Le BotNets contano molte migliaia di zombie, e a volte vengono affittate per compiere attacchi.

Le azioni criminose compute possono essere:

* Attacchi di Diniego di Servizio Distribuito (DDOS)
* Campagne di spam o di _phishing_
* _Scraping_ (copia totale) di siti web per impersonarli
* Diffusione di virus e vermi

I BOT malefici non sono “unfair”: eseguono operazioni che violano la legge. Paesi diversi però hanno leggi diverse.

In particolare non è ben definita globalmente la posizione legale di un paese che ospità un Bot che compie le sue operazioni al di fuori di tale paese: tocca agli altri difendersi.

Se un Bot compie 10 connessioni di rete al secondo, 1000 Bot con attacco coordinato vanno meglio, e si arriva ad un milione di nodi per alcuni BotNet.

In casi moderni i nodi non sono PC ma oggetti stupidi dell’**Internet of Things**. Nel 2016 l’attacco _Mirai_ è stato compiuto da un milione di telecamere di sorveglianza infettate, e ha “tirato giu” la CNN e il Guardian. Questo sarà un problema interessante per il prossimo futuro.

### Difesa dai BOT

* **BOT Malevoli**
  * **CAPTCHA**: attività per discriminazione tra essere umano e robot - _Test di Turing_
    * Esempio: riconoscimento immagini
    * Ma col _Machine Learning_ i BOT stanno diventando bravi
  * Limitazione di richieste e traffico (_throttling_)

* **BOT Malefici**
  * Impedire la comunicazione diretta tra computer interni alla rete e l’esterno
    * Uso di Proxy
    * Monitorare il traffico in uscita
    * Egress Filtering
    * Net-based Intrusion Detection Systems (N-IDS)

Il vecchio problema del Test di Turing è di far parlare un essere umano tramite terminale, con qualcuno nell’altra stanza, e decidere se è un umano o un computer.

Le cose che i computer sanno fare peggio sono il riconoscimento delle immagini, e i Captcha sono programmi che si basano proprio su questo.

“Captcha” viene da “capture”, con la modifica che lo fa sembrare la parola slang americana “gotcha” - I got you - ti ho beccato.

I programmi di Intelligenza Artificiale, in particolare di Deep Learning, stanno però diventando sempre più bravi nel riconoscimento di immagini.

Tali programmi hanno bisogno però di essere addestrati, fornendo loro immagini e dicendogli cosa sono. Da qui imparano.

La cosa malefica è che una buona parte dei Captcha presenti in rete non sono Test di Turing veri, ma istanze di training per i motori di Deep Learning. Noi stiamo insegnando ai computer in modo che poi loro possano impersonarci.

L’unico modo efficace di contrastare i Bot è di rallentarne le operazioni: un massimo al minuto.

“Throttle” vuol dire “strozzare”.

Gli zombie vanno sempre combattuti. Non si può impedire che vengano installati a nostra insaputa, ma si può contrastare la loro comunicazione tra i nostri computer e lo hacker che li controlla.

Lo **Egress Filtering** - filtraggio in uscita - presuppone che anche i nostri computer possano eseguire operazioni malefiche nei confronti di terzi, e le bloccano.

Gli **IDS Net-based** ispezionano quindi anche i pacchetti in uscita per difendere il resto del modo da noi.

Anzichè proteggere migliaia di computer aziendali dall’impianto surrettizio di Bots, è più facile costringere il traffico attraverso un Proxy, e sterilizzare tale macchina dai Bot.
