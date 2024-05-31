# ﻿**MODULO 11: EQUILIBRADORES DE CARGA**

## **Terminología tecnológica**

|**Término**|**Definición**|
| - | - |
|**Amazon ElasticCache**|Servicio web que facilita la implementación, el funcionamiento y el escalado de una caché en memoria en la nube. Mejora el rendimiento de aplicaciones web al permitir la recuperación rápida de datos desde cachés en memoria, en lugar de depender de bases de datos más lentas basadas en disco.|
|**Caché**|Capa de almacenamiento de datos de alta velocidad que almacena un subconjunto de datos, normalmente de naturaleza transitoria. Permite que las solicitudes futuras se entreguen más rápido que si se accediera directamente a la ubicación de los datos en el almacenamiento principal.|
|**Almacenamiento de datos en caché**|Reutilización eficiente de datos previamente recuperados o calculados. Los datos de la caché se almacenan en hardware de acceso rápido, como la memoria de acceso aleatorio (RAM), y también se pueden utilizar con componentes de software.|
|**Elastic Load Balancing (ELB)**|Distribuye automáticamente el tráfico entrante de aplicaciones en varios destinos, como instancias de Amazon EC2, contenedores, direcciones IP y funciones de AWS Lambda. Evita la sobrecarga de un solo servidor al dirigir el tráfico hacia otras instancias establecidas previamente.|
|**Memoria de acceso aleatorio (RAM)**|Almacenamiento volátil y temporal que retiene datos mientras un equipo está en uso. Desaparece una vez que la máquina se apaga o se completa la tarea. La memoria virtual complementa la RAM y se almacena en la memoria de solo lectura (ROM) cuando no hay suficiente memoria temporal disponible.|

## **Antecedentes y conceptos erróneos:**

Las herramientas son principalmente aquellas que pueden recuperar datos rápidamente y distribuir datos entre varios servidores en respuesta a los altibajos de la demanda, y lo hacen de una forma rentable en la que solo se cobra por uso.

Las aplicaciones y los sitios web a menudo proporcionan una amplia gama de datos y servicios a los usuarios. Dentro de esta amplia gama de datos, a menudo hay un subconjunto más pequeño de datos que se solicitan y a los que se accede con más frecuencia.

Para este tipo de datos muy solicitados o que requieren un uso intensivo de memoria, un servicio de almacenamiento en caché de datos como ElastiCache puede ayudar a garantizar que se pueda acceder a los datos y procesarlos con extrema rapidez. Este servicio funciona almacenando los datos en una memoria extremadamente rápida, pero temporal, que es más rápida que el almacenamiento basado en disco. La desventaja es que la memoria rápida tiene menos espacio de almacenamiento y no almacena los datos de forma permanente.

![](Aspose.Words.7e53f03a-f63a-44c4-b886-878a67d14974.001.png)

![](Aspose.Words.7e53f03a-f63a-44c4-b886-878a67d14974.002.png)

El tráfico intenso puede apagar aplicaciones y sitios web si el servidor no puede manejar la carga. Por eso AWS cuenta con ELB, que puede detectar cuando hay demasiadas solicitudes y desviar automáticamente el tráfico hacia un nuevo servidor para mantener la velocidad y la estabilidad. Existen tres tipos de ELB en AWS.

Balanceador de carga de aplicaciones: El balanceador de carga de aplicaciones es el más adecuado para compensar la carga del tráfico del protocolo de transferencia de hipertexto (HTTP) y HTTP seguro (HTTPS) y proporciona el enrutamiento de solicitudes avanzado dirigido a la entrega de arquitecturas de aplicaciones modernas, incluidos microservicios y contenedores. Operando a nivel de solicitud individual (capa 7), el balanceador de carga de aplicaciones dirige el tráfico a los destinos de Amazon Virtual Private Cloud (Amazon VPC) en función del contenido de la solicitud.

La compensación del balanceador de carga de aplicaciones se realiza en función del contenido del localizador de recursos uniforme (URL). Por ejemplo, si el URL termina en /main, la solicitud se dirigirá a una instancia; si el URL termina en blog/, se dirigirá a otra instancia si se ha realizado el trabajo de definición del balanceador de carga de aplicaciones por adelantado para hacer que esto suceda.

Balanceador de carga de red: El balanceador de carga de red es el más adecuado para compensar la carga del tráfico del protocolo de control de transmisión (TCP), el protocolo de datagramas de usuario (UDP) y la Transport Layer Security (TLS) donde se requiere un rendimiento extremo. El balanceador de carga de red, que funciona a nivel de conexión (capa 4), dirige el tráfico a los destinos dentro de la Amazon VPC y es capaz de gestionar millones de solicitudes por segundo mientras mantiene latencias ultrabajas. El balanceador de carga de red también está optimizado para manejar patrones de tráfico repentinos y volátiles.

Debido al aumento de la velocidad que se puede lograr en la capa de conexión, el tipo de compensación de carga del balanceador de carga de red es más conveniente cuando se intenta evitar mayores volúmenes de tráfico de red. Por ejemplo, para evitar retrasos cuando el interés en un sitio web se vuelve viral, elegirá utilizar la compensación del balanceador de carga de red.

Balanceador de carga clásico: El balanceador de carga clásico proporciona una compensación de carga básica en varias instancias EC2 y funciona a petición y según los niveles de conexión. El balanceador de carga clásico está diseñado para aplicaciones que se construyeron dentro de la red EC2-Classic.

![](Aspose.Words.7e53f03a-f63a-44c4-b886-878a67d14974.003.png)

