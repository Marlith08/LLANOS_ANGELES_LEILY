**MODULO 10: BASES DE DATOS**

|**Término**|**Definición**|
| - | - |
|**Base de datos relacional**|Colección de conjuntos organizados como registros y columnas en tablas. Se definen relaciones entre las tablas. Utiliza el lenguaje de consulta estructurada (SQL) para interactuar con la base de datos.|
|**Amazon Relational Database Service (Amazon RDS)**|Permite a los desarrolladores crear y administrar bases de datos relacionales en la nube. Facilita el seguimiento, organización y búsqueda eficiente de grandes cantidades de datos.|
|**Amazon DynamoDB**|Servicio de base de datos no relacional de AWS. Los datos se almacenan en pares clave-valor.|
|**Base de datos no relacional**|También conocida como base de datos “No SQL” o “No Solo SQL”. Cada entrada se almacena en un par clave-valor, y puede tener diferentes valores adjuntos a una clave.|
|**Amazon Redshift**|Servicio de almacenamiento de datos de AWS que permite consultar grandes cantidades de datos rápidamente para inteligencia empresarial (BI).|
|**Procesamiento de transacciones en línea (OLTP)**|Categoría de procesamiento de datos centrada en tareas de transacciones, como inserción, actualización o eliminación de pequeñas cantidades de datos en una base de datos.|
|**Procesamiento analítico en línea (OLAP)**|Método informático que permite a los usuarios extraer y consultar datos eficientemente para analizarlos desde diferentes perspectivas.|
|**Amazon Aurora**|Motor de base de datos relacional compatible con MySQL y PostgreSQL, diseñado para la nube. Combina rendimiento y disponibilidad de bases de datos empresariales con la simplicidad de bases de datos de código abierto.|
|**MySQL**|Sistema de administración de base de datos relacional de código abierto.|


Antecedentes y conceptos erróneos.

Las operaciones OLAP son principalmente de solo lectura; es decir, leen los datos y realizan varios tipos de procesamiento, como suma, agrupación y clasificación.

Sin embargo, las operaciones del OLTP necesitan actualizar la base de datos además de leerla. La actualización puede consistir en agregar, modificar o eliminar valores

El OLTP se realiza mejor en bases de datos no relacionales, mientras que los procesos del OLAP se realizan mejor en bases de datos relacionales.

**Comparación de OLTP y OLAP**

|**OLTP**|**OLAP**|
| - | - |
|<p>- Gestiona los datos operativos recientes.</p><p>- El tamaño es más pequeño, normalmente oscila entre 100 MB y 10 GB.</p><p>- El objetivo es realizar operaciones diarias.</p><p>- Utiliza consultas sencillas.</p><p>- Velocidades de procesamiento más rápidas.</p><p>- Requiere operaciones de lectura/escritura.</p>|<p>- Gestiona todos los datos históricos.</p><p>- El tamaño es mayor, normalmente oscila entre 1 TB y 100 PB.</p><p>- El objetivo es tomar decisiones desde orígenes de datos de gran tamaño.</p><p>- Utiliza consultas complejas.</p><p>- Funciona a velocidades de procesamiento más lentas.</p><p>- Requiere solo operaciones de lectura.</p>|

**Aplicaciones del OLTP**

- Registrar pedidos en línea.
- Procesar compras.
- Almacenar detalles de clientes.

**Aplicaciones del OLAP**

- Analizar los patrones de compra para hacer recomendaciones.
- Hacer un seguimiento de las tendencias de compra para hacer publicidad específica.
- Analizar las tendencias estacionales de compra para asegurarse de que los artículos estén en stock.

**Servicios de bases de datos de AWS**

**Amazon RDS** es la base de datos relacional clásica que utiliza SQL, Oracle, Aurora u otros sistemas de base de datos similares. Se utiliza principalmente para el OLTP.  Imagine que se trata de un libro de calificaciones en el que cada estudiante es una fila y todos los estudiantes tienen el mismo número de tareas (columnas). Las empresas pueden utilizar el código para buscar datos específicos en función de la información de las filas y columnas. Amazon RDS resulta útil para las empresas que almacenan una cantidad moderada de datos de estructura uniforme, lo que significa que cada ID único (como el nombre del estudiante) se adjunta al mismo número de puntos de datos (calificaciones).

Amazon RDS se utiliza principalmente para el OLTP porque tiene mejores métodos para mantener la integridad y consistencia de la base de datos al procesar datos.

**DynamoDB** es una base de datos no relacional, lo que significa que no se pueden utilizar sistemas tradicionales como SQL o Aurora. Cada elemento de la base de datos se almacena como un par clave-valor o un archivo de notación de objetos de JavaScript (JSON). Esto significa que cada fila puede tener un número diferente de columnas. No es necesario que todas las entradas se emparejen de la misma manera. Esto permite una flexibilidad en el procesamiento que funciona bien para los blogs, los videojuegos y la publicidad. 

**Aurora** es un motor de base de datos relacional diseñado específicamente para funcionar con la nube de AWS. Aurora es hasta cinco veces más rápido que las bases de datos MySQL estándar y tres veces más rápido que las bases de datos PostgreSQL estándar. Está diseñado para proporcionar la seguridad, la disponibilidad y la fiabilidad de las bases de datos comerciales a una décima parte del costo. Aurora está completamente administrada por Amazon RDS, que automatiza tareas administrativas que consumen mucho tiempo, tales como aprovisionar hardware, configurar una base de datos, aplicar parches y realizar copias de seguridad.

**Amazon Redshift** es un almacén de datos rápido y completamente administrado que hace eficiente y rentable analizar todos sus datos a través de SQL estándar y de las herramientas de inteligencia empresarial existentes.

**Laboratorio**

De manera predeterminada, el grupo de seguridad predeterminado de la VPC no permite el tráfico entrante de SQL Server desde fuentes externas. En esta tarea, activarás las conexiones entrantes de SQL Server desde tu dirección IP.

