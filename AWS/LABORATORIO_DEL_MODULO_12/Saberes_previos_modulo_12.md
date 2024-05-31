# ﻿**MODULO 12: ELASTIC BEANSTALK Y CLOUDFORMATION**

## **Terminología tecnológica**

|**AWS Elastic Beanstalk:**|Elastic Beanstalk administra automáticamente los detalles de implementación del aprovisionamiento de capacidad, el balanceo de carga, el escalado automático y el monitoreo del estado de una aplicación. En muchos sentidos, utilizar Elastic Beanstalk es como ejecutar una macro o un archivo por lotes que coloca un contenedor alrededor de una aplicación existente para que se ejecute sin problemas en la nube de Amazon Web Services (AWS).|
| :-: | - |
|**AWS CloudFormation:**|<p>Este servicio brinda a los desarrolladores y empresas una manera fácil de crear un conjunto de recursos de AWS relacionados y aprovisionarlos de forma ordenada y previsible. CloudFormation proporciona un medio para combinar una pila de servicios de AWS, similar a escribir macros o archivos por lotes en Linux o Microsoft Windows.</p><p></p>|
|**Pila**|<p>Conjunto de recursos de AWS que puede administrar como una sola unidad. Puede crear, actualizar o eliminar un conjunto de recursos mediante la creación, actualización o eliminación de pilas.</p><p></p>|

## **Antecedentes y conceptos erróneos**

**Elastic Beanstalk** es un servicio fácil de utilizar destinado a implementar y escalar aplicaciones y servicios web desarrollados con Java, .NET, PHP, Node.js, Python, Ruby, Go y Docker en servidores conocidos como Apache, Nginx, Passenger, e IIS.

Una vez que usted carga el código, Elastic Beanstalk automáticamente administra la implementación, desde el aprovisionamiento de capacidad, el balanceo de carga y el escalado automático hasta el monitoreo del estado de las aplicaciones. Al mismo tiempo, usted mantiene el control total de los recursos de AWS que alimentan la aplicación y puede acceder a los recursos subyacentes en cualquier momento.

Beneficios de Elastic Beanstalk:

1. Inicio rápido y sencillo
   1. Elastic Beanstalk es la manera más rápida y sencilla de implementar su aplicación en AWS.
1. Productividad del desarrollador
   1. Elastic Beanstalk aprovisiona y opera la infraestructura y administra la pila de la aplicación (plataforma) por usted, para que no tenga que dedicar tiempo ni adquirir la experiencia.
1. Imposibilidad de que se produzca un crecimiento excesivo
   1. Elastic Beanstalk escala automáticamente la aplicación de forma ascendente o descendente en función de las necesidades específicas de su aplicación mediante configuraciones de escalado automático fáciles de ajustar.
1. Control total de los recursos
   1. Tiene la libertad de seleccionar los recursos de AWS, como el tipo de instancia de Amazon Elastic Compute Cloud (Amazon EC2), que son óptimos para su aplicación.

**CloudFormation**

CloudFormation proporciona un lenguaje común que le permite describir y aprovisionar todos los recursos de la infraestructura de su entorno en la nube. CloudFormation le permite utilizar lenguajes de programación o un archivo de texto simple para modelar y aprovisionar, de manera automatizada y segura, todos los recursos necesarios para las aplicaciones en todas las regiones y cuentas de AWS.

Beneficios de CloudFormation

1. Modelar todo.
   1. CloudFormation le permite modelar toda su infraestructura con un archivo de texto o lenguajes de programación.
1. Automatizar e implementar.
   1. CloudFormation aprovisiona sus recursos de manera segura y repetible, lo que le permite crear y recrear su infraestructura y aplicaciones sin tener que realizar acciones manuales ni escribir scripts personalizados.
1. Trabajar con código.
   1. La codificación de la infraestructura le permite tratar su infraestructura como código.

` `![](Aspose.Words.6090d161-e4f2-4535-827e-76149ecd6994.001.png)

**¿En qué se diferencia Elastic Beanstalk de CloudFormation?**

Estos servicios están diseñados para complementarse entre sí. Elastic Beanstalk proporciona un entorno para implementar y ejecutar aplicaciones en la nube con facilidad. Está integrado con herramientas para desarrolladores y proporciona una experiencia única para que administre el ciclo de vida de las aplicaciones. CloudFormation es un mecanismo de aprovisionamiento práctico para una amplia gama de recursos de AWS. Admite las necesidades de infraestructura de muchos tipos diferentes de aplicaciones, como aplicaciones empresariales existentes, heredadas o creadas con diversos recursos de AWS y soluciones basadas en contenedores (incluidas aquellas creadas con Elastic Beanstalk).

Para ser claros, Elastic Beanstalk es como ejecutar un archivo.bat y CloudFormation es como escribirlo. Elastic Beanstalk permite a los desarrolladores cargar y ejecutar su código; luego, se encarga de toda la configuración de fondo en la nube, como lanzar instancias EC2 y asociar almacenamiento en bloques elástico. Con CloudFormation, básicamente está configurando una plantilla para todos los recursos en la nube que desea ejecutar para que todo se pueda realizar de una sola vez y de manera repetible.

CloudFormation admite entornos de aplicaciones de Elastic Beanstalk como uno de los tipos de recursos de AWS. Esto le permite, por ejemplo, crear y administrar una aplicación alojada en Elastic Beanstalk, junto con una base de datos de Amazon Relational Database Service (Amazon RDS) para almacenar los datos de la aplicación. Además de las instancias de base de datos de RDS, también se puede agregar al grupo cualquier otro recurso de AWS compatible.

