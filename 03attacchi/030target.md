# Analisi dei Bersagli

## Killchain

Uno hacker lavora in due modalità:

* Senza target preciso
  * Gira per l’internet e conquista macchine deboli a caso
* Con target preciso
  * Applica una sequenza di operazioni, la Killchain

## OSINT

![OSINT](../gitbook/images/osint.png)

Prima di qualsiasi attacco mirato l’attaccante deve acquisire informazioni sul bersaglio.

Molte informazioni sono reperibili in rete senza destare sospetti: **Open Source Intelligence** (_OSINT_):

* Dati pubblici economici o legali
* Motori di ricerca
* Siti web
* Conferenze e ambienti accademici
* Blogs e Social Networking
* Metadati da foto e documenti

In particolare il DNS (_Domain Name System_) può essere interrogato per avere informazioni registrate del dominio:

* Server web e di posta elettronica
* Fornitori di Accesso e Servizio
* Nomi e indirizzi dei responsabili

### Google Hacking

Google permette stringhe di ricerca con qualificatori sintattici e operatori logici nella stringa di ricerca, p.es.

* site:nomesito  tutte le pagine indicizzate nel sito
* `frase site:nomesito`  contenenti la frase
* `link:nomesito`  altre pagine con link al sito
* `allintext:frase`  tutti i siti contenenti la frase
* `allintitle:frase`  frase nel titolo
* `cache:urlpagina`  per pagine rimosse

Esistono numerose utilities per compiere Google Hacking:

* Gooscan (Linux): http://dl.dropbox.com/u/10761700/gooscan.tar.bz2
* Google Hacks (Windows): http://google-hacks.softonic.it/

Attenzione: la scansione diretta dei server Google è contro i Termini di Servizio.

## Strumenti di OSINT

* **WaybackMachine** (https://archive.org/web/web.php)
  * 334 miliardi di pagine web del passato, archiviate
* **TinEye** (https://www.tineye.com/)
  * Ricerca i siti dove compare una data immagine
  * 30 miliardi di immagini catalogate
* **Maltego** (http://www.peekyou.com/)
  * Commerciale, ma ottimo
  * Cerca tutte le informazioni disponibili su vari servizi: web, email, social, documenti pubblici, …
* **Shodan** (https://www.shodan.io/)
  * Cerca sui dispositivi correntemente connessi alla rete, anche di _Internet of Things_ (frigoriferi, telecamere, ...)
* **Google Hacking DataBase** (https://www.exploit-db.com/google-hacking-database/)
  * Vulnerabilità trovate da Google nella sua indicizzazione

## Footprinting


## Fingerprinting

Serve a determinare il sistema operativo dei target, anche versioni e implementazioni specifiche e compiere una prima scansione delle vulnerabilità più palesi. Si divide in:

* **Fingerprinting Attivo**, contatta la macchina bersaglio
  * Invia stimoli e riceve responsi
  * Vede il comportamento del target allo stimolo con pacchetti errati
  * Si basa su un database di responsi possibili
* **Fingerprinting Passivo**, non contatta il bersaglio
  * Ispeziona i dettagli interni dei pacchetti ricevuti
  * Nota i campi inutilizzati delle testate TCP/IP
  * Osservala presenza e tipo di opzioni
  * Determina l'uso dei flag TCP - Push, Urgent, Fin
  * Vede la frequenza di vari tipi di traffico
  * Acquisisce informazioni sulla vittima derivate da altri siti
