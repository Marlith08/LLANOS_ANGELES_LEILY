**Laboratorio del módulo 9: Creación de una alarma de CloudWatch que inicie un mensaje de Amazon SNS**

**Tarea 1. Crear y suscribirse a un tema de SNS**

- Selecciona el menú **Servicios**, localiza la sección **Integración de aplicaciones** y elige **Simple Notification Service**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.001.png)

- En el panel de navegación izquierdo, selecciona **Temas**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.002.png)

- Selecciona **Crear un tema**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.003.png)**


![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.004.png)

- En **Tipo**, selecciona **Estándar**

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.005.png)

- En **Nombre**, introduce MoneyAlert

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.006.png)

- Selecciona **Crear un tema**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.007.png)

- En la sección **Suscripciones**, elige **Crear suscripción**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.008.png)

- En **ARN del tema**, selecciona el tema **MoneyAlert** que has creado.
- Para **Protocolo**, selecciona **Correo electrónico** para recibir una alerta por correo.
- En **Punto de enlace**, introduce la dirección de correo electrónico.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.009.png)

- Selecciona **Crear suscripción**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.010.png)

**Tarea 2. Crear una alarma de CloudWatch.**

- Selecciona el menú **Servicios**, localiza la sección **Administración y gobernanza** y elige **CloudWatch**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.011.png)

- En el panel de navegación izquierdo, selecciona **Alarmas**.
- Selecciona **Crear alarmas** y después **Crear alarma**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.012.png)

- Selecciona **Seleccionar métrica**.
- ![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.013.png)Selecciona **Facturación**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.014.png)

- Selecciona **Cargo total estimado**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.015.png)

- Marca la casilla **EstimatedCharges**.
- Selecciona **Seleccionar métrica.**

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.016.png)

- En la sección **Condiciones**, configura lo siguiente:
  - En **Tipo de límite**, selecciona **Estático**.
  - En **Siempre que EstimatedCharges sea...**, selecciona **Mayor**.
  - En **que...**, introduce 100 en el cuadro de texto.
- Selecciona **Siguiente**

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.017.png)

- En la sección **Notificación**, configura lo siguiente:
  - En **Activador de estado de alarma**, selecciona **En modo alarma**.
  - Para **Enviar una notificación al siguiente tema de SNS**, selecciona **Seleccione un tema de SNS existente**.
  - En **Enviar una notificación a...**, selecciona el tema **MoneyAlert**.
- Selecciona **Siguiente**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.018.png)

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.019.png)

- En **Nombre de la alarma**, escribe MoneyAlertAlarm
- Selecciona **Siguiente**.

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.020.png)

- Creamos la alarma

![](Aspose.Words.6ea30aa9-be85-44c9-a6e9-47e454a8e2d6.021.png)

