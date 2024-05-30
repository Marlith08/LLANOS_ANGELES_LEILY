# ﻿**Laboratorio del módulo 14: Calculadora de precios de AWS**

## **Pasos del laboratorio**

1. Navega hasta [Pricing Calculator](https://calculator.aws/) y elige **Crear una estimación**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.001.png)

2. Para crear la estimación de costes de Amazon EC2, configura las siguientes opciones:
   - Deja seleccionada la opción **Buscar por tipo de ubicación**.
   - En **Elija un tipo de ubicación**, selecciona **Región**.
   - En **Elija una región**, selecciona **EE. UU. Oeste (Oregón)**. 
   - En **Buscar un servicio**, escribe "ec2" y, luego, en el cuadro **Amazon EC2** de la lista de resultados filtrados, selecciona **Configurar**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.002.png)

3. En la ventana **Configure Amazon EC2** (Configurar Amazon EC2), configura las siguientes opciones:
   - En **Descripción**, escribe "on-demand EC2 instance".

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.003.png)

   - En **Sistema operativo**, elige **Linux**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.004.png)

  - En **Número de instancias**, especifica"1".

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.005.png)

   - En **Buscar tipo de instancia**, especifica "t2.medium" y selecciona ese tipo de instancia en la lista de resultados filtrados.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.006.png)

4. En la sección **Opciones de pago**, elige **Bajo demanda** y configura las siguientes opciones:
    - En **Uso** introduce "8".
    - En **Tipo de uso**, elige **Horas/día**.
    - Selecciona **Guardar y agregar servicio**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.007.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.008.png)

5. Para crear la estimación de coste de Amazon S3, en la zona de búsqueda **Buscar un servicio**, escribe "S3". A continuación, selecciona **Configurar** en el cuadro **Amazon Simple Storage Service (S3)** de la lista de resultados filtrados.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.009.png)

6. En la ventana **Configure Amazon Simple Storage Service (S3)** (Configurar Amazon Simple Storage Service), configura las siguientes opciones:
   - En **Descripción**, escribe "data storage".

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.010.png)

  - En **Select S3 Storage classes and other features** (Seleccionar clases de almacenamiento de S3 y otras funciones), deja seleccionadas las dos,**S3 Standard** y **Transferencia de datos**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.011.png)

   - En **S3 Standard Storage** (Almacenamiento S3 Standard), introduce "60", y en **Unidad**, selecciona **GB al mes**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.012.png)

   - En **How will data be moved into S3 Standard?** **The specified amount of data is already stored in S3 Standard** 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.013.png)

7. En **GET, SELECT y todas las demás solicitudes de S3 Standard**, introduce "100".

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.014.png)

8. En la sección **Transferencia de datos**, configura las siguientes opciones para **Transferencia de datos de salida**:
   - En **Data transfer to** (Destino de transferencia de datos), elige **Internet**. 
   - En **Ingrese la cantidad**, especifica"3".
   - En **Data amount** (Cantidad de datos), elige **GB al mes**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.015.png)

    - Selecciona **Guardar y agregar servicio**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.016.png)

    - Selecciona **Ver resumen**. 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.017.png)

Ten en cuenta que ahora tienes dos elementos en tu estimación. Una línea muestra el coste de la instancia de EC2 y la otra muestra el coste del almacenamiento de Amazon S3. 

9. Para añadir el coste de un plan de soporte básico a la estimación, elige **Adición de compatibilidad**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.018.png)

10. En la página **Estimación de soporte**, configura las siguientes opciones:
   - En **Descripción**, escribe "basic support".
   - Deja seleccionados el resto de los valores predeterminados, incluido **Plan Basic Support**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.019.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.020.png)

**Consejo**: Ten en cuenta las diferencias de precios entre los distintos planes de soporte que aparecen.

   - Selecciona **Agregar a mi estimación**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.021.png)

Ten en cuenta que el coste estimado del **plan Basic Support** ha añadido **0,00 USD** a la estimación de costes total. Si hubieras elegido un plan de soporte superior, el coste asociado sería superior.

11. Para exportar la estimación, selecciona el formato que quieras en **Exportar**. Por ejemplo, selecciona **PDF**. 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.022.png)

   - En el cuadro de diálogo que se abre, elige **Aceptar**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_14/Imagenes/Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.023.png)

## ¡**Excelente**! 🌻💦
