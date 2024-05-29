# ﻿**Laboratorio del módulo 7: Introducción a IAM**

## **Tarea 1. Explorar usuarios y grupos**

- En el menú **servicios** seleccionamos **IAM**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.001.png)

- En el panel de la izquierda seleccionamos **Usuarios**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.002.png)

- Seleccionamos el nombre **user-1**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.003.png)

- Selecciona la pestaña **Grupos**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.004.png)

- Selecciona la pestaña **Credenciales de seguridad**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.005.png)

- En el panel de navegación de la izquierda, selecciona **Grupos de usuarios**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.006.png)

- Selecciona el nombre del grupo **EC2-Support**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.007.png)

- Selecciona la pestaña **Permisos**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.008.png)

- En **Nombre de la política**, elige el enlace de la política **AmazonEC2ReadOnlyAccess**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.009.png)

- Selecciona la pestaña **{} JSON**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.010.png)

- Los enunciados de una política de IAM tienen la siguiente estructura básica:
  - **Efecto** nos indica si *Permitir* o *Denegar* los permisos.
  - **Acción** especifica las llamadas a la API que se pueden realizar desde un servicio de AWS (por ejemplo, *cloudwatch:ListMetrics*).
  - **Recurso** define el alcance de las entidades cubiertas por la regla de la política (por ejemplo, un bucket de Amazon Simple Storage Service [Amazon S3] o una instancia de Amazon EC2 específicos; un asterisco [\*] significa *cualquier recurso*).

- En el panel de navegación de la izquierda, selecciona **Grupos de usuarios**.


![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.011.png)

- Elige el nombre del grupo **S3-Support**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.012.png)

- Selecciona la pestaña **Permisos**.
- En **Nombre de la política**, elige el enlace de la política **AmazonS3ReadOnlyAccess**.


![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.013.png)

- Selecciona la pestaña **{} JSON**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.014.png)

- En el panel de navegación de la izquierda, selecciona **Grupos de usuarios**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.015.png)

- Elige el nombre del grupo **EC2-Admin**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.016.png)

- Selecciona la pestaña **Permisos**.
- En **Nombre de la política**, elige el nombre de la política **EC2-Admin-Policy**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.017.png)

- Selecciona la pestaña **JSON**.
- En la parte inferior de la pantalla, selecciona **Cancelar** para cerrar la política.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.018.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.019.png)

### **Escenario empresarial**

|**Usuario**|**En el grupo**|**Permisos**|
| :- | :- | :- |
|**user-1**|**S3-Support**|**Acceso de solo lectura a Amazon S3**|
|**user-2**|**EC2-Support**|**Acceso de solo lectura a Amazon EC2**|
|**user-3**|**EC2-Admin**|**Ver, iniciar y detener instancias de Amazon EC2**|
**


## **Tarea 2. Añadir usuarios a grupos**

### **Añadir a user-1 al grupo S3-Support**

- En el panel de navegación izquierdo, selecciona **Grupos de usuarios**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.020.png)

- Elige el nombre del grupo **S3-Support**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.021.png)

- En la pestaña **Usuarios**, elige **Añadir usuarios**.
- Selecciona **user-1** y después **Añadir usuarios**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.022.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.023.png)

### **Añadir a user-2 al grupo EC2-Support**

- En el panel de navegación de la izquierda, selecciona **Grupos de usuarios**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.024.png)

- Utiliza lo aprendido de los pasos anteriores para añadir a *user-2* al grupo *EC2-Support*.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.025.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.026.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.027.png)

### **Añadir a user-3 al grupo EC2-Admin**

- Utiliza lo aprendido de los pasos anteriores para añadir a *user-3* al grupo *EC2-Admin*.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.028.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.029.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.030.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.031.png)

- En el panel de navegación de la izquierda, selecciona **Grupos de usuarios**.
- Cada grupo debe tener un **1** en la columna **Usuarios**. Indica el número de usuarios de cada grupo.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.032.png)

## **Tarea 3. Iniciar sesión y probar usuarios**

### **Obtener la URL de inicio de sesión de la consola**

- En el panel de navegación de la izquierda, selecciona **Panel**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.033.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.034.png)

### **Probar permisos de user-1**

- En el panel de navegación de la izquierda, selecciona **Panel**.
- Inicia sesión con las siguientes credenciales:
  - **Nombre de usuario de IAM:** user-1
  - **Contraseña:** Lab-Password1

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.035.png)

- Selecciona el menú **Servicios** y luego **S3**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.036.png)

- Elige el nombre de uno de los buckets y explora el contenido.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.037.png)

- Selecciona el menú **Servicios** y después **EC2**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.038.png)

- En el panel de navegación izquierdo, selecciona **Instancias**.
- No aparece ninguna instancia.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.039.png)

- En primer lugar, cierra la sesión de *user-1* en la consola:
  - En la esquina superior derecha de la página, selecciona **user-1**.
  - Selecciona **Cerrar sesión**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.040.png)

### **Probar permisos de user-2**

- Inicia sesión con las siguientes credenciales:
  - **Nombre de usuario de IAM:** user-2
  - **Contraseña:** Lab-Password2

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.041.png)

- Selecciona el menú **Servicios** y después **EC2**.
- En el panel de navegación de la izquierda, selecciona **Instancias**.
- Ahora puedes ver una instancia de EC2

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.042.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.043.png)

- Selecciona el menú **Estado de la instancia** y, a continuación, selecciona **Detener instancia**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.044.png)

- Aparece un mensaje de error que indica que *no estás autorizado a realizar esta operación*.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.045.png)

- Selecciona el menú **Servicios** y luego **S3**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.046.png)

- Un mensaje de error indica que *no tienes permisos para enumerar buckets* porque *user-2* no tiene permiso para usar Amazon S3.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.047.png)

- En primer lugar, cierra la sesión de *user-2* en la consola:
  - En la esquina superior derecha de la página, selecciona **user-2**.
  - Selecciona **Cerrar sesión**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.048.png)

### **Probar permisos de user-3**

- Inicia sesión con las siguientes credenciales:
  - **Nombre de usuario de IAM:** user-3
  - **Contraseña:** Lab-Password3

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.049.png)

- Selecciona el menú **Servicios** y después **EC2**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.050.png)

- En el panel de navegación de la izquierda, selecciona **Instancias**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.051.png)

- Selecciona el menú **Estado de la instancia** y, a continuación, selecciona **Detener instancia**.
- Para confirmar que quieres detener la instancia, selecciona **Detener**.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.052.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.053.png)

- Esta vez, la acción se realiza correctamente porque *user-3* tiene permiso para detener instancias de EC2.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.054.png)

- Cierra la ventana del navegador privado.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/AWS/LABORATORIO_DEL_MODULO_7/Imagenes/Aspose.Words.4a62318b-2e86-4300-bfb1-27fa99ca0cb9.055.png)

### **¡EXCELENTE!**



