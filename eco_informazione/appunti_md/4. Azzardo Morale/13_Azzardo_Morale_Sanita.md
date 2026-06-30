---
tags: [economia-informazione, azzardo-morale, selezione-avversa, sanità, assicurazione, equità]
aliases: [Sanità e Informazione, Health Care Moral Hazard, AS in Sanità]
links: [01_Definizione_e_Timing, 09_Beni_di_Credenza, 11_Copertura_Assicurativa_Kerschbamer, 14_RAND_Esperimento_Assicurativo, 2. Selezione Avversa/05_Equilibrio_di_Mercato_Adverse_Selection]
---

# Azzardo Morale e Selezione Avversa nel Mercato Sanitario

## Il mercato sanitario come caso paradigmatico

Il mercato delle cure mediche è l'applicazione più importante e politicamente rilevante di tutti i problemi di informazione asimmetrica studiati nel corso. Qui convivono, in forma acuta, tre tipi distinti di asimmetria informativa:

> [!definition]
> **Selezione avversa in sanità**: l'impresa assicurativa conosce la distribuzione del rischio sanitario nella popolazione, ma non il rischio individuale del singolo assicurato, che conosce meglio la propria salute. Gli individui ad alto rischio tendono ad acquistare copertura più ampia, mentre quelli sani rinunciano a polizze costose.
>
> **Azzardo morale del consumatore (*consumer moral hazard*)**: una volta assicurato, l'individuo può modificare il proprio comportamento in modi non osservabili dall'assicuratore, sia riducendo gli investimenti preventivi (*ex ante*) sia aumentando il consumo di cure (*ex post*).
>
> **Azzardo morale del produttore (*supplier/producer moral hazard*)**: il medico o la struttura sanitaria non sopporta direttamente il costo dei trattamenti prescritti, il che può indurre sovra-prescrizione o sopravvalutazione del bisogno del paziente.

## La struttura dell'asimmetria informativa

In sanità, la relazione informativa è **tripartita**:

$$\text{Assicuratore} \xleftarrow{\text{premi}} \text{Paziente (Principale)} \xrightarrow{\text{delega diagnosi}} \text{Medico (Agente)}$$

- L'**assicuratore** non conosce né il tipo di rischio del paziente (SA) né le sue azioni (AM del consumatore).
- Il **medico** ha informazione superiore sulle condizioni del paziente, ma non sopporta il costo delle cure (AM del produttore).
- Il **paziente** è nel mezzo: conosce il proprio tipo meglio dell'assicuratore, ma sa meno del medico sulle cure appropriate.

La sanità è quindi, simultaneamente, un mercato di [[09_Beni_di_Credenza|credence goods]] (tra paziente e medico) e un mercato assicurativo con SA e AM (tra paziente e assicuratore).

## Perché l'accesso alla sanità è importante

Il mercato sanitario differisce da altri mercati non solo per le asimmetrie informative, ma per ragioni etiche e distributive fondamentali:

**La correlazione tra salute e povertà**: le persone più povere tendono ad essere malate più frequentemente e più gravemente. Hanno speranze di vita più basse e livelli di salute inferiori. Questa correlazione è documentata sia *all'interno* dei paesi (disuguaglianze geografiche interne) sia *tra* paesi (correlazione PIL-aspettativa di vita).

> [!example]
> **L'esempio del tram di Torino**: su una linea tranviaria che attraversa Torino dalla collina dei quartieri benestanti al quartiere operaio di Vallette, i passeggeri che salgono perdono circa mezzo anno di aspettativa di vita per ogni chilometro percorso verso ovest. Tra la collina e Vallette, la differenza è di oltre 4 anni di vita.

**La causalità doppia**: la relazione tra povertà e salute non è unidirezionale. La povertà peggiora la salute (accesso limitato a cure, nutrizione, condizioni abitative) ma anche la cattiva salute causa e aggrava la povertà (perdita di produttività, costi di cura, incapacità di lavorare). Intervenire sulla salute ha quindi effetti redistributivi che vanno oltre il benessere immediato.

**L'esternalità umanitaria**: le preferenze della società sembrano incorporare una preoccupazione per le diseguaglianze in salute più forte di quella per le diseguaglianze di reddito. L'evidenza mostra che anche i cittadini che normalmente si oppongono alla redistribuzione del reddito sono favorevoli alla sanità universale. Questo giustifica un ruolo del governo nel mercato sanitario.

