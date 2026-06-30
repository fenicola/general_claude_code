---
tags: [economia-informazione, reputazione, teoria-dei-giochi, beni-pubblici, cooperazione, andreoni]
aliases: [Public Good Game, Gioco dei Beni Pubblici, Esperimento Andreoni, Free-riding]
links: [02_Trust_Game_e_Reputazione, 09_Punizione_Altruistica_e_Ultimatum]
---

# Public Good Game e l'Esperimento di Andreoni

## Perché studiare la cooperazione

La capacità di cooperare all'interno dei gruppi è uno degli elementi che hanno favorito il successo delle società umane. La cooperazione, però, **non nasce spontaneamente**: ogni individuo ha un incentivo a comportarsi da **free-rider**, cioè a beneficiare dei vantaggi collettivi senza contribuire ai costi. Il *Public Good Game* è lo strumento sperimentale con cui gli economisti studiano questa tensione tra interesse individuale ed efficienza collettiva.

> [!definition] Beni pubblici
> Un **bene pubblico** ha due proprietà:
> - **Non escludibilità** — è difficile (o impossibile) impedire ad altri di beneficiarne.
> - **Non rivalità** — il consumo da parte di un individuo non riduce il beneficio disponibile per gli altri.
>
> Esempio classico: l'**illuminazione stradale** 💡. Se installo un lampione davanti a casa, anche i vicini ne godono (non posso escluderli) e il loro godimento non riduce il mio (non c'è rivalità).

---

## Il gioco: struttura formale

Ogni giocatore dispone di una **dotazione iniziale** $y$ e decide quanto investire nel bene pubblico attraverso il proprio **contributo** $g_i$. Una volta prodotto, il bene è goduto da tutti, indipendentemente da chi ha contribuito.

Il **payoff individuale** è:

$$
\pi_i = y - g_i + a \sum_{j=1}^{n} g_j
$$

dove:
- $n$ = numero di giocatori
- $y$ = dotazione iniziale
- $g_i$ = contributo del giocatore $i$
- $a$ = rendimento (marginale) individuale del bene pubblico

La condizione cruciale sui parametri è:

$$
0 < a < 1 < n\,a
$$

> [!intuition] Lettura della condizione
> - $a < 1$ → per il **singolo** individuo contribuire **non conviene**: ogni euro versato gli rende solo $a < 1$ euro. È il cuore dell'incentivo al free-riding.
> - $n\,a > 1$ → per il **gruppo** il bene pubblico è **socialmente efficiente**: ogni euro versato genera $n\,a > 1$ euro complessivi di beneficio.
>
> È la stessa struttura di incentivi del [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]], ma con $n$ giocatori.

---

## L'equilibrio di Nash: nessuno contribuisce

Poiché contribuire è individualmente svantaggioso ($a < 1$), la strategia dominante di ciascun giocatore è non versare nulla. L'**equilibrio di Nash** è quindi:

$$
g_i^* = 0 \qquad \forall i
$$

> [!warning] Il fallimento della cooperazione
> In equilibrio **nessuno contribuisce**, perché ogni individuo preferisce beneficiare del contributo altrui senza sostenere costi. Si realizza un esito **Pareto-inefficiente**: il bene socialmente desiderabile non viene prodotto. È proprio per questo che molti beni pubblici vengono prodotti direttamente dallo **Stato** attraverso la tassazione obbligatoria.

---

## L'anomalia sperimentale: la cooperazione decade

Negli esperimenti il comportamento osservato **contraddice** la previsione teorica:

- All'inizio le persone **tendono a cooperare** e a contribuire al bene pubblico.
- Solo successivamente i contributi **diminuiscono gradualmente**, fino a convergere verso l'equilibrio di free-riding ($g = 0$).

Per spiegare questo *decadimento progressivo* della cooperazione sono state proposte due ipotesi concorrenti:

> [!note] Strategies Hypothesis (ipotesi strategica)
> Esistono individui con diversi livelli di razionalità:
> - i soggetti **più razionali** cooperano inizialmente *in modo strategico*;
> - i soggetti **meno razionali** interpretano questo come segnale di cooperazione stabile e continuano a contribuire.
>
> A quel punto i giocatori più razionali smettono progressivamente di contribuire e **sfruttano** (free-riding) il comportamento cooperativo altrui. Il decadimento sarebbe quindi un fenomeno *strategico*.

