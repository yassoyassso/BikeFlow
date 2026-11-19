**PROJECT PLAN**

# BikeFlow

*Sistema intelligente di bike sharing*

|  |  |
|---|---|
| Corso | Ingegneria del software |
| Anno accademico | 2026/2027 |
| Documento | Project Plan – Piano di progetto |
| Versione | 1.0 |
| Data | 18 novembre 2026 |
| Gruppo | Sara Onunifi, Yassir khariche, Mohamed Amine Guelmine |
| Repository GitHub | https://github.com/ykhariche-cell/BikeFlow |
| Condiviso con | garganti (professore), silviabonfanti (esercitatrice) |

### Componenti del gruppo

| Nome e cognome | Matricola | Account GitHub |
|---|---|---|
| Sara Ounifi | 1099090 | saraounifi |
| Yassir Khariche | 1099122 | ykhariche-cell |
| Amine Guelmine | 1081219 | Aamine00 |

*L’assegnazione dei moduli (Componente 1, 2, 3) e dei ruoli di gestione ai singoli componenti non è ancora definita e sarà registrata nel documento di Project Management.*

### Storia delle versioni

| Versione | Data | Modifiche |
|---|---|---|
| 1.0 | 18/11/2026 | Prima versione del piano di progetto |

*Documento strutturato secondo i punti del Capitolo 2.1 indicati nel materiale del corso.*

## 1. Introduzione

### 1.1 Panoramica del progetto
*rivedere la descrizione*
BikeFlow è un’applicazione software progettata per gestire un servizio di bike sharing. Il sistema permette agli utenti di noleggiare biciclette in modo semplice ed efficiente, promuovendo una mobilità urbana sostenibile.

Attraverso l’applicazione, gli utenti possono registrarsi, effettuare l’accesso, cercare biciclette disponibili, prenotarle, iniziare e terminare un noleggio e gestire i pagamenti. Il sistema include inoltre un’area amministrativa per gestire utenti, biciclette, stazioni, manutenzioni e informazioni sui noleggi.

### 1.2 Obiettivi del progetto

- Consentire agli utenti di registrarsi e gestire il proprio account.
- Fornire informazioni sulle stazioni e mostrare la disponibilità delle biciclette.
- Consentire la prenotazione delle biciclette.
- Gestire l’inizio e la conclusione dei noleggi.
- Calcolare i costi in base alla durata e al tipo di abbonamento.
- Consentire agli amministratori di gestire biciclette e stazioni.
- Monitorare le attività di manutenzione e i problemi segnalati.
- aggiungiamo un operatore fisico che si occupa della manutenzione?

### 1.3 Ambito del progetto

**Area utente:**  Registrazione e accesso tramite nome e cognome, email o numero di telefono ; gestione del profilo personale con informazioni tipo numero di telefono, email, nome e cognome, indirizzo e possibilità di log out; ricerca delle biciclette disponibili usiamo il gps? barra di ricerca?; prenotazioni no; avvio e conclusione dei noleggi; storico dei noleggi; gestione di abbonamenti e pagamenti. 


**Area amministratore:** gestione degli utenti, delle biciclette e delle stazioni; gestione della manutenzione; monitoraggio dei noleggi; statistiche del sistema.

**Fuori dal perimetro.** Nella versione iniziale non saranno integrati fornitori di pagamento reali, dispositivi GPS o lucchetti fisici per le biciclette: pagamenti e hardware sono simulati. Eventuali estensioni (ad esempio biciclette elettriche con gestione della batteria) sono considerate sviluppi futuri.


### 1.4 Risultati attesi

Il risultato atteso è un’applicazione funzionante e documentata che implementi le principali funzionalità di un sistema di bike sharing. Il progetto comprenderà anche diagrammi UML, documentazione tecnica, test automatici e un repository GitHub con il codice sorgente completo.

## 2. Modello di processo

Il progetto seguirà un modello **iterativo e incrementale guidato dai casi d’uso**, a timebox. Organizziomao  il lavoro è organizzato in una fase di avvio, quattro iterazioni di due settimane e una chiusura finale??

**Avvio.** Si definiscono perimetro, requisiti ad alto livello, use case diagram, class diagram di dominio e architettura di massima. Si configurano repository, progetto Maven e board GitHub. La fase produce il project plan e la prima versione della specifica dei requisiti.

