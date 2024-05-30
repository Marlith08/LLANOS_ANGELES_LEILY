**Laboratorio del módulo 10: Creación de una instancia de base de datos de Amazon RDS**

**Tarea 1. Configurar una instancia de base de datos de RDS**

- Elige el menú **Servicios**, localiza la categoría **Base de datos** y, a continuación, elige **RDS**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.001.png)

- Selecciona **Crear base de datos**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.002.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.003.png)

- En la sección **Configuración**, configura:
  - En **Tipo de motor**, elige **Microsoft SQL Server**.
  - En **Tamaño de la instancia de base de datos**, selecciona **Capa gratuita**
  - Marca la casilla situada junto a **Generación automática de contraseña**.
- Selecciona **Crear base de datos**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.004.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.005.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.006.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.007.png)

- En el banner de la parte superior de la página, selecciona **Ver detalles de credenciales**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.008.png)

**Tarea 2. Descargar e instalar SQL Server Management Studio**

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.009.png)

**Tarea 3. Hacer que la base de datos sea accesible públicamente**

- En la consola de Amazon RDS, selecciona el nombre de la base de datos de SQL Server que creaste.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.010.png)

- En la sección **Conectividad y seguridad**, para **Seguridad**, observa que **Accesibilidad pública** está actualmente establecida en **No**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.011.png)**


- Para cambiar esta configuración, selecciona **Modificar** en la parte superior de la página.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.012.png)

- Desplázate hacia abajo hasta la sección **Conectividad** y amplía **Configuración adicional**.
- En **Acceso público**, selecciona **Accesible públicamente**.
- Desplázate hasta la parte inferior de la página y selecciona **Continuar**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.013.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.014.png)

- En la sección **Programación de modificaciones**, para **Cuándo aplicar modificaciones**, selecciona **Aplicar inmediatamente**.
- Selecciona **Modificar la instancia de base de datos**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.015.png)

**Tarea 4. Actualizar tu grupo de seguridad de VPC**

- Copia el valor de **IPv4** en un editor de texto para utilizarlo más adelante en este laboratorio.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.016.png)

- Elige el nombre de la base de datos que has creado.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.017.png)

- En la sección **Conectividad y seguridad**, bajo **Grupos de seguridad de VPC**, elige el nombre del grupo de seguridad.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.018.png)

- En la página **Grupos de seguridad**, selecciona la pestaña **Reglas de entrada**.
- Selecciona **Editar reglas de entrada** y después **Añadir regla**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.019.png)

- En la página **Grupos de seguridad**, selecciona la pestaña **Reglas de entrada**.
- Selecciona **Editar reglas de entrada** y después **Añadir regla**.
- En **Tipo**, elige **MSSQL**.
- En **Fuente**, selecciona **Personalizada** e introduce tu dirección IP o la dirección IP de la instancia de WindowsWorkstation en el cuadro de texto.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.020.png)

**Tarea 5. Conectarse a la instancia de base de datos**

- Elige el nombre de la base de datos que has creado.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.021.png)

- En la pestaña **Conectividad y seguridad**, copia el valor de **Punto de enlace** a un editor de texto.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.022.png)

- En **Nombre de servidor**, introduce el valor del punto de enlace de la base de datos que has copiado.
- Al final del valor del punto de enlace, añade una coma (,) y el número de puerto (el número de puerto predeterminado es **1433**).
- En **Autenticación**, selecciona **Autenticación de SQL Server**.
- En **Iniciar sesión**, introduce el nombre de usuario de la instancia de base de datos.
  - También se le denomina nombre de usuario del administrador. El valor predeterminado es **admin**.
- En **Contraseña**, introduce la contraseña que has copiado para la instancia de base de datos.
- Selecciona **Conectar**.

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.023.png)

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.024.png)

**Tarea 6. Explorar la estructura de la base de datos relacional**

![](Aspose.Words.bdd961be-cda2-4675-9fac-e6352844873f.025.png)

**¡Excelente!**

