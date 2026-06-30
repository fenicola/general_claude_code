---
tags: [economia-informazione, game-theory, giochi-ripetuti, cooperazione, trigger-strategies]
aliases: [Giochi Ripetuti Indefiniti, Indefinitely Repeated Games, Grim Trigger, Tit-for-Tat, Infinite Repetition]
links: [06_Dilemma_Prigioniero, 07_Giochi_Dinamici_Sequenziali, 08_Giochi_Ripetuti_Finiti, 10_Folk_Theorem, 0. Intro/08_Azzardo_morale, 0. Intro/03_Beni_comuni, 0. Intro/04_Principale_e_agente]
---

# Giochi Ripetuti Indefinitamente (e Infinitamente)

## Definizione Formale

> [!definition] Gioco Ripetuto Indefinitamente
> Un gioco è **ripetuto indefinitamente** quando i giocatori sanno che il gioco è finito, ma non sanno quando terminerà. Si modella assumendo che ad ogni round ci sia una probabilità fissa $P \in (0, 1)$ che il gioco continui al round successivo, e una probabilità $(1-P)$ che termini. Il **valore atteso del numero di round** è $\frac{1}{1-P}$.
>
> Un gioco è **ripetuto infinitamente** quando i giocatori credono che il gioco andrà avanti per sempre. Le cedute future vengono scontate con un **fattore di sconto** $F = \frac{1}{1+r}$, dove $r$ è il tasso di interesse.

> [C, p. 204–209] "Se un gioco è ripetuto un numero infinito di volte i giocatori credono che ci sarà sempre un'altra ripetizione. In un gioco ripetuto indefinitamente i giocatori sanno che c'è un ultimo round ma non sanno quando sarà."

> [C, p. 232–233] Formalmente, i due giochi — ripetizione infinita con sconto $F$ e ripetizione indefinita con probabilità di continuazione $P$ — sono equivalenti se $F = P$. I payoff hanno la stessa struttura matematica.

## Intuizione Economica

> [!intuition]
> La chiave di questo risultato è la **shadow of the future**: la minaccia di punire domani chi defeziona oggi deve essere sufficientemente pesante da scoraggiare la defezione. Se il futuro conta abbastanza (alto $P$ o alto $F$), la cooperazione diventa razionale.
>
> Il meccanismo è semplice: se coopero oggi, guadagno $a$ (payoff da cooperazione) per un numero atteso di round; se defeziono, guadagno $c$ oggi ma poi l'altro mi punisce e guadagno solo $d$ per sempre. La defezione conviene solo se il guadagno immediato supera le perdite future scontate.
>
> Questo spiega perché le relazioni commerciali di lungo periodo tendono ad essere più cooperative: il valore del futuro è alto, il che rende la punizione una minaccia credibile e la cooperazione razionale.

## Le Trigger Strategies

> [!definition] Trigger Strategy
> Una **trigger strategy** (strategia di innesco/punizione) è una meta-strategia che prescrive di cooperare finché l'altro coopera, ma di "innescare" una punizione non appena l'altro defeziona. Esempi:
>
> - **Grim Trigger** (*strategia crudele*): coopera finché l'altro coopera; se l'altro defeziona *una volta*, defeziona per sempre.
> - **Tit-for-Tat**: nell'primo round coopera; in ogni round successivo ripeti l'azione dell'altro al round precedente (coopera se ha cooperato, defeziona se ha defezionato).
> - **Tit-for-Two-Tat**: defeziona solo se l'altro ha defezionato due volte di fila.

Le trigger strategies sono anche chiamate *stick-and-carrot strategies*: la cooperazione è il "carrot" (incentivo), la punizione è il "stick" (deterrenza).

## Modello: Condizione di Cooperazione nel Gioco Indefinito

Consideriamo il PD generalizzato con payoff $c > a > d > b$.

**Payoff atteso se entrambi cooperano** (con strategia Grim di entrambi):

$$EP(c,c) = a + aP + aP^2 + \ldots = \frac{a}{1-P}$$

Questa è la somma di una serie geometrica infinita: se il gioco continua con probabilità $P$ ad ogni round, il payoff atteso totale è $a/(1-P)$.

