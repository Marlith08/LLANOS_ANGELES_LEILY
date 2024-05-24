**LABORATORIO DEL MÓDULO 5: USO DE CLOUDFRONT COMO CDN PARA UN SITIO WEB.**

**Tarea 1. Crear un bucket de S3 mediante AWS CLI**

**1.-Ingresamos a servicios y seleccionamos cloudshell**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.001.png)

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.002.png)

**Tarea 2. Añadir una política de bucket**

**2.-Seleccionamos servicios y abrimos S3**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.003.png)

**3.-Click en el bucket creado.**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.004.png)

**4.-Click en permisos**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.005.png)

**5.-Seleccionamos editar en bloquear acceso público**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.006.png)

**6.-Click para desactivar el bloqueo**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.007.png)

**7.-Guardamos cambios**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.008.png)

**8.-Seleccionamos editar en propiedad de objeto**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.009.png)

**9.-Seleccionamos ACL habilitadas**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.010.png)

**10.-Guardamos cambios**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.011.png)

**11.-Seleccionamos editar en política de bucket**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.012.png)

**12.-Colocamos la política de bucquet**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.013.png)

**Guardamos cambios**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.014.png)

**Tarea 3. Subir un documento HTML**

**13.-Selecciona la pestaña Objetos**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.015.png)

**14.-Selecciona cargar**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.016.png)

**15.-Subimos el archivo index**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.017.png)

**16.-Brindamos los permisos**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.018.png)

**17.-Cargamos**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.019.png)

**Tarea 4. Probar el sitio web**

**18.-Seleccionamos la pestaña propiedades**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.020.png)

**19.-En alojamiento de sitios de web estáticos seleccionamos editar**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.021.png)

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.022.png)

**20.-Guardamos**

**Tarea 5. Crear una distribución de CloudFront para servir al sitio web**

**21.-Seleccionamos cloudfront**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.023.png)

**22.-Seleccionamos…**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.024.png)

**23.-Seleccionamos el punto de enlace de nuestro bucket creado.**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.025.png)

**24.-Seleccionamos HTTP Y HTTPS en política de protocolo**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.026.png)

**25.-Seleccionamos no habilitar protección de seguridad**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.027.png)

**26.-Creamos distribución**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.028.png)

**Cargamos nuestra imagen en el bucket**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.029.png)

**27.-En un block de notas implementamos un archivo html con lo que deseamos mostrar en el navegador.**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.030.png)

**28.-Abrimos el archivo.**

![](Aspose.Words.f59b07ce-47bc-4763-a65e-959466a7bdff.031.png)

