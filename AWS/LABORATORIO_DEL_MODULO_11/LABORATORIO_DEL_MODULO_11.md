# **Laboratorio del módulo 11: Uso de balanceadores de carga**

## **Tarea 1. Lanzar una instancia de EC2**

- En el cuadro de búsqueda a la derecha de **Servicios**, busca y selecciona **EC2** para abrir la consola de EC2.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.001.png)

- Selecciona el botón **Lanzar instancia** en medio de la página y luego selecciona **Lanzar instancia** en el menú desplegable.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.002.png)

- En el panel *Nombre y etiquetas*:
  - En **Nombre**, introduce Web Server 1

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.003.png)

- En el panel *Aplicación e imágenes del SO*:
  - Para **Inicio rápido**, mantén el **Amazon Linux** predeterminado seleccionado

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.004.png)

- En el panel *Tipo de instancia*:
  - Mantén el tipo de instancia predeterminado, **t2.micro**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.005.png)

- En el panel *Par de claves (inicio de sesión)*:
  - En la lista desplegable **Nombre del par de claves - *obligatorio***, selecciona **vockey**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.006.png)

- En la sección *Configuraciones de red*, selecciona **Editar**.
  - En la lista desplegable **Subred**, selecciona la subred existente en la **Zona de disponibilidad us-east-1a**.
  - Para **Nombre del grupo de seguridad - *obligatorio***, introduce Web Server security group
  - En **Descripción - *obligatorio***, introduce Security group for my web server
  - En la sección **Reglas de grupos de seguridad de entrada**, selecciona **Eliminar** para eliminar la regla predeterminada.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.007.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.008.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.009.png)

- Selecciona **Añadir regla del grupo de seguridad** para configurar una nueva regla según la siguiente información
  - **Tipo:** HTTP
  - **Tipo de origen:** Cualquiera

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.010.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.011.png)

- Desplázate hacia abajo y amplía el panel **Detalles avanzados**. Allí, configura lo siguiente:
  - Desplázate hacia abajo hasta el campo **Datos de usuario**.
  - Copia el siguiente código y pégalo en el campo **Datos de usuario**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.012.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.013.png)

- Selecciona **Lanzar instancia**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.014.png)

## **Tarea 2. Acceder al sitio web de la instancia de EC2**

- Selecciona la instancia de **Web Server 1** que creaste antes en este laboratorio.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.015.png)

- En la pestaña **Detalles**, copia la **Dirección IPv4 pública** de tu instancia, a continuación, abre una nueva pestaña en tu navegador web y pega y carga la dirección

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.016.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.017.png)

## **Tarea 3. Crear una segunda instancia de EC2 para el balanceo de carga**

- Selecciona la instancia **Web Server 1**.
- En el menú **Acciones**, selecciona **Imágenes y plantillas** y después selecciona **Lanzar más como esta**

- ![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.018.png)**
  En el panel **Nombre y etiquetas**, cambia el nombre a Web Server 2.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.019.png)

- En la sección **Par de claves (inicio de sesión)**, en la lista desplegable **Nombre del par de claves - *obligatorio***, selecciona **vockey**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.020.png)

- En la lista desplegable **Subred**, selecciona la subred existente en la **Zona de disponibilidad us-east-1b**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.021.png)

- Desplázate hacia abajo y expande la sección **Detalles avanzados**, y después desplázate hacia abajo hasta el campo **Datos de usuario**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.022.png)

- Selecciona **Lanzar instancia**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.023.png)

## **Tarea 4. Acceder al sitio web en la segunda instancia de EC2**

- Selecciona la instancia **Web Server 2**.
- En la pestaña **Detalles**, copia la **Dirección IPv4 pública** de tu instancia, a continuación abre una nueva pestaña en tu navegador web y pega y carga la dirección.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.024.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.025.png)

## **Tarea 5. Crear un balanceador de carga**

- De vuelta en la consola de EC2, en el panel de navegación izquierdo, bajo **Balanceo de carga**, selecciona **Balanceadores de carga**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.026.png)

- Selecciona **Crear balanceador de carga**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.027.png)

- En **Application Load Balancer**, selecciona **Crear**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.028.png)

- En el panel *Configuración básica*:
  - En **Nombre**, introduce myloadbalancer.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.029.png)

- En el panel *Asignación de red*:
  - Bajo **Asignaciones**, selecciona las zonas de disponibilidad en las que hayas creado las dos instancias.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.030.png)

- En el panel *Asignación de red*:
  - Bajo **Asignaciones**, selecciona las zonas de disponibilidad en las que hayas creado las dos instancias.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.031.png)

- En el panel *Agentes de escucha y direccionamiento*:
  - Selecciona **Crear grupo de destino**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.032.png)

- En el panel *Configuración básica*:
  - Mantén el tipo de destino configurado como **Instancias**.
  - En **Nombre del grupo de destino**, introduce myalbTG.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.033.png)

- En el panel *Comprobaciones de estado*:
  - Para **Ruta de comprobación de estado**, introduce index.html después de la barra inclinada ( / )

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.034.png)

- Selecciona **Siguiente**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.035.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.036.png)

- Selecciona **Incluir como pendiente a continuación**.
  - Verifica que ambas instancias aparezcan ahora en la lista de **Destinos** a continuación.
- Selecciona **Crear grupo de destino**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.037.png)

- En la sección **Agentes de escucha y direccionamiento**, bajo **Agente de escucha** selecciona el icono de actualización .
- En el menú desplegable, selecciona el grupo de destino **myalbTG** que creaste.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.038.png)

- Desplázate hacia abajo y selecciona **Crear balanceador de carga**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.039.png)

## **Tarea 6. Probar el balanceador de carga**

- Selecciona el balanceador de carga que acabas de crear y expande la sección **Detalles**.
- Bajo **Detalles**, copia el valor del **Nombre de DNS** en tu portapapeles.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.040.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_11/Imagenes/Aspose.Words.1f680561-9e50-4d8e-aa11-f1af1dedd288.041.png)

## **¡Excelente!** 🌻💦