**Iterazioni.** Ogni iterazione realizza un sottoinsieme di casi d’uso, scelto per priorità e rischio, e contiene un piccolo ciclo completo: affinamento dei requisiti, modellazione UML e design, implementazione, test e integrazione. Le iterazioni sono gestite con le milestone di GitHub e con issue assegnate a una persona.

| Iterazione | Contenuto | Incremento |
|---|---|---|
| It.1 | Registrazione e accesso, biciclette e stazioni, disponibilità | Utenti, flotta, stazioni e persistenza di base |
| It.2 | Prenotazione, noleggio, restituzione, tariffa e pagamento simulato | Ciclo completo del noleggio |
| It.3 | Abbonamenti, segnalazione guasti, manutenzione | Abbonamenti e manutenzione |
| It.4 | Funzioni amministrative, report e statistiche, refactoring | Backoffice e consolidamento |

**Chiusura di ogni iterazione.** Review con demo interna, esecuzione di tutti i test, tag di release nel repository e breve retrospettiva (cosa ha funzionato, cosa cambiare). Rischi e calendario vengono rivisti e le differenze rispetto al piano sono annotate nella sezione Modifiche.

**Chiusura finale.** Completamento della documentazione, verifica del progetto e preparazione della presentazione, senza nuove funzionalità.

Il modello è stato scelto perché il perimetro è chiaro ma il rischio di integrazione tra i tre moduli è reale: le iterazioni permettono di integrare presto e di tagliare le funzionalità meno prioritarie se i tempi stringono. 

## 3. Organizzazione del progetto

Il progetto sarà realizzato da un gruppo di tre studenti. Il lavoro è organizzato su due livelli: tre **moduli** di sviluppo, ciascuno con un componente responsabile, e quattro **ruoli di gestione**.

### 3.1 Moduli di sviluppo

| Componente | Area principale | Responsabilità |
|---|---|---|
| Componente 1 | Utenti e amministrazione | Registrazione, accesso, profili e funzioni amministrative |
| Componente 2 | Biciclette e stazioni | Gestione biciclette e stazioni, disponibilità, manutenzione + segnalazione guasti |
| Componente 3 | Prenotazioni e Costi| Prenotazioni, noleggi, restituzioni, calcolo dei costi |

### 3.2 Ruoli di gestione

I ruoli sono **definiti ma non ancora assegnati** ai componenti. L’assegnazione sarà registrata nel documento di Project Management, con una persona di riferimento per ogni ruolo. Con tre componenti, due dei ruoli (tipicamente project manager e configuration manager) possono essere accorpati; ogni componente avrà comunque almeno un ruolo di gestione oltre alla responsabilità di un modulo.

| Ruolo | Responsabilità |
|---|---|
| Project manager | Pianificazione, calendario, monitoraggio, iterazioni e retrospettive, project plan |
| Configuration manager | Repository GitHub, branch e pull request, tag di release, board, convenzioni |
| Responsabile requisiti e modellazione | Specifica dei requisiti, use case, diagrammi UML e progetto StarUML |
| Responsabile qualità e test | Piano di test, JUnit, copertura, metriche, code review |

### 3.3 Schema organizzativo

Il gruppo adotta uno schema di tipo **democratico decentralizzato** (tra pari), adatto a tre persone con lo stesso livello di esperienza. Le decisioni tecniche importanti sono prese insieme; la responsabilità del singolo modulo e del singolo ruolo resta della persona assegnata.

### 3.4 Responsabilità condivise

Analisi dei requisiti, diagrammi UML, architettura software, integrazione dei moduli, test, documentazione e presentazione finale sono attività condivise: ognuna ha un responsabile di ruolo (sezione 10) ma tutti i componenti contribuiscono.

### 3.5 Comunicazione

Il gruppo organizzerà incontri per discutere i progressi, assegnare i compiti e risolvere i problemi. GitHub è la piattaforma principale di collaborazione: ogni componente aggiorna lo stato delle proprie issue e comunica i progressi sulla board.

## 4. Standard, linee guida e procedure

### 4.1 Standard di sviluppo

