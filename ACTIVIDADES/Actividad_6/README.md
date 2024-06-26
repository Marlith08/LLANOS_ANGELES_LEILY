﻿![ref1](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.001.png)
 <p align="center">
 **Departamento Académico de Ingeniería**
 </p>

**C8280 -Comunicación de Datos y Redes**

**Actividad 6: Crear una red con un switch y un router - Modo**

**Físico**
# ` 	`**Topología**
![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.002.png)
# ` 	`**Tabla de asignación de direcciones**

<table><tr><th valign="bottom"><b>Dispositivo</b></th><th valign="bottom"><b>Interfaz</b></th><th valign="bottom"><b>Dirección IP / Prefijo</b></th><th><b>Puerta de enlace predeterminada</b></th></tr>
<tr><td rowspan="7" valign="top"><p><b>R1</b></p><p><b><i>R1</i></b></p><p><b><i>R1</i></b></p><p><b><i>R1</i></b></p><p><b><i>R1</i></b></p><p><b><i>R1</i></b></p><p><b>S1</b></p></td><td rowspan="3" valign="bottom"><p>G0/0/0</p><p><i>G0/0/0</i></p><p><i>G0/0/0</i></p></td><td valign="top">192\.168.0.1 /24</td><td rowspan="3" valign="top"><p>N/D</p><p><i>N/D</i></p><p><i>N/D</i></p></td></tr>
<tr><td valign="top">2001:db8:acad: :1/64</td></tr>
<tr><td valign="top">fe80::1</td></tr>
<tr><td rowspan="3" valign="bottom"><p>G0/0/1</p><p><i>G0/0/1</i></p><p><i>G0/0/1</i></p></td><td valign="top">192\.168.1.1 /24</td><td rowspan="3" valign="top"><p>N/D</p><p><i>N/D</i></p><p><i>N/A</i></p></td></tr>
<tr><td valign="top">2001:db8:acad:1: :1/64</td></tr>
<tr><td valign="top">fe80::1</td></tr>
<tr><td valign="top">VLAN 1</td><td valign="top">192\.168.1.2 /24</td><td valign="top">192\.168.1.1</td></tr>
<tr><td rowspan="2" valign="bottom"><p><b>PC-A</b></p><p><b><i>PC-A</i></b></p></td><td rowspan="2" valign="bottom"><p>NIC</p><p><i>NIC</i></p></td><td valign="top">192\.168.1.3 /24</td><td valign="top">192\.168.1.1</td></tr>
<tr><td valign="top">2001:db8:acad:1: :3/64</td><td valign="top">fe80::1</td></tr>
<tr><td rowspan="2" valign="bottom"><p><b>PC-B</b></p><p><b><i>PC-B</i></b></p></td><td rowspan="2" valign="bottom"><p>NIC</p><p><i>NIC</i></p></td><td valign="top">192\.168.0.3 /24</td><td valign="top">192\.168.0.1</td></tr>
<tr><td valign="top">2001:db8:acad: :3/64</td><td valign="top">fe80::1</td></tr>
</table>
# **Objetivos**
**Parte 1: Configurar la topología**

**Parte 2: Configurar los dispositivos y verificar la conectividad**

**Parte 3: Mostrar información del dispositivo**
# **Aspectos básicos/situación**
En esta actividad de Packet Tracer Modo Físico, conectará el equipo tal como se muestra en el diagrama de topología. Luego, configura los dispositivos según la tabla de direccionamiento. Cuando se haya guardado la configuración, la verificará probando la conectividad de red.

Una vez que los dispositivos estén configurados y que se haya verificado la conectividad de red, utilizará los comandos del IOS para recuperar la información de los dispositivos y responder preguntas sobre los equipos de red.

Esta actividad brinda la ayuda mínima con los comandos que se necesitan para configurar el router.
# **Instrucciones**
## **1 . Configura la topología de red**
1. Mueva el router y el switch requeridos del **Estante** al **Rack**.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.003.png)

1. Mueva los PCs requeridos del **Estante** a la **Mesa**.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.004.png)

