**Laboratorio del módulo 14: Calculadora de precios de AWS**

**Pasos del laboratorio**

1. Navega hasta [Pricing Calculator](https://calculator.aws/) y elige **Crear una estimación**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.001.png)

1. Para crear la estimación de costes de Amazon EC2, configura las siguientes opciones:
   1. Deja seleccionada la opción **Buscar por tipo de ubicación**.
   1. En **Elija un tipo de ubicación**, selecciona **Región**.
   1. En **Elija una región**, selecciona **EE. UU. Oeste (Oregón)**. 
   1. En **Buscar un servicio**, escribe "ec2" y, luego, en el cuadro **Amazon EC2** de la lista de resultados filtrados, selecciona **Configurar**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.002.png)

1. En la ventana **Configure Amazon EC2** (Configurar Amazon EC2), configura las siguientes opciones:
   1. En **Descripción**, escribe "on-demand EC2 instance".

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.003.png)

1. En **Sistema operativo**, elige **Linux**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.004.png)

1. En **Número de instancias**, especifica"1".

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.005.png)

1. En **Buscar tipo de instancia**, especifica "t2.medium" y selecciona ese tipo de instancia en la lista de resultados filtrados.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.006.png)

1. En la sección **Opciones de pago**, elige **Bajo demanda** y configura las siguientes opciones:
   1. En **Uso** introduce "8".
   1. En **Tipo de uso**, elige **Horas/día**.
   1. Selecciona **Guardar y agregar servicio**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.007.png)

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.008.png)

1. Para crear la estimación de coste de Amazon S3, en la zona de búsqueda **Buscar un servicio**, escribe "S3". A continuación, selecciona **Configurar** en el cuadro **Amazon Simple Storage Service (S3)** de la lista de resultados filtrados.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.009.png)

1. En la ventana **Configure Amazon Simple Storage Service (S3)** (Configurar Amazon Simple Storage Service), configura las siguientes opciones:
   1. En **Descripción**, escribe "data storage".

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.010.png)

1. En **Select S3 Storage classes and other features** (Seleccionar clases de almacenamiento de S3 y otras funciones), deja seleccionadas las dos,**S3 Standard** y **Transferencia de datos**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.011.png)

1. En **S3 Standard Storage** (Almacenamiento S3 Standard), introduce "60", y en **Unidad**, selecciona **GB al mes**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.012.png)

1. En **How will data be moved into S3 Standard?** **The specified amount of data is already stored in S3 Standard** 

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.013.png)

1. En **GET, SELECT y todas las demás solicitudes de S3 Standard**, introduce "100".

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.014.png)

1. En la sección **Transferencia de datos**, configura las siguientes opciones para **Transferencia de datos de salida**:
   1. En **Data transfer to** (Destino de transferencia de datos), elige **Internet**. 
   1. En **Ingrese la cantidad**, especifica"3".
   1. En **Data amount** (Cantidad de datos), elige **GB al mes**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.015.png)

1. Selecciona **Guardar y agregar servicio**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.016.png)

1. Selecciona **Ver resumen**. 

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.017.png)

Ten en cuenta que ahora tienes dos elementos en tu estimación. Una línea muestra el coste de la instancia de EC2 y la otra muestra el coste del almacenamiento de Amazon S3. 

1. Para añadir el coste de un plan de soporte básico a la estimación, elige **Adición de compatibilidad**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.018.png)

1. En la página **Estimación de soporte**, configura las siguientes opciones:
   1. En **Descripción**, escribe "basic support".
   1. Deja seleccionados el resto de los valores predeterminados, incluido **Plan Basic Support**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.019.png)

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.020.png)

**Consejo**: Ten en cuenta las diferencias de precios entre los distintos planes de soporte que aparecen.

1. Selecciona **Agregar a mi estimación**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.021.png)

Ten en cuenta que el coste estimado del **plan Basic Support** ha añadido **0,00 USD** a la estimación de costes total. Si hubieras elegido un plan de soporte superior, el coste asociado sería superior.

1. Para exportar la estimación, selecciona el formato que quieras en **Exportar**. Por ejemplo, selecciona **PDF**. 

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.022.png)

1. En el cuadro de diálogo que se abre, elige **Aceptar**.

![](Aspose.Words.76e534b8-3f3e-4833-af4c-66267e4436cf.023.png)

¡Excelente!
