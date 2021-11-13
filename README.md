# TP5
Tecnología SAR: Inundaciones e índices de vegetación
- Universidad de Costa Rica 
- GF-0618 FOTOGRAMETRÍA Y TELEDETECCIÓN
- MSc.María José Molina Montero
- Estudiantes: Steven Guillén-Ana López

## Contenido teórico : Defina e Ilustre los siguientes conceptos

### **Microondas**
- Las microondas en el espectro electromagnético abarcan longitudes de onda larga que van en el rango de 1cm y 1m. 
> las microondas tienen propiedades especiales que son importantes en la teledetección, debido a su mayor longitud de onda comparado con las señales ópticas y de infrarrojo. A mayores longitudes de onda la radiación de microondas puede penetrar a través de las nubes, polvo, neblina y lluvia, además estas longitudes de onda son menos susceptibles a la dispersión atmosférica, que afecta en gran medida a las señales ópticas (Canada Centre for Remote Sensing citado en Acevedo, 2011,p.02).


<img src="tablamicro.png" alt="Girl in a jacket" width="600" height="300">

> Fuente: ARSET, 2020
> 
**Figura 1.**
Región de microondas en espectro electromagnético

Las ondas se identifican por su longitud de onda y frecuencia, junto a ello sobresalen parámetros como la amplitud, que es el máximo desplazamiento de una onda desde su posición de equilibrio. Además de la intensidad, entendida como el promedio de potencia transferida durante un período de onda. Las microondas operan en un rango de frecuencia mucho más bajo que las ópticas y reconocer su fase (posición en tiempo y espacio) es fundamental para entender su propagación en la superficie terrestre. (Applied Remote Sensing Training Program , 2021).


<img src="microonda.jpg" alt="Girl in a jacket" width="600" height="300">

> Fuente: Ruíz, 2015

**Figura 2.**
Energía emitida por la Tierra y ventana atmosférica en la región de microondas

Esta ventana atmosférica permite que la señal emitida por la antena logre llegar a la superficie terreste evitando factores que alteran el pulso electromagnético. 

### **Retrodispersión**
> “La energía retrodispersada (backscattered) recibida por el sensor se amplifica y procesa para obtener la posición, las propiedades eléctricas y las propiedades superficiales de los objetos” (Ruíz, 2015, p.02).
 
<img src="retrodispersion.png" alt="Girl in a jacket" width="600" height="300">

> Fuente: Meyer, 2019
 
**Figura 3.**
Los tres tipos principales de dispersión considerados para los datos SAR. 

Se puede entender como la energía dispersada de vuelta una vez que la señal ha interactuado con el objeto presente en la superficie. La retrodispersión puede disminuir con un mayor ángulo de incidencia, es decir, si un radar observa el mismo objeto a distintos ángulos la retrodispersión será distinta.

### **Constante dieléctrica**

<img src="dialectricacons.png" alt="Girl in a jacket" width="600" height="300">

> Fuente: Meyer, 2019
>
**Figura 4.**
Penetración de la señal SAR por longitud de onda

Este concepto esta sumamente relacionado con la retrodispersión pues las propiedades dieléctricas de un medio explican cómo una señal de microondas de longitud de onda interactúa con un medio de dispersión como la superficie de la Tierra o un dosel de vegetación. Estas propiedades dictan cuánto de la radiación entrante se dispersa en la superficie, cuánta señal penetra en el medio y cuánta de la energía se pierde en el medio a través de la absorción (Meyer, 2019).

### **Bandas en RADAR para aplicaciones ambientales**

Desde análisis realizado por Meyer (2019) la banda X se utiliza principalmente para el monitoreo urbano y de infraestructura pues en zonas de vegetación los sensores se dispersan principalmente en las copas los árboles, destaca  que las señales de banda C y L penetran cada vez más más profundo en el volumen de la vegetación siendo adecuadas para el estudio de la estructura en la vegetación, cuantificar la biomasa y cartografiar zonas de inundación.

Comúnmente se utilizan polarizaciones lineales y los sensores SAR propagan o reciben energía con una polarización horizontal o vertical. La diferencia entre componentes perpendiculares es de cero grados evitando el desfase al momento de la propagación.

