---
tags: [economia-informazione, selezione-avversa, inefficienza, rimedi, gresham, segnalazione]
aliases: [Implicazioni Selezione Avversa, Rimedi Selezione Avversa, Legge Gresham Economia]
links: [02_Mercato_dei_Limoni_Intuizione, 05_Equilibrio_di_Mercato_Adverse_Selection, 06_Variazioni_del_Modello]
---

# Inefficienza e Implicazioni della Selezione Avversa

## L'Inefficienza come Fallimento del Mercato

> [!definition]
> Il risultato della selezione avversa costituisce un **fallimento del mercato** (*market failure*) e produce un esito **Pareto-inefficiente**: esistono allocazioni alternative (ad es. lo scambio delle auto di alta qualità) che sarebbero preferite da entrambe le parti — compratore e venditore — ma che non si realizzano a causa dell'asimmetria informativa. Il mercato non riesce a "trovare" queste allocazioni perché il prezzo non può trasmettere in modo credibile l'informazione sulla qualità.

L'inefficienza non è banale: non basta che il mercato "funzioni male" per chiamarlo inefficiente in senso paretiano. Ci vuole una perdita di surplus reale. Nel modello di Akerlof, l'inefficienza è evidente:

- Con informazione perfetta: *tutte* le auto vengono scambiate a prezzi che soddisfano entrambe le parti → surplus totale = $\frac{1}{2} \cdot \frac{3}{2} \cdot \int_0^2 q \, f(q) \, dq$ (massimizzato)
- Con informazione asimmetrica: *nessuna* auto viene scambiata → surplus totale = 0

La perdita è totale nel modello base, parziale nelle variazioni ([[06_Variazioni_del_Modello]]).

---

## Asimmetria vs. Incompletezza: La Distinzione Cruciale

> [!intuition]
> L'inefficienza dipende dall'**asimmetria** dell'informazione, non dalla sua incompletezza. Questa distinzione è fondamentale:
>
> - **Informazione incompleta (simmetrica)**: nessuno conosce la qualità esatta, ma tutti hanno la stessa ignoranza → il mercato funziona normalmente, i prezzi riflettono le aspettative comuni
> - **Informazione asimmetrica**: il venditore sa qualcosa che il compratore non sa → i prezzi non possono più svolgere il ruolo di segnale credibile → selezione avversa

Come dimostrato in [[05_Equilibrio_di_Mercato_Adverse_Selection]], se anche i venditori ignorassero la propria qualità, il mercato funzionerebbe: tutti scambierebbero alla qualità media, senza alcuna selezione avversa. Il problema nasce quando *qualcuno* sa e *qualcun altro* no.

> [M] L'inefficienza dipende dall'asimmetria dell'informazione, non dalla sua incompletezza. Il mercato dei beni usati è caratterizzato da un prezzo che riflette la qualità media degli stessi, che è più bassa di quella dei beni nuovi. Supponiamo ora che anche i venditori non possano osservare la qualità delle proprie auto: nessuna selezione avversa!

---

## La Legge di Gresham

> [!intuition]
> La **Legge di Gresham** è un principio della storia monetaria: *"la moneta cattiva scaccia quella buona"* (*bad money drives out good money*). In un sistema bimetallico (oro e argento) o in presenza di monete di diverso peso ma stesso valore nominale, le monete "cattive" (meno pregiate) tendono a circolare mentre quelle "buone" vengono tesaurizzate o esportate. Gresham lo osservò nell'Inghilterra del XVI secolo.
>
> L'analogia con la selezione avversa è perfetta: in un mercato con asimmetria informativa, i "beni cattivi" (auto di bassa qualità) scacciano i "beni buoni" (auto di alta qualità) dal mercato. Il meccanismo è speculare: chi ha un bene buono non lo vende perché non riesce a spuntare un prezzo adeguato; chi ha un bene cattivo ha ogni interesse a venderlo a un prezzo "medio".

---

## La Legge di Groucho Marx

