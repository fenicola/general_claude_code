---
tags: [economia-informazione, selezione-avversa, assicurazione, hirshleifer, test-genetici, pooling, separating]
aliases: [Effetto Distruzione Assicurazione, Hirshleifer Effect, Assicurazione Vita e Selezione Avversa, Test Genetici]
links: [07_Inefficienza_e_Implicazioni, 09_Modello_Wilson_Equilibri_Multipli, 12_Confronto_Utilita_Equilibri_Assicurativi]
---

# Assicurazione Vita e l'Effetto di Distruzione dell'Assicurazione

## Il Mercato Assicurativo come Arena della Selezione Avversa

Il mercato assicurativo è il banco di prova classico della selezione avversa. Chi acquista assicurazione conosce il proprio rischio meglio di chi la offre. Nei mercati della salute e della vita, questo vantaggio informativo degli assicurati può essere amplificato dalla disponibilità di test genetici, creando un paradosso: **più informazione può distruggere la capacità di assicurarsi**.

> [!definition]
> L'**effetto di distruzione dell'assicurazione** (*insurance destruction effect*, noto anche come **Effetto Hirshleifer**) si verifica quando la disponibilità di informazioni sui rischi individuali — siano esse di dominio pubblico o privato — impedisce la realizzazione di accordi assicurativi che sarebbero stati possibili in assenza di quella stessa informazione. In altri termini: *più informazione può rendere impossibile l'assicurazione* contro certi rischi, distruggendo guadagni dallo scambio.

Il fenomeno è descritto formalmente da Hirshleifer e Riley (1992) e richiamato in Birchler & Bütler al Capitolo 13D. Il paradosso è catturato dall'aneddoto della pizza nelle slide: Eugene, scoprendo di avere la Regina di Picche, si appropria di tutte le fette. Senza l'informazione, il gruppo avrebbe condiviso equamente. L'informazione ha distrutto la possibilità di condivisione del rischio.

> [BB, p. 286] L'effetto di distruzione dell'assicurazione: in un gruppo non informato, gli accordi di condivisione del rischio sono possibili; una volta rilasciata informazione sugli esiti, tali accordi non sono più realizzabili.

---

## Il Modello Formale: Struttura di Base

### La Popolazione

Consideriamo una popolazione divisa in due tipi genetici:

| Dimensione | Gruppo di rischio | Pr(sano) | Pr(malato) |
|:---:|:---:|:---:|:---:|
| $1-g$ | Basso rischio | $\pi > \frac{1}{2}$ | $1-\pi$ |
| $g$ | Alto rischio | $1-\pi$ | $\pi$ |

La frazione $g$ della popolazione porta un gene che aumenta la probabilità di contrarre una certa malattia a $\pi > 1/2$. I restanti $1-g$ hanno una probabilità di ammalarsi pari a $1-\pi < 1/2$.

### La Sequenza Temporale

$$t=0 \xrightarrow{\text{individui apprendono il proprio tipo}} t=1 \xrightarrow{\text{possono acquistare assicurazione}} t=2 \xrightarrow{\text{esito: malati o sani}}$$

### Preferenze e Assicurazione

- Il danno da malattia vale $D$ (costo delle cure, perdita di reddito, ecc.).
- Il reddito base è $Y$.
- Il premio assicurativo è pari al costo sanitario atteso dell'individuo.
- Chi non si assicura subisce un costo psicologico aggiuntivo di avversione al rischio: una frazione $v$ del costo atteso di malattia ($v \cdot \pi_i \cdot D$, dove $\pi_i$ è la probabilità individuale di ammalarsi).

---

## Scenario 1 — Nessuna Informazione (No-Info)

In questo scenario, i test genetici non sono disponibili: nessun individuo conosce il proprio tipo. L'assicuratore non può distinguere i tipi e fronteggia una popolazione con rischio medio:

$$\bar{\pi} = [g\pi + (1-g)(1-\pi)]$$

L'assicuratore offre un **premio unico** $z = \bar{\pi} D$. Un individuo acquista assicurazione se:

$$z < (1+v)\bar{\pi}D$$

Poiché $z = \bar{\pi}D$, la condizione è $\bar{\pi}D < (1+v)\bar{\pi}D$, cioè $1 < 1+v$, vera per $v>0$. **Tutti si assicurano.** L'utilità attesa è:

$$U = Y - \bar{\pi}D$$

Il risparmio $v\bar{\pi}D$ rispetto alla situazione non assicurata rappresenta il **guadagno dallo scambio**: i premi pagati coprono esattamente i costi attesi, e tutti evitano la perdita di utilità da rischio.

---

## Scenario 2 — Informazione Pubblica

Ora i risultati dei test genetici sono pubblici. L'assicuratore può distinguere i tipi e offre premi differenziati:

$$z_L = (1-\pi)D \quad \text{(per i basso-rischio)}$$
$$z_H = \pi D \quad \text{(per gli alto-rischio)}$$

Entrambi i tipi acquistano assicurazione (i guadagni attesi superano i premi), ma con utilità diverse:

