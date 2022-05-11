--- 
title: "Anvendt kvantitativ analyse"
author: ""
date: "Siste endring 11 mai, 2022"
site: bookdown::bookdown_site
bibliography: bibliografi.bib
csl: chicago-author-date.csl
---


```{=html}
<input onclick="codefolder(&#39;pre.sourceCode&#39;);" type="button" value="Hide Code" id="codefolder-button" style="position: absolute; right: 8%; z-index: 200"/>
<script>
  function codefolder(query) {

    var x = document.querySelectorAll(query);
    if (x.length === 0) return;

    function toggle_vis(o) {
      var d = o.style.display;
      o.style.display = (d === 'block' || d === '') ? 'none':'block';
    }

    for (i = 0; i < x.length; i++) {
      var y = x[i];
      toggle_vis(y);
    }

    var elem = document.getElementById("codefolder-button");
    if (elem.value === "Hide Code") elem.value = "Show Code";
    else elem.value = "Hide Code";
  }
</script>
<script>
  window.addEventListener('load', function () {
    codefolder('pre.sourceCode');
  });
</script>
```

# Introduksjon {.unnumbered}

Dette notatet gir en introduksjon til anvendt kvantitativ analyse rettet mot samfunnsvitenskapene. 

Innholdet er under utvikling og oppdateres jevnlig om enn noe uregelmessig. Tilbakemeldinger og innspill bes gitt til [Nils Kvilvang](mailto:nils.kvilvang@inn.no).

![Bilde: Ukjent opphav](Doubleblind.png)

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
   <td style="text-align:left;width: 40em; "> Lagt til PCA. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 01.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Oppdatert regresjonskapittel med flere analyser av uteliggere. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 07.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Lagt til delkapittel om Exploratory Factor Analysis </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 09.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Rettet div. skrivefeil. Lagt til IV regresjon. </td>
  </tr>
  <tr>
   <td style="text-align:left;width: 8em; "> 10.mai 2022 </td>
   <td style="text-align:left;width: 40em; "> Eksempel på IV regresjon </td>
  </tr>
</tbody>
</table>

