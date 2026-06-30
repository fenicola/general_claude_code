---
tags: [economia-informazione, segnalazione, modello-formale, capitale-umano]
aliases: [Esempio Numerico Spence, Casi Base, Caso A Caso B, No-Signalling]
links: [03_Modello_di_Spence, 05_Equilibrio_Separatore, 07_Equilibrio_Aggregante_Pooling]
---

# Esempio Numerico: Il Setup e i Casi Base (A e B)

## Il Setup

> [!definition]
> L'esempio numerico della lezione (slide 14) considera due tipi di candidati:
> - **Tipo L** (*low*): produttività $= 1$, quota nella popolazione $= q$
> - **Tipo H** (*high*): produttività $= 2$, quota nella popolazione $= 1-q$
>
> Tre ipotesi cruciali:
> 1. La **produttività è fissa**: l'istruzione *non* la modifica (così il modello isola il puro effetto-segnale, distinto dal capitale umano).
> 2. Il **salario di riserva è molto basso**: i lavoratori accettano comunque di lavorare.
> 3. Il mercato del lavoro è **competitivo**: i datori fanno profitti attesi nulli.

Su questo setup si confrontano tre regimi informativi: informazione perfetta (Caso A), informazione imperfetta senza segnalazione (Caso B), informazione imperfetta con segnalazione (Caso C). I primi due sono i benchmark; il terzo è il modello vero e proprio, sviluppato in [[05_Equilibrio_Separatore]] e [[07_Equilibrio_Aggregante_Pooling]].

---

## Caso A — Informazione Perfetta (benchmark di efficienza)

> [!definition]
> Se il datore **osserva la produttività** di ciascun candidato, in concorrenza è ottimale pagare ciascuno al proprio prodotto marginale (slide 15):
> $$ w_L = 1 \qquad w_H = 2 $$

È la soluzione classica della concorrenza perfetta: ogni lavoratore è remunerato esattamente quanto produce, i profitti sono nulli, l'allocazione è efficiente. **Non c'è alcun costo di segnalazione** perché non serve segnalare nulla.

Questo caso è il **metro di efficienza** rispetto al quale giudicare gli altri: come vedremo in [[06_Proprieta_Equilibrio_Separatore]], l'informazione completa **Pareto-domina** tutti gli equilibri separatori, perché ottiene gli stessi salari ma senza sprecare risorse in istruzione segnaletica.

---

## Caso B — Informazione Imperfetta, Nessuna Segnalazione (pooling sull'ignoranza)

> [!definition]
> Se il datore **non osserva** la produttività e **non esiste** alcun segnale, è ottimale (in concorrenza) pagare **lo stesso salario a tutti**, pari alla produttività media (slide 16):
> $$ w = (\text{prod. } L)\cdot q + (\text{prod. } H)\cdot(1-q) = 1\cdot q + 2\cdot(1-q) $$
> $$ \boxed{w = 2 - q} $$

Il salario unico $w = 2-q$ è la produttività attesa della popolazione. Alcune osservazioni:

- **Il salario decresce in $q$**: più sono numerosi i tipi L (più alto $q$), più basso il salario medio offerto a tutti. È l'esternalità informativa dei tipi bassi sui tipi alti, già incontrata nella [[2. Selezione Avversa/02_Mercato_dei_Limoni_Intuizione|selezione avversa]].
- **Profitti incrociati nulli in media, ma non individualmente**: il datore *perde* su ogni H (paga $2-q < 2$... no: paga $2-q$ a chi produce $2$, quindi **guadagna** su H) e *guadagna/perde* a seconda del tipo. Precisamente: paga $2-q$ a chi produce $1$ (tipo L) → **perdita** $1-(2-q)=q-1<0$ su ogni L; paga $2-q$ a chi produce $2$ (tipo H) → **profitto** $2-(2-q)=q>0$ su ogni H. In media i profitti si annullano: $q\cdot(1-(2-q)) + (1-q)\cdot(2-(2-q)) = 0$.

> [!intuition]
> Nel Caso B i tipi H **sussidiano** i tipi L: l'impossibilità di distinguerli costringe il datore a un salario medio che sovra-paga i meno produttivi e sotto-paga i più produttivi. È esattamente questa la situazione che il tipo H vorrebbe superare segnalando la propria qualità — purché il costo del segnale non sia troppo alto (vedi [[06_Proprieta_Equilibrio_Separatore]], punto 7).