$$\hat{U}_L = Y - (1-\pi)D$$
$$\hat{U}_H = Y - \pi D$$

Poiché $\pi > 1/2$, abbiamo $\hat{U}_L > \hat{U}_H$: **i basso-rischio stanno meglio dei alto-rischio**. Il grado di "discriminazione" assicurativa dipende da $\pi$: quanto più $\pi$ si avvicina a 1, tanto più alto-rischio si avvicina a pagare il costo intero della malattia senza vera assicurazione.

**L'assicurazione ora copre solo il rischio di ammalarsi, dato il tipo genetico — non il rischio di essere nato portatore del gene.** Questa è l'essenza dell'effetto di distruzione: l'informazione ha eliminato la possibilità di assicurarsi contro il rischio genetico.

> [!intuition]
> Senza informazione, tutti condividono il rischio genetico: i basso-rischio "sussidiano" gli alto-rischio attraverso un premio comune. Con informazione pubblica, questo trasferimento di rischio scompare. Gli alto-rischio (che sono anche i più poveri di salute) pagano premi più alti, proprio quando ne hanno più bisogno. L'informazione ha distrutto la mutualizzazione del rischio genetico.

[BB, p. 288]

---

## Scenario 3 — Informazione Asimmetrica

Questo è il caso più realistico: gli individui conoscono il proprio tipo genetico (hanno fatto il test), ma l'assicuratore non può osservarlo. L'assicuratore sa però che gli individui *sanno*. La selezione avversa è quindi possibile.

L'assicuratore ha due strategie disponibili:

### Equilibrio di Pooling

L'assicuratore offre un premio unico $z^{LH}$ accettabile da entrambi i tipi. Per esistere, il premio deve soddisfare contemporaneamente:

- Deve essere almeno sufficiente a coprire i costi medi: $z^{LH} \geq [g\pi + (1-g)(1-\pi)]D = \bar{\pi}D$
- Deve essere abbastanza basso da attirare anche i basso-rischio: $z^{LH} \leq (1+v)(1-\pi)D$

Combinando le due condizioni, l'**equilibrio di pooling esiste** se e solo se:

$$\frac{v}{g} \geq \frac{2\pi - 1}{1-\pi} \tag{13.1}$$

Interpretazione di $(13.1)$: l'equilibrio di pooling è più probabile quando:
- $v$ è alto (forte avversione al rischio: entrambi i tipi sono disposti a pagare un premio elevato pur di essere coperti),
- $g$ è basso (pochi portatori del gene: la contaminazione del pool è limitata),
- $\pi$ è vicino a $1/2$ (le differenze di rischio sono piccole).

Se esiste un equilibrio di pooling competitivo, il premio è:

$$z^{LH} = [g\pi + (1-g)(1-\pi)]D = \bar{\pi}D$$

e l'utilità di entrambi i tipi è $U_L^{LH} = U_H^{LH} = Y - \bar{\pi}D$: **identica a quella del caso no-info**. Sebbene gli individui conoscano il proprio tipo, non possono usare questa informazione. Gli alto-rischio si "nascondono" nella popolazione, trasferendo parte del loro costo assicurativo ai basso-rischio — lo stesso meccanismo della selezione avversa del mercato delle auto.

### Equilibrio di Separazione (Separating Equilibrium)

Se la condizione $(13.1)$ non è soddisfatta, il pooling non è possibile. L'assicuratore può assicurare solo gli **alto-rischio** (che sono disposti ad accettare qualsiasi premio inferiore a $\pi D$).

Il premio competitivo per i soli alto-rischio è $z_H^H = \pi D$ (come nel caso di informazione pubblica). I basso-rischio rimangono senza assicurazione e incorrono in una perdita secca:

$$\tilde{U}_L = Y - (1-v)(1-\pi)D$$
$$\tilde{U}_H = Y - \pi D$$

Il risultato è inefficiente: $1-g$ individui basso-rischio restano non assicurati e subiscono il costo psicologico del rischio non coperto. Questo è l'**effetto di selezione avversa** puro: l'assicuratore non riesce a offrire contratti profittevoli ai basso-rischio perché sono contaminati dagli alto-rischio che li imiterebbero.

> [!summary]
> L'effetto di distruzione dell'assicurazione si manifesta nell'informazione pubblica (che elimina la copertura del rischio genetico) e nella selezione avversa (che nell'equilibrio separante lascia i basso-rischio non assicurati). In entrambi i casi, l'informazione — pubblica o asimmetrica — distrugge forme di condivisione del rischio che sarebbero state possibili in sua assenza.

[BB, pp. 288-291]

---

## L'Assicurazione Obbligatoria

L'assicurazione obbligatoria (*mandatory insurance*) risolve il problema imponendo a tutti di acquistare assicurazione a un premio unico $\bar{z} = \bar{\pi}D$, indipendentemente dal tipo. L'assicuratore non distingue i tipi (o non gli è consentito farlo).

Il risultato è **identico a quello del pooling volontario** quando esiste, e **implementa il pooling anche quando non esisterebbe** come equilibrio volontario. L'assicurazione obbligatoria risolve quindi la selezione avversa nel mercato assicurativo imponendo dall'esterno la mutualizzazione del rischio.

