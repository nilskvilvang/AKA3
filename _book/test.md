---
title: "Untitled"
output: html_document
date: '2022-07-13'
---


```r
pacman::p_load(tidyverse, caret, readxl, equatiomatic)
```


```r
Ames4_trening2 <- read_xlsx("Ames4_trening.xlsx")
Ames4_test2 <- read_xlsx("Ames4_test.xlsx")
```


I kapittelet om regresjonsanalyse brukte vi R-funksjonen "lm" for lineære modeller. Det kan vi også bruke her, men vi velger å bruket pakken "caret" fordi den inneholder en rekke modeller for maskinlæring og funksjoner som er hendige i ulike teknikker i maskinlæring.


```r
trn_kontrl <- trainControl(method = "none")
enkelregr <- train(SalePrice ~ Gr.Liv.Area, data = Ames4_trening2, method = "glm", trControl = trn_kontrl)
```

Caret, gjennom funksjonen train(), gir oss en modell med følgende informasjon:


```r
names(enkelregr$finalModel)
#>  [1] "coefficients"      "residuals"        
#>  [3] "fitted.values"     "effects"          
#>  [5] "R"                 "rank"             
#>  [7] "qr"                "family"           
#>  [9] "linear.predictors" "deviance"         
#> [11] "aic"               "null.deviance"    
#> [13] "iter"              "weights"          
#> [15] "prior.weights"     "df.residual"      
#> [17] "df.null"           "y"                
#> [19] "converged"         "boundary"         
#> [21] "model"             "formula"          
#> [23] "terms"             "data"             
#> [25] "offset"            "control"          
#> [27] "method"            "contrasts"        
#> [29] "xlevels"           "xNames"           
#> [31] "problemType"       "tuneValue"        
#> [33] "obsLevels"         "param"
```

Vi kan aksessere detaljer for alle disse gjennom f.eks.


```r
coef(enkelregr$finalModel)
#> (Intercept) Gr.Liv.Area 
#>  55322.5073     73.7485
```

Regresjonslikningen for vår modell blir da:


```r
enkelregr2 <- lm(SalePrice ~ Gr.Liv.Area, data = Ames4_trening2)
extract_eq(enkelregr2)
```

$$
\operatorname{SalePrice} = \alpha + \beta_{1}(\operatorname{Gr.Liv.Area}) + \epsilon
$$

