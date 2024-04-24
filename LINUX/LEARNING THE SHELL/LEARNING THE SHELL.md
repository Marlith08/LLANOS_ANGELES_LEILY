# **<p align="center">LEARNING THE SHELL</p>**
# **🐚 INTRODUCCIÓN AL SHELL 🐚**

El Shell es una interfaz de línea de comandos que nos permite interactuar con el sistema operativo de nuestra computadora mediante el uso de comandos de texto. A través del Shell, podemos ejecutar diversas tareas como navegar por el sistema de archivos, manipular archivos y directorios, ejecutar programas y automatizar tareas mediante scripts.

En este archivo, exploraremos los conceptos básicos del Shell y aprenderemos a utilizar algunos de los comandos más comunes. Desde la navegación por el sistema de archivos hasta la manipulación de archivos y la redirección de entrada/salida, este documento proporcionará una guía paso a paso para familiarizarse con el uso del Shell en entornos Unix y Unix-like.

¡Sigue leyendo para descubrir cómo aprovechar al máximo el poder del Shell y mejorar tu flujo de trabajo en la terminal! 🚀

## **Contenido:**

## 1. **What is “the Shell”?**

Ingresamos a la terminar y tenemos en cuenta el aviso de Shell donde contine nuestro nombre de usuario y el nombre de la máquina, asimismo el signo dólar.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.001.png)

Verificamos si todo está correcto, por lo cual ingresamos cualquier palabra y nos debe de retornar error:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.002.png)

Procedemos a presionar la tecla de flecha hacia arriba

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.003.png)

Presionamos la tecla de flecha hacia abajo

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.004.png).

También podemos hacer uso de las flechas a la izquierda y derecha, estos nos permiten desplazarnos en la línea de comando.

Hacemos uso de Ratón

-Copiar texto:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.005.png)

## 2. **Navigation**
- **Pwd:**

Utilizamos pwd para ver el nombre del directorio que estamos utilizando.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.006.png)

- **ls:**

Usamos el comando ls para listar los archivos en el directorio de trabajo.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.007.png)

- **cd**

Usamos cd para cambiar el directorio de trabajo.

**Nombres de ruta absolutos:**

En este caso comienzan con el directorio de raíz y sigue el árbol cd /hasta completar la ruta al archivo deseado.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.008.png)

**Nombres de rutas relativos:**

En esta ruta comienza desde el directorio, donde se utiliza las notaciones especiales de “.” (directorio de trabajo) y “..” (directorio principal)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.009.png)

Para caso anterior realizamos una ruta más corta cd con el directorio de trabajo.

Atajos:

Con cd cambiamos de directorio de trabajo a nuestro directorio principal.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.010.png)

## 3. **Looking Around**
- ls:

Es utilizado para enumerar el contenido de un directorio, puede ser utilizado de las siguientes formas:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.011.png)

- **ls /bin**: enumera los archivos en el /bin directorio

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.012.png)

- **ls -l:** enumera los archivos en el directorio de trabajo en formato largo

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.013.png)

- **ls -l /etc /bin:** enumera los archivos en el /bin y el /etc directorio de formato largo.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.014.png)

- **ls -la ..:** Enumera todos los archivos en el padre de trabajo directorio en formato largo

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.015.png)

Una mirada más cercana a formato largo:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.016.png)

En este caso podemos observar los siguientes (recorrido de derecha a izquierda:

- **Nombre del archivo:** Nos brinda el nombre del archivo o directorio.
- **Tiempo de modificación:** Nos muestra la última vez que se modificó el archivo, si la modificación es de más de 6 meses, se muestra el año.
- **Tamaño:** El archivo en bytes
- **Grupo:** El grupo que tienen permisos al archivo.
- **Propietario:** Nombre del usuario
- **Permiso de archivo:** Acceso al archivo. “\_”(ordinario), “d”(directorio)

- **less:**

Es un programa que nos permite ver archivos de texto

- **Sintaxis:**

less archivo\_comand

- **Comandos:**
- **Page Up or b:** Desplace hacia atrás una página

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.017.png)

- **Page Down or space:** Desplace hacia adelante una página

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.018.png)

- **G:** Vaya al final del archivo del texto

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.019.png)

- **1G:** vaya al principio del archivo de texto

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.020.png)

- **/characters:** busque en el archivo de texto una ocurrencia, de los caracteres especificados

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.021.png)

- **N:** repita la búsqueda anterior

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.022.png)

- **H:** mostrar una lista completa menos comandos y opciones

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.023.png)

- **Q:** salir

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.024.png)

- **file:**

Examina un archivo y nos dirá que tipo de archivo es.

- **sintaxis:**

