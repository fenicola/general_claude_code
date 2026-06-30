---
tags: [economia-informazione, selezione-avversa, assicurazione, pooling, separating, utilita, ex-ante, ex-post]
aliases: [Confronto Utilità Equilibri Assicurativi, Tabella Utilità Assicurazione, Ex Ante Ex Post Assicurazione]
links: [11_Assicurazione_Vita_Effetto_Distruzione, 07_Inefficienza_e_Implicazioni]
---

# Confronto delle Utilità nei Diversi Equilibri Assicurativi

## Il Quadro dei Tre Scenari

Il modello dell'effetto di distruzione dell'assicurazione, sviluppato in [[11_Assicurazione_Vita_Effetto_Distruzione]], genera tre possibili regimi di mercato:

1. **Informazione pubblica**: l'assicuratore conosce il tipo di ogni individuo e offre premi differenziati.
2. **Equilibrio di pooling**: l'assicuratore offre un premio unico che attrae entrambi i tipi (sia volontariamente, sia in regime no-info, sia con assicurazione obbligatoria).
3. **Equilibrio separante**: l'assicuratore può assicurare solo gli alto-rischio; i basso-rischio rimangono scoperti.

Una domanda naturale è: **quale regime preferisce ciascun agente?** La risposta dipende crucialmente da *quando* poniamo la domanda: prima (*ex ante*) o dopo (*ex post*) la rivelazione del tipo genetico.

---

## La Tabella dei Livelli di Utilità

La tabella riassume i livelli di utilità nei tre scenari per le tre categorie di individui:

$$\begin{array}{lccc}
 & \textbf{Info. Pubblica} & \textbf{Pooling} & \textbf{Separante} \\
\hline
\textbf{Ex ante} & Y - \bar{\pi}D & Y - \bar{\pi}D & Y - [\bar{\pi} + v(1-g)(1-\pi)]D \\
\textbf{Basso-rischio} & Y - (1-\pi)D & Y - \bar{\pi}D & Y - (1+v)(1-\pi)D \\
\textbf{Alto-rischio} & Y - \pi D & Y - \bar{\pi}D & Y - \pi D \\
\hline
\end{array}$$

dove $\bar{\pi} = g\pi + (1-g)(1-\pi)$ è il rischio medio della popolazione e $(1-\pi) < \bar{\pi} < \pi$.

---

## Analisi Ex Ante: Prima del Test

**Ex ante**, nessun individuo conosce il proprio tipo. L'utilità è calcolata rispetto all'incertezza sia sulla malattia *che* sul tipo genetico.

### Informazione Pubblica vs. Pooling

A prima vista, i livelli di utilità attesa ex ante sembrano identici tra informazione pubblica e pooling: entrambi danno $Y - \bar{\pi}D$. Ma questa equivalenza è fuorviante.

> [!intuition]
> Nel **pooling**, il payoff è *sicuro* $Y - \bar{\pi}D$, indipendente dal tipo che si scoprirà. Nell'**informazione pubblica**, il payoff ex ante è $Y - \bar{\pi}D$ *in attesa*, ma con varianza positiva: chi risulterà basso-rischio otterrà $Y-(1-\pi)D$, chi risulterà alto-rischio otterrà $Y-\pi D$. Entrambi si rivelano solo dopo il test. Per un individuo avverso al rischio, la certezza del pooling è preferibile all'incertezza dell'informazione pubblica, anche a parità di valore atteso.

Formalmente, per un individuo avverso al rischio (utilità concava), vale la preferenza:

$$\underbrace{Y - \bar{\pi}D}_{\text{pooling (certo)}} \succ \underbrace{(1-g)[Y-(1-\pi)D] + g[Y-\pi D]}_{\text{info. pubblica (rischioso)}} = Y - \bar{\pi}D$$

Il pooling **Pareto-domina** l'informazione pubblica per individui avversi al rischio, anche se i valori attesi sono uguali. Sarebbe Pareto-ottimale **sopprimere l'informazione pubblica** o **rendere obbligatoria l'assicurazione**.

### Separante vs. Pooling

L'equilibrio separante è chiaramente peggiore del pooling ex ante:

$$Y - \bar{\pi}D \quad > \quad Y - [\bar{\pi} + v(1-g)(1-\pi)]D$$

perché $v(1-g)(1-\pi) > 0$. Nel separante, i basso-rischio non si assicurano e subiscono una perdita secca da avversione al rischio. **Quando non esiste un equilibrio di pooling, l'assicurazione obbligatoria Pareto-domina il laissez-faire.**

[BB, p. 291]

---

## Analisi Ex Post: Dopo il Test

Una volta noto il proprio tipo genetico, gli interessi divergono:

### Basso-Rischio (Ex Post)

I basso-rischio preferiscono l'informazione pubblica: $Y-(1-\pi)D > Y-\bar{\pi}D$ perché $(1-\pi) < \bar{\pi}$ (pagano un premio più basso). Tra pooling e separante, il confronto è:

$$Y - \bar{\pi}D \quad \text{vs.} \quad Y - (1+v)(1-\pi)D$$

Il basso-rischio preferisce il pooling se $\bar{\pi} < (1+v)(1-\pi)$, che riorganizzando dà:

$$\frac{v}{g} \geq \frac{2\pi-1}{1-\pi}$$