## Selezione avversa e il problema della copertura

Se le compagnie assicurative usano il **community rating** (stessa tariffa per tutti), si innesca la selezione avversa:

- Solo chi ha rischio medio o superiore alla media compra la polizza.
- Le persone sane abbandonano il mercato → il premio sale.
- Il ciclo si ripete → *spirale verso il basso* (*death spiral*).

Se invece usano il **risk rating** individuale:

$$p_i = \text{rischio}_i \times \text{costo atteso}$$

i premi diventano proibitivi proprio per i più malati — ovvero per chi ne ha più bisogno. Negli USA, prima della riforma sanitaria del 2010, oltre il 20% della popolazione non aveva copertura assicurativa.

## Le due forme di azzardo morale del consumatore

> [!definition]
> **Azzardo morale ex ante** (Ehrlich e Becker 1972): prima di ammalarsi, l'individuo assicurato investe *meno* nella propria salute rispetto a un individuo non assicurato. Fuma di più, si esercita di meno, mangia male — perché le conseguenze finanziarie della malattia sono assorbite dall'assicurazione. Il rischio è *endogeno*: le azioni dell'individuo influenzano la probabilità di ammalarsi.
>
> **Azzardo morale ex post** (Pauly 1968): una volta ammalatoasi, l'individuo assicurato consuma *più* cure mediche di quanto farebbe se le pagasse di tasca propria. Il prezzo percepito del servizio sanitario è inferiore al costo reale, quindi la domanda aumenta.

**Qual è l'azione nascosta?**

Nel moral hazard ex post, l'azione nascosta può essere interpretata in modi diversi (Cutler e Zeckhauser 2000): il paziente o il medico non si impegnano a cercare il fornitore più efficiente, semplicemente perché l'assicurazione azzera l'incentivo a risparmiare. Il problema può essere riformulato come un problema di tipo nascosto (*hidden type*) — non ogni individuo assicurato reagisce allo stesso modo all'assicurazione.

## L'obiezione di Gladwell: il moral hazard esiste davvero?

Un punto di vista critico è stato espresso da Malcolm Gladwell in un articolo del New Yorker (2005):

> *"Il moral hazard ha senso... solo se consumiamo l'assistenza sanitaria come consumiamo altri beni di consumo. Andiamo dal medico a malincuore, solo perché siamo malati. Il moral hazard è esagerato. La domanda di assistenza sanitaria è illimitata? Non è vero... Le persone amano davvero andare dal medico? Si ricoverano in ospedale invece di giocare a golf?"*

L'argomento di Gladwell è che la domanda di cure mediche è fondamentalmente diversa dalla domanda di beni ordinari: le persone non consumano cure per piacere. Se questo è vero, la riduzione del costo marginale tramite l'assicurazione avrebbe scarso effetto sulla domanda.

La risposta a questa obiezione è empirica: l'unico modo per sapere se il moral hazard esiste e quanto è grande è misurarlo.

## Assicurazione sociale come soluzione

La risposta istituzionale ai problemi di SA e AM in sanità è l'**assicurazione sociale obbligatoria**:

- **Pool obbligatorio dei rischi**: lo Stato assicura l'"inassicurabile" tramite copertura universale obbligatoria.
- **Eliminazione della spirale avversa**: con adesione obbligatoria, il pool include sia i sani sia i malati.
- **Lo Stato come terza parte**: il governo entra nella relazione paziente-medico come finanziatore, il che crea il problema del moral hazard del produttore su scala sistemica.

La [[14_RAND_Esperimento_Assicurativo|risposta empirica definitiva]] alla domanda se il moral hazard esiste arriva dall'esperimento randomizzato RAND.

> [!summary]
> Il mercato sanitario è l'arena principale in cui si incontrano selezione avversa, azzardo morale ex ante ed ex post, e azzardo morale del produttore (second-degree moral hazard). La SA in un sistema a premi di mercato porta a copertura insufficiente e premi proibitivi per i più fragili. La risposta istituzionale — assicurazione sociale obbligatoria — risolve la SA ma crea nuove forme di AM sistemico. La questione se e quanto il moral hazard del consumatore sia empiricamente rilevante è risolta da esperimenti randomizzati come il RAND HIE.