| Strumento | Scopo |
|---|---|
| Java | Linguaggio di programmazione |
| Eclipse | Ambiente di sviluppo (progetti Eclipse) |
| Maven | Gestione delle dipendenze e della build |
| Git e GitHub | Controllo di versione e collaborazione |
| StarUML 5 | Modellazione UML e generazione dello scheletro del codice |
| JUnit | Test automatici |
| Database embedded | Memorizzazione dei dati, senza servizi esterni |

### 4.2 Linee guida di programmazione

- Usare nomi significativi per classi, metodi e variabili.
- Organizzare l’applicazione in package Java per modulo, con alta coesione e basso accoppiamento e **senza cicli di dipendenza tra package**.
- Applicare incapsulamento e information hiding (*private*, *public* e visibilità di package).
- Usare interfacce e classi astratte quando opportuno; applicare ereditarità e polimorfismo con *@Override*.
- Usare le caratteristiche di Java (collection framework, stream, record, Optional) e i costrutti moderni del linguaggio.
- Evitare la duplicazione del codice; scrivere codice leggibile e manutenibile.

### 4.3 Struttura del repository e dei progetti

- Root del repository con il nome dell’applicazione, con le cartelle **documenti/** (documentazione e progetto StarUML) e **codice/** (progetti Eclipse). Il file *.project* è nei progetti, non nella root.
- Progetti Eclipse con una sigla del gruppo (ad esempio *BF_core*, *BF_gui*); nessun nome generico.
- Progetti Maven con i test in *src/test/java*, almeno una dipendenza esterna (log4j), nessun riferimento a percorsi assoluti.
- File *.gitignore* per i file generati (*.class*, cartella *target*), senza escludere *.project*.
- Database embedded e nessun servizio esterno da installare.

### 4.4 Standard di documentazione

La documentazione è organizzata in sei documenti: Project Plan; Project Management; Requisiti; Design; Testing; Maintenance (sezione 14).

### 4.5 Procedure di controllo versione

- Le **issue** assegnano e tracciano i compiti; le **milestone** corrispondono alle iterazioni.
- Il branch *main* è protetto: nessun commit diretto. Ogni funzionalità è sviluppata in un branch dedicato (*feature/nome-breve*).
- Ogni integrazione avviene con una **pull request** che richiede la **code review** di almeno un altro componente e il superamento dei test.
- I commit hanno messaggi chiari e sono collegati alle issue (ad esempio *Fixes #12*); ogni componente committa il proprio lavoro in modo da lasciare traccia dei contributi.
- Documentazione e codice sono aggiornati con commit progressivi, non caricati a fine progetto.

## 5. Attività di gestione

### 5.1 Pianificazione

All’inizio del progetto il gruppo definisce obiettivi, requisiti funzionali e non funzionali, responsabilità, fasi di sviluppo, carico di lavoro stimato, scadenze e risultati attesi. Prima di ogni iterazione si scelgono i casi d’uso da realizzare.

### 5.2 Monitoraggio dei progressi

Il gruppo controlla regolarmente le attività completate, quelle in corso, i compiti rimanenti, i problemi incontrati e il rispetto del calendario, usando GitHub Projects (bacheca Kanban), le milestone e un registro delle ore svolte da ciascun componente.

### 5.3 Coordinamento del gruppo

Ogni componente è responsabile del modulo assegnato. Le decisioni tecniche più importanti sono discusse insieme, per garantire coerenza tra le diverse parti dell’applicazione.

### 5.4 Gestione dell’integrazione

I tre moduli sono sviluppati separatamente e integrati al termine di ogni iterazione. Prima di integrare nuovo codice, il gruppo verifica che il progetto venga compilato correttamente e che le funzionalità già presenti continuino a funzionare. Le interfacce condivise tra i moduli sono definite in anticipo.

## 6. Rischi

| Rischio | Prob. | Impatto | Mitigazione |
|---|---|---|---|
| Perimetro troppo ampio | Media | Alto | Funzionalità classificate per priorità; in caso di ritardo si taglia It.4 (report e statistiche) |
| Conflitti di merge e problemi di integrazione tra i moduli | Alta | Medio | Integrazione a fine di ogni iterazione, branch brevi, interfacce condivise definite in anticipo |
| Squilibrio del carico e dei contributi | Media | Alto | Issue assegnate a persone, registro delle ore, controllo a ogni iterazione |
| Sovrapposizione con altri esami e disponibilità limitata | Alta | Medio | Pausa natalizia come buffer, calendario con margine, priorità alle funzioni essenziali |
| Concorrenza sulla stessa bicicletta (doppia prenotazione) | Media | Medio | Transazioni sul database e test dedicati |
| Incoerenze nei dati | Media | Alto | Convalida delle operazioni sul database e vincoli di integrità |
| Codice generato da StarUML poco utile | Media | Basso | Generare solo lo scheletro delle classi e completare a mano, indicando le classi generate |
| Documentazione e diagrammi lasciati alla fine | Media | Alto | Diagrammi assegnati a iterazioni precise; il 70% del tempo è pianificato su requisiti, modellazione e design |
| Errori software | Alta | Medio | Test regolari e code review |
| Perdita dei file di progetto | Bassa | Alto | Repository GitHub e commit regolari |

### 6.1 Gestione dei rischi

Il gruppo monitora i rischi durante tutto il progetto e li rivede alla fine di ogni iterazione. Se un rischio si verifica, i componenti ne valutano l’impatto e individuano una soluzione adeguata. Viene data priorità ai rischi che potrebbero compromettere le funzionalità principali o la consegna finale.

## 7. Personale

Il progetto coinvolge tre studenti. Ognuno è responsabile di un modulo di sviluppo (sezione 3.1) e di almeno un ruolo di gestione (sezione 3.2), assegnati come indicato nel documento di Project Management.

### 7.1 Componente 1 – Utenti e amministrazione

Registrazione degli utenti; accesso e autenticazione; gestione del profilo; gestione degli abbonamenti; funzionalità amministrative; amministrazione degli utenti.

### 7.2 Componente 2 – Biciclette e stazioni

Gestione delle informazioni sulle biciclette; gestione delle stazioni; disponibilità delle biciclette; gestione dello stato delle biciclette; gestione della manutenzione; segnalazione dei problemi.

### 7.3 Componente 3 – Prenotazioni e pagamenti

Prenotazione delle biciclette; avvio dei noleggi; conclusione dei noleggi; storico dei noleggi; calcolo dei costi; gestione dei pagamenti.

### 7.4 Attività condivise

Ingegneria dei requisiti; modellazione UML; architettura e progettazione software; integrazione del codice; test; documentazione; presentazione finale.

### 7.5 Carico di lavoro stimato

Il carico di lavoro stimato è di circa 40 ore per persona, per un totale di circa 120 ore per l’intero gruppo. La ripartizione per attività è nella sezione 12.3.

## 8. Metodi e tecniche

### 8.1 Tecnologie

L’applicazione sarà sviluppata in Java, con Eclipse come ambiente di sviluppo e Maven per la gestione delle dipendenze. Git e GitHub sono usati per il controllo di versione e la collaborazione. Le scelte tecniche principali sono:

- **Interfaccia:** applicazione desktop con Java Swing (inclusa nel JDK, senza dipendenze aggiuntive).
- **Database:** database embedded H2, con accesso tramite JDBC e uno strato di accesso ai dati (DAO).
- **Logging:** libreria esterna log4j, gestita con Maven.

### 8.2 Modellazione UML

Il progetto includerà i seguenti diagrammi UML, realizzati con StarUML (il file di progetto sarà caricato nel repository):

- Use case diagram.
- Class diagram, dal quale sarà generata una prima versione del codice Java; le classi generate e poi modificate saranno indicate nella relazione.
- State machine diagram.
- Sequence diagram.
- Communication diagram oppure timing diagram.
- Activity diagram.
- Component diagram e package diagram.

### 8.3 Architettura e progettazione software

L’applicazione sarà organizzata in moduli separati: gestione utenti, gestione biciclette e stazioni, gestione noleggi, gestione pagamenti e amministrazione. L’architettura seguirà uno **stile a livelli** (presentazione, logica di business, accesso ai dati) e sarà descritta con almeno due viste architetturali: una vista a componenti e connettori e una vista a package.

La progettazione seguirà i principi della programmazione a oggetti e applicherà almeno due design pattern studiati durante il corso. Sono previsti **State** (stato della bicicletta), **Strategy** (calcolo delle tariffe) e **Observer** (notifiche), con eventuale uso di Factory.

### 8.4 Gestione del database

Le principali entità sono Utenti, Biciclette, Stazioni, Prenotazioni, Noleggi, Pagamenti, Abbonamenti e registrazioni di Manutenzione. I vincoli di integrità e le transazioni garantiscono la coerenza dei dati, in particolare per la concorrenza sulla stessa bicicletta.

### 8.5 Tecniche di test

JUnit sarà utilizzato per realizzare test unitari automatici. I test verificano la correttezza delle principali operazioni, tra cui registrazione, prenotazioni, noleggi, restituzioni e calcolo dei costi, e sono descritti nel documento di Testing.

## 9. Assicurazione della qualità

L’assicurazione della qualità è parte integrante del processo di sviluppo. Il gruppo si concentra sulle seguenti caratteristiche:

- **Correttezza:** l’applicazione deve soddisfare i requisiti specificati.
- **Affidabilità:** il sistema deve funzionare correttamente e gestire gli errori.
- **Usabilità:** l’applicazione deve essere semplice e comprensibile.
- **Manutenibilità:** il codice deve essere organizzato, leggibile e facile da modificare.
- **Efficienza:** le operazioni principali devono essere eseguite senza ritardi inutili.
- **Sicurezza:** le informazioni degli utenti e le operazioni amministrative devono essere protette da adeguati controlli di accesso (password con hash, permessi per ruolo).

### 9.1 Attività di controllo qualità

Revisioni del codice tramite pull request; test unitari; test di integrazione; verifica dei requisiti; verifica dei diagrammi UML; controlli di coerenza del database.

### 9.2 Metriche e strumenti

| Obiettivo | Strumento o metrica | Soglia indicativa |
|---|---|---|
| Copertura dei test | JaCoCo (o EclEmma) | Almeno 70% sulla logica di business |
| Analisi statica | SonarLint, PMD | Nessun problema bloccante |
| Dipendenze tra package | JDepend | Nessun ciclo tra package |
| Complessità del codice | Complessità ciclomatica (McCabe) su una parte significativa | Valori contenuti sui metodi principali |

Una funzionalità è considerata completata quando funziona correttamente, i relativi test sono superati, la pull request è stata approvata e i diagrammi interessati sono aggiornati.

## 10. Pacchetti di lavoro

Il progetto è suddiviso in pacchetti di lavoro per organizzare le attività e definire i risultati attesi. Ogni pacchetto ha un responsabile (un modulo o un ruolo di gestione) mentre gli altri componenti contribuiscono dove indicato.

| Pacchetto | Attività | Responsabile | Iter. |
|---|---|---|---|
| WP1 – Analisi dei requisiti | Identificare attori e requisiti funzionali e non funzionali | Resp. requisiti e modellazione | Avvio, It.1–4 |
| WP2 – Pianificazione | Definire obiettivi, calendario, rischi e responsabilità | Project manager | Avvio |
| WP3 – Modellazione UML | Creare i diagrammi UML richiesti | Resp. requisiti e modellazione | Avvio, It.1–3 |
| WP4 – Gestione utenti | Registrazione, accesso e profili | Componente 1 | It.1 |
| WP5 – Biciclette e stazioni | Biciclette, stazioni, disponibilità, guasti e manutenzione | Componente 2 | It.1, It.3 |
| WP6 – Gestione noleggi | Prenotazioni, noleggi e restituzioni | Componente 3 | It.2 |
| WP7 – Gestione pagamenti | Calcolo dei costi e pagamenti simulati | Componente 3 | It.2 |
| WP8 – Abbonamenti e amministrazione | Abbonamenti, funzioni amministrative, report | Componente 1 | It.3, It.4 |
| WP9 – Database e integrazione | Accesso al database e integrazione dei moduli | Configuration manager | It.1–4 |
| WP10 – Test | Implementare ed eseguire test JUnit, misurare la copertura | Resp. qualità e test | It.1–4 |
| WP11 – Documentazione | Preparare la documentazione tecnica (6 documenti) | Project manager | It.1–4 |
| WP12 – Consegna finale | Verificare l’applicazione e preparare la presentazione | Project manager | Chiusura |

L’avanzamento è monitorato tramite le issue GitHub, le milestone e la bacheca del progetto.

## 11. Risorse

### 11.1 Risorse software

| Risorsa | Scopo |
|---|---|
| Java | Sviluppo dell’applicazione |
| Eclipse | Ambiente di sviluppo integrato |
| Maven | Gestione delle dipendenze |
| Git e GitHub | Controllo di versione e collaborazione |
| StarUML 5 (gratuito) | Diagrammi UML e generazione dello scheletro del codice |
| JUnit | Test unitari |
| H2 (database embedded) | Memorizzazione dei dati |
| Log4j | Registrazione degli eventi dell’applicazione |
| JaCoCo, SonarLint, PMD, JDepend | Copertura dei test, analisi statica e analisi delle dipendenze |

### 11.2 Risorse hardware

Ogni componente del gruppo utilizza un computer personale adatto allo sviluppo Java. È necessaria una connessione Internet per accedere a GitHub e condividere i file del progetto.

### 11.3 Risorse umane

Il progetto è realizzato da tre studenti. Ogni componente contribuisce alle attività di sviluppo, modellazione, test e documentazione.

## 12. Modifiche

Durante lo sviluppo potrebbe essere necessario modificare il piano di progetto o i requisiti iniziali. Le modifiche potranno riguardare requisiti funzionali, progettazione software, struttura del database, interfaccia utente, implementazione o calendario. Eventuali aggiornamenti successivi del piano saranno registrati nella tabella delle versioni in copertina.

### 12.1 Procedura di gestione delle modifiche

- Un componente individua la necessità di una modifica.
- La modifica viene descritta in una GitHub Issue.
- Il gruppo ne valuta importanza e impatto.
- Il gruppo decide se accettarla, rifiutarla o rimandarla.
- Se accettata, il componente responsabile la implementa in un branch separato.
- La modifica viene controllata tramite Pull Request e Code Review.
- Dopo l’approvazione, la modifica viene integrata nel branch principale.
- La documentazione e i test correlati vengono aggiornati.

Tutte le modifiche significative sono tracciate tramite GitHub, così da mantenere uno storico del progetto.

## 13. Consegna

### 13.1 Risultati finali da consegnare

| Documento | Contenuto |
|---|---|
| 1 – Project Plan | Organizzazione del progetto, modello di processo, rischi, risorse, calendario e pacchetti di lavoro |
| 2 – Project Management | Ciclo di vita del software, gestione della configurazione e organizzazione del gruppo |
| 3 – Requisiti | Requisiti funzionali e non funzionali, casi d’uso e caratteristiche di qualità del software |
| 4 – Design | Diagrammi UML, architettura software, progettazione e design pattern |
| 5 – Testing | Casi di test, implementazione JUnit, copertura e risultati dei test |
| 6 – Maintenance | Attività di refactoring e documentazione della manutenzione |

Il progetto StarUML contenente i diagrammi sarà caricato nel repository insieme alla documentazione.

### 13.2 Consegna del software

L’applicazione completa sarà caricata nel repository GitHub, condiviso con gli account **garganti** e **silviabonfanti**. Il repository conterrà codice sorgente Java, file di configurazione Maven, file dei progetti Eclipse, test JUnit, diagrammi UML, documentazione e istruzioni per eseguire l’applicazione. 

### 13.3 Presentazione finale

Il progetto sarà presentato durante l’esame orale. Ogni componente presenterà il proprio contributo e spiegherà le attività svolte. Sarà inoltre preparata una dimostrazione dell’applicazione.

### 13.4 Criteri di completamento

- I requisiti principali sono stati implementati.
- L’applicazione funziona correttamente.
- Tutti i diagrammi UML richiesti sono disponibili.
- I test JUnit sono stati implementati.
- La documentazione è completa.
- Il repository GitHub contiene il progetto completo.
- Tutti e tre i componenti sono in grado di spiegare il proprio contributo.

## Conclusione

BikeFlow si propone di offrire una soluzione software completa per la gestione di un servizio di bike sharing. Il progetto permetterà ai tre componenti del gruppo di applicare i principali concetti dell’ingegneria del software, tra cui analisi dei requisiti, pianificazione, modellazione UML, architettura software, programmazione a oggetti, test e manutenzione.

La suddivisione delle responsabilità, insieme al processo di sviluppo iterativo e incrementale, aiuterà il gruppo a organizzare il lavoro in modo efficiente e a realizzare un’applicazione funzionante e ben documentata.