1. Conecta los dispositivos como se muestra en la **Topologia** y en la **Tabla de asignación de direcciones**.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.005.png)

1. Encienda todos los dispositivos.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.006.png)
## **2. Configurar los dispositivos y verificar la conectividad**
En esta parte deberás configurar la topología de la red y los parámetros básicos, como las direcciones IP de las interfaces, el acceso de los dispositivos y las contraseñas. Consulte la **Topología** y la **Tabla de asignación de direcciones** que se encuentran al inicio de esta actividad para conocer los nombres de los dispositivos y la información de las direcciones.

**Asignar información de IP estática a las interfaces de la PC**

1. Configura la dirección IP, la máscara de subred y los parámetros del gateway predeterminado en la PC-A.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.007.png)

1. Configura la dirección IP, la máscara de subred y los parámetros del gateway predeterminado en la PC-B.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.008.png)

1. En una ventana con el símbolo del sistema en la PC-A, haga ping a la PC-B.

   Pregunta: ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.009.png)

   ¿Por qué los pings no fueron correctos?

   Porque aún falta configurar los switches y routers para que establezca una conexión.

**Configura el router**

1. Acceda al router mediante el puerto de consola y habilite el modo EXEC con privilegios.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.010.png)

1. Ingresa al modo de configuración.
1. ![ref2](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.11.png)

1. Asigna el nombre de dispositivo al router.

   ![ref3](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.012.png)

1. Asigna **class** como la contraseña cifrada del modo EXEC privilegiado.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.013.png)

1. Asigna **cisco** como la contraseña de la consola y habilite el inicio de sesión.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.014.png)

1. Asigne **cisco** como la contraseña de vty y habilite el inicio de sesión.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.015.png)

1. Encripta las contraseñas de texto sin formato.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.016.png)

1. Crea un aviso que advierta a todo el que acceda al dispositivo que el acceso no autorizado está prohibido.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.017.png)

1. Configura y activa las dos interfaces en el router.

   **INTERFAZ G0/0/0**

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.018.png)

   **INTERFAZ G0/0/1**

   ![Pantalla de computadora con letras Descripción generada automáticamente con confianza media](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.019.png)

1. Configura una descripción de interfaz para cada interfaz e indique qué dispositivo está conectado.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.020.png)

5. Para habilitar el enrutamiento IPv6, ingrese el comando **ipv6 unicast-routing**.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.021.png)

5. Guardar la configuración en ejecución en el archivo de configuración de inicio

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.022.png)

5. Configura el reloj en el router.

   **Nota:** Utiliza el signo de interrogación (**?**) para poder determinar la secuencia correcta de parámetros necesarios para ejecutar este comando.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.023.png)

*Cerrar la ventana de configuración*

5. En una ventana con el símbolo del sistema en la PC-A, haga ping a la PC-B.

   ![Calendario Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.024.png)

   **Nota**: Si los pings no son correctos, es posible que debas desactivar el Firewall.Pregunta:

   ¿Fueron correctos los pings? Explica.

   Sí, fueron correcto porque hemos realiza una buna configuración tanto a la PC-A, PC-B como al router con sus diferentes interfaces, direcciones ip, Subnet Mask.

**Configura el switch.**

En este paso, configura el nombre de host, la interfaz de VLAN 1 y su puerta de enlace predeterminada.

*Abrir la ventana de configuración*

1. Acceda al switch mediante el puerto de consola y habilite al modo EXEC con privilegios.

   ![Interfaz de usuario gráfica Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.025.png)

1. Ingresa al modo de configuración.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.026.png)

1. Asigna un nombre de dispositivo al switch.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.027.png)

1. Configura y activa la interfaz VLAN en el switch S1.
1. ![Captura de pantalla de un celular Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.028.png)Configura la puerta de enlace predeterminada para el switch S1.

   ![Una captura de pantalla de un celular con texto e imagen Descripción generada automáticamente con confianza media](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.029.png)

9. Guarda la configuración en ejecución en el archivo de configuración de inicio

   ![Una captura de pantalla de un celular con texto e imagen Descripción generada automáticamente con confianza baja](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.030.png)

