---
tags: [economia-informazione, segnalazione, screening, timing]
aliases: [Signalling vs Screening, Chi muove per primo]
links: [02_Educazione_come_Segnale_Credibile, 03_Modello_di_Spence, 07_Equilibrio_Aggregante_Pooling]
---

# Segnalazione vs Screening: Chi Muove per Primo

## Il Problema Comune e le Due Soluzioni Speculari

> [!definition]
> **Segnalazione** e **screening** sono due meccanismi che affrontano la stessa situazione — informazione nascosta *ex ante*, come nei mercati con [[2. Selezione Avversa/01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste|selezione avversa]] — ma differiscono per **chi inizia la sequenza di mosse**:
> - **Segnalazione (signalling):** la parte *informata* muove per prima, scegliendo un'azione osservabile e credibile (un *segnale*); la parte non informata risponde.
> - **Screening:** la parte *non informata* muove per prima, offrendo un *menù di contratti*; la parte informata risponde scegliendo l'opzione preferita (autoselezione).

In entrambi i casi l'obiettivo è "tradurre" un'informazione privata in qualcosa di osservabile, così da ristabilire scambi efficienti che la pura selezione avversa impedirebbe.

> [BB, p. 305] Le ricerche di Spence e Stiglitz hanno mostrato che l'informazione privata può essere trasmessa in modo credibile tra le parti: una parte non informata può separare le parti informate tramite *screening*, mentre una parte informata può rivelare credibilmente la propria informazione tramite *signalling*.

---

## Il Timing della Segnalazione

Nella segnalazione la sequenza temporale è (slide 4):

$$
t=0:\ \text{Natura sceglie il tipo } (H/L) \;\to\; t=1:\ \text{l'agente invia un segnale} \;\to\; t=2:\ \text{il principale offre un contratto} \;\to\; t=3:\ \text{l'agente accetta o rifiuta}
$$

Il punto cruciale è che **l'agente informato agisce prima** che il principale formuli l'offerta. Il segnale (ad es. il livello di istruzione) è già "sul tavolo" quando il datore di lavoro decide il salario.

> [!intuition]
> Si pensi a un candidato che si presenta con una laurea *prima* del colloquio. La laurea è il segnale, scelto e "pagato" dal candidato in anticipo; il datore di lavoro la osserva e su quella base forma le proprie aspettative e propone uno stipendio. L'iniziativa parte da chi sa.

---

## Il Timing dello Screening

Nello screening l'ordine si **inverte** (slide 5):

$$
t=0:\ \text{Natura sceglie il tipo } (H/L) \;\to\; t=1:\ \text{il principale offre un menù di contratti} \;\to\; t=2:\ \text{l'agente accetta o rifiuta} \;\to\; t=3:\ \text{l'agente invia un segnale verificabile}
$$

Qui è la parte non informata a costruire i contratti in modo che ciascun tipo, scegliendo razionalmente, **si tradisca** rivelando il proprio tipo (vincoli di autoselezione / *incentive compatibility*). È il meccanismo del modello Cabernet–Merlot di Birchler & Bütler e dei contratti assicurativi separatori.

> [BB, p. 337] In un gioco di segnalazione la parte informata muove per prima, a differenza del gioco di screening usato nel testo principale. La segnalazione è un'attività che è meno costosa per chi offre un prodotto di alta qualità rispetto a chi ne offre uno di bassa qualità.

---

## Perché la Segnalazione è "Più Complicata" dello Screening

> [!intuition]
> Nello screening, è il progettista del menù (la parte informata sulle proprie intenzioni, ignorante sul tipo altrui) a controllare le regole del gioco. Nella segnalazione, invece, il payoff che la parte informata può aspettarsi **dipende dalle credenze (*beliefs*) che la parte non informata si formerà dopo aver osservato il segnale**. Queste credenze non sono date una volta per tutte: vanno determinate *in equilibrio*, e devono risultare confermate. È per questo che la segnalazione produce facilmente **molteplici equilibri** (separatori e aggreganti) — vedi [[05_Equilibrio_Separatore]] e [[07_Equilibrio_Aggregante_Pooling]].

> [BB, p. 337] La segnalazione è considerevolmente più delicata dello screening, perché il payoff che una parte segnalante può attendersi dipende dalle credenze che la parte non informata mantiene dopo aver osservato l'attività di segnalazione.

---

## Cosa Può Servire da Segnale

Qualunque azione osservabile e differenzialmente costosa può fungere da segnale:

- **Istruzione** (il caso canonico di Spence) → [[02_Educazione_come_Segnale_Credibile]]
- **Garanzie** sul prodotto (chi vende cattiva qualità non può permettersi garanzie generose)
- **Marchi / brand names**, il cui valore sarebbe distrutto vendendo qualità scadente
- **Pubblicità** costosa, **prezzi predatori**, **consumo cospicuo** → [[09_Applicazioni_Teoria_del_Segnale]]

> [BB, p. 337] Garanzie, marchi (il cui valore sarebbe danneggiato dalla vendita di cattiva qualità), istruzione: tutti questi possono servire da segnali.

---

## Take-home message

> [!summary]
> Segnalazione e screening risolvono lo stesso problema di asimmetria informativa ex ante, ma con sequenze di mosse opposte: nella **segnalazione muove per prima la parte informata** (sceglie un segnale costoso), nello **screening muove per prima la parte non informata** (propone un menù di contratti per l'autoselezione). La segnalazione è analiticamente più scivolosa perché il rendimento del segnale dipende dalle credenze che il ricevente formerà — credenze che vanno determinate e confermate in equilibrio. Questa dipendenza dalle aspettative è all'origine della molteplicità di equilibri (separatori e aggreganti) che caratterizza i modelli di segnalazione.

---

## Vedi anche

- [[02_Educazione_come_Segnale_Credibile]] — Perché un segnale è credibile: la proprietà di single-crossing
- [[03_Modello_di_Spence]] — La formalizzazione del processo di segnalazione
- [[07_Equilibrio_Aggregante_Pooling]] — Quando il segnale *non* riesce a separare i tipi
- [[2. Selezione Avversa/12_Confronto_Utilita_Equilibri_Assicurativi]] — Lo screening assicurativo come meccanismo speculare

---

## Connessioni con il Vault

**Da `0. Intro`:**
- [[0. Intro/06_Segnalazione|Segnalazione]] e [[0. Intro/07_Screening|Screening]] — le due note panoramiche introduttive si espandono qui nel modello formale

**Da `1. GT`:**
- [[1. GT/07_Giochi_Dinamici_Sequenziali|Giochi Sequenziali]] — entrambi i meccanismi sono giochi in forma estesa con informazione incompleta; cambia solo l'ordine delle mosse e quindi la struttura dell'albero

**Da `2. Selezione Avversa`:**
- [[2. Selezione Avversa/01_Informazione_Asimmetrica_e_Caratteristiche_Nascoste|Info Asimmetrica]] — la stessa struttura *ex-ante hidden information* che genera selezione avversa
- [[2. Selezione Avversa/07_Inefficienza_e_Implicazioni|Inefficienza e Rimedi]] — segnalazione e screening sono i rimedi decentralizzati lì elencati