<img src="bandas.png" alt="Girl in a jacket" width="600" height="300">

> Fuente: ARSET, 2020

**Figura 5.**
Bandas en Radar y aplicaciones

### **Radar de Aértura Sintética**

Los radares de apertura sintética (SAR) generan imágenes radar de reflectividad de alta resolución. Estos sensores se basan en el uso de un radar (acrónimo de Radio Detection And Ranging). Es un sistema activo, es decir, genera su propia fuente de energía. Emiten una señal de microondas con propiedades conocidas y la fuerza de la energía retrodispersada por el objeto es detectada por el radar. Además de ello, los radares miden el tiempo que tarda la señal en viajar hasta la superficie terrestre y regresar a la antena, de esta forma determinan la ubicación un objeto.

<img src="sarimag.png" alt="Girl in a jacket" width="600" height="300">

> Fuente: Meyer, 2019
> 
**Figura 6.** 
Geometría SAR


De acuerdo como Meyer (2019) a diferencia de la mayoría de los sistemas de imágenes ópticas, que apuntan sus sensores hacia el nadir, la antena de un radar apunta lejos del nadir por un llamado ángulo de mirada que ilumina una franja continua en el suelo a medida que la aeronave se mueve. Los SAR transmiten señales de microondas en un ángulo oblicuo y miden la parte retrodispersada (en la dirección del sensor) de esta señal, para analizar características en la superficie (p.21-25).