**Payoff atteso se Joe defeziona oggi** (l'altro gioca Grim, quindi da domani in poi è defezione reciproca):

$$EP(d,c) = c + dP + dP^2 + \ldots = c + \frac{dP}{1-P}$$

**Condizione affinché la cooperazione sia un SPNE**:

$$EP(c,c) \geq EP(d,c)$$
$$\frac{a}{1-P} \geq c + \frac{dP}{1-P}$$

Svolgendo l'algebra:
$$a \geq c(1-P) + dP = c - cP + dP$$
$$a - c \geq P(d - c)$$

Poiché $a < c$ e $d < c$, entrambi i lati sono negativi; dividendo per $(d-c) < 0$, l'inequazione si inverte:

$$\boxed{P \geq \frac{a-c}{d-c}}$$

Questa è la **condizione critica**: se la probabilità di continuazione supera questa soglia, cooperare (e minacciare Grim) è un SPNE.

> [!example] Applicazione numerica con l'esempio delle slide
> Con il PD standard delle slide: $a=1$ (CC), $b=-1$ (CD), $c=2$ (DC), $d=0$ (DD):
> $$P \geq \frac{1-2}{0-2} = \frac{-1}{-2} = \frac{1}{2}$$
> Dunque: se $P > 1/2$, la cooperazione sostenuta dal Grim Trigger è un SPNE. Il valore critico $P^* = 1/2$ significa che il gioco deve continuare con probabilità almeno del 50% ad ogni round affinché la cooperazione sia razionale.

## Ripetizione Infinita con Sconto

Per il gioco **infinitamente** ripetuto con fattore di sconto $F = 1/(1+r)$, la matematica è identica con $F$ al posto di $P$:

$$EP(c,c) = \frac{a}{1-F}, \quad EP(d,c) = c + \frac{dF}{1-F}$$

**Condizione di cooperazione**:
$$\boxed{F \geq \frac{a-c}{d-c}}$$

> [C, p. 206–209] "Come finché i payoff futuri hanno un valore positivo, i benefici della cooperazione infinita tenderanno a superare qualsiasi guadagno a breve termine dalla defezione."

## Confronto tra Grim e Tit-for-Tat

| Caratteristica | Grim Trigger | Tit-for-Tat |
|---|---|---|
| Punizione | Permanente (defeziona per sempre) | Temporanea (una sola mossa) |
| Perdono | Nessuno | Immediato dopo cooperazione |
| Robustezza a errori | Fragile: un errore porta a defez. eterna | Resistente: si riprende |
| Credibilità | Alta (deterrenza massima) | Moderata |

> [C, p. 208] "Il Folk Theorem dice che un numero infinito di strategie può far rispettare qualsiasi dato esito in un gioco ripetuto indefinitamente o infinitamente come il PD ripetuto. Ad esempio, una strategia più indulgente come il tit-for-tat può anch'essa ottenere un esito cooperativo."

## Implicazioni Economiche

La condizione $P \geq (a-c)/(d-c)$ ha profonde implicazioni:

1. **Frequenza delle interazioni**: più frequentemente si interagisce, maggiore è il valore del futuro → più facile sostenere la cooperazione.

2. **Stabilità del mercato**: mercati stabili (bassa probabilità di uscita) favoriscono la cooperazione (implicita o esplicita tra oligopolisti).

3. **Tassi di interesse**: alti $r$ abbassano $F$, rendendo la cooperazione più difficile. I periodi di alta inflazione/instabilità tendono a distruggere le relazioni cooperative.

4. **Politica antitrust**: la legge interviene proprio perché nei mercati oligopolistici la ripetizione crea le condizioni per la collusione tacita — una forma di cooperazione che danneggia i consumatori.

> [BB, p. 222–224] Birchler & Bütler discutono come nei mercati reali le relazioni di lungo periodo tra banca e cliente, o tra fornitore e acquirente, siano sostenute proprio da questo meccanismo di reputazione e punizione implicita.

> [!summary] Take-home message
> La ripetizione indefinita risolve il paradosso del [[06_Dilemma_Prigioniero|Dilemma del Prigioniero]]: se la probabilità di continuazione è sufficientemente alta ($P > (a-c)/(d-c)$), le trigger strategies rendono la cooperazione un SPNE. Il meccanismo è la **shadow of the future**: la minaccia credibile di punire la defezione con la perdita dei benefici futuri coooperativi. Questo risultato ha applicazioni vastissime in economia industriale, macroeconomia e teoria contrattuale. La logica è la stessa per la ripetizione infinita con sconto $F$. Il [[10_Folk_Theorem]] generalizza questo risultato in modo sorprendente.

## 🔗 Connessioni con l'Economia dell'Informazione

I **giochi ripetuti indefinitamente** sono il fondamento formale di alcuni dei meccanismi chiave dell'economia dell'informazione:

- **Reputazione e qualità** ([[0. Intro/08_Azzardo_morale|azzardo morale]]): un esperto (medico, meccanico, avvocato) che si preoccupa della reputazione futura può essere disciplinato dalla minaccia di perdere clienti — una forma di "grim trigger" decentralizzato che rende razionale il comportamento onesto anche senza enforcement formale.
- **Governance dei beni comuni** ([[0. Intro/03_Beni_comuni|beni comuni]]): Ostrom (Nobel 2009) mostra empiricamente che le comunità che gestiscono beni comuni ricorrono a regole di punizione escalante — trigger strategies reali in giochi ripetuti tra gli stessi utenti.
- **Contratti relazionali** ([[0. Intro/04_Principale_e_agente|Principale–Agente]]): quando i contratti formali sono incompleti (non tutti gli stati del mondo sono verificabili), le parti si affidano a impegni impliciti sostenuti dalla reputazione. La condizione $P \geq (a-c)/(d-c)$ stabilisce quando questo è sostenibile in equilibrio.
- **Collusione implicita**: imprese oligopolistiche che non si accordano esplicitamente possono comunque colludere sui prezzi se $P$ è alto — il che è il fondamento economico del diritto antitrust nelle industrie concentrate.