> [BB, p. 290] L'assicurazione obbligatoria implementa l'equilibrio di pooling quando non esisterebbe (quando la condizione 13.1 non è soddisfatta) o quando l'assicuratore non offrirebbe un contratto di pooling.

---

## Test Genetici e Implicazioni di Politica

L'analisi ha implicazioni concrete per il dibattito sui test genetici e sulla regolazione delle assicurazioni:

**Scenario senza trattamento disponibile:** Se non esiste un trattamento per la malattia identificata dal gene, il test genetico è "profezia senza prevenzione" (*prophecy without prevention*). In questo caso, l'effetto di distruzione dell'assicurazione domina: la disponibilità del test peggiora il benessere di chi non lo ha ancora fatto.

**Scenario con trattamento disponibile:** Se esiste un trattamento efficace, il test genetico ha un valore terapeutico diretto. Qui l'assicurazione obbligatoria è preferibile al divieto del test: permette la diagnosi e il trattamento, condividendo il costo assicurativo.

> [!example]
> Il caso della malattia di Huntington — neurodegenerativa, ereditaria, incurabile — è paradigmatico. Come descritto nel box di Birchler & Bütler, le sorelle Wexler, figlia di una malata di Huntington, hanno contribuito alla scoperta dei marcatori genetici della malattia nel 1983. Ma questa scoperta ha posto loro un dilemma: dovevano fare il test? Sapere con certezza di portare il gene (con 50% di probabilità) avrebbe eliminato la "negazione utile" (*denial*) che le aiutava ad andare avanti. Nancy Wexler ha risposto: preferivano non sapere. La disponibilità del test non era un beneficio automatico.

[BB, Box 13.1]

**La paradossale politica del "non sapere":** Ex ante — prima di conoscere il proprio tipo — tutti gli individui avversi al rischio preferiscono che l'informazione genetica non sia disponibile (o che non sia usabile dalle assicurazioni), perché ciò preserva la possibilità di assicurarsi contro il rischio genetico stesso. Ex post — dopo il test — i basso-rischio preferiscono poter rivelare il proprio stato per pagare premi inferiori. Questa divergenza tra preferenze ex ante e ex post rende la politica difficile: **la maggioranza ex post (i basso-rischio) resiste all'assicurazione obbligatoria che sarebbe ottimale ex ante**.

> [!summary]
> L'effetto di distruzione dell'assicurazione mostra che l'informazione non è sempre un bene pubblico economico. La disponibilità di test genetici — combinata con la selezione avversa — può eliminare mercati assicurativi mutualmente vantaggiosi. Ex ante, esisterebbe consenso unanime per l'assicurazione obbligatoria o per il divieto dei test. Ma ex post, chi risulta basso-rischio ha incentivo a uscire dal pool, distruggendo l'equilibrio di pooling. La politica dell'assicurazione obbligatoria (come nei sistemi sanitari pubblici europei) può essere interpretata come la soluzione istituzionale a questo problema di impegno (*commitment problem*).

[BB, pp. 292-293]

---

## Vedi Anche

- [[07_Inefficienza_e_Implicazioni]] — La selezione avversa come fallimento del mercato
- [[09_Modello_Wilson_Equilibri_Multipli]] — Gli equilibri multipli nel mercato con asimmetria informativa
- [[12_Confronto_Utilita_Equilibri_Assicurativi]] — Il confronto formale delle utilità nei diversi scenari
- [[10_Malpractice_Medica_Selezione_Avversa]] — Selezione avversa nel mercato medico

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/05_Selezione_avversa|Selezione avversa — Introduzione]] — questa nota è l'applicazione più profonda del meccanismo base: nel mercato assicurativo la selezione avversa si manifesta come "death spiral" (la spirale della morte citata nell'introduzione)
- [[0. Intro/01_Coordinamento_e_incentivi|Coordinamento e incentivi]] — l'assicurazione obbligatoria come soluzione istituzionale al commitment problem è un esempio di come le *istituzioni* (Stato, contratti sociali) risolvono problemi che il mercato non può risolvere da solo

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — il problema del commitment ("pre-impegnarsi al pooling prima che i tipi si rivelino") è il classico problema dell'impegno credibile nei giochi sequenziali: l'assicurazione obbligatoria funziona perché *rimuove* il nodo decisionale successivo alla rivelazione del tipo
- [[1. GT/05_Chicken_Game|Chicken Game]] — la dinamica ex ante / ex post ricorda la struttura del Chicken: ex ante tutti preferiscono il pooling (come preferiscono che nessuno sfidi); ex post chi scopre di essere basso-rischio ha incentivo a "sterzare" (uscire dal pool), rendendo insostenibile l'equilibrio cooperativo
- [[1. GT/08_Giochi_Ripetuti_Finiti|Giochi Ripetuti Finiti]] — in un sistema assicurativo volontario con orizzonte finito, l'equilibrio di pooling si dissolve per backward induction nell'ultimo periodo: i basso-rischio escono, il mercato si avvelena, e i premi salgono fino al collasso