> [!note] Learning Hypothesis (ipotesi dell'apprendimento)
> I giocatori **non conoscono** subito la strategia ottimale. Iniziano cooperando, ma per **tentativi ed errori** imparano gradualmente che l'equilibrio di Nash consiste nel non contribuire. Nel tempo i contributi si riducono fino a zero. Il decadimento sarebbe quindi un fenomeno di *apprendimento*.

---

## L'esperimento di Andreoni

**Andreoni** costruisce un disegno sperimentale per discriminare tra le due ipotesi.

### Test della Strategies Hypothesis: Partners vs Strangers

Confronta due condizioni:

1. **Partners** — gli stessi soggetti interagiscono ripetutamente nello stesso gruppo.
2. **Strangers** — i partecipanti vengono continuamente rimescolati in gruppi diversi.

> [!tip] Previsione
> Se l'ipotesi strategica fosse corretta, il decadimento della cooperazione dovrebbe essere **più forte tra gli strangers**: senza una relazione continuativa, i giocatori razionali hanno maggiore incentivo a sfruttare gli altri tramite free-riding.

**Risultato:** la previsione **non è confermata**. La cooperazione non è più elevata tra i partner; anzi, in diversi round il livello medio di contribuzione è **persino maggiore tra gli strangers**. Questo **indebolisce** la Strategies Hypothesis.

### Test della Learning Hypothesis: il restart

Andreoni introduce una seconda modifica: i soggetti sanno che il gioco durerà un numero limitato di round (es. 10), ma — una volta finito — il gioco **ricomincia da capo** in modo inatteso.

> [!tip] Previsione
> Se l'ipotesi dell'apprendimento fosse corretta, dopo aver "imparato" che l'equilibrio è il free-riding, alla ripartenza i giocatori dovrebbero scegliere **immediatamente** $g = 0$.

**Risultato:** anche questa previsione **non è confermata**. Quando il gioco ricomincia, i partecipanti **tornano a cooperare**, nonostante avessero già "imparato" nella partita precedente che l'equilibrio tende al free-riding.

> [!summary] Cosa ci dice l'esperimento di Andreoni
> Il decadimento della cooperazione **non** è spiegato bene né dall'ipotesi strategica né da quella dell'apprendimento. Il comportamento umano non dipende solo da calcoli strettamente razionali: gli individui tendono a **cooperare quando percepiscono cooperazione** negli altri e a **ridurre i contributi quando osservano opportunismo**. La cooperazione è guidata da **reciprocità, fiducia e norme sociali**, più che dalla convergenza verso l'equilibrio teorico di Nash.

---

## Perché alcuni cooperano e altri no: i tipi comportamentali

Un filone successivo indaga l'**eterogeneità** dei comportamenti. A ogni partecipante si chiede quanto contribuirebbe *condizionatamente* al contributo medio degli altri (la domanda viene ripetuta per ogni possibile livello medio degli altri). Questo permette di classificare i soggetti in **tipi comportamentali**:

| Tipo | Comportamento |
|---|---|
| **Free-riders** | Non contribuiscono mai |
| **Conditional cooperators** | Cooperano solo se vedono cooperare gli altri |
| **Hump-shaped** | Aumentano inizialmente la cooperazione, poi la riducono |
| **Cooperatori incondizionati** | Pochi individui che cooperano quasi sempre, a prescindere dagli altri |

> [!important] Il ruolo dei conditional cooperators
> Circa il **50% dei soggetti** è composto da *conditional cooperators*. Questo spiega il decadimento osservato: all'inizio molti cooperano perché si **aspettano** cooperazione; quando però incontrano anche un solo **free-rider**, smettono progressivamente di contribuire. Il comportamento si trasmette agli altri membri, producendo un **crollo generale** della cooperazione fino alla convergenza verso il free-riding.

Questo prepara la domanda della nota successiva: **come si può sostenere la cooperazione** nonostante i free-rider? → la risposta è la [[09_Punizione_Altruistica_e_Ultimatum|punizione altruistica]].

---

## 🔗 Connessioni

- Logica analoga a $n$ giocatori: [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]
- Cooperazione sostenibile nei giochi ripetuti: [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]], [[1. GT/10_Folk_Theorem|Folk Theorem]]
- Il rimedio alla non-cooperazione: [[09_Punizione_Altruistica_e_Ultimatum|Punizione Altruistica e Gioco dell'Ultimatum]]
- La reputazione come altro rimedio decentralizzato: [[01_Mercati_Reputazionali]], [[02_Trust_Game_e_Reputazione]]
- Critica all'assunto di puro auto-interesse: [[06_Psicologia_degli_Incentivi]]
