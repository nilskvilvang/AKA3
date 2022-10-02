--- 
title: "Anvendt kvantitativ analyse"
author: "Nils Kvilvang"
date: "02 oktober, 2022"
site: bookdown::bookdown_site
bibliography: bibliografi.bib
csl: chicago-author-date.csl
---

# Introduksjon {.unnumbered}

Dette notatet gir en introduksjon til anvendt kvantitativ analyse rettet mot samfunnsvitenskapene. 

Innholdet er under utvikling og oppdateres jevnlig om enn noe uregelmessig. Tilbakemeldinger og innspill bes gitt til [Nils Kvilvang](mailto:nils.kvilvang@inn.no).

![Bilde: Gjengitt uten kreditering et stort antall steder, men i @gleitmanPsychology2011, s.28, fig. 1.8 er illustrasjonen signert Chase](Doubleblind.png){width=80%}

## Versjoner {.unnumbered}

<table class='gmisc_table' style='border-collapse: collapse; margin-top: 1em; margin-bottom: 1em;' >
<thead>
<tr><th style='border-bottom: 1px solid grey; border-top: 2px solid grey;'></th>
<th style='font-weight: 900; border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;'>Dato</th>
<th style='font-weight: 900; border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;'>Endring</th>
</tr>
</thead>
<tbody>
<tr>
<td style='text-align: left;'>1</td>
<td style='text-align: center;'>22.apr 2022</td>
<td style='text-align: center;'>Grunnversjon</td>
</tr>
<tr>
<td style='text-align: left;'>2</td>
<td style='text-align: center;'>22.apr 2022</td>
<td style='text-align: center;'>Lagt til kapittel om regresjonsanalyse</td>
</tr>
<tr>
<td style='text-align: left;'>3</td>
<td style='text-align: center;'>23.apr 2022</td>
<td style='text-align: center;'>Oppdatert kode embedding av filer. Korrektur. Endret på rekkefølge to delkapitler.</td>
</tr>
<tr>
<td style='text-align: left;'>4</td>
<td style='text-align: center;'>01.mai 2022</td>
<td style='text-align: center;'>Lagt til PCA</td>
</tr>
<tr>
<td style='text-align: left;'>5</td>
<td style='text-align: center;'>01.mai 2022</td>
<td style='text-align: center;'>Oppdatert regresjonskapittel med flere analyser av uteliggere</td>
</tr>
<tr>
<td style='text-align: left;'>6</td>
<td style='text-align: center;'>07.mai 2022</td>
<td style='text-align: center;'>Lagt til delkapittel om Exploratory Factor Analysis</td>
</tr>
<tr>
<td style='text-align: left;'>7</td>
<td style='text-align: center;'>09.mai 2022</td>
<td style='text-align: center;'>Rettet div. skrivefeil. Lagt til IV regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>8</td>
<td style='text-align: center;'>10.mai 2022</td>
<td style='text-align: center;'>Eksempel på IV regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>9</td>
<td style='text-align: center;'>12.mai 2022</td>
<td style='text-align: center;'>Endret til summarytools for beskrivende statistikk</td>
</tr>
<tr>
<td style='text-align: left;'>10</td>
<td style='text-align: center;'>16.mai 2022</td>
<td style='text-align: center;'>Oppdatert histogrammer med ggplot2</td>
</tr>
<tr>
<td style='text-align: left;'>11</td>
<td style='text-align: center;'>23.mai 2022</td>
<td style='text-align: center;'>Lagt til delkapittel om CF</td>
</tr>
<tr>
<td style='text-align: left;'>12</td>
<td style='text-align: center;'>24.mai 2022</td>
<td style='text-align: center;'>CV på multippel regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>13</td>
<td style='text-align: center;'>04.juni 2022</td>
<td style='text-align: center;'>Nytt kapittel 2 (ikke komplett</td>
</tr>
<tr>
<td style='text-align: left;'>14</td>
<td style='text-align: center;'>05.juni 2022</td>
<td style='text-align: center;'>Oppdatert kapittel 2. Lagt til CLT og Chebyshev i vedlegg. Nytt kapittel 3. Nytt kapittel 4.</td>
</tr>
<tr>
<td style='text-align: left;'>15</td>
<td style='text-align: center;'>06.juni 2022</td>
<td style='text-align: center;'>Nytt kapittel 5.</td>
</tr>
<tr>
<td style='text-align: left;'>16</td>
<td style='text-align: center;'>07.juni 2022</td>
<td style='text-align: center;'>Deler av nytt delkapittel 6.</td>
</tr>
<tr>
<td style='text-align: left;'>17</td>
<td style='text-align: center;'>08.juni 2022</td>
<td style='text-align: center;'>Lagt til test av normalfordeling i kap.2.</td>
</tr>
<tr>
<td style='text-align: left;'>18</td>
<td style='text-align: center;'>10.juni 2022</td>
<td style='text-align: center;'>Lagt til delkapittel i t-tester. Komplettert kap 6 ANOVA med nytt delkapittel.</td>
</tr>
<tr>
<td style='text-align: left;'>19</td>
<td style='text-align: center;'>12.juni 2022</td>
<td style='text-align: center;'>Komplettert kap 6 ANOVA med siste delkapittel.</td>
</tr>
<tr>
<td style='text-align: left;'>20</td>
<td style='text-align: center;'>13.juni 2022</td>
<td style='text-align: center;'>Kapittel MANOVA</td>
</tr>
<tr>
<td style='text-align: left;'>21</td>
<td style='text-align: center;'>18.juni 2022</td>
<td style='text-align: center;'>Logistisk regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>22</td>
<td style='text-align: center;'>19.juni 2022</td>
<td style='text-align: center;'>Ordinal og multinomial logistisk regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>23</td>
<td style='text-align: center;'>20.juni 2022</td>
<td style='text-align: center;'>Lett revisjon innledningskapittel. </td>
</tr>
<tr>
<td style='text-align: left;'>24</td>
<td style='text-align: center;'>02.juli 2022</td>
<td style='text-align: center;'>Mindre oppdateringer kap 1. Delvis innhold kap.12</td>
</tr>
<tr>
<td style='text-align: left;'>25</td>
<td style='text-align: center;'>05.juli 2022</td>
<td style='text-align: center;'>Kort forklaring om utregning av R^2. Endret rekkefølge kapitler. Start kap om maskinlæring.</td>
</tr>
<tr>
<td style='text-align: left;'>26</td>
<td style='text-align: center;'>06.juli 2022</td>
<td style='text-align: center;'>Polynomial regresjon lagt til</td>
</tr>
<tr>
<td style='text-align: left;'>27</td>
<td style='text-align: center;'>08.juli 2022</td>
<td style='text-align: center;'>SVR</td>
</tr>
<tr>
<td style='text-align: left;'>28</td>
<td style='text-align: center;'>09.juli 2022</td>
<td style='text-align: center;'>DTR</td>
</tr>
<tr>
<td style='text-align: left;'>29</td>
<td style='text-align: center;'>11.juli 2022</td>
<td style='text-align: center;'>Endret i regresjonsdel ML</td>
</tr>
<tr>
<td style='text-align: left;'>30</td>
<td style='text-align: center;'>19.juli 2022</td>
<td style='text-align: center;'>Lagt til i ML. Ryddet opp i kap 2, 3, 4, 5, 6 og 7. Lagt til nytt stoff i kap.4</td>
</tr>
<tr>
<td style='text-align: left;'>31</td>
<td style='text-align: center;'>23.juli 2022</td>
<td style='text-align: center;'>Lagt til i og redigert kap.9. Redigert kap 10, 11 og 12.</td>
</tr>
<tr>
<td style='text-align: left;'>32</td>
<td style='text-align: center;'>24.juli 2022</td>
<td style='text-align: center;'>Redigert kap 13. Redigert kap 14</td>
</tr>
<tr>
<td style='text-align: left;'>33</td>
<td style='text-align: center;'>26.juli 2022</td>
<td style='text-align: center;'>Lagt til og redigert kap 15</td>
</tr>
<tr>
<td style='text-align: left;'>34</td>
<td style='text-align: center;'>24.aug 2022</td>
<td style='text-align: center;'>Redigert kap 3, Ridge regresjon</td>
</tr>
<tr>
<td style='text-align: left;'>35</td>
<td style='text-align: center;'>27.aug 2022</td>
<td style='text-align: center;'>Lagt til nytt kap 11</td>
</tr>
<tr>
<td style='text-align: left;'>36</td>
<td style='text-align: center;'>29.aug 2022</td>
<td style='text-align: center;'>Noe korrekturlesing</td>
</tr>
<tr>
<td style='text-align: left;'>37</td>
<td style='text-align: center;'>31.aug 2022</td>
<td style='text-align: center;'>Utfylling kap 16</td>
</tr>
<tr>
<td style='text-align: left;'>38</td>
<td style='text-align: center;'>03.sep 2022</td>
<td style='text-align: center;'>Lagt til eksempel logistisk regresjon kap 16</td>
</tr>
<tr>
<td style='text-align: left;'>39</td>
<td style='text-align: center;'>04.sep 2022</td>
<td style='text-align: center;'>K-NN i kap 16</td>
</tr>
<tr>
<td style='text-align: left;'>40</td>
<td style='text-align: center;'>12.sep 2022</td>
<td style='text-align: center;'>SVM i kap 16</td>
</tr>
<tr>
<td style='text-align: left;'>41</td>
<td style='text-align: center;'>27.sep 2022</td>
<td style='text-align: center;'>Kernel SVM i kap 16</td>
</tr>
<tr>
<td style='text-align: left;'>42</td>
<td style='text-align: center;'>30.sep 2022</td>
<td style='text-align: center;'>Decision Tree, Random Forest og Naiv Bayes klassifisering</td>
</tr>
<tr>
<td style='border-bottom: 2px solid grey; text-align: left;'>43</td>
<td style='border-bottom: 2px solid grey; text-align: center;'>02.okt 2022</td>
<td style='border-bottom: 2px solid grey; text-align: center;'>Eksempel type I og II feil</td>
</tr>
</tbody>
</table>

