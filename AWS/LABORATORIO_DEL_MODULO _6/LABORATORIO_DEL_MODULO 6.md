**Laboratorio del módulo 6: Asociar un volumen de EBS**

**Tarea 1. Comenzar a crear la instancia y asignarle un nombre**

- Seleccionamos el menú **Servicios** y seleccionamos **EC2.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.001.png)

- Seleccionamos el botón de **lanzar instancia**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.002.png)

- Colocamos un nombre a la **instancia.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.003.png)

**Tarea 2. Imágenes de aplicación y SO**

- Seleccionamos **AMI** 
- Mantenemos **Amazon Linux** 
- Mantenemos **Amazon Linux** **2023 AMI x86\_64(HVM)**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.004.png)

**Tarea 3. Elegir el tipo de instancia**

- Especificamos un tipo de instancia **t2.micro**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.005.png)

**Tarea 4. Seleccionar un par de claves**

- Seleccionamos el par clave que deseamos asociar con la instancia.
- Seleccionamos **vockey**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.006.png)

**Tarea 5. Configuración de red**

- Seleccionamos **editar**.
- Mantenemos la **subred**.
- Seleccionamos crear grupo de seguridad.
- Nombre del grupo de seguridad: **Web Server**.
- Descripción: **Security group for my web server**.
- Seleccionamos **eliminar**.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.007.png)

**Tarea 6. Configurar el almacenamiento**

- Mantenemos la configuración predeterminada.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.008.png)

**Tarea 7: Detalles avanzados**

- Configuramos un script.
- Insertamos el código en **Datos de usuario**.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.009.png)

**Tarea 8: Revisar la instancia y lanzarla**

- Lanzamos la instancia.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.010.png)

- Verificamos que se haya ejecutado correctamente.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.011.png)

**Tarea 9. Acceder a la instancia de EC2**

- Copiamos el valor de la Dirección IPv4 pública de la instancia.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.012.png)

- Abrimos en una pestaña nueva
- Aparece cargando debido a que falta actualizar el grupo de seguridad.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.013.png)

**Tarea 10. Actualizar el grupo de seguridad**

- En **Red y seguridad**, seleccionamos **Grupos de seguridad.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.014.png)

- Seleccionamos el grupo de seguridad que creamos y seleccionamos **Reglas de entrada.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.015.png)

**Tarea 11: Crear una regla de entrada**

- Seleccionamos **Editar reglas de entrada.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.016.png)

Configuramos lo siguiente:

- **Tipo:** HTTP
- **Fuente:** Cualquier lugar-IPv4
- Seleccionamos **Guardar reglas**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.017.png)

**Tarea 12. Probar la regla**

- Actualizamos la pestaña ya previamente abierta.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.018.png)

**Tarea 13: Adjuntar un volumen de EBS a la instancia de EC2**

- Regresamos a la instancia y verificamos la **zona de disponibilidad.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.019.png)

- En el panel seleccionamos **Elastic Block Store**, y seleccionamos **volúmenes.**

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.020.png)

- Seleccionamos **Crear volumen**.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.021.png)

- El tamaño: **1GiB**
- Seleccionamos la **zona de disponibilidad.**
- Crear volumen.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.022.png)

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.023.png)

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.024.png)

- Seleccionamos el nuevo volumen con un tamaño de 1 GiB. A continuación, elegimos **Acciones** y **Asociar volumen**.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.025.png)

- Seleccionamos nuestra instancia.
- Asociar volumen.

![](Aspose.Words.c8a22f22-18da-43e0-8595-98711afdad99.026.png)

**¡Excelente!**

