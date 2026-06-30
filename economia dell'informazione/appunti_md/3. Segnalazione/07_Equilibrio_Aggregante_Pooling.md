---
tags: [economia-informazione, segnalazione, equilibrio-aggregante, pooling, modello-formale]
aliases: [Equilibrio Aggregante, Pooling Equilibrium, Pooling Segnalazione]
links: [05_Equilibrio_Separatore, 04_Esempio_Numerico_Casi_Base, 06_Proprieta_Equilibrio_Separatore]
---

# L'Equilibrio Aggregante (Pooling Equilibrium)

## L'Idea

> [!definition]
> In un **equilibrio aggregante (pooling)** entrambi i tipi mandano lo **stesso segnale** e ricevono lo **stesso salario**: vengono "messi insieme" (*pooled*) e restano indistinguibili. A differenza del [[05_Equilibrio_Separatore|separatore]], il segnale **non è informativo** e l'investimento in istruzione, se positivo, è puro spreco.

> [BB] In alcuni casi entrambi i tipi inviano lo stesso segnale e ricevono lo stesso salario: vengono "pooled" — la buona istruzione non implica necessariamente alta produttività.

---

## Le Credenze che Sostengono il Pooling

Perché il pooling sia un equilibrio servono credenze diverse da quelle del separatore. Si supponga che i datori credano (slide 35):

$$
\text{(i)}\quad y < y^* \;\Rightarrow\; L \text{ con certezza}
$$
$$
\text{(ii)}\quad y \ge y^* \;\Rightarrow\; L \text{ con prob. } q,\ H \text{ con prob. } (1-q)
$$

In parole: chi non raggiunge la soglia è sicuramente un tipo basso; chi la raggiunge potrebbe essere *qualunque* tipo, nelle proporzioni della popolazione. La buona istruzione, sotto queste credenze, non garantisce alta produttività.

I salari competitivi (produttività attesa) che ne derivano sono (slide 36):

$$
w(y < y^*) = 1 \qquad\qquad w(y \ge y^*) = 1\cdot q + 2\cdot(1-q) = 2 - q
$$

Si noti: chi segnala riceve $2-q$, **lo stesso salario del Caso B** ([[04_Esempio_Numerico_Casi_Base|no-signalling]]), perché il datore non riesce comunque a distinguere i tipi tra chi ha $y\ge y^*$.

---

## La Condizione di Esistenza del Pooling

Perché *entrambi* i tipi scelgano $y=y^*$ (anziché $y=0$), il rendimento netto da segnalare deve superare quello da non segnalare per ciascuno (slide 37).

### Per il tipo L

$$
w(y^*) - c_L(y^*) \ge w(0) \;\Longrightarrow\; (2-q) - y^* \ge 1 \;\Longrightarrow\; \boxed{1 - q \ge y^*}
$$

### Per il tipo H

$$
w(y^*) - c_H(y^*) \ge w(0) \;\Longrightarrow\; (2-q) - \frac{y^*}{2} \ge 1 \;\Longrightarrow\; \boxed{1 - q \ge \frac{y^*}{2}}
$$

### La condizione vincolante

> [!definition]
> Se è soddisfatta la condizione del tipo L, $1-q \ge y^*$, allora quella del tipo H, $1-q \ge y^*/2$, è soddisfatta **a fortiori** (perché $y^*/2 < y^*$). Dunque la **condizione vincolante** per il pooling è:
> $$ \boxed{1 - q \ge y^*} $$

> [!intuition]
> Il vincolo dice che la soglia $y^*$ dev'essere **abbastanza bassa**. Per il pooling il tipo critico è l'**L**: è lui ad avere il costo di segnalazione più alto, quindi è lui il primo a rinunciare se $y^*$ cresce. Se persino l'L (il più riluttante) trova conveniente segnalare, allora a maggior ragione lo trova l'H. È il contrario del separatore, dove il vincolo critico superiore riguardava l'H.

---

## La Lettura Grafica: i Rendimenti a, b, c (versione pooling)

Nel grafico delle slide 38–46 (con $w(y\ge y^*) = 2-q$):

- **$a$ = rendimento netto di L con $y=y^*$** $= (2-q) - y^*$ (slide 41)
- **$b$ = rendimento netto di L con $y=0$** $= 1$ (slide 42), con $b < a$ — proprio la condizione $1-q \ge y^*$
- **$c$ = rendimento netto di H con $y=y^*$** $= (2-q) - y^*/2$ (slide 45), con $c > b$

Da cui (slide 46):

$$
c > a > b \quad\Longrightarrow\quad \text{conviene a } \textbf{entrambi} \text{ scegliere } y = y^*
$$