**Verifica la conectividad de extremo a extremo.**

9. Desde la PC-A, haga ping a la PC-B.

   ![Imagen que contiene Calendario Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.031.png)

9. Desde S1, ping PC-B.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.032.png)

Todos los pings deben tener éxito.

*Cerrar la ventana de configuración*
## **3. Muestra la información del dispositivo**
En la parte 3, utilizará los comandos **show** para recuperar información del router y del switch.

**Muestra la tabla de routing en el router.**

1. Utiliza el comando **show ip route** en R1 para responder las preguntas siguientes.

   ![Interfaz de usuario gráfica, Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.033.png)

   *Abra la ventana de configuración* Preguntas:

   ¿Qué código se utiliza en la tabla de enrutamiento para indicar una red conectada directamente?

   Se usa el código C

***Escriba sus respuestas aquí.***

¿Cuántas entradas de ruta están codificadas con un código C en la tabla de enrutamiento?

2

***Escriba sus respuestas aquí.***

¿Qué tipos de interfaces están asociadas a las rutas con código C?

`		`g0/0/0  y g0/0/1

***Escriba sus respuestas aquí.***

1. Usa el comando **show ipv6 route** en R1 para ver las rutas de IPv6.

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.034.png)

**Muestra la información de la interfaz en el R1.**

1. Utiliza el comando **show interface g0/0/1** para responder las preguntas siguientes.

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.035.png)

   ¿Cuál es el estado operativo de la interfaz G0/0/1?

   El estado es à CONNECTED

   ***Escriba sus respuestas aquí.***

   ¿Cuál es la dirección de control de acceso a los medios (MAC) de la interfaz G0/0/1?

   La dirección de control de acceso a los medios (MAC) de la interfaz GigabitEthernet0/0/1 es:

0060\.4731.8102

***Escriba sus respuestas aquí.***

¿Cómo se muestra la dirección de Internet en este comando?

La dirección de Internet (o dirección IP) se muestra en este comando en la línea que comienza con "Internet address", seguido de la dirección IP y la máscara de subred en formato CIDR. En este caso, la dirección de Internet es: 192.168.1.1/24***Escriba sus respuestas aquí.***

1. Para obtener información sobre IPv6, escribe el comando **show ipv6 interface *interface.***

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.036.png)

**Muestra una lista de resumen de las interfaces del router y del switch**

Existen varios comandos que se pueden utilizar para verificar la configuración de interfaz. Uno de los más útiles es el comando **show ip interface brief**. El resultado del comando muestra una lista resumida de las interfaces en el dispositivo y brinda información inmediata sobre el estado de cada interfaz.

1. Ingresa el comando **show ip interface brief** en R1.

   R1# **show ip interface brief**

   ![](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.037.png)

1. Ingresa el comando **show ipv6 interface brief** en R1 para ver información de IPv6 de las interfaces.

   R1# **show ipv6 interface brief**

   ![Texto Descripción generada automáticamente](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.038.png)

*Cerrar la ventana de configuración*

1. Ingresa el comando **show ip interface brief** en S1.

   *Abrir la ventana de configuración* S1# **show ip interface brief**

   ![Interfaz de usuario gráfica, Texto Descripción generada automáticamente con confianza media](https://github.com/Marlith08/CDR_GRUPO_4/blob/main/Actividades/Actividad_6/IMAGENES/Aspose.Words.b3ee5210-5704-4e3c-90f1-bc0ba5b6ce3a.039.png)

*Cierre la ventana de configuración*
# **Preguntas**
1. Si la interfaz G0/0/1 se mostrará administratively down, ¿qué comando de configuración de interfaz usaría para activar la interfaz?

   Usaría no shutdown

   ***Escriba sus respuestas aquí.***

1. ¿Qué ocurriría si hubiera configurado incorrectamente la interfaz G0/0/1 en el router con una dirección IP 192.168.1.2?

   Errores con las direcciones IP, donde la máscara de Subred sería incorrecta y no podríamos hacer conexiones entre los dispositivos.

   ***Escriba sus respuestas aquí.***
Comunicación de Datos y Redes
