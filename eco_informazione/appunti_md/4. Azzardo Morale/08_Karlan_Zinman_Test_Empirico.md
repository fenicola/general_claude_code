---
tags: [economia-informazione, azzardo-morale, test-empirico, selezione-avversa, credito, quasi-esperimento, karlan-zinman]
aliases: [Karlan Zinman 2009, Observing the Unobservables, Test Empirico AM SA]
links: [01_Definizione_e_Timing, 06_Framework_PA_Corporate_Governance]
---

# Karlan & Zinman (2009): Identificare l'Inidentificabile

## Il Problema di Identificazione

> [!definition]
> Il **problema di identificazione** delle asimmetrie informative nel mercato del credito è il seguente: osserviamo che chi paga tassi d'interesse più alti tende ad avere default più elevati. Ma questo può essere dovuto a **due meccanismi completamente diversi**:
> - **Selezione avversa** (*hidden information*): chi ha alta probabilità di default ex-ante è più disposto ad accettare tassi alti, poiché conta di non ripagare comunque. Il meccanismo è ex-ante, sulla selezione.
> - **Azzardo morale** (*hidden action*): un tasso alto riduce ex-post l'incentivo a fare effort per ripagare il debito — o direttamente (costa troppo ripagare con interessi alti) o indirettamente (riduce il valore del rapporto futuro con il creditore).

> [Karlan & Zinman, 2009, p. 1993] Le teorie mostrano che le frizioni informative e i conseguenti fallimenti del mercato del credito possono creare inefficienze sia a livello micro sia macro, attraverso sottoinvestimento o sovrainvestimento, e trappole della povertà.

La distinzione non è accademica: il rimedio ottimale dipende da quale meccanismo domina. La selezione avversa richiede screening ex-ante (raccolta di informazioni, collateral, menus di contratti); l'azzardo morale richiede incentivi ex-post (contratti contingenti, incentivi dinamici alla reputazione).

Il problema è che entrambi i meccanismi producono la stessa **correlazione osservabile** tra tasso d'interesse e default — dunque i dati osservazionali non permettono di distinguerli.

---

## Il Disegno Sperimentale: Come Separare i Meccanismi

**Contesto** (slide 15): 57.533 ex-clienti di un istituto di microcredito nel Sud Africa con buona storia di rimborso. Prestiti di piccola entità (circa $150), senza collateral, con piano di rimborso mensile fisso. Il 75% dei clienti aveva un tasso del 11,75% mensile.

### La Tripla Randomizzazione

Gli autori inviano ai clienti offerte di prestito con **tre tassi randomizzati indipendentemente**:

| Variabile | Descrizione | Funzione |
|---|---|---|
| $r^o$ (offer rate) | Tasso pubblicizzato nell'offerta diretta | Determina chi risponde (selezione) |
| $r^c$ (contract rate) | Tasso effettivo del contratto, rivelato solo dopo l'accettazione | Determina il costo ex-post del prestito |
| $r^f$ (future rate) | Tasso sui prestiti futuri, condizionato alla buona storia di rimborso | Determina l'incentivo dinamico alla reputazione |

Questa struttura è **ingeniosamente intrecciata**: $r^o$ e $r^c$ possono essere uguali o diversi; $r^f$ può essere uguale o inferiore a $r^c$. La randomizzazione **spezza** le correlazioni che normalmente rendono impossibile la separazione.

### Mappatura Meccanismi → Variazioni Sperimentali

Il punto chiave è che ogni coppia di celle nella matrice sperimentale isola un meccanismo diverso (slide 21-23):

```
                    │  High r^c  │     Low r^c        │
                    │            │  Dynamic  No dyn.  │
────────────────────┼────────────┼───────────────────┤
High offer rate r^o │  r^c = r^o │ r^c<r^o  r^c<r^o  │
                    │            │ r^f=r^c            │
────────────────────┼────────────┼───────────────────┤
Low offer rate r^o  │            │ r^c=r^o  r^c=r^o  │
                    │            │ r^f=r^c            │
```

**Hidden Information (Selezione Avversa)** → asse verticale: confronto tra chi riceve *High Offer Rate* e chi riceve *Low Offer Rate*, tenendo fisso $r^c$. Chi accetta con un tasso offerto alto è sistematicamente più rischioso ex-ante? Se sì, troveremo che i tassi d'offerta alti attraggono clienti con maggiore propensione al default — indipendentemente dal tasso contrattuale.

**Hidden Action 1 (Azzardo Morale da tasso corrente)** → asse orizzontale: confronto tra *High r^c* e *Low r^c* a parità di *High Offer Rate*. Stessi clienti (stessa distribuzione di tipi) ma diverso tasso contrattuale. Qualsiasi differenza nel default riflette un effetto comportamentale del tasso corrente sul livello di sforzo del debitore.

**Hidden Action 2 (Azzardo Morale da incentivi futuri)** → confronto tra Dynamic Incentive e No Dynamic Incentive a parità di Low Contract Rate e High Offer Rate. La sola differenza è la promessa di un tasso migliore nel futuro in caso di buona performance. Se questo cambia il comportamento, si misura direttamente il valore degli **incentivi dinamici reputazionali**.

> [!intuition]
> Il design è un **esperimento naturale** elegante: non osserva lo sforzo del debitore (per definizione non osservabile), ma usa le variazioni esogene casuali nelle tre dimensioni del contratto per **inferire** quale meccanismo è responsabile delle differenze di default. È un'applicazione diretta della logica dell'identificazione causale via variabile strumentale.

---

## Il Modello Teorico Sottostante (Slide 26)

Il processo si articola in tre stadi:

