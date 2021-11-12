# TP5
Tecnología SAR: Inundaciones e índices de vegetación
- Universidad de Costa Rica 
- GF-0618 FOTOGRAMETRÍA Y TELEDETECCIÓN
- MSc.María José Molina Montero
- Estudiantes: Steven Guillén-Ana López

## Contenido teórico : Defina e Ilustre los siguientes conceptos

**Microondas**
- Las microondas en el espectro electromagnético abarcan longitudes extensas que van en el rango de 1cm y 1m. 
> las microondas tienen propiedades especiales que son importantes en la teledetección, debido a su mayor longitud de onda comparado con las señales ópticas y de infrarrojo. A mayores longitudes de onda la radiación de microondas puede penetrar a través de las nubes, polvo, neblina y lluvia, además estas longitudes de onda son menos susceptibles a la dispersión atmosférica, que afecta en gran medida a las señales ópticas (Canada Centre for Remote Sensing citado en Acevedo, 2011,p.02).

**Figura 1.**
Región de microondas en espectro electromagnético

![](tablamicro.png)
> Fuente: ARSET, 2020

Las ondas se identifican por su longitud de onda y frecuencia, junto a ello sobresalen parámetros como la amplitud, que es el máximo desplazamiento de una onda desde su posición de equilibrio. Además de la intensidad, entendida como el promedio de potencia transferida durante un período de onda. Las microondas operan en un rango de frecuencia mucho más bajo que las ópticas y reconocer su fase (posición en tiempo y espacio) es fundamental para entender su propagación en la superficie terrestre. (Applied Remote Sensing Training Program , 2020).

**Figura 2.**
Energía emitida por la Tierra y ventana atmosférica en la región de microondas
![](microonda.jpg)
> Fuente: Ruíz, 2015

Esta ventana atmosférica permite que la señal emitida por la antena logre llegar a la superficie terreste evitando factores que alteran el pulso electromagnético. 

**Retrodispersión**
- Es la energía dispersada de vuelta una vez que la señal ha interactuado con el objeto presente en la superficie. La retrodispersión puede disminuir con un mayor ángulo de incidencia, es decir, si un radar observa el mismo objeto a distintos ángulos la retrodispersión será distinta.
**Figura 3.**
![](retrodispersion.png)
> Fuente: Meyer, 2019
> “La energía retrodispersada (backscattered) recibida por el sensor se amplifica y procesa para obtener la posición, las propiedades eléctricas y las propiedades superficiales de los objetos” (Ruíz, 2015, p.02).


## Metodología
[Código en GEE Inundaciones](https://code.earthengine.google.com/eea6817e2f6e61a4680d05f9a7a1bee5)





## Resultados y Conclusiones

### Detección de inundaciones
Para la detección de cambios y monitoreo de cuerpos de agua en grandes extensiones, la utilización de la banda C de Radar de Apertura Sintética (SAR) es muy efectiva. Además, utilizar esta tecnología permite, en un país tropical como el nuestro, acceder a imágenes sin distorsiones asociadas a nubes. La metodología de detección de cambios mediante mecanismos de retrodispersión junto al uso de un umbral adecuado, permitió conocer las áreas que fueron inundadas después del huracán Otto.
.

Al crear la composición de imágenes con la polarización VV del antes y el después de la inundación se pudo visualizar una gama de colores del morado al verde, en donde el morado corresponde a las zonas en las que antes de la inundación se veían brillantes y después del huracán se veían oscuras por la poca señal que volvía al sensor, los colores blancos corresponden a zonas donde no hubo cambio, y los colores verde a zonas en donde la retrodispersión aumentó y por tanto la señal, pero no significa que allí hubo una inundación del todo, sino que quiere decir hay una superficie muy húmeda y rugosa, como por ejemplo el lago de la figura [].
 
 figuras