file name\_of\_file

Puede reconocer la mayoría de los tipos de texto

**Ejemplo:**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.025.png)

En este caso no se muestra nada, porque no hemos subido ningún archivo.

## 4. **A Guideed Tour**
- **cd:** permite cambiar de directorio.
- **ls:** para enumerar el contenido del directorio.
- **file** : para determinar su conenido de un archivo interesante
- **less :** para ver archivos de texto

**Directorios:**

- **/**  : directorio raíz donde el sistema del archivo comienza

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.026.png)

- **/boot** : es donde el kernel y archivos se guardan.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.027.png)

Y si con los demás comandos.

En el casos de /lb, me sale error

Para crear enlaces simbólicos, utilizamos el ln comando

## 5. **Manipulating Files**
- **cp-** : copia archivos y directorios
- **mv** : mover o cambiar el nombre de archivos y directorios
- **rm**: eliminar archivos y directorios
- **mkdir** : crea directorios

**Wldcards:**

Contamos con los comandos:

- **\***

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.028.png)

- **?** 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.029.png)

- **[characters]**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.030.png)

- **¡[¡characters]**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.031.png)

Resumen de comodines y sus significados

**Patrones**

- **\***
- **g\***
- **b\*.txt**
- **Data???**
- **[abc]\***
- **[[:upper:]]\***
- **BACKUP.[[:digit:]][[:digit:]]**
- **\*[![:lower:]]**

Ejemplos de coincidencia de comodines

- **Cp:** copia del programa archivos y directorios (copia un solo archivo)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.032.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.033.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.034.png)

- **Ejemplos del comando cp**
- **Mv.** Se mueve o cambia de nombre archivos y directorios.
- **Mv incluyen:**
- **Mv file1 file2:** 
- **Mv -i file1 fil2**
- **Mv file1 file2 dir1**
- **Mv dir1 dir 2**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.035.png)

- **Ejemplos del comando mv**
- **Rm:** elimina archivos y directorios
- **rm file1 file2:** Elimina el archivo1 y archivo 2
- **rm -i file1 file2:** como arriba, el usuario se solicita antes de eliminar cada archivo
- **rm -r dir1 dir 2:** Directorio dir1 y 2 se eliminan juntos

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.036.png)

- **mkdir:** se utiliza el comando para crear directorios
- **Comandos wildcards	:**
- **cp \*.txt text\_files:** Copia todos los archivos en el directorio de trabajo actual
- **mv dir ../\*.bak dir2:** Mueve el subdirectorio dir 1 y todos los archivos que terminan en “.bak”
- **rm \*~:** Elimina todos los archivos en el directorio d etrabajo actual

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.037.png)

## 6. **Working with Commands**

- **Type:** Mostrar información sobre el tipo de comando 
- **Which:** localizar un comando
- **Help**: Mostrar página de referencia para Shell builtin
- **Man**: Mostrar una referencia de comando en línea

**Identificar comandos:**

- **Type** 

Sintaxis type comando 

Mostramos tres comandos diferentes:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.038.png)

- **Which**

Determina la ubicación exacta de un programa ejecutable

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.039.png)

- **Help**

Tiene una instlación de ayuda incorporada para cada uno de los Shell construidos.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.040.png)

**#**Cuando aparecen corchetes en la descripción de un comando sintaxis, indica elementos opcionales.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.041.png)

- **Man:** se utiliza para ver el programa de paginación

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.042.png)

## 7. **I/O Redirection**

Salida estándar 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.043.png)

- **Sobreescritura**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.044.png)

- **Entrada estándar:**

La entrada estandar obtiene su contenido del teclado

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.045.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.046.png)

- **Tuberías**

Redirecciona la entrada y salida y conecta múltiples comandos

- **ls -l | les** 

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.047.png)

- **Comandos:**
- **Ls -lt | head:** muestra los 10 primeros elementos

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.048.png)

- **Du | sort -nr:** muestra la lista de ordenadores desde muy grande a más pequeño.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.049.png)

- **Find . +type f +print | wc -1 :** muestra el número total de archivos

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.050.png)

**Filters:**

Toman entrada estándar y realiza una operación sobre el y envía resultados a la salida estándar.

**Comandos:**

-sort :  Ordena la entrada y emite el resultado de la salida estándar 

-uniq: Elimina líneas duplicadas de datos.

-grep : Examina cada línea de dato que recibe de entrada y salida.

-fmt: Lee texto de entrada y salida estándar.

-pr : Toma entrada de texto de entrada estándar y divide los datos en páginas con saltos de página, encabezados y pies

-head : sale las primer líneas de entrada

-tail: Sale las últimas líneas de entrada

