---
lang: ca
title: Mètriques de codi obert
description: Preneu decisions informades per a ajudar el vostre projecte de codi obert a millorar, mesurant i fent seguiment del seu èxit.
class: metrics
order: 9
image: /assets/images/cards/metrics.png
related:
  - finding
  - best-practices
---

## Per què mesurar res?

Les dades, quan s'utilitzen amb seny, us poden ajudar a prendre millors decisions com a gestor de codi obert.

Amb més informació, podeu:

* Entendre com responen els usuaris a noves funcions
* Esbrinar d'on venen els usuaris nous
* Identificar, i decidir si doneu suport a, un cas o funcionalitat atípic
* Quantificar la popularitat del projecte
* Entendre com s'utilitza el projecte
* Aconseguir diners amb patrocinadors i beques

Per exemple, [ a Homebrew](https://github.com/Homebrew/brew/blob/bbed7246bc5c5b7acb8c1d427d10b43e090dfd39/docs/Analytics.md) troben que el Google Analytics els ajuda a prioritzar la feina:

> El Homebrew s'ofereix debades i gestionat completament per voluntaris en el seu temps lliure. Com a resultat, no tenim els recursos per a fer estudis detallats dels usuaris del Homebrew per a decidir la millor manera de dissenyar futures funcionalitats i prioritzar la feina actual. Els agregats d'analítiques anònimes d'usuaris ens permeten prioritzar la correcció d'errors i funcionalitats basant-nos en com, on i quan utilitza la gent el Homebrew.

La popularitat no ho és tot. Tothom entra al món del codi obert per raons diferents. Si el vostre objectiu com a gestor de codi obert és presumir de la vostra feina, sigueu transparent amb el vostre codi, o simplement passeu-ho bé: les mètriques potser no us importen tant.

Si _esteu_ interessat a entendre el vostre projecte a un nivell més profund, informeu-vos de com analitzar l'activitat del vostre projecte.

## Descobriment

Abans que ningú pugui utilitzar o contribuir al vostre projecte, cal que sàpiguen que existeix. Pregunteu-vos: _la gent troba aquest projecte?_

![Traffic graph](/assets/images/metrics/repo_traffic_graphs_tooltip.png)

Si teniu el projecte hostatjat al GitHub, [podeu veure](https://help.github.com/articles/about-repository-graphs/#traffic) quanta gent arriba al vostre projecte i des d'on venen. A la pàgina del projecte, feu clic a «Insights», i després a «Traffic». En aquesta pàgina, podreu veure:

* **Visualitzacions totals de la pàgina:** Us mostra quantes vegades s'ha visualitzat el projecte

* **Visitants únics totals:** Us mostra quanta gent ha visualitzat el projecte

* **Llocs de procedència:** Us mostra d'on venen els visitants. Aquesta mètrica us pot ajudar a entendre on contactar amb la vostra audiència i si els esforços de promoció estan funcionant o no.

* **Contingut popular:** Us mostra on van els visitants dins el projecte, detallat per visualitzacions de pàgina i visitants únics.

[Les estreles del GitHub](https://help.github.com/articles/about-stars/) també us poden servir de base per a mesurar la popularitat. Tot i que les estreles del GitHub no necessàriament es correlacionen amb les baixades i l'ús, us poden mostrar quanta gent s'assabenta del vostre treball.

Potser també us interessaria [rastrejar la descobribilitat en llocs específics](https://opensource.com/business/16/6/pirate-metrics): per exemple, al Google PageRank, el tràfic de referència del lloc web del projecte, o referències d'altres projectes o llocs web de codi obert.

## Ús

La gent troba el vostre projecte en aquesta cosa tan salvatge i embogida que diem «internet». Idealment, quan veuen el projecte, senten la necessitat de fer alguna cosa. La segona pregunta que voleu fer és: _fa servir la gent aquest projecte?_

Si utilitzeu un gestor de paquets, com ara npm o RubyGems.org, per a distribuir el projecte, podríeu rastrejar les seves baixades.

Cada gestor de paquets podria utilitzar definicions lleugerament diferents de «baixada», i les baixades no es correlacionen necessàriament amb les instal·lacions o l'ús, però aporta una base per a fer comparacions. Proveu de fer servir [Libraries.io](https://libraries.io/) per a rastrejar les estadístiques d'ús entre els gestors de paquets més populars.

Si el vostre projecte és al GitHub, torneu a la pàgina «Traffic». Podeu utilitzar el [gràfic de clonatge](https://github.com/blog/1873-clone-graphs) per a veure quantes vegades s'ha clonat el projecte en un dia en concret, detallat per clons totals i clonadors únics.

![Clone graph](/assets/images/metrics/clone_graph.png)

Si l'ús és baix comparat amb el nombre total de persones que han descobert el projecte, hi ha dos problemes a considerar. Podria ser que:

* El projecte no atrau satisfactòriament la vostra audiència, o
* Esteu atraient l'audiència equivocada

Per exemple, si el projecte acaba a la portada del Hacker News, probablement veureu un repunt als descobriments (trànsit), però una ràtio de conversió baixa, perquè heu arribat a tothom amb Hacker News. Per contra, si el vostre projecte Ruby es presenta a una conferència de Ruby, és més probable que veieu una ràtio de conversió alta des d'una audiència objectiu.

Proveu d'entendre d'on prové la vostra audiència i demaneu comentaris externs a la pàgina del projecte per a entendre quin dels dos problemes és el que patiu.

Una vegada sapigueu que la gent fa servir el vostre projecte, podríeu voler provar d'entendre què fan amb ell. L'estan fent servir fent projectes paral·lels basats en el vostre codi, afegint-hi funcionalitats? L'estan fent servir per a fins científics o empresarials?

## Retenció

La gent troba el vostre projecte i el fa servir. La pregunta següent que voleu fer és: _està la gent contribuint al projecte?_

Mai és tard per a començar a pensar en els col·laboradors. Sense la gent que s'hi involucra, us arrisqueu a quedar en una situació malsana on el projecte és _popular_ (el fa servir molta gent) però no _recolzat_ (no té prou temps de manteniment per a assolir la demanda).

La retenció també requereix un [influx de col·laboradors nous](http://blog.abigailcabunoc.com/increasing-developer-engagement-at-mozilla-science-learning-advocacy#contributor-pathways_2), ja que els que abans hi eren actius acabaran anant a altres coses.

Alguns exemples de mètriques de la comunitat que podríeu voler rastrejar regularment:

* **Recompte de col·laboradors totals i nombre d'aportacions per col·laborador:** Us mostra quants col·laboradors teniu, i quins són més o menys actius. Al GitHub, podeu veure-ho a «Insights» -> «Contributors». A hores d'ara, aquest gràfic només compta els col·laboradors que han aportat a la branca predefinida del repositori.

![Contributor graph](/assets/images/metrics/repo_contributors_specific_graph.png)

* **Col·laboradors nouvinguts, casuals i habituals:** Us ajuda a rastrejar si esteu obtenint col·laboradors nous, i si hi tornen. (Els col·laboradors casuals són aqueslls amb un nombre d'aportacions baix. És decisió vostra si això vol dir una aportació, menys de 5 o una altra cosa). Sense col·laboradors nous, la comunitat del projecte es pot estancar.

* **Nombre de problemes (*issues*) i peticions d'integració (*pull request*) pendents:** Si aquests nombres són molt alts, podríeu necessitar ajuda fent triatge de problemes i revisió de codi.

* **Nombre de problemes i peticions d'integració _creats_:** Que hi hagi problemes creats significa que algú es preocupa prou pel vostre projecte com per a obrir-ne. Si aquest nombre augmenta en el temps, suggereix que la gent s'interessa pel projecte.

* **Tipus de contribucions:** Per exemple, aportacions, correcció d'errors o faltes d'ortografia, o comentaris en un problema.

<aside markdown="1" class="pquote">
<img src="https://avatars.githubusercontent.com/arfon?s=180" class="pquote-avatar" alt="avatar" /> El codi obert és més que només codi. Els projectes de codi obert exitosos inclouen contribucions al codi i a la documentació, a més de converses sobre aquests canvis.

<p markdown="1" class="pquote-credit">
  — @arfon, ["The Shape of Open Source"](https://github.com/blog/2195-the-shape-of-open-source)
</p></aside>

## Activitat dels mantenidors

Finalment, voldreu tancar el bucle assegurant-vos que els mantenidors del projecte són capaços de gestionar el volum de contribucions rebut. L'última pregunta que voleu fer és: _esic (o estem) reaccionant davant la comunitat?_

Els mantenidors que no reaccionen es converteixen en un coll d'ampolla per als projectes de codi obert. Si algú envia una contribució, però mai no rep resposta d'un mantenidor, podria sentir-se desalenat i marxar.

[Estudis de Mozilla](https://docs.google.com/presentation/d/1hsJLv1ieSqtXBzd5YZusY-mB8e1VJzaeOmh8Q4VeMio/edit#slide=id.g43d857af8_0177) suggereixen que la capacitat de reacció dels mantenidors és un factor crític per a encoratjar les contribucions recursives.

Considereu rastrejar quant trigueu (qualsevol dels mantenidors) en reaccionar a les contribucions, sigui a un problema o a una petició d'integració. Reaccionar no vol dir realitzar una acció. Pot ser tan simple com dir: _«Gràcies per l'enviament! Ho revisaré la setmana pròxima.»_

També podríeu mesurar el temps que us cal per a moure-us entre nivells al procés de contribució, com ara:

* Temps mitjà que un problema queda pendent
* Si els problemes es tanquen per peticions d'integració
* Si els problemes obsolets es tanquen
* Temps mitjà per a integrar una petició d'integració

## Feu servir 📊 per a aprendre sobre la gent

Comprendre les mètriques us ajudarà a construir un projecte de codi obert actiu i brollant. Tot i si no rastregeu totes les mètriques del tauler, utilitzeu el marc de treball anterior per a focalitzar la vostra atenció en el tipus de comportament que ajudarà el projecte a reeixir.

[CHAOSS](https://chaoss.community/) és una comunitat de codi obert acollidora centrada en analítiques, mètriques i programari per a la salut de les comunitats.