che è esattamente la condizione $(13.1)$ di esistenza del pooling. Dunque: i basso-rischio preferiscono il pooling *se e solo se* l'equilibrio di pooling esiste. Se esistesse ma non fosse offerto dall'assicuratore, accetterebbero l'assicurazione obbligatoria.

### Alto-Rischio (Ex Post)

Per gli alto-rischio, $Y-\bar{\pi}D > Y-\pi D$ perché $\bar{\pi} < \pi$. Gli alto-rischio preferiscono **sempre** il pooling rispetto all'informazione pubblica o al separante: si "nascondono" nel pool e trasferiscono parte del loro costo ai basso-rischio. Beneficiano dell'assicurazione obbligatoria ogni volta che il pooling non si realizza spontaneamente.

---

## Il Problema di Impegno Politico

> [!intuition]
> **Il paradosso temporale della politica assicurativa.** Ex ante (prima del test), c'è consenso unanime verso il pooling o l'assicurazione obbligatoria: nessuno sa se sarà basso o alto rischio. Sarebbe razionale per tutti "pre-impegnarsi" a un sistema di pooling. Tuttavia, una volta rivelati i tipi, la maggioranza (i basso-rischio, che nella popolazione sono $1-g$) ha interesse a uscire dal pool. Se $g$ è piccolo (gene raro), la maggioranza ex post resiste all'assicurazione obbligatoria, anche se ex ante l'avrebbe votata.
>
> Questo è un classico problema di impegno: le preferenze cambiano con l'informazione, e le istituzioni devono essere progettate tenendo conto di questo cambiamento. Un sistema di assicurazione obbligatoria istituito *prima* che il test genetico sia disponibile — o *prima* che le persone si testino — gode di un consenso politico che potrebbe non esistere più dopo.

[BB, p. 292]

---

## Implicazioni Normative

Il confronto sistematico delle utilità porta a tre indicazioni di politica:

**1. Divieto di test o non utilizzo dei risultati:** Se l'assicurazione è volontaria e i risultati dei test possono essere usati dall'assicuratore, il rischio è l'equilibrio separante — il peggiore ex ante. Vietare i test o vietare all'assicuratore di usarli riporta al pooling, ma crea incentivi privati a fare test e nascondere i risultati.

**2. Assicurazione obbligatoria:** Implementa il pooling indipendentemente dall'informazione disponibile. È il meccanismo più robusto, ma richiede un consenso politico che potrebbe essere difficile da mantenere ex post.

**3. Informazione pubblica senza pooling obbligatorio:** Porta all'equilibrio con premi differenziati. È preferito ex post dai basso-rischio, ma peggiora la condizione ex ante di tutti rispetto al pooling.

> [!summary]
> La scelta del regime assicurativo in presenza di test genetici implica un trade-off fondamentale tra efficienza ex ante (pooling, assicurazione obbligatoria) ed efficienza ex post (premi differenziati per i basso-rischio). Le istituzioni di welfare state — sanità pubblica universale, assicurazione obbligatoria — possono essere interpretate come risposte a questo trade-off: pre-impegnano la società al pooling prima che le differenze di rischio siano note, realizzando guadagni di benessere che il mercato volontario non riuscirebbe a produrre.

[BB, p. 292]

---

## Vedi Anche

- [[11_Assicurazione_Vita_Effetto_Distruzione]] — Il modello formale dell'effetto di distruzione
- [[07_Inefficienza_e_Implicazioni]] — Le implicazioni generali della selezione avversa
- [[10_Malpractice_Medica_Selezione_Avversa]] — Un altro caso in cui le riforme producono selezione avversa

---

## Connessioni con il Vault

> [!note] Nota terminale
> Questa è la nota conclusiva della cartella 2. Si collega in modo privilegiato alla tematica dell'ottimo contrattuale e dei meccanismi di incentivo che verranno sviluppati nelle lezioni successive.

**Da `0. Intro`:**
- [[0. Intro/07_Screening|Screening]] — la tabella delle utilità qui analizzata è la struttura formale sottostante al meccanismo di screening: un menù di contratti (pooling vs separante) che induce l'auto-selezione; il Principale sceglie il contratto che massimizza la propria utilità soggetto ai vincoli di partecipazione e di incentivo compatibilità
- [[0. Intro/01_Coordinamento_e_incentivi|Coordinamento e incentivi]] — l'assicurazione obbligatoria come ottimo ex ante è l'esempio di istituzione che risolve il problema di coordinamento: tutti vogliono il pooling prima di sapere il proprio tipo, ma nessuno può impegnarsi unilateralmente a restare nel pool

**Da `1. GT`:**
- [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] — i tre regimi (pooling, separante, informazione pubblica) sono tre NE del gioco assicurativo con informazione asimmetrica; la tabella delle utilità mostra che il NE dipende criticamente dall'insieme di strategie disponibili (obbligatorietà, divieto test, ecc.)
- [[1. GT/09_Giochi_Ripetuti_Indefiniti|Giochi Ripetuti Indefiniti]] — il regime di pooling volontario può essere sostenuto come NE di un gioco ripetuto indefinitamente se e solo se i basso-rischio danno abbastanza peso al futuro ($\delta$ abbastanza alto); altrimenti, la defezione (uscita dal pool) è la strategia dominante nel gioco one-shot
