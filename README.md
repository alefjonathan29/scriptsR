
<!-- README.md gernando arquivo para o Github ler como inicial -->

# Primeiro teste com o Github

Estarei iniciando a inserir meus aquivos aqui, para ter o controle de
versões, procedimento que pode auxiliar muito no desenvolvimento de
projetos.

<img src="http://www.ppge.ufrpe.br/sites/ppge.ufrpe.br/files/styles/large/public/field/image/alef_campo.jpg?itok=fcw7whOQ" alt="The rmarkddown hex sticker" align="right" width="200" style="padding: 0 15px; float: right;"/>

Pelo visto posso inserir links diretos: <https://www.r-project.org/>

Ou mesmo inserir como link em um texto, por exemplo: [Clique
aqui](https://www.r-project.org/)

#### Inserindo marcadores.

  - Marcador inicial
      - Submarcador 1
      - Submarcacor 2

#### Inserindo código

Inserido código sem mostrar a saída.

``` r
library(tidyverse)
head(mtcars)
```

Inserindo código mostrando a saída

``` r
library(tidyverse)
```

    ## ── Attaching packages ────────────────── tidyverse 1.3.0 ──

    ## ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
    ## ✓ tibble  3.0.3     ✓ dplyr   1.0.2
    ## ✓ tidyr   1.1.2     ✓ stringr 1.4.0
    ## ✓ readr   1.3.1     ✓ forcats 0.5.0

    ## ── Conflicts ───────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
head(mtcars)
```

    ##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
    ## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
    ## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
    ## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
    ## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
    ## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
    ## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1

Inserindo código mostando e apresentando só a
    saída

    ##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
    ## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
    ## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
    ## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
    ## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
    ## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
    ## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1

Gerando gráficos

``` r
#message=FALSE, permite não mostrar a saída gerada pelo library()
library(ggplot2)
library(esquisse)

dados <- mtcars
head(dados)
```

    ##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
    ## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
    ## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
    ## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
    ## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
    ## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
    ## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1

``` r
ggplot(dados) +
 aes(x = wt, y = disp, colour = carb) +
 geom_point(size = 2.5, colour = "#2171b5") +
 geom_smooth(span = 0.75) +
 scale_color_viridis_c(option = "magma") +
 theme_bw()
```

![](README_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

#### Inseriando Imagem

<img src="https://raw.githubusercontent.com/allisonhorst/stats-illustrations/master/rstats-artwork/code_hero.jpg" width= "500" align="center">
