# Attacchi Avanzati

## Threat

![TipiThreat](../gitbook/images/tipithreat.png)

Un **threat** è una minaccia potenziale ad un sistema informativo con più o meno difese.

Quando le difese sono superate si ha un **breach** (ingresso).

Conseguentemente al breach si possono avere danni.

Sono visti tre livelli di threat:

* **Unsophisticated** (non sofisticato)
  * Di bassa intelligenza
  * Le normali difese bastano
* **Smart** (intelligente)
  * Con strumenti intelligenti
  * Più difficile contrasto
* **Advanced** (avanzato)
  * Con molti strumenti d’attacco
  * Molto ardui da contrastare

Se l’attacco è pesante e continuato vi si dà l’attributo **Persistent** (persistente).

Una minaccia ha un obiettivo definito e non è traffico casuale.

Una minaccia non sofisticata è un esecizio hacker da principiante.

Una minaccia _smart_ è più complessa, contiene dissimulazione, ha un inventore più capace, e richiede una difesa più pianificata. Si tratta comunque sempre di una tipologia singola di attacco.

Uno **Advanced Threat** è superintelligente, usa molte tipologie di attacco simultanee, è costato svilupparlo e costa mantenerlo.

_Persistent_ denota solo che l’attacco dura nel tempo. In realtà solo le minacce Advanced sono anche Persistent, le altre due sono di scopo ridotto e per gli attaccanti non ne vale la pena.

### Advanced Persistent Threat

I target di _Advanced Persistent Threats_ (**APT**) sono sistemi di alto valore, non PC.

Gli APT Hackers sono gruppi organizzati o enti segreti statali, poichè la conduzione di attacchi APT richiede molte risorse, e gli APT Hackers devono essere molto competenti.

I sistemi target hanno già di solito elevate difese passive e sistemi di detezione e prevenzione intrusioni, ma:

* Possono venire infettati internamente da malware apposito
* Vengono usate spesso vulnerabilità non ancora scoperte, per cui non esistono divese (**Zero Day Vulnerabilities**)
* Le operazioni sono condotte in modalità _stealth_ e ben dissimulate
* Lo APT viene a volte scoperto molto dopo (mesi) il suo impianto, quando ha causato danni considerevoli
* C’è spesso l’elemento sorpresa: tipi di attacchi innovativi e non previsti.

Uno **0day** - _Zero Day Vulnerability_ o _Virus_ o _Attack_ - è qualcosa che non si era visto prima, e come con un nuovo virus biologico non vi è immunità nè vaccini. Ci vuole tempo a svilupparli e intanto i sistemi sono vulnerabili.

Uno APT può venir percepito una vergogna per le grosse ditte o enti statali che lo subiscono, e a volte quando è scoperto non viene ammesso. Questo è vero soprattutto per gli Enti Finanziari, che perderebbero reputazione e clienti.

A volte la denuncia che un ente ha subito un APT può essere _fake_, allo scopo di danneggiarli. Purtroppo se si può dimostrare di aver subito un APT, non si pò facilmente dimostrare di non averlo subito. I fake news sono comunque sempre un grosso problema di reputazione.

### PenTesting e APT

![PenAPT](../gitbook/images/penapt.png)

Le attività di un _Penetration Tester_ e di un _APT Hacker_ sono simili, ma hanno anche differenze notevoli.

Un PenTester compie attività legali, evidentemente un APT Hacker no.
