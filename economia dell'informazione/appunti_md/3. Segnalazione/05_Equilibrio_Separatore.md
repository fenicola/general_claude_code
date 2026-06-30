---
tags: [economia-informazione, segnalazione, equilibrio-separatore, single-crossing, modello-formale]
aliases: [Equilibrio Separatore, Separating Equilibrium, Wage Offer Schedule]
links: [04_Esempio_Numerico_Casi_Base, 02_Educazione_come_Segnale_Credibile, 06_Proprieta_Equilibrio_Separatore]
---

# L'Equilibrio Separatore (Separating Equilibrium)

## L'Idea

> [!definition]
> In un **equilibrio separatore** i due tipi scelgono livelli di istruzione *diversi* e vengono perciò *riconosciuti e remunerati diversamente*. Il segnale è **informativo**: osservandolo, il datore inferisce correttamente il tipo. Nel modello, i tipi L scelgono $y=0$ e i tipi H scelgono $y=y^*$, con i datori che pagano $w=1$ a chi ha $y<y^*$ e $w=2$ a chi ha $y \ge y^*$.

---

## Le Strategie e le Credenze in Equilibrio

Le strategie candidate all'equilibrio sono (slide 29):

- **Lavoratori:** L investe $y=0$; H investe $y=y^*$.
- **Datori (credenze):** $y < y^* \Rightarrow$ il candidato è L; $y \ge y^* \Rightarrow$ è H.
- **Datori (salari):** $w=1$ a L, $w=2$ a H.

Lo **schema salariale** ne risulta a gradino (slide 18–20):

$$
w(y) = \begin{cases} 1 & \text{se } y < y^* \\ 2 & \text{se } y \ge y^* \end{cases}
$$

Le credenze sono **confermate**? Sì: in equilibrio L sceglie $y=0 < y^*$ (e viene letto come L) e H sceglie $y=y^*$ (e viene letto come H). Le aspettative dei datori si auto-realizzano, quindi le condizioni di equilibrio del [[03_Modello_di_Spence|modello di Spence]] sono soddisfatte.

> [!intuition]
> Dato lo schema a gradino, l'unica **scelta ottimale** per qualunque lavoratore è $y=0$ oppure $y=y^*$ (slide 20): qualsiasi $y$ intermedio costa di più senza dare salario aggiuntivo, e qualsiasi $y>y^*$ costa di più senza alzare ulteriormente il salario. Si confrontano quindi solo due opzioni: non segnalare ($y=0$, salario 1) o segnalare ($y=y^*$, salario 2).

---

## La Derivazione delle Condizioni di Esistenza

Per avere un equilibrio separatore serve che **L scelga davvero $y=0$** e **H scelga davvero $y=y^*$**. Si confrontano i rendimenti netti (salario meno costo).

### Condizione per il tipo L (non deve imitare)

Il tipo L preferisce $y=0$ se il rendimento netto da non segnalare è almeno pari a quello da segnalare (slide 30):

$$
\underbrace{w(0)}_{=1} \;\ge\; \underbrace{w(y^*) - c_L(y^*)}_{= 2 - y^*}
$$

$$
1 \ge 2 - y^* \;\Longrightarrow\; \boxed{y^* \ge 1}
$$

Interpretazione: la soglia $y^*$ dev'essere **abbastanza alta** da scoraggiare l'imitazione del tipo L. Se l'istruzione richiesta è troppo poca, anche l'L troverebbe conveniente prenderla per spacciarsi da H.

### Condizione per il tipo H (deve voler segnalare)

Il tipo H preferisce $y=y^*$ se il rendimento netto da segnalare è almeno pari a quello da non segnalare:

$$
\underbrace{w(y^*) - c_H(y^*)}_{= 2 - y^*/2} \;\ge\; \underbrace{w(0)}_{=1}
$$

$$
2 - \frac{y^*}{2} \ge 1 \;\Longrightarrow\; \boxed{y^* \le 2}
$$

Interpretazione: la soglia $y^*$ dev'essere **abbastanza bassa** da non scoraggiare nemmeno il tipo H. Se l'istruzione richiesta è troppa, persino l'H rinuncerebbe a segnalare.

### Il risultato

> [!definition]
> Date le credenze dei datori, un equilibrio separatore esiste **per ogni soglia** $y^*$ tale che:
> $$ \boxed{1 \le y^* \le 2} $$

> [BB, p. 338] Il livello massimo di segnalazione accettabile per un individuo di alta abilità è $b_2$; il minimo richiesto per segnalare alta abilità in presenza di individui di bassa abilità è $b_1$. (Nel nostro esempio numerico: $b_1 = y^*_{\min} = 1$ e $b_2 = y^*_{\max} = 2$.)

