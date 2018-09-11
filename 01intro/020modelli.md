# Modelli di Sicurezza Informatica

Per poter capire cos'è e cosa coinvolge la sicurezza informatica è necessario un **modello** che la descriva, e dal quale sia posssibile trarre conseguenze e arrivare a decisioni.

Si sono evoluti una serie di modelli per rappresentare le situazioni di cybersecurity, gli attaccanti coinvolti, la tipologia di operazioni, i danni causati.

Fin dagli anni '90 in America si è affermato il modello di sicurezza detto in italiano **Modello RID**. Con varie sigle e alcune piccole varianti, questo modello rimane tuttora di base per l'intercomunicazione tra persone che si occupano di difesa informatica.

Questo modello si concentra sugli attacchi ai dati e alla loro compromissione: definisce tre tipi di motivi per gli attacchi e separa attacchi compiuti da gruppi e da individui.

![Modelli](../gitbook/images/modelli.png)

Il _Modello RID_ è l'abbreviazione dei termini:

* **Riservatezza** - dalla segretezza alla privacy
* **Integrità** - autorevolezza dei dati
* **Disponibilità** - contro l'indisponibilità di servizio

![RID](../gitbook/images/rid.png)

Il _Modello RID_ si preoccupa della sicurezza in termini di **dati** e **programmi eseguibili**.

## Riservatezza

Mantenere la riservatezza significa impedire che chi non è autorizzato venga a conoscenza dei dati.

E' uno spettro di aspetti, i cui capi sono:

![TopSecret](../gitbook/images/topsecret.png)

* **Segretezza**
  * Proprietà intellettuale
  * Piani del business
  * Segreti dell’organizzazione

![GooglePriv](../gitbook/images/googlepriv.png)

* **Privacy**
  * Informazioni di identificazione personale
  * Informazioni relative alla salute, idee, orientamenti, fede
  * Dati finanziari e di pagamento

La sua protezione è un requisito fondamentale, legale o contrattuale.

## Integrità

L'inegrità consiste nel consentire la produzione, modifica o cancellazione dei dati solo agli autorizzati.

Le modifiche non autorizzate possono essere:

* **Incidentali** (rumore, ...)
* **Intenzionali** (frode, …)

Nel mantenimento dell'integrità ccorre occuparsi sia della _protezione dei dati_ che della _protezione dei programmi eseguibili_ (codice software).

* La protezione dei **dati** si ottiene con:
  * Validazione degli ingressi dati da parte degli utenti
  * Gestione degli errori umani e di sistema
  * Gestione dei troncamenti o arrotondamenti impropri, che sono un'intrinseca conseguenza della rappresentazione dei numeri da parte del computer
  * Gestione degli errori nella comunicazione in rete
* La protezione dei **programmi** si ottiene con i seguenti accorgimenti:
  * Gestione delle versioni prodotte in modo che non interferiscano tra loro
  * Monitorare e combattere le infezioni da virus e altri programmi malefici
  * Garantire l'affidabilità dei programmi e l'assenza di _bachi_

### Non Ripudio

Il _Non Ripudio_ è una conseguenza della manutenzione dell'_integrità_. Qualcuno lo indica come categoria separate, ma solitamente ricade nella categoria _Integrità_ della triade _RID_.

Si ha **ripudio** quando l'autore dei dati o dei programmi nega di esserlo e non si assume la responsabilità.

Il **Non Ripudio** è l'identificazione positiva ed univoca dell’autore di un cambiamento ai dati o al codice dei programmi.

Questa è una preoccupazione relativamente recente ma percepita di notevole importanza. 

## Disponibilità

I processi, i prodotti e i dati informatici devono essere disponibili per le persone autorizzate quando è necessario che esse li usino.

Ciò puo essere impedito da:

* **Eventi catastrofici**
  * Geoambientali (alluvioni, terremoti, ecc)
  * Geopolitici (guerre, ecc.)
* **Guasti di sistema**
  * Software di base
  * Software applicativo
* **Errori umani** (comportamento **colposo**)
  * Configurazioni, ecc.
* **Attacchi intenzionali** (comportamento **doloso**)
  * Indisponibilità di Servizio - incluso virus e altro software malefico di varie tipologie
  * Indisponibilità di Servizio Distribuito - attacco da parte di un'intera rete

### Considerazioni

Alcune frasi e vocaboli sono connessi alla disponibilità dei sistemi:

* **Punto Singolo di Fallimento**
  * Componente critica del sistema, senza il quale il servizio informatico cessa di funzionare
  * E' da evitare accuratamente nella progettazione degli applicativi
* **Resilienza**
  * Indica un'adattamento automatico a situazioni di funzionamento anomale (ma previste) e non ottimali
  * Evita una totale cessazione del servizio per guasti minori
  * Si ottiene con la ridondanza dei componenti critici
* **Replicazione dei Dati**
  * Salvataggi automatici con uso automatico delle copie in caso di problemi alla versione principale
  * Si chiamano anche soluzioni di _Alta disponibilità_ - tendono ad essere costose
* **Scalabilità**
  * Il successo era imprevisto, magari perchè era un progetto prototipo o temporaneo, ed ora è problematico
  * Allocazione elastica delle risorse, _a richiesta_ - Vantaggio delle soluzioni cosiddette _Cloud_
* **Resilienza**
  * _Degrado parziale_ del servizio- mantenere le operazioni vitali e sacrificare quelle meno importanti
  * Piani di _Recupero da Disastri_, che potrebbero altrimenti essere definitivi e fatali per l'azienda. E' una necessità specie in un paese con elevati rischi sismici o idrogeologici.