---

## Il Ponte verso il Caso C (Segnalazione)

Il Caso A è efficiente ma irrealistico (la produttività non è osservabile). Il Caso B è realistico ma penalizza i tipi H. La domanda diventa: **i tipi H possono fare qualcosa per distinguersi?** La risposta è investire in istruzione $y$ in modo che il datore creda che solo gli H raggiungano un certo livello-soglia $y^*$.

Questo introduce i **costi di segnalazione** (con single-crossing, vedi [[02_Educazione_come_Segnale_Credibile]]):

$$
c_L(y) = y \qquad\qquad c_H(y) = \frac{y}{2}
$$

e lo **schema salariale a gradino** che il datore offre, dato il proprio credo (slide 17):

$$
w(y) = \begin{cases} 1 & \text{se } y < y^* \\ 2 & \text{se } y \ge y^* \end{cases}
$$

Da qui si sviluppano i due esiti possibili: l'[[05_Equilibrio_Separatore|equilibrio separatore]] (i tipi si distinguono) e l'[[07_Equilibrio_Aggregante_Pooling|equilibrio aggregante]] (i tipi restano confusi).

---

## Quadro di Sintesi dei Salari

| Regime | Salario tipo L | Salario tipo H | Costo di segnalazione | Efficienza |
|---|---|---|---|---|
| **A** — Info perfetta | $1$ | $2$ | nessuno | efficiente (benchmark) |
| **B** — No segnalazione | $2-q$ | $2-q$ | nessuno | redistribuisce (H sussidia... no, H sovra-remunerato) |
| **C** — Separatore | $1$ | $2$ | $H$ paga $c_H(y^*)$ | inefficiente (spreco $c_H(y^*)$) |
| **C** — Pooling | $2-q$ | $2-q$ | entrambi pagano | inefficiente (spreco puro) |

> [!intuition]
> Nota la simmetria: il **separatore** replica i salari del Caso A (info perfetta) ma con un costo di segnalazione sprecato; il **pooling** replica i salari del Caso B (no segnalazione) ma, se $y^*>0$, con un costo di segnalazione *del tutto inutile*. In entrambi i casi C la segnalazione introduce una perdita rispetto al benchmark corrispondente.

---

## Take-home message

> [!summary]
> Il setup ha due tipi (L produttività 1 quota $q$; H produttività 2 quota $1-q$), con produttività fissa e mercato competitivo. **Caso A (info perfetta):** ciascuno è pagato al prodotto marginale, $w_L=1$, $w_H=2$, nessun costo — è il benchmark efficiente. **Caso B (no segnalazione):** salario unico pari alla produttività media $w=2-q$, decrescente in $q$; i tipi H risultano sovra-remunerati e gli L sotto-remunerati rispetto al loro prodotto, con profitti medi nulli. Questi due casi inquadrano il problema: l'informazione perfetta è efficiente ma indisponibile, l'assenza di segnale comprime tutti sulla media. La segnalazione (Caso C) è il tentativo dei tipi H di distinguersi, al prezzo di un costo di istruzione $c_H(y^*)$ — che però è puro spreco rispetto al Caso A.

---

## Vedi anche

- [[03_Modello_di_Spence]] — La cornice teorica del processo di segnalazione
- [[02_Educazione_come_Segnale_Credibile]] — I costi $c_L=y$, $c_H=y/2$ e il single-crossing
- [[05_Equilibrio_Separatore]] — Il Caso C che separa i tipi
- [[07_Equilibrio_Aggregante_Pooling]] — Il Caso C che non separa i tipi

---

## Connessioni con il Vault

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/03_Modello_Formale_Due_Qualita|Modello a Due Qualità]] — stessa logica del salario/prezzo medio: il pooling sul valore atteso ($w=2-q$ qui, $p=E[V]$ là) penalizza la qualità alta
- [[2. Selezione Avversa/02_Mercato_dei_Limoni_Intuizione|Mercato dei Limoni]] — l'esternalità dei tipi bassi (auto/lavoratori) che abbassa il prezzo/salario medio

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — il salario competitivo $w=2-q$ del Caso B è l'unico salario coerente con profitti nulli e nessun segnale: un equilibrio in cui nessuno devia