## Metodología
[Código en GEE Inundaciones](https://code.earthengine.google.com/eea6817e2f6e61a4680d05f9a7a1bee5)

[Código en GGE índice de Vegetación con Radar](https://code.earthengine.google.com/aae609a07c80fb869b729654ec96504a)

## Diagramas de flujos

![](inundacionsar.jpeg)

![](vegetacion.jpeg)



## Resultados y Conclusiones

### Detección de inundaciones
Para la detección de cambios y monitoreo de cuerpos de agua en grandes extensiones, la utilización de la banda C de Radar de Apertura Sintética (SAR) es muy efectiva. Además, utilizar esta tecnología permite, en un país tropical como el nuestro, acceder a imágenes sin distorsiones asociadas a nubes. La metodología de detección de cambios mediante mecanismos de retrodispersión junto al uso de un umbral adecuado, permitió conocer las áreas que fueron inundadas después del huracán Otto.

<img src="inundauno.jpeg" alt="Girl in a jacket" width="600" height="300">

**Figura 7.**
Imágenes antes y después del huracán Otto

Al crear la composición de imágenes con la polarización VV del antes y el después de la inundación se pudo visualizar una gama de colores del morado al verde, en donde el morado corresponde a las zonas en las que antes de la inundación se veían brillantes y después del huracán se veían oscuras por la poca señal que volvía al sensor, los colores blancos corresponden a zonas donde no hubo cambio, y los colores verde a zonas en donde la retrodispersión aumentó y por tanto la señal, pero no significa que allí hubo una inundación del todo, sino que quiere decir hay una superficie muy húmeda y rugosa, como por ejemplo el lago de la figura [].

<img src="inundados.jpeg" alt="Girl in a jacket" width="600" height="300">

**Figura 8.**
Composición de imágenes

El ruido que resulta en la composición (Figura  ) se corrigió con el filtro de speckle, el cual hizo que homogeneizaran los pixeles claros y oscuros, conservando los bordes de las coberturas y la textura de la imagen.

 <img src="inundatres.jpg" alt="Girl in a jacket" width="600" height="300">
 
**Figura 9.**
Aplicación filtro de speckle

Seguidamente, se aplico una diferencia de mosaicos lo cual hizo que se inviertieran los valores, es decir que se pasaran los valores más oscuros a los más claros en las zonas de inundación, esto con el objetivo de ver los valores pixel que tiene un área determinada y que, junto a la correcta asignación del umbral (en este caso 1.50), permite ver los números de cambio para las inundaciones.

<img src="inundacuatro.jpeg" alt="Girl in a jacket" width="600" height="300">

**Figura 10.**
Aplicación de la diferencia a los mosaicos

Haciendo cambios en el umbral, se observó que entre menos restrictivo sea, más se llenará de ruido la imagen, porque los pixeles dispersos serán contemplados como inundados. Es necesario probar cual umbral va a ser adecuado para el proyecto.

<img src="inundacinco.jpeg" alt="Girl in a jacket" width="600" height="300">

**Figura 11.**
Áreas inundadas

### Indice de Vegetación por Radar (RVI)
Una vez ejecutado el código con bandas de polarización V-V y V-H. Al visualizar los datos y gráficos resultantes, el índice oscila entre 0 y 1 , los valores cercanos a 0 pueden referirse a coberturas lisas o descubiertas con colores rojos , en contraste, el crecimiento del índice se relaciona con mayor cobertura vegetal donde resaltan colores verdes y amarillos.

<img src="rviuno.png" alt="Girl in a jacket" width="600" height="300">

**Figura 12.**
Visualización del cambio en RVI entre los meses de Enero y Marzo

El uso de distintas fechas facilita un análisis temporal pues los resultados en cada mes pueden evidenciar cambios en la vegetación, por ejemplo, el crecimiento de un cultivo que produce un aumento en el índice o por lo contrario puede evidenciar la presecia de plagas en los cultivos que pueden generar la pérdida de una plantación, además de ello,  un suelo liso que se prepara para el proceso de siembra arrojara índices más bajos. En el caso analizado hay un cambio claro en los niveles de retrodispersión posterior a la Zafra realizada en el cultivo de Caña de azúcar pasando a colores más rojos en el mes de marzo donde hay una disminución del RVI.


<img src="rvidrastico.png" alt="Girl in a jacket" width="600" height="300">

**Figura 13.** 
Cambio drástico del RVI 

Los resultados evidencian cambios muy drásticos como en la figura 13, puede responder a una zona de cultivo muy densa en el mes de Enero que luego tiene un cambio sustancial de acuerdo con los valores arrojados en Marzo. 

<img src="moderado.png" alt="Girl in a jacket" width="600" height="300">

**Figura 14.**
Cambio moderado RVI.

En otra finca los resultados en el índice son moderados, puede responder a una zona en la cual el crecimiento de la caña no tuvo tanto desarrollo y al momento de realizar la Zafra el cambio no es tan drástico.

![](graficorvi.png)

**Figura 15.** 
Gráfico resultante RVI durante un año

Se obtiene un gráfico con múltiples líneas pues se analizó cada polígono de las 27 fincas. Es un año de análisis que representa las diferencias en los niveles de retrodispersión. Es sumamente variable ya que puede responder a periodos de tiempo en los que se prepara el suelo para la siembra, otros meses con crecimiento vigoroso del cultivo con índices mayores. Además, es fundamental conocer si todas las fincas tienen el mismo patrón de siembra. Datos que solamente se pueden obtener en campo, por ello siempre se resalta la capacidad del profesional en Geografía para crear una relación entre los datos visualizados por medio de herramientas tecnológicas que luego deben ser corroborados en campo.


                                                       Referencias

Acevo Herrera, R. (2011). *Sistemas de teledetección activos y pasivos embarcados en sistemas aéreos no tripulados para la monitorización de la tierra. Universitat Politècnica de Catalunya.*

Applied Remote Sensing Training Program (ARSET).(2020). *Mapeo y Monitoreo de Bosques con Datos SAR: Análisis Multi-Temporal* https://appliedsciences.nasa.gov/sites/default/files/2020-11/SAR_Part1_Spanish.pdf

Applied Remote Sensing Training Program.(ARSET).(2021). *Clasificación de Cultivos Agrícolas con Radar de Apertura Sintética y Teledetección Óptica* https://appliedsciences.nasa.gov/sites/default/files/2021-10/Ag_Part1_Edited_HM_JO_HM_Span.pdf

Meyer, F. (2019). Spaceborne Synthetic Aperture Radar: *Principles, data access, and basic processing techniques. Synthetic Aperture Radar (SAR) Handbook: Comprehensive Methodologies for Forest Monitoring and Biomass Estimation, 21-64.

Ruiz Fernández, L. Á. (2015). *Sensores de microondas en teledetección–II: Aspectos radiométricos.* https://riunet.upv.es/handle/10251/51662





                                                       
                                                  
                                                       
 
