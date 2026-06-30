---
title: "I beni comuni: la tragedia dei commons e il dilemma del pescatore"
tags:
  - economia-informazione
  - beni-comuni
  - fallimento-mercato
  - teoria-dei-giochi
  - dilemma-del-prigioniero
created: 2026-06-20
related:
  - "[[01_Coordinamento_e_incentivi]]"
  - "[[02_Mercato_e_Hayek]]"
  - "[[09_Nobel]]"
  - "[[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]"
  - "[[1. GT/01_Strategia_Dominante|Strategia Dominante]]"
  - "[[1. GT/04_Giochi_Coordinamento|Giochi di Coordinamento]]"
---

# I beni comuni: la tragedia dei *commons*

Il mercato lasciato a sé non sempre coordina bene: i **fallimenti di mercato**
sono casi in cui le scelte individualmente razionali producono un esito
collettivamente inefficiente. Il caso paradigmatico è la **tragedia dei beni
comuni** (*Tragedy of the Commons*).

> [!definition] Tragedia dei beni comuni
> Quando una risorsa è **non escludibile** (non si può impedire l'accesso) ma
> **rivale** nel consumo (ciò che prendo io non resta agli altri), ogni individuo
> ha l'incentivo a sfruttarla il più possibile. La somma di questi comportamenti
> individualmente razionali porta all'**esaurimento** della risorsa.

## Il dilemma del pescatore (*Fisherman's Dilemma*)

Due (gruppi di) pescatori scelgono se pescare **sotto** (*Below*) o **sopra**
(*Above*) il limite sostenibile. La matrice dei payoff $(\text{Tu},\ \text{Gli altri})$ è:

|  | **Altri: Below** | **Altri: Above** |
|---|---|---|
| **Tu: Below** | $(10,\ 10)$ | $(0,\ 11)$ |
| **Tu: Above** | $(11,\ 0)$ | $(1,\ 1)$ |

Lettura degli esiti (dal punto di vista "Tu"):

- **Migliore** $(11)$: gli altri pescano sotto il limite, ma tu **bari** e peschi di più.
- **Secondo migliore** $(10)$: tutti pescano sotto il limite (cooperazione).
- **Piuttosto male** $(1)$: tutti pescano sopra il limite.
- **Pessimo** $(0)$: gli altri pescano sopra il limite, e tu — per qualche motivo — no.

> [!intuition] Strategia dominante e morale
> **Qualunque cosa facciano gli altri, ti conviene sempre barare** (*Above*):
> - se gli altri pescano *Below*: $11 > 10$;
> - se gli altri pescano *Above*: $1 > 0$.
>
> "Above" è quindi **strategia dominante** per entrambi. L'equilibrio è
> $(\text{Above},\ \text{Above}) = (1,1)$ (un [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]]), **Pareto-dominato** da
> $(\text{Below},\ \text{Below}) = (10,10)$.
>
> **Morale (take-home):** se non regolata, tutti barano e la risorsa comune si
> esaurisce.

Questo è formalmente un [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]]:
l'incentivo individuale è in conflitto con l'ottimo collettivo. La soluzione
richiede un intervento esterno — lo **Stato** (regolazione, sanzioni) o forme di
governance collettiva (vedi [[09_Nobel|Elinor Ostrom, Nobel 2009]]).

## Evidenza empirica

> [!example] Halibut del Nord-Pacifico
> Le slide riportano la Fig. 2 di **Stavins (2011)** sull'*halibut* del
> Nord-Pacifico: in assenza di regolazione efficace, lo stock (tonnellate) si
> riduce nel tempo — un'illustrazione empirica della tragedia dei *commons*.

## Riferimenti dai libri

> [!quote] Dal libro [C] — *A Guide to Game Theory*, §3.6 "Prisoners' dilemma and open-access resources" (p. 68)
> «[...] the free-rider effect impacts on the provision of public goods. It shows
> that if the parties who stand to gain from the provision of a public good act in
> their own self-interest the public good is unlikely to be supplied.
> **Non-excludability** and **non-rivalry** reduce the private incentives to
> contribute [...]. Ocean fisheries and the large tracts of tropical rain forest
> [...] are effect[ively open-access resources].»

- **[C]** Carmichael, cap. 3 *Prisoners' Dilemma* — §3.5 *public goods*, §3.6
  *open-access resources*, §3.8 *resolving the prisoners' dilemma*. Mostra come la
  pesca oceanica e le foreste pluviali siano risorse ad accesso aperto soggette
  alla stessa logica. → Vedi [[1. GT/06_Dilemma_Prigioniero]] e [[1. GT/01_Strategia_Dominante]]
- **[BB]** cap. 9 *Coordination problems* — fallimenti di coordinamento ed
  equilibri multipli (collegato a [[01_Coordinamento_e_incentivi]]).
- **[M]** Molho — esternalità e fallimenti di mercato.

## 🔗 Connessioni con la Teoria dei Giochi

Il dilemma del pescatore è **formalmente identico** al [[1. GT/06_Dilemma_Prigioniero|Dilemma del Prigioniero]] (cap. 3 di Carmichael): la struttura dei payoff soddisfa $c > a > d > b$, con *Above* come strategia strettamente dominante ([[1. GT/01_Strategia_Dominante|strategia dominante]]). I concetti di [[1. GT/03_Nash_Equilibrium|Nash Equilibrium]] e di [[1. GT/04_Giochi_Coordinamento|gioco di coordinamento]] permettono di formalizzare sia il fallimento cooperativo sia le condizioni per risolverlo (regolazione, ripetizione, norme). In particolare, la **governance delle risorse comuni** studiata da Elinor Ostrom ([[09_Nobel|Nobel 2009]]) può essere modellata come un [[1. GT/09_Giochi_Ripetuti_Indefiniti|gioco ripetuto indefinitamente]], in cui la minaccia di esclusione futura rende razionale il rispetto del limite sostenibile.