L'ordine $c>a>b$ riassume tutto: entrambi i tipi preferiscono segnalare, ed è per questo che si "ammucchiano" sullo stesso $y^*$.

---

## È Davvero un Equilibrio? La Verifica delle Credenze

Bisogna controllare che le credenze (i)–(ii) siano **confermate** (slide 47):

- **Nessun lavoratore sceglie $y < y^*$** → la credenza (i) "chi sta sotto è L" non viene mai messa alla prova (è vuota in equilibrio, ma serve come *minaccia fuori dall'equilibrio*).
- Tra chi sceglie $y \ge y^*$ ci sono esattamente una quota $q$ di L e $1-q$ di H (tutti segnalano, quindi la composizione di chi segnala è quella della popolazione) → la credenza (ii) è **confermata**. ✓

Le credenze si auto-realizzano: è un equilibrio.

---

## Il Caso Limite e l'Inutilità del Segnale

> [!intuition]
> Supponiamo $q \ge \tfrac12$: allora la condizione $1-q \ge y^*$ impone $y^* \le \tfrac12$ (slide 49). Due sotto-casi:
> - **$y^* = 0$** (che soddisfa la condizione): l'esito coincide *esattamente* con la [[04_Esempio_Numerico_Casi_Base|non-segnalazione]] — tutti ricevono $w=2-q$ senza costi.
> - **$y^* > 0$ con $1-q \ge y^*$ ancora valida**: è *razionale* per i lavoratori pagare il costo di segnalazione **anche se non porta alcun beneficio** — tutti ricevono comunque $w=2-q$, ma hanno sprecato risorse in istruzione.

Questo è il cuore paradossale del pooling: i lavoratori bruciano risorse in un segnale **del tutto inutile**, semplicemente perché le credenze dei datori puniscono ($w=1$) chi non lo fa. La minaccia fuori-equilibrio "chi non segnala è L" basta a costringere tutti a segnalare a vuoto.

> [BB, p. 338] La segnalazione non fa parte del contratto in senso stretto: la parte segnalante si limita ad aspettarsi che il proprio payoff dipenda dal livello dell'attività di segnalazione.

---

## Pooling vs Separatore: Quadro di Confronto

| | **Separatore** | **Pooling** |
|---|---|---|
| Scelte | L: $y=0$; H: $y=y^*$ | entrambi: $y=y^*$ |
| Salari | $w_L=1$, $w_H=2$ | $w=2-q$ per chi segnala |
| Segnale | informativo | non informativo |
| Condizione | $1 \le y^* \le 2$ | $1-q \ge y^*$ |
| Tipo critico | H (vincolo superiore) | L (vincolo) |
| Ruolo di $q$ | irrilevante | centrale |
| Spreco | $c_H(y^*)$ (solo H) | $c(y^*)$ per tutti, *puro* |

---

## Take-home message

> [!summary]
> Nell'equilibrio aggregante entrambi i tipi scelgono lo stesso segnale $y=y^*$ e ricevono lo stesso salario $w=2-q$ (come nel Caso B): il segnale **non è informativo**. Le credenze che lo sostengono puniscono con $w=1$ chiunque resti sotto soglia, mentre attribuiscono a chi segnala la produttività media. La condizione di esistenza è $1-q \ge y^*$ (la soglia dev'essere abbastanza bassa); il **tipo critico è l'L**, il più riluttante a causa del costo più alto. Graficamente $c>a>b$. Caso paradossale: se $y^*>0$ ma la condizione regge, i lavoratori **pagano un costo di segnalazione del tutto inutile** — ricevono comunque $2-q$ — solo perché la minaccia fuori-equilibrio li costringe. Il pooling con $y^*=0$ coincide con la non-segnalazione.

---

## Vedi anche

- [[05_Equilibrio_Separatore]] — L'esito che differenzia i tipi (confronto diretto)
- [[04_Esempio_Numerico_Casi_Base]] — Il Caso B e il salario $w=2-q$
- [[06_Proprieta_Equilibrio_Separatore]] — Le proprietà dell'altro esito
- [[03_Modello_di_Spence]] — La definizione di equilibrio (credenze confermate) qui verificata

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — le credenze "fuori dall'equilibrio" (cosa pensa il datore di chi devia a $y<y^*$) sono ciò che, nei giochi di segnalazione, va specificato per sostenere il pooling; è il tema dei *refinements* (es. equilibrio bayesiano perfetto)
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — anche il pooling è un Nash: date le credenze e i salari, nessun tipo vuole deviare

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/11_Assicurazione_Vita_Effetto_Distruzione|Effetto Distruzione]] — il pooling assicurativo (tutti allo stesso premio medio) è l'analogo del pooling salariale qui: tipi diversi messi insieme allo stesso prezzo/salario medio