---

## La Lettura Grafica: i Rendimenti Netti a, b, c

Il grafico costruito progressivamente nelle slide 21–28 mette insieme schema salariale e curve di costo. Si definiscono tre rendimenti netti:

- **$b$ = rendimento netto di L con $y=0$** $= w(0) - 0 = 1$ (slide 24).
- **$a$ = rendimento netto di L con $y=y^*$** $= w(y^*) - c_L(y^*) = 2 - y^*$ (slide 23). È la distanza verticale tra il salario $2$ e la retta di costo $c_L$ valutata in $y^*$.
- **$c$ = rendimento netto di H con $y=y^*$** $= w(y^*) - c_H(y^*) = 2 - y^*/2$ (slide 27).

Le condizioni di equilibrio si leggono allora come confronti diretti (slide 28):

$$
a < b \;\Longleftrightarrow\; 2-y^* < 1 \;\Longleftrightarrow\; y^* > 1 \quad\Rightarrow\quad \text{meglio per L scegliere } y=0
$$

$$
c > b \;\Longleftrightarrow\; 2 - \tfrac{y^*}{2} > 1 \;\Longleftrightarrow\; y^* < 2 \quad\Rightarrow\quad \text{meglio per H scegliere } y=y^*
$$

> [!intuition]
> Il segreto è tutto nel **single-crossing** ([[02_Educazione_come_Segnale_Credibile]]): poiché $c_L$ è più ripida di $c_H$, esiste una fascia di valori $y^* \in [1,2]$ in cui lo *stesso* livello-soglia costa "troppo" all'L (che rinuncia) ma "il giusto" all'H (che investe). Senza il differenziale di costo, le due condizioni $y^*\ge 1$ e $y^*\le 2$ non potrebbero essere soddisfatte insieme e la separazione fallirebbe.

---

## Un Esempio Concreto

> [!example]
> Prendiamo $y^* = 1$ (la soglia minima). Allora:
> - Tipo L: rendimento da $y=0$ è $1$; rendimento da $y=1$ è $2 - c_L(1) = 2 - 1 = 1$. È **indifferente**, e (per la condizione debole) sceglie $y=0$ → letto come L, paga $w=1$.
> - Tipo H: rendimento da $y=0$ è $1$; rendimento da $y=1$ è $2 - c_H(1) = 2 - 0{,}5 = 1{,}5 > 1$. **Segnala** → letto come H, paga $w=2$, rendimento netto $1{,}5$.
>
> I tipi si separano: L resta a $y=0$ con salario $1$, H prende $y=1$ con salario $2$ e rendimento netto $1{,}5$. Le credenze sono confermate. ✓

---

## Take-home message

> [!summary]
> Nell'equilibrio separatore i tipi L scelgono $y=0$ e gli H scelgono $y=y^*$, ricevendo rispettivamente $w=1$ e $w=2$: il segnale è informativo e ciascuno è pagato alla propria produttività. L'equilibrio esiste per ogni soglia $1 \le y^* \le 2$. La condizione inferiore $y^*\ge1$ impedisce l'imitazione del tipo L (la soglia è abbastanza alta); la condizione superiore $y^*\le2$ garantisce che persino l'H voglia segnalare (la soglia non è troppo alta). Le due condizioni sono compatibili **solo grazie al single-crossing** ($c_L=y > c_H=y/2$). Graficamente si leggono come confronti tra i rendimenti netti $a$, $b$, $c$: $a<b$ (L preferisce $y=0$) e $c>b$ (H preferisce $y=y^*$).

---

## Vedi anche

- [[04_Esempio_Numerico_Casi_Base]] — Setup e benchmark (Casi A e B)
- [[02_Educazione_come_Segnale_Credibile]] — Il single-crossing che rende compatibili le due condizioni
- [[06_Proprieta_Equilibrio_Separatore]] — Cosa implica l'intervallo $1 \le y^* \le 2$: molteplicità, Pareto-ranking, esternalità
- [[07_Equilibrio_Aggregante_Pooling]] — L'esito alternativo, quando il segnale *non* separa

---

## Connessioni con il Vault

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — le condizioni $y^*\ge1$ e $y^*\le2$ sono i **vincoli di incentive compatibility** che rendono le strategie reciproche miglior risposta: nessun tipo vuole deviare
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — la riduzione delle scelte ottimali a $\{y=0, y=y^*\}$ è backward induction sull'albero del gioco

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/12_Confronto_Utilita_Equilibri_Assicurativi|Confronto Utilità]] — l'equilibrio separatore assicurativo (Rothschild–Stiglitz) ha la stessa logica: i tipi si autoselezionano e i vincoli di IC determinano l'esistenza dell'equilibrio
