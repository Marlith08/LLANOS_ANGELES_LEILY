# ﻿**Módulo 2: Estructuras de la nube**

## **Terminología tecnológica.**

|**Zona de disponibilidad**|Uno o varios centros de datos que albergan muchos servidores. Cada región tiene varias ubicaciones aisladas conocidas como zonas de disponibilidad. Cada zona de disponibilidad está aislada, pero las zonas de disponibilidad de una región están conectadas mediante enlaces de baja latencia. Una zona de disponibilidad se representa mediante un código de región seguido de un identificador de letra, por ejemplo, **us-east-1a.**|
| :-: | - |
|**Ubicación de borde**|Un sitio en el que se pueden almacenar los datos para obtener una latencia más baja. A menudo, las ubicaciones de borde estarán cerca de las zonas de gran población que generarán volúmenes de tráfico elevados.|
|**Infraestructura como servicio (IaaS)**|Un modelo en el que se utilizan máquinas virtuales y servidores para que los clientes alojen una amplia gama de aplicaciones y para que se proporcionen servicios de TI.|
|**Latencia**|El retraso que se produce antes de que se inicie una transferencia de datos después de que se hayan solicitado los datos.|
|**Plataforma como servicio (PaaS)**|Un modelo que proporciona una plataforma virtual para que los clientes creen software personalizado|
|**Región**|Un área en la que se almacenan los datos. El almacenamiento de datos en una región que tiene más cerca explica, entre otros motivos, por qué es posible acceder a ellos a la velocidad de la luz.|
|**Software como servicio (SaaS)**|<p>Un modelo que proporciona aplicaciones que utilizan Internet gestionadas por un tercero.</p><p></p>|

##**Antecedentes y conceptos erróneos**

AWS Global Cloud Infrastructure es la plataforma en la nube más segura, extensa y fiable que ofrece más de 200 servicios completos de centros de datos de todo el mundo. Esta infraestructura se compone de muchos componentes diferentes, incluidas regiones, zonas de disponibilidad y ubicaciones de borde. 

Las diferencias entre los componentes de la infraestructura pueden ser confusas porque todos están interconectados y están relacionados con el diseño físico de la nube de AWS. Es bueno tener un ejemplo visual concreto.

**Región > zona de disponibilidad > ubicación de borde.**

- **IaaS:** Estos servicios contienen los componentes básicos de la nube. Proporcionan acceso a los equipos, físicos y virtuales, así como a las funciones de red y al espacio de almacenamiento. Piense en IaaS como si se tratase de alquilar una cocina. Puede usar todos los diferentes electrodomésticos (batidoras, licuadoras, fregaderos) y puede alquilar una cocina con mejores electrodomésticos si los necesita.
  - Ejemplos: Amazon Elastic Compute Cloud (Amazon EC2), Rackspace, Google Compute Engine
- **PaaS:** Estos servicios son las herramientas necesarias para administrar el hardware subyacente y lanzar aplicaciones. Incluyen entornos de programación, plataformas de pruebas de aplicaciones y lanzadores de aplicaciones. Piense en PaaS como si fuera a un restaurante. No está administrando los electrodomésticos de la cocina, pero puedes pedirle al camarero o al chef que haga las cosas como desee.
  - Ejemplos: AWS Elastic Beanstalk, Microsoft Azure, SaaS de Google App Engine
- **Saas:** Estos servicios son las aplicaciones y el software reales proporcionados a través de Internet. No es el responsable de administrar o instalar el software; solo tiene que acceder a él y usarlo. Piense en la SaaS como si estuviera comiendo en un buffet libre. Tiene acceso a cualquier comida que se sirva. No controla lo que se hace ni cómo se hace, pero puede usar todo lo que quiera.
  - Ejemplos: Dropbox, Slack, Spotify, YouTube, Microsoft Office 365, Gmail

![PaaS o IaaS? - Por una nube sostenible](Aspose.Words.ec65c308-b70d-4f75-a784-a914a7bfb552.001.png)
