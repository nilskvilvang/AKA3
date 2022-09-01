--- 
title: "Anvendt kvantitativ analyse"
author: "Nils Kvilvang"
date: "01 september, 2022"
site: bookdown::bookdown_site
bibliography: bibliografi.bib
csl: chicago-author-date.csl
---

# Introduksjon {.unnumbered}

Dette notatet gir en introduksjon til anvendt kvantitativ analyse rettet mot samfunnsvitenskapene. 

Innholdet er under utvikling og oppdateres jevnlig om enn noe uregelmessig. Tilbakemeldinger og innspill bes gitt til [Nils Kvilvang](mailto:nils.kvilvang@inn.no).

![Bilde: Gjengitt uten kreditering et stort antall steder, men i @gleitmanPsychology2011, s.28, fig. 1.8 er illustrasjonen signert Chase](Doubleblind.png){width=80%}

## Versjoner {.unnumbered}

<table class=" lightable-classic" style="font-size: 12px; font-family: Cambria; width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
  <tr>
   <th style="text-align:left;"> Dato </th>
   <th style="text-align:left;"> Endring </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;width: 8em; "> 22.apr 2022 </td>
   <td style="text-align:left;width: 40em; "> Grunnversjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 22.apr 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til kapittel om regresjonsanalyse </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 23.apr 2022 </td>
   <td style="text-align:left;width: 40em; "> Oppdatert kode embedding av filer. Korrektur. Endret på rekkefølge to delkapitler. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 01.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til PCA </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 01.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Oppdatert regresjonskapittel med flere analyser av uteliggere </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 07.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til delkapittel om Exploratory Factor Analysis </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 09.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Rettet div. skrivefeil. Lagt til IV regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 10.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Eksempel på IV regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 12.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Endret til summarytools for beskrivende statistikk </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 16.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Oppdatert histogrammer med ggplot2 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 23.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til delkapittel om CF </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 24.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> CV på multippel regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 04.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Nytt kapittel 2 (ikke komplett </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 05.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Oppdatert kapittel 2. Lagt til CLT og Chebyshev i vedlegg. Nytt kapittel 3. Nytt kapittel 4. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 06.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Nytt kapittel 5. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 07.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Deler av nytt delkapittel 6. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 08.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til test av normalfordeling i kap.2. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 10.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til delkapittel i t-tester. Komplettert kap 6 ANOVA med nytt delkapittel. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 12.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Komplettert kap 6 ANOVA med siste delkapittel. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 13.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Kapittel MANOVA </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 18.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Logistisk regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 19.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Ordinal og multinomial logistisk regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 20.juni 2022 </td>
   <td style="text-align:left;width: 40em; "> Lett revisjon innledningskapittel. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 02.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Mindre oppdateringer kap 1. Delvis innhold kap.12 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 05.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Kort forklaring om utregning av R^2. Endret rekkefølge kapitler. Start kap om maskinlæring. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 06.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Polynomial regresjon lagt til </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 08.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> SVR </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 09.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> DTR </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 11.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Endret i regresjonsdel ML </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 19.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til i ML. Ryddet opp i kap 2, 3, 4, 5, 6 og 7. Lagt til nytt stoff i kap.4 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 23.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til i og redigert kap.9. Redigert kap 10, 11 og 12. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 24.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Redigert kap 13. Redigert kap 14 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 26.juli 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til og redigert kap 15 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 24.aug 2022 </td>
   <td style="text-align:left;width: 40em; "> Redigert kap 3, Ridge regresjon </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 27.aug 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til nytt kap 11 </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 29.aug 2022 </td>
   <td style="text-align:left;width: 40em; "> Noe korrekturlesing </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 31.aug 2022 </td>
   <td style="text-align:left;width: 40em; "> Utfylling kap 16 </td>
  </tr>
</tbody>
</table>

