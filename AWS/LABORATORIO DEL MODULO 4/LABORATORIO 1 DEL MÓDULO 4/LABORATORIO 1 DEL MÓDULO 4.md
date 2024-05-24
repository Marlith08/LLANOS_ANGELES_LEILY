**LABORATORIO 1 MÓDULO 4: LANZAMIENTO DE UNA INSTANCIA EC2**

**Tarea 1: Comenzar a crear la instancia y asignarle un nombre.**

**1.-Seleccionamos EC2** 

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.001.png)

**2.- Seleccionamos lanzar instancia.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.002.png)

**3.-Colocaamos un nombre a la instancia**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.003.png)

**Tarea 2. Imágenes de aplicación y SO**

**4.- En AMI mantenemos Amazon Linux, Amazon Linux 2023 y 64 bits(x86).**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.004.png)

**Tarea 3. Elegir el tipo de instancia**

**5.- Como instancia mantenemos t2.micro.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.005.png)

**Tarea 4. Seleccionar un par de claves**

**6.- Seleccionamos vockey**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.006.png)**Tarea 5. Configuración de red**

**7.- Seleccionamos editar**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.007.png)

**8.- Mantenemos los ajustes para VPC**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.008.png)

**9.- En firewall dejamos en lo predeterminado.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.009.png)

**10.- Configuramos el nuevo grupo de seguridad, eliminamos la regla de entrada**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.010.png)

**Tarea 6. Configurar el almacenamiento**

**11.- Mantenemos la configuración de almacenamiento**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.011.png)

**Tarea 7: Detalles avanzados**

**12.- Configuramos un script que será ejecutada en la instancia.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.012.png)

**Tarea 8: Revisar la instancia y lanzarla**

**13.- Seleccionamos lanzar instancia
![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.013.png)**

**14.- Seleccionamos ver todas las instancias**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.014.png)

**15.- Seleccionamos la instancia creada, revisamos en la pestaña detalles y ubicamos la dirección DNS de IPv4 pública.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.015.png)

**Tarea 9. Acceder a la instancia de EC2**

**16.- Copiamos la dirección DNS IPv4 pública en una nueva pestaña de nuestro buscador.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.016.png)

**Sale cargando debido a que falta un paso más.**

**Tarea 10. Actualizar el grupo de seguridad**

**17.- En el panel izquierdo seleccionamos grupos de seguridad.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.017.png)

**18..- Seleccionamos el grupo de seguridad y click en reglas de entrada.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.018.png)

**Tarea 11: Crear una regla de entrada**

**19.- Click en editar regla de entrada**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.019.png)

**20.- Configura lo siguiente:**

- **Tipo: HTTP**
- **Fuente: Cualquier lugar-IPv4**
- **Selecciona Guardar reglas**

**La nueva regla HTTP de entrada crea una entrada para las direcciones IP IPv4 IP (0.0.0.0/0) y IPv6 (::/0).**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.020.png)

**Tarea 12. Probar la regla**

**21.- Una vez guardada volvemos a la pestaña que intentamos abrir y volvemos a cargar, nos debe de aparecer el nombre colocado en el script.**

![](Aspose.Words.0aefe64f-3641-4651-9282-e9ae6818ddcb.021.png)
