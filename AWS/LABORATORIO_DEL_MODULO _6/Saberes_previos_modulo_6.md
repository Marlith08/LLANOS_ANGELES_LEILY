**MODULO 6: ALMACENAMIENTO VIRTUAL** 

**Terminología Tecnológica**

|**Término**|**Definición**|
| - | - |
|**Amazon Elastic Block Store (Amazon EBS)**|Almacenamiento para instancias específicas de Amazon EC2. Es la unidad de almacenamiento de la instancia EC2.|
|**Amazon Elastic Compute Cloud (Amazon EC2)**|Servicio web que ofrece capacidad informática escalable en la nube. Equivalente a alquilar una computadora en la nube.|
|**Unidad de disco duro (HDD)**|Almacenamiento más lento que utiliza un disco giratorio para guardar datos.|
|**Operaciones de entrada y salida por segundo (IOPS)**|Medida de rendimiento que compara dispositivos de almacenamiento, como HDD y SSD.|
|**Unidad de estado sólido (SSD)**|Almacenamiento muy rápido que utiliza memoria flash en lugar de un disco giratorio.|

**Antecedentes y conceptos erróneos:**

- El almacenamiento de Amazon EBS se implementa como una serie de bloques de longitud fija que el sistema operativo puede leer y escribir.
- El almacenamiento de Amazon S3 se implementa como un objeto que la aplicación que lo utiliza debe leer y escribir.
- Amazon EBS solo se puede utilizar cuando se adjunta a una instancia EC2. En cambio, se puede acceder a Amazon S3 de manera independiente mediante los protocolos del Protocolo de transferencia de hipertexto (HTTP).
- Amazon EBS no puede contener tantos datos como Amazon S3.
- Amazon EBS solo puede adjuntarse a una instancia EC2, mientras que varias instancias EC2 pueden acceder a los datos de un bucket de S3.
- Amazon S3 presenta más demoras que Amazon EBS a la hora de escribir datos.
- El modelo de datos de consistencia final se implementa de forma diferente entre Amazon EBS y Amazon S3. La consistencia final significa que, si se realiza una escritura seguida de una lectura, los datos leídos acabarán siendo los mismos que los escritos. Con Amazon EBS, la demora para lograr esta consistencia es casi nula, mientras que podría ser considerablemente mayor con Amazon S3.
- Los volúmenes de EBS se cifran en su totalidad, mientras que los objetos de Amazon S3 se cifran de forma individual mediante el cifrado del lado del servidor (SSE).
- Amazon EBS incluye tres tipos de volúmenes, mientras que Amazon S3 incluye más tipos:
- S3 Standard
- S3 Standard-Infrequent Access (S3 Standard-IA)
- S3 One Zone-Infrequent Access (S3 One Zone-IA)
- S3 Intelligent-Tiering
- S3 Glacier
- S3 Glacier Deep Archive



**Laboratorio**

Las etiquetas te permiten clasificar los recursos de AWS de diferentes maneras: por ejemplo, por finalidad, propietario o entorno. Esto es útil cuando tienes muchos recursos del mismo tipo: puedes identificar rápidamente un recurso específico en función de las etiquetas que le hayas asignado. Cada etiqueta consta de un clave valor y un valor, que tú defines.

**Nota**: *Name* es otra etiqueta diferente. La *clave* de esta etiqueta es Name y el *valor* es Web Server 1.

El tipo de imagen de máquina de Amazon (AMI) que selecciones determina el sistema operativo (SO) que se ejecutará en la instancia de EC2 que inicies. En este caso, has seleccionado Amazon Linux 2023 como SO invitado.

El tipo de instancia define los recursos de hadware asignados a la instancia. Este tipo de instancia tiene 1 unidad de procesamiento central virtual (CPU) y 11 GiB de memoria.

Para la clave de vockey que has seleccionado te permitirá conectarte a esta instancia mediante SSH después de que se haya iniciado. 

La red indica la nube virtual privada (VPC) en la que quieres lanzar la instancia. Puede tener varias redes; por ejemplo, una para desarrolla, una segunda para pruebas y una tercera para producción.

Un grupo de seguridad actúa como un firewall virtual que controla el tráfico de una o varias instancias. Cuando inicias una instancia, la asocias a uno o varios grupos de seguridad. Añades reglas a cada grupo de seguridad que permite que el trafico fluya a sus instancias asociadas o desde ellas. Las reglas de un grupo de seguridad se pueden modificar en cualquier momento. Las nuevas reglas se aplican automáticamente a todas las instancias que estén asociadas al grupo de seguridad.

**Nota:** Una dirección *pública* significa que se puede acceder a la instancia desde Internet. Cada instancia que recibe una dirección IP pública también recibe un nombre de host DNS externo: por ejemplo, ec2-xxx-xxx-xxx-xxx.compute-1.amazonaws.com. AWS resuelve un nombre de host DNS externo en la dirección IP *pública* de la instancia cuando se la comunicación proviene de fuera de su VPC. Cuando la comunicación proviene de dentro de su VPC, el nombre de host DNS se resuelve en la dirección IPv4 *privada*.