## Modello RID ed Attaccanti

Il _Modello RID_ non definisce soltanto le categorie di dati e programmi che devono essere difese, ma indica anche quali siano gli **Attori** o **Figure Attive**, che altro non sono che eufemismi per **Attaccanti**.

![Figure Attive](../gitbook/images/figatt.png)

Tali categorie sono sei.

Innanzi tutto viene fatta una distinzione, lungo il bordo destro del diagramma, tra i **gruppi** di attaccanti (primi tre) e i **singoli** attaccanti (secondi tre). I gruppi hanno evidentemente più risorse dei singoli ed in media costituiscono un probleme maggiore.

Vengono poi indicati, lungo il bordo sinistro del diagramma, tre raggruppamenti che indicano i **motivi** che guidano gli attaccanti. Questi possono essere:

* **alti ideali** - patria, libertà, religione, visione del mondo - tutto quello che in passato e presente causa _guerre_. Infatti gli attaccanti di questo tipo sono coinvolti nell'attività detta **Cyberwarfare** o Guerra Cibernetica.
* **lucro** - vantaggio monetario o di potere ottenuto con strumenti informatici ma con attività illegali
* **psicologie perverse** - le motivazioni rimanenti raggruppate e varie, che hanno valenza dannosa o distruttiva nella società civile. Possono andare dalla vendetta alla pirateria, al danno inconsulto, alla mera affermazione di potere malefico.

Esaminiamo brevemente le categorie descritte dal _Modello RID_.

### Servizi Segreti e Nazionali

Il loro scopo è di favorire il _bene_ e di combattere il _male_. Al limite cinico, è di favorire _noi_ e di combattere gli _altri_, anche dal punto di vista di manutenzione dei diritti _democratici_, dei vantaggi commerciali, della predominanza politica.

Qui si trovano i vari tipi di Polizie Postali ed Informatiche, i sistemi di difesa nazionali, le agenzie nazionali di _Intelligence_ (o di spionaggio che dir si voglia).

L'enfasi è sulla **difesa**.

### Terroristi e Nemici

Questa è una categoria molto simile alla precedente come metodi di base, se non fosse che qui le attività sono _contro di noi_: contro la libertà, democrazia, tolleranza, _valori_ nostri. Evidentemente si può _comprendere_, ma non _giustificare_ nè tantomeno _tollerare_ il nemico.

Le attività sono preponderantemente di **attacco** o di preparazione ad esso.

### Mafie e Spionaggio Industriale

La differenza tra le due sottocategorie è che le _Mafie_ non sono enti giuridici riconosciuti, a differenza delle Aziende o Ditte commerciali o industriali.

L'attività criminale condotta consiste nel carpire informazioni riservate della concorrenza o di altri enti o cittadini, allo scopo di avere vantaggi principalmente monetari per sè.

Viene condotto anche il furto d'identità finanziario, il ricatto, il riciclaggio di denaro, gli assassini o i furti su commissione, ed ogni altro crimine che possa avvalersi direttamente o indirettamente dei mezzi informatici.

Molte grosse ditte possiedono dipartimenti dissimulati di _Intelligence Competitiva_.

### Criminali Privati

Le operazioni sono potenzialmente tutte quelle della categoria precedente, ma i mezzi sono più limitati.

Il singolo criminale deve al più presto _attualizzare_ i suoi guadagni, quindi le operazioni in questa categoria tendono ad essere più limitate di scopo e più veloci nell'esecuzione.

### Vendicatori

Il loro scopo non è il vantaggio personale ma il danno al bersaglio, che può essere una ditta, un grosso ente statale o privato, od una concezione generica pseudo-filosofica della realtà.

Vi si trovano sia i licenziati, spesso con competenze informatiche, che gli ecologisti, i protestatari, i paladini di cause.

Alcuni gruppi di rilievo in questa categoria sono **Anonymous**, oramai una sigla generica e inafferrabile per chi voglia compiere attacchi _politici_, e gli **Hacktivists**, gruppi ecologici e politicizzati che danneggiano siti o infrastrutture di governi illiberali, vivisezionisti, ditte OGM, TAV, ecc.

### Hackers

Tendenzialmente giovani, maschi e socialmente disadattati ma dotati di intelligenza e spesso notevoli capacità, compiono azioni illegali per **vanteria** nei confronti dei pari, o per **uso di sistemi** a cui non avrebbero accesso.

Si trovano tra loro i **pirati** informatici e i **Cyberpunk**, seguaci di filosofie anarchiche fantastiche o basate sui giochi di ruolo.

Gli hacker di _talento_ si trasformano più tardi in _criminali_ o vengono spesso fagocitati da mafie, spionaggio industriale o addirittura servizi nazionali o terroristici.

## Tipo di Operazioni

Le operazioni condotte dagli attaccanti possono essere:

### Aperte

* L’attaccante può essere identificato, e portare comunque a termine le operazioni
* Sono tipicamente danni: distruzione di dati, diniego di servizio, guerra cibernetica associata alla guerra calda
* Non sono molto comuni

### Coperte

* E’ indispensabile che l’attaccante non venga identificato durante le operazioni poichè il difensore può contrastare l’attacco e possono avvenire ritorsioni fisiche o legali
* Esempi sono: spionaggio e furto di dati, frodi e furto di valore, impersonazioni e furto di identità
* Sono molto comuni
* Il difensore può accorgersi del danno subito molto dopo la conclusione delle operazioni
