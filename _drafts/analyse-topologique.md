---
layout: "post"
title: "Analyse topologique"
date: "2016-03-13 22:59"
---

Nous avons mené une analyse topologique consistant à modéliser le réseau des _personnages_ de l'univers.  
Pour cela, nous avons extrait du corpus des contributions _personnages_ une large matrice carrée d'ordre 1212 (nombre de personnages) et dont chaque coefficient comptabilise le nombre de mentions d'un personnage (ligne) vers un autre (colonne).  

<div class="divencadree">
  <div style="display:inline-block; vertical-align:middle; width:30%">
    <img src="{{ site.github.url }}/img/capture_post_erickfoax.png">
    <!-- <small>Erick Foax @Laura</small> -->
  </div>
  <div style="display:inline-block; vertical-align:middle; width:5%;">
    <span style="color:grey"><i class="fa fa-arrow-right"></i></span>
  </div>
  <div style="display:inline-block; vertical-align:middle; width:20%">
    <style type="text/css">
      .tg6  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
      .tg6 td{font-size:0.5em;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#fff;}
      .tg6 th{font-size:0.5em;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#f0f0f0;}
      .tg6 .tg-s6z2{text-align:center}
      .tg6 .tg-031e{background-color:#f0f0f0;font-weight:bold}
    </style>
  <table class="tg6">
    <tr>
      <th class="tg-031e"></th>
      <th class="tg-s6z2">Erick Foax</th>
      <th class="tg-s6z2">Laura</th>
    </tr>
    <tr>
      <td class="tg-031e">Erick Foax</td>
      <td class="tg-s6z2">-</td>
      <td class="tg-s6z2">1</td>
    </tr>
    <tr>
      <td class="tg-031e">Laura</td>
      <td class="tg-s6z2">0</td>
      <td class="tg-s6z2">-</td>
    </tr>
  </table>
  </div>
  <div style="display:inline-block; vertical-align:middle; width:5%">
    <span style="color:grey"><i class="fa fa-arrow-right"></i></span>
  </div>
  <div style="display:inline-block; vertical-align:middle; width:30%">
    <img src="{{ site.github.url }}/img/graph.png">
  </div>
</div>    

Figure : _De la mention à la matrice jusqu'à la représentation en réseau_
{: .figurelegende}

Cette matrice représente l'ensemble des interactions entre personnages, c’est-à-dire des mentions (@Laura par exemple). Elle est la somme des interactions sur toute la durée de l’expérience, éclipsant la dimension temporelle offerte par le corpus (chaque contribution étant horodatée).  
Cette mise à plat nécessaire pour la modélisation générale du réseau a servi de point de départ à l'analyse statistique et à la représentation du réseau, effectuées sur le logiciel Gephi.

## Analyse Gephi
Gephi




Ce corpus consiste en une base de données SQL de plusieurs tables, dont une comprenant 21&nbsp;761 contributions produites par les auteurs dans la rubrique «&nbsp;Vos personnages&nbsp;». En réalité, ce sont 11&nbsp;280 contributions originales[^1] qui ont été produites par 398 auteurs actifs (sur 2&nbsp;633 inscrits), et racontant les histoires solitaires ou collectives de 1&nbsp;212 personnages .




[^1]: Lorsqu’une contribution mentionne un autre personnage, elle se retrouve publiée sur la page de l’auteur et du personnage mentionné, produisant en base de données deux entrées distinctes pour une seule contribution originale.
