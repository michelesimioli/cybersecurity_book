# La Difesa

Non esiste una formula unica e globale per definire la difesa da attacchi informatici.

Vi sono però alcuni principi _strategici_ di base per l'impostazione di una difesa efficace.

## Modello a Forchetta

La difesa globale dei sistemi può essere rappresentata da una forchetta a tre punte:

* Difesa - opporre resistenza agli attacchi
* Detezione - accorgersi degli attacchi in corso
* Responso - contrastare gli attacchi

### Difesa

#### Difesa Passiva

Consiste nell'applicare le **migliori pratiche** (_best practices_) di ingegneria informatica:

* firewalls e filtraggio pacchetti
* uso di _proxy_ per impedire il collegamento diretto interno-esterno
* corrette procedure di _backup_ e _restore_
* autenticazioni multifattore
* permessi minimi per il lavoro da svolgere
* uso pervasivo di comunicazioni crittografate
* difesa fisica dei sistemi
* eliminazione dei servizi inutili
* limitazione della diffusione delle informazioni

#### Difesa in Profondità

I sistemi sono difesi a più livelli:

* firewall perimetrale esterno
* zona smilitarizzata intermedia - _DeMilitarized Zone (DMZ)
* segmentazione delle reti interne
* firewall personali

#### Difesa Dinamica

I sistemi non sono costantemente sotto attacco, ma lo possono divenire in qualsiasi momento. La difesa consiste di **profili di difesa**, a livelli differenti, con la possibilità di passare rapidamente da un profilo all'altro.

Si va da una situazione _rilassata_ in cui il lavoro è normale, ad una elevazione della sicurezza con limitazioni al lavoro possibile, ad eventualmente un livello massimo con distacco dalla rete e cessazione temporanea del lavoro.

### Detezione

Molti attacchi informatici sono noti (dal Catalogo CVE per esempio) e hanno **segnature** specifiche, cioè pacchetti software particolari, sequenze particolari schemi riconoscibili.

Esiste software che è in grado di riconoscere queste _segnature_, gli **Intrusion Detection Systems** (IDS) - Sistemi di Detezione Intrusioni.

Questi sono di due tipi principali:

* **Net IDS** (N-IDS) - monitorizzano attività sospette sulla rete
* **Host IDS** (H-IDS) - monitorizzano attività sospette sui singoli computer

Le attività avvengono di solito in simultanea su parecchi computer e in più luoghi della rete. Uno IDS è quindi costituito da più **sonde** che raccolgono i dati anomali, che comunicano con una **console di controllo**.

Quest'ultima analizza i dati sospetti, conduce correlazioni, consulta basi di dati di vulnerabilità, ed eventualmente allerta il personale o il sistema di _responso_.

### Responso

Tipicamente deve essere identificato ed adeguatamente incaricato del personale che si occupa di **Incident Response** - Responso agli Incidenti.

La squadra di responso deve avere l'autorità per intraprendere azioni contrastive agli attacchi, anche a costo di ridurre la produttività aziendale.

Devono essere preventivamente identificati **scenari di responso** che elencano le azioni da eseguire.

Devono essere condotti test a intervalli regolari per assicurasi della efficacia delle azioni di responso.

## Addestramento del Personale

Il miglior sistema tecnologico di difesa informatica non è valido se il personale non è addestrato ad usarlo.

Inoltre molte _esposizioni_ dipendono da comportamenti del personale che sono forse accettabili su PC personali, ma non sicuramente durante l'utilizzo dei sistemi informativi aziendali.

E' necessario che esista un documento esplicito di **Policy di Sicurezza**, che indichi:

* le azioni non concesse
* il monitoraggio in essere
* i responsabili esecutivi
* le penalità per trasgressioni

E' necessaria una **campagna di addestramento** per il personale che:

* permetta di acquisire consapevolezza sui problemi di sicurezza
* descriva i pericoli e le contromisure
* indichi e motivi le pratiche pericolose
* si assicuri della ricezione delle informazioni fornite

