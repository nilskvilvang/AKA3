--- 
title: "Anvendt kvantitativ analyse"
author: "Nils Kvilvang"
date: "08 juni, 2022"
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
   <th style="text-align:left;"> Nivå </th>
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
   <td style="text-align:left;width: 40em; "> Deler av nytt delkapittel 6. Lagt til test av normalfordeling i kap.2 </td>
  </tr>
</tbody>
</table>

