**Laboratorio del módulo 12: Uso de Elastic Beanstalk y CloudFormation**

**Tarea 1. Implementar una aplicación mediante Elastic Beanstalk**

- Selecciona el menú **Servicios**, localiza los servicios de **Computación** y luego selecciona **Elastic Beanstalk**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.001.png)

- Selecciona **Crear aplicación**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.002.png)

- En **Nombre de la aplicación**, escribe un nombre para la aplicación; por ejemplo, MyLabApp

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.003.png)

- En **Plataforma**, selecciona **PHP**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.004.png)

- En **Código de la aplicación**, selecciona **Aplicación de ejemplo**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.005.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.006.png)

- Bajo **Roles de servicio existentes**, abre el menú desplegable y selecciona **EMR\_EC2\_DefaultRole**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.007.png)

- Bajo **Par de claves de EC2**, abre el menú desplegable y selecciona **vockey**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.008.png)

- Bajo **Perfil de instancia de EC2**, abre el menú desplegable y selecciona **EMR\_EC2\_DefaultRole**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.009.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.010.png)

- Bajo **VPC**, selecciona la VPC disponible.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.011.png)

- Bajo **Dirección IP pública**, selecciona **Activada**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.012.png)

- Bajo **Subredes de instancia**, selecciona al menos dos.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.013.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.014.png)

- Bajo **Grupos de seguridad de EC2**, selecciona el grupo **predeterminado**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.015.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.016.png)

- Bajo **Informes de estado**, selecciona **Básico**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.017.png)

- Bajo **Actualizaciones administradas**, anula la selección como **Activadas**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.018.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.019.png)

- Selecciona **Enviar**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.020.png)

- Vuelve a la pestaña de la consola de Elastic Beanstalk.
- Selecciona **Cargar e implementar**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.021.png)

- Selecciona **Elegir archivo**, navega hasta y selecciona el archivo *php.zip* que acabas de descargar y elige **Abrir**.
- Selecciona **Implementar**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.022.png)

- Para ver tu sitio web PHP, bajo **Información general del entorno**, selecciona **Dominio**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.023.png)

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.024.png)

**Tarea 2. Implementar una aplicación mediante CloudFormation**

- Vuelve a la pestaña de la consola de administración de AWS.
- Selecciona el menú **Servicios**, localiza los servicios de **Computación** y selecciona **EC2**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.025.png)

- En el panel de navegación izquierdo, en **Red y seguridad**, selecciona **Pares de claves**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.026.png)

- Selecciona **Crear par de claves**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.027.png)

- En **Nombre**, introduce CFLearner

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.028.png)

- Selecciona **Crear par de claves**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.029.png)

- Cuando se abra la ventana de descarga, selecciona **Cancelar**. No es necesario descargar el archivo.
- Selecciona el menú **Servicios**, localiza los servicios de **Administración y gobernanza** y elige **CloudFormation**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.030.png)

- Selecciona **Crear pila** y, a continuación, elige **Con recursos nuevos (estándar)**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.031.png)

- En la sección **Requisito previo**, elige **Utilizar una plantilla de ejemplo**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.032.png)

- En la sección **Seleccionar una plantilla de ejemplo**, selecciona **Blog de WordPress**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.033.png)

- Selecciona **Siguiente**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.034.png)

- En **Nombre de la pila**, escribe: WordPressStack

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.035.png)

- En la sección **Parámetros**, configura lo siguiente:
- **DBPassword:** escribe Testing1
- **DBUser:** escribe testadmin
- **KeyName:** selecciona el par de claves **CFLearner**
- Selecciona **Siguiente** y, a continuación, 

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.036.png)

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.037.png)

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.038.png)

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.039.png)

- selecciona **Siguiente** de nuevo.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.040.png)

- Revisa la configuración de la pila y, a continuación, selecciona **Enviar**.

![](Aspose.Words.7ae0dcd9-79ca-40aa-8472-fe40f76f582f.041.png)

¡Excelente!