> [!example]
> Groucho Marx diceva: *"Non mi iscriverei mai a un club che accettasse me come membro."*
>
> Il parallelo economico è illuminante: un compratore razionale non vuole acquistare un bene che un venditore razionale e informato è disposto a cedere. Se il venditore vuole vendere, significa che il bene vale *meno* del prezzo di mercato per lui — altrimenti lo terrebbe. Questo ragionamento porta il compratore a offrire sempre di meno, il che esclude sempre di più i beni di qualità... e così via.
>
> Più formalmente: qualsiasi prezzo che induci il venditore a vendere è un segnale che il bene vale *meno* di quel prezzo. Offrire di più per avere beni migliori non funziona, perché attira *anche* beni peggiori (quelli che prima il venditore teneva).

---

## Il Doppio Ruolo del Prezzo

Una delle osservazioni più profonde del modello di Akerlof è che il prezzo svolge un **doppio ruolo** che normalmente è separato:

1. **Ruolo allocativo**: equilibra domanda e offerta (il ruolo "classico")
2. **Ruolo di selezione della qualità**: determina la composizione qualitativa dei beni offerti

Questi due ruoli entrano in conflitto in presenza di asimmetria informativa. Quando il prezzo scende (come farebbe in un mercato con eccesso d'offerta), la teoria standard prevede un aumento della domanda. Ma qui, una riduzione di prezzo cambia anche la qualità media offerta (peggiora), riducendo la disponibilità a pagare dei compratori. Il prezzo non può svolgere simultaneamente entrambe le funzioni.

> [M] I prezzi svolgono un duplice ruolo: determinano la qualità media dei beni venduti *ed* equilibrano la quantità domandata e offerta.

---

## Il Problema dell'Arbitraggio

> [!example]
> Perché i prezzi delle auto usate sono inferiori a quelli delle auto nuove? La risposta ovvia è il deprezzamento fisico. Ma c'è una ragione aggiuntiva: la selezione avversa.
>
> Un'auto nuova viene valutata alla qualità media di quel modello. Appena viene portata via dal concessionario, diventa "usata" e la sua qualità è privata: solo il proprietario sa se è difettosa o no. Il prezzo crolla non solo per il deprezzamento fisico, ma perché il mercato sa che se è già in vendita dopo pochissimo tempo, probabilmente c'è qualcosa che non va.
>
> **Opportunità di arbitraggio**: se i prezzi del nuovo e dell'usato fossero uguali, si potrebbe comprare un'auto nuova, scoprire che è difettosa, e rivenderla al prezzo del nuovo — trasferendo il difetto al prossimo compratore. La selezione avversa giustifica lo sconto sul mercato dell'usato come meccanismo di protezione del compratore.

---

## Implicazioni più Generali

La selezione avversa si manifesta in molti contesti:

**Mercati assicurativi**: chi si assicura conosce il proprio rischio meglio della compagnia. Chi ha un rischio elevato tende ad assicurarsi di più, alzando il costo medio per la compagnia, che alza i premi, il che scoraggia chi ha basso rischio... finché rimangono solo gli ad alto rischio.

> [BB, pp. 284-286] Due risposte possibili alla selezione avversa nei mercati assicurativi: (1) rendere l'assicurazione obbligatoria; (2) vietare l'uso di certe informazioni. L'assicurazione obbligatoria permette di assicurare al prezzo medio della popolazione intera senza perdite.

**Mercato del lavoro**: i lavoratori conoscono le proprie abilità meglio dei datori di lavoro. I lavoratori di bassa qualità possono spacciarsi per lavoratori di alta qualità, aumentando il rischio di selezione avversa nelle assunzioni.

**Mercato del credito**: i mutuatari conoscono la rischiosità del proprio progetto. Le banche non possono distinguere i mutuatari a basso e alto rischio, il che porta a tassi d'interesse che scoraggiano i progetti sicuri e premiano quelli rischiosi.

**Politica e pubblica amministrazione**: citato nelle slide come ambito dove la selezione avversa colpisce (politici, manager pubblici, insegnanti, infermieri).

---

## Perché la "Cheap Talk" Non Risolve il Problema

> [!intuition]
> La soluzione ovvia sembrerebbe essere: il venditore dichiara la qualità effettiva della sua auto. Ma perché mai un compratore dovrebbe credergli?
>
> Se le dichiarazioni di qualità non sono verificabili (non costano nulla, non sono vincolanti), allora il venditore di un'auto di bassa qualità ha ogni incentivo a dichiarare di avere un'auto di alta qualità. Le dichiarazioni non costano nulla — sono "cheap talk" — e quindi non trasmettono informazione credibile.
>
> Perché una dichiarazione di qualità sia credibile, deve essere **costosa da imitare** per chi ha bassa qualità: questo è il principio della segnalazione (*signalling*), che richiede che i segnali siano *costosi* e *differenzialmente* costosi per diversi tipi.

---

## I Rimedi alla Selezione Avversa

Le principali soluzioni proposte dalla letteratura sono:

**Regolazione**: obbligare alla divulgazione di informazioni (es. certificati di revisione per le auto, dichiarazioni sui rischi assicurativi). Riduce l'asimmetria direttamente.

**Reputazione**: in mercati con interazioni ripetute, il venditore di bassa qualità perde clienti nel tempo. Il futuro diventa un "collaterale" che incentiva la qualità. Ma la reputazione funziona solo se il valore futuro è abbastanza alto.

**Segnalazione** (*signalling*): il venditore di alta qualità invia segnali costosi che il venditore di bassa qualità non può permettersi di imitare (es. garanzie, diplomi, marchi). Questo è il tema della Lezione 8+.

**Screening**: il compratore progetta un "menu" di contratti tale da far autoselezionare i tipi (es. polizze assicurative con diversi premi e franchigie). Anche questo richiede che i tipi abbiano preferenze diverse.

> [M] Questo problema può essere mitigato in modi diversi: regolazione, reputazione, segnalazione.

---

## Take-home message

> [!summary]
> La selezione avversa produce un fallimento del mercato Pareto-inefficiente: scambi potenzialmente vantaggiosi non si realizzano perché il prezzo non può trasmettere in modo credibile l'informazione sulla qualità. La causa è l'*asimmetria* informativa, non l'incompletezza: se tutti fossero egualmente ignoranti, il mercato funzionerebbe. La Legge di Gresham e la paradossale "Legge di Groucho Marx" catturano l'intuizione: i beni cattivi scacciano i buoni, e i compratori razionali non vogliono comprare ciò che il venditore razionale vuole vendere. I rimedi — regolazione, reputazione, segnalazione, screening — cercano tutti di ridurre o eliminare l'asimmetria, rendendo credibili le dichiarazioni sulla qualità.

---

## Vedi anche

- [[01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste]] — La natura dell'asimmetria
- [[02_Mercato_dei_Limoni_Intuizione]] — L'intuizione di Akerlof
- [[05_Equilibrio_di_Mercato_Adverse_Selection]] — La dimostrazione che l'asimmetria è la causa
- [[06_Variazioni_del_Modello]] — Quando l'inefficienza è parziale, non totale

---

## Connessioni con il Vault

> [!note] Nota strategica
> Questa è la nota-cerniera tra il modello formale e le soluzioni. I rimedi qui elencati corrispondono alle note successive del corso (segnalazione, screening) e si collegano direttamente ai concetti di equilibrio della Teoria dei Giochi.

**Da `0. Intro`:**
- [[0. Intro/06_Segnalazione|Segnalazione]] — il rimedio della segnalazione qui introdotto è sviluppato in dettaglio: il titolo di studio come segnale costoso e credibile di produttività
- [[0. Intro/07_Screening|Screening]] — il rimedio dello screening: il menù di contratti con cui il Principale non-informato induce l'auto-selezione dei tipi
- [[0. Intro/08_Azzardo_morale|Azzardo morale]] — mentre la selezione avversa è asimmetria *ex-ante*, l'azzardo morale è asimmetria *ex-post*; la distinzione è cruciale per identificare il rimedio giusto
- [[0. Intro/09_Nobel|Premi Nobel]] — Akerlof (Nobel 2001) per la selezione avversa; Spence (Nobel 2001) per la segnalazione come rimedio

**Da `1. GT`:**
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — la *reputazione* come rimedio funziona esattamente come la cooperazione in un gioco ripetuto indefinitamente: il venditore di alta qualità ha incentivo a mantenerla se e solo se $\delta \cdot V_{futuro} > \text{guadagno dalla defezione oggi}$
- [[1. GT/10_Folk_Theorem|Folk Theorem]] — il Folk Theorem garantisce che la cooperazione (qualità alta) possa essere un equilibrio in giochi ripetuti indefinitamente, purché $\delta$ sia abbastanza alto; questo è il fondamento teorico della reputazione come soluzione alla selezione avversa