1. Il cliente decide se chiedere il prestito al tasso offerto $r^o$
2. Il creditore abbassa casualmente il tasso per alcuni clienti a $r^c < r^o$, con ulteriore randomizzazione che abbassa $r^f = r^c < r^o$. Dato $r^c$ e $r^f$, il debitore sceglie l'effort $e \in [e_{\min}, e_{\max}]$ per generare flussi di cassa
3. I flussi di cassa si realizzano e il debitore decide se ripagare

**Previsione chiave**: l'effort è **decrescente sia in $r^c$ sia in $r^f$**. Perché?

- Un tasso contrattuale alto $r^c$ rende il debito più oneroso → riduce il net return dal rimborso → meno incentivo a fare sforzo per ripagare (*effetto HA1*)
- Un tasso futuro alto $r^f$ riduce il valore del rapporto futuro con il creditore → meno incentivo reputazionale al rimborso *oggi* (*effetto HA2*)

---

## L'Equazione di Stima

$$y_{it} = \alpha + \beta_1 X_{it} + \beta_2 r^o_{it} + \beta_3 r^c_{it} + \beta_4 r^f_{it} + \varepsilon_{it}$$

Dove:
- $y_{it}$ è una misura di default del cliente $i$ al tempo $t$ (tre misure: proporzione mensile arretrata, proporzione di mesi in arretrato, status "in collezione")
- $X_{it}$ è un vettore di condizioni di randomizzazione (controlli)
- $\beta_2$ (coefficiente su $r^o$) cattura l'**effetto di informazione nascosta** (selezione avversa)
- $\beta_3$ (coefficiente su $r^c$) cattura l'**effetto HA1** (azzardo morale via tasso corrente)
- $\beta_4$ (coefficiente su $r^f$) cattura l'**effetto HA2** (azzardo morale via incentivi futuri)

---

## Risultati (Table I, slide 29-31)

| Effetto | Meccanismo | Risultato | Significatività |
|---|---|---|---|
| Contract rate ($r^c$) | **HA1** | Positivo e significativo su "Proportion months in arrears" (col. 3) | * |
| Dynamic incentive dummy ($r^f$) | **HA2** | Negativo e significativo su 3 delle 4 misure principali | ** |
| Offer rate ($r^o$) | **Hidden Information** | Positivo ma non significativo | — |

**Interpretazione**:

- L'**azzardo morale domina**: sia HA1 sia (soprattutto) HA2 sono empiricamente rilevanti e statisticamente significativi. HA2 — l'effetto degli incentivi dinamici futuri — è il driver principale: chi ha la promessa di un tasso migliore in futuro fa più sforzo per ripagare oggi.

- L'**evidenza per la selezione avversa è debole**: il coefficiente su $r^o$ è positivo (nella direzione attesa) ma non significativo nelle principali specificazioni. Gli effetti di selezione ex-ante sembrano modesti rispetto agli effetti comportamentali ex-post.

> [!example]
> Un coefficiente di $-0.025$ su HA2 per la misura "Account in collection" (col. 5) significa che ricevere l'incentivo dinamico (promessa di tasso futuro basso) riduce la probabilità di entrare in status di default grave di circa 2.5 punti percentuali — su una media del 12%, è una riduzione economicamente rilevante del 20%.

---

## Conclusioni e Implicazioni (Slide 32)

> [!summary]
> **Risultati principali di Karlan & Zinman (2009)**:
> 1. **Azzardo morale significativo**: documentato empiricamente e causalmente identificato nel mercato del credito. L'effetto è principalmente guidato dagli incentivi dinamici reputazionali ($r^f$), non dal tasso corrente ($r^c$).
> 2. **Selezione avversa debole**: l'evidenza per la selezione ex-ante su informazione nascosta è presente ma non statisticamente robusta.
> 3. **Magnitude**: l'azzardo morale spiega approssimativamente dal 13% al 21% dei default nel campione.
> 4. **Implicazione di policy**: dato che l'azzardo morale domina, i meccanismi di incentivo dinamico (reputazione, tassi futuri condizionati alla performance) sono strumenti di policy più efficaci dello screening ex-ante.

> [!intuition]
> Questo studio è un esempio perfetto di come il design sperimentale riesca a identificare causalmente meccanismi che i dati osservazionali non permettono di separare. La logica è analoga al test empirico su selezione avversa vs. azzardo morale in assicurazioni (Chiappori & Salanié, 2000): serve una variazione esogena che spezzi la correlazione naturale tra tipo e comportamento.

---

## Connessione con il Modello Teorico del Blocco 1

| Elemento teorico (Blocco 1) | Equivalente empirico (KZ 2009) |
|---|---|
| Sforzo $e \in \{e_1, e_2\}$ | Effort $e \in [e_{\min}, e_{\max}]$ nella generazione di flussi di cassa |
| Azione nascosta | Effort del debitore non osservabile dal creditore |
| Contratto contingente | Tasso condizionato alla performance: $r^f < r^c$ se rimborso puntuale |
| Incentivo dinamico (giochi ripetuti) | Promessa di $r^f$ favorevole → HA2 |
| Premio di rischio $\Delta$ | Il tasso aggiuntivo sul credito compensa il rischio di default (azzardo morale) |

---

## Vedi Anche

- [[01_Definizione_e_Timing]] — La distinzione teorica hidden information / hidden action
- [[04_Secondo_Migliore_Sforzo_Non_Osservabile]] — Il contratto contingente (IC) che emerge empiricamente come incentivo dinamico
- [[3. Segnalazione/08_Test_Empirico_GED|Test Empirico GED]] — Confronto metodologico: quasi-esperimento per identificare effetti causali
- [[2. Selezione Avversa/10_Malpractice_Medica_Selezione_Avversa|Malpractice Medica]] — Altro esempio di identificazione empirica di asimmetria informativa
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — La reputazione (equivalente di $r^f$) come meccanismo di incentivo
