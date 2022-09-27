# DolarBlue_vs_DolarOficial
______-

## API BCRA
Enlace de la página: https://estadisticasbcra.com/  
Documentación: https://estadisticasbcra.com/api/documentacion

Informe sobre dólar en Argentina para un grupo financiero. Tener en cuenta que la gerencia le puede llegar a requerir nuevas consultas.

Importar librerías  
Automatizar código  
Token BCRA  
Endpoints: se pueden utilizar los que se consideren necesarios  
Autorización y requests  
Función para convertir Json a Dataframe  
Limpieza de datos  
___________
* Últimos 365 días:
* 1) Día con mayor variación en la brecha, respecto al día anterior:

    | Fecha               |   Variación |
    |:--------------------|--------------------------:|
    | 2022-07-22  |                   160.48 |.

    ![variación](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico01.png)

* 2) Top 5 días con mayor volatilidad:

    |Fecha      |    Volatilidad|
    |:----------|----------:|
    |2021-11-12 |   0.053035|
    |2022-02-04 |   0.059963|
    |2022-05-23 |   0.062813|
    |2022-07-29 |   0.171625|

    ![Volatilidad](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico02.png)


* 3) Semana con mayor variación en la brecha 

    |   Semana |    mean |
    |:---------:|--------:|
    |       29 | 144.868 |

    ![varia_brecha](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico03.png)


* 4) Día de la semana donde hay mayor variación en la brecha   

    | Fecha               | Day    |   Diferencia |
    |:--------------------|:-------|-------------:|
    | 2022-07-04  | Monday |    8.0% |

    ![dia_brecha](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico04.png)

## General:

* 5) Con la info histórica del valor del dólar y del blue, realizar un análisis exploratorio. Cruzar la data con sucesos importantes a nivel político-económico y graficar mes a mes.

    | AnioMes   |   Valor_var_usd_vs_usd_of | Evento              | Tipo_Evento   |
    |:----------|--------------------------:|:--------------------|:--------------|
    | 2022-08   |                  119.58  | Sergio Massa        | econ          |
    | 2022-07   |                  112.71  | Silvina Batakis     | econ          |
    | 2022-07   |                  112.71  | Sergio Massa        | econ          |
    | 2014-10   |                   78.80 | Alejandro Vanoli    | bcra          |
    | 2013-11   |                   63.78 | Juan Carlos Fábrega | bcra          |
    | 2013-11   |                   63.78 | Axel Kicillof       | econ          |
    | 2012-08   |                   37.06 | Cepo al Dolar       | misc          |

    ![eventos](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico05.png)


* 6) Implementar una regresión lineal (una para cada tipo de dólar) para predecir el valor del dólar en:

    |Precio dolar                                              |     |
    |:---------------------------------------------------------|-----:|
    |para la fecha: 2022-12-26  el valor del dolar Blue es de: | 5.04|
    |para la fecha: 2023-03-26  el valor del dolar Blue es de: | 5.14 |
    |para la fecha: 2023-09-27  el valor del dolar Blue es de: | 5.34 |


* 8) Mejor momento para comprar dolár oficial y venderlo a dolár blu
 
    | Mejor dia para Comprar fue:    | Date      |   Variacion_usd_of |
    |---:|:--------------------|-------------------:|
    |  | 2021-11-24  |        0.000198807 |
    |  | 2021-09-28  |        0.000101348 |
    |  | 2021-10-05  |        0.000101122 |
    |  | 2021-11-30  |        9.90884e-05 |
    

    |Mejor dia para Vender fue:       | Date    |   Variacion_usd |
    |----:|:--------------------|----------------:|
    |  | 2022-06-14  |       0.037037  |
    |  | 2022-07-04  |       0.0878661 |
    |  | 2022-07-08  |       0.0622568 |
    |  | 2022-07-13  |       0.0404412 |
    |  | 2022-07-20  |       0.0531561 |
    |  | 2022-07-21  |       0.0630915 |


    ![moment](https://github.com/Jhlirion/DolarBlue_vs_DolarOficial/blob/main/src/grafico07.png)