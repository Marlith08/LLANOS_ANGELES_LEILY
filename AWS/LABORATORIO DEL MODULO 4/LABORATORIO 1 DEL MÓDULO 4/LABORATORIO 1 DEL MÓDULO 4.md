<h1>LABORATORIO 1 MÓDULO 4: LANZAMIENTO DE UNA INSTANCIA EC2</h1>

<h2> Tarea 1: Comenzar a crear la instancia y asignarle un nombre. </h2>

**1.-Seleccionamos EC2** 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.001.png)

**2.- Seleccionamos lanzar instancia.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.002.png)

**3.-Colocaamos un nombre a la instancia**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.003.png)

<h2>Tarea 2. Imágenes de aplicación y SO</h2>

**4.- En AMI mantenemos Amazon Linux, Amazon Linux 2023 y 64 bits(x86).**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.004.png)

<h2>Tarea 3. Elegir el tipo de instancia</h2>

**5.- Como instancia mantenemos t2.micro.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.005.png)

<h2>Tarea 4. Seleccionar un par de claves</h2>

**6.- Seleccionamos vockey**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.006.png)

<h2>Tarea 5. Configuración de red</h2>

**7.- Seleccionamos editar**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.007.png)

**8.- Mantenemos los ajustes para VPC**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.008.png)

**9.- En firewall dejamos en lo predeterminado.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.009.png)

**10.- Configuramos el nuevo grupo de seguridad, eliminamos la regla de entrada**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.010.png)

<h2>Tarea 6. Configurar el almacenamiento</h2>

**11.- Mantenemos la configuración de almacenamiento**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.011.png)

<h2>Tarea 7: Detalles avanzados</h2>

**12.- Configuramos un script que será ejecutada en la instancia.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.012.png)

<h2>Tarea 8: Revisar la instancia y lanzarla</h2>

**13.- Seleccionamos lanzar instancia**
![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.013.png)

**14.- Seleccionamos ver todas las instancias**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.014.png)

**15.- Seleccionamos la instancia creada, revisamos en la pestaña detalles y ubicamos la dirección DNS de IPv4 pública.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.015.png)

<h2>Tarea 9. Acceder a la instancia de EC2</h2>

**16.- Copiamos la dirección DNS IPv4 pública en una nueva pestaña de nuestro buscador.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.016.png)

**Sale cargando debido a que falta un paso más.**

<h2>Tarea 10. Actualizar el grupo de seguridad</h2>

**17.- En el panel izquierdo seleccionamos grupos de seguridad.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.017.png)

**18..- Seleccionamos el grupo de seguridad y click en reglas de entrada.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.018.png)

<h2>Tarea 11: Crear una regla de entrada</h2>

**19.- Click en editar regla de entrada**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.019.png)

**20.- Configura lo siguiente:**

- **Tipo: HTTP**
- **Fuente: Cualquier lugar-IPv4**
- **Selecciona Guardar reglas**

**La nueva regla HTTP de entrada crea una entrada para las direcciones IP IPv4 IP (0.0.0.0/0) y IPv6 (::/0).**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.020.png)

<h2>Tarea 12. Probar la regla</h2>

**21.- Una vez guardada volvemos a la pestaña que intentamos abrir y volvemos a cargar, nos debe de aparecer el nombre colocado en el script.**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO%20DEL%20MODULO%204/LABORATORIO%201%20DEL%20M%C3%93DULO%204/Imagenes/Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.021.png)