-tr: Traduce personajes

-sed: Realiza traducciones de texto amplia

-awk : expresión para construir

## 8. **Expansion:**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.051.png)

Implica que coincide con cualquier personaje en un nombre de archivo

- **Expansión de nombre de ruta**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.052.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.053.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.054.png)

- **Expansión tilde**

Se expnde el nombre del directorio de inicio del usuario

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.055.png)

Si el usuario “foo” tiene cuenta entonces

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.056.png)

- **Expresión aritmética:**

**Sintaxis**

**&((expresión))**

- **Expresiones anidadas**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.057.png)

- Con paréntesis individual

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.058.png)

- **División de enteros y su resto:**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.059.png)

- **Brace Expansion**

**Nos permite crear múltiples cadenas de texto:**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.060.png)

**Rango de caracteres individuales**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.061.png)

**Letras en orden inverso**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.062.png)

**Los limites pueden estar anidados**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.063.png)

Nos permite crear lista de archivos o directorios.

Ejemplo:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.064.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.065.png)

- **Parameter Expansion**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.066.png)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.067.png)

- **Quoting**

Nos permiten controlar lo que hemos venido realizando

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.068.png)

- **Doubles Quotes**

Podemos realizar citas dobles de las siguientes maneras.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.069.png)

- **Single Quotas**

Para suprimir las expansiones usamos comillas individuales

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.070.png)

- **Escaping Characters**

Para citar un solo personaje y usamos escape para eliminar el significado

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.071.png)

- **More backslash Tricks**

Usamos las opciones de formulario largo puede hacer una sola comando en línea muy larga, para lo cual usamos salto de línea.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.072.png)

También se puede usar los siguiente:

- **\n :** agregan líneas en blanco
- **\t :** inserta pestaña horizontal en el texto
  **\a** : hacer nuestra terminal pita
- **\\ :** insertar reacción inversa
- **\f :** enviar a la impresora

## 9. **Permissions**

Implica que más de un usuario puede controlar u operar una computadora al mismo tiempo

- **chmod:** modifica derechos de acceso a archivos

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.073.png)

- **Su:** temporalmente convierte al superusuario
- **Sudo:** temporalmente convierte al super usuario
- **Chown** cambiar propiedad del archivo
- **Chgrp:** cambiar a propiedad del grupo de archivo

**File permissions:**

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.074.png)

**Valor y su significado**

- 777 à(rwxrwxrwx)
- 755 à(rwxr-xr-x)
- 700 à(rwx-----)
- 666 à(rw-rw-rw-)
- 644 à(rw-r-r-)
- 600 à(rw-----)

**Permisos de directorio**

- r- : permite enumerar el contenido del directorio
- w- : Permite crear archivos dentro del directorio, eliminad o renombrado
- x- : Permite ingresar un directorio (i.e.cd dir)

**Convertirse en Superusuario por un corto de tiempo**

Nos permite realizar tareas importantes de administración del sistema:

- **Su**

Para tener más privilegios

- **Sudo some\_command**

Para tener en cuenta desde la raíz 

- **Sudo -i**

Cambio de propiedad de archivos:

Para este caso podemos usar **chown**

Cambio de propiedad de  grupo:

Usamos **chgrp**

## 10. **Job Control**

Comandos:

- **ps-** lista el proceso que se ejecutan en el sistema
- **kill-** enviar una señal a uno o más procesos (generalmente a "matar" un proceso)
- **jobs-** una forma alternativa de enumerar sus propios procesos
- **bg-** poner un proceso en el fondo
- **fg-** poner un proceso en primer plano

Ejemplo:

**Xload** nos muestra gráfico que representa la carga del sistema

Poner un programa en el fondo

Nos permite regresar, puesto que el proceso se puso en el fondo.

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.075.png)

- **Listado de procesos en ejecución:**

Podemos usar **jobs** o **ps** para mostrar la lista de procesos que hemos lanzado

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.076.png)

- **Matar un proceso:**

Se usa para deshacer un proceso que no responde:

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.077.png)

**Kil**l es utilizado para matar procesos, donde su propósito es enviar señales a procesos

Señales admitidas

- **1 ASUSPIRAR: Cuelga la seña**
- **2 ASIGNT: interrumpe la señal**
- **15 ASIGTERM: Señala la terminación**
- **9 ASIGKILL: Mata la señal**

Se usa **ps** para obtener la identificación del proceso (PID)

![](https://github.com/Marlith08/LLANOS_ANGELES_LEILY/blob/main/LINUX/LEARNING%20THE%20SHELL/Imagenes/Aspose.Words.cb406443-52a1-43f4-93f0-7e4f3122d1ce.078.png)
