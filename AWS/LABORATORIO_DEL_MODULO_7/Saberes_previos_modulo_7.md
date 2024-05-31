# ﻿**MODULO 7: Seguridad I**

## **Terminología Tecnológica**

|**Término**|**Definición**|
| :- | :- |
|**AWS Identity and Access Management (IAM)**|Aplica controles para usuarios que necesitan acceder a recursos informáticos.|
|**Rol**|Identidad de IAM con permisos específicos.|
|**Usuario**|Entidad creada en AWS para representar a personas o aplicaciones que interactúan con AWS. Compuesto por nombre y credenciales.|
|**Grupo de seguridad**|Actúa como firewall virtual para controlar tráfico entrante y saliente en instancias.|
|**Política**|Objeto de AWS que define permisos cuando se asocia a una identidad o recurso. Evaluada por AWS en solicitudes de entidades principales.|
|**Amazon Inspector**|Ayuda a identificar vulnerabilidades de seguridad y desviaciones de prácticas recomendadas en aplicaciones antes y durante la ejecución.|
|**Grupo de IAM**|Conjunto de usuarios de IAM con permisos específicos. Facilita la administración de permisos.|
|**Usuario raíz**|Identidad inicial con acceso total a todos los servicios y recursos de AWS al crear una cuenta.|
|**Credencial**|Verifica la identidad del usuario y su permiso para acceder a recursos solicitados.|
|**Habilitación de Multi-Factor Authentication (MFA)**|Requiere autenticación con dos o más métodos independientes.|
|**Notación de objetos JavaScript (JSON)**|Sintaxis para almacenar e intercambiar datos.|
|**Multi-Factor Authentication (MFA)**|Sistema de seguridad que verifica la identidad mediante múltiples métodos independientes.|

## **Antecedentes y conceptos erróneos:**

Prácticas recomendadas de IAM

1. Bloquee las claves de acceso de usuario raíz de la cuenta de AWS.
- La clave de acceso del usuario raíz de su cuenta de AWS le da acceso completo a todos sus recursos en todos los servicios de AWS, incluso a su información de facturación. No puede reducir los permisos asociados a la clave de acceso de usuario raíz de su cuenta de AWS. Por lo tanto, proteja su clave de acceso de usuario raíz como lo haría con los números de su tarjeta de crédito o cualquier otra información secreta confidencial.

1. Cree usuarios individuales de IAM.
- No utilice las credenciales de usuario raíz de su cuenta de AWS para acceder a AWS, y no dé sus credenciales a ninguna otra persona. En su lugar, cree usuarios individuales para cualquier persona que necesite acceder a su cuenta de AWS.
- Al crear usuarios IAM individuales para las personas que acceden a su cuenta, puede dar a cada usuario de IAM un conjunto exclusivo de credenciales de seguridad. También puede conceder permisos diferentes a cada usuario de IAM. Si es necesario, puede cambiar o revocar los permisos de un usuario de IAM en cualquier momento.

1. Utilice grupos de usuarios para asignar permisos a los usuarios de IAM. 
- En lugar de definir permisos para usuarios individuales de IAM, lo más conveniente es que cree grupos que se relacionen con las funciones del trabajo (administradores, desarrolladores, contadores, etc.). A continuación, defina los permisos pertinentes para cada grupo. Por último, asigne usuarios de IAM a esos grupos. Todos los usuarios de un grupo de IAM heredan los permisos asignados al grupo. De esta forma, puede hacer cambios para todos los miembros de un grupo en un solo lugar.

1. Conceda menos privilegios.
- Cuando cree políticas de IAM, siga los consejos de seguridad estándar de conceder menos privilegios o conceder solo los permisos necesarios para realizar una tarea. Determine qué deben hacer los usuarios (y roles) y, a continuación, cree políticas que les permitan realizar solo esas tareas.

1. Comience a utilizar los permisos con las políticas administradas de AWS.
- Proporcionar a sus empleados solo los permisos que necesitan requiere tiempo y un conocimiento detallado de las políticas de IAM. Si desea comenzar rápidamente, puede utilizar las políticas administradas de AWS para otorgar a sus empleados los permisos que necesitan para comenzar. Estas políticas ya están disponibles en su cuenta, y AWS se encarga de mantenerlas y actualizarlas.
- Las políticas administradas de AWS están diseñadas para proporcionar permisos a muchos casos de uso comunes. Las políticas administradas de AWS le facilitarán la tarea de asignar de los permisos adecuados a los usuarios, grupos de usuarios y roles en lugar de tener que escribir las políticas usted mismo.

1. Valide sus políticas.
- Es una práctica recomendada que valide las políticas que crea. Puede realizar la validación de políticas cuando crea y edita políticas JSON. IAM identifica cualquier error de sintaxis JSON, mientras que IAM Access Analyzer proporciona más de 100 comprobaciones de políticas y recomendaciones procesables para ayudarlo a crear políticas seguras y funcionales.

1. Utilice políticas administradas por el cliente en lugar de políticas en línea.
- En el caso de las políticas personalizadas, le recomendamos que utilice políticas administradas en lugar de políticas en línea. Una ventaja clave del uso de estas políticas es que puede ver todas las políticas administradas en un solo lugar. Las políticas integradas son aquellas que solo existen en una identidad de IAM (usuario, grupo de usuarios o rol). Las políticas administradas son recursos de IAM independientes que se pueden adjuntar a varias identidades.

1. Utilice los niveles de acceso para revisar los permisos de IAM.
- Para mejorar la seguridad de su cuenta de AWS, debe revisar y supervisar periódicamente cada una de sus políticas de IAM. Asegúrese de que sus políticas otorguen la menor cantidad de privilegios necesarios para llevar a cabo solo las acciones necesarias.

1. Configure una política de contraseñas seguras para los usuarios. 
- Si permite que los usuarios cambien sus propias contraseñas, solicite que creen contraseñas seguras y que las cambien regularmente.
- Puede utilizar la política de contraseñas para definir requisitos de contraseña, como la longitud mínima, si requiere caracteres no alfabéticos, con qué frecuencia debe cambiarla, etc.

1. Habilite la MFA. 
- Solicite la autenticación multifactor (MFA) para todos los usuarios de su cuenta. Con la MFA, los usuarios tendrán un dispositivo que generará una respuesta a un desafío de autenticación. Se requieren tanto las credenciales del usuario como la respuesta generada por el dispositivo para completar el proceso de inicio de sesión. Si la contraseña o las claves de acceso de un usuario se ven comprometidas, los recursos de la cuenta seguirán estando seguros gracias al requisito de autenticación adicional.

1. Utilice roles para aplicaciones que se ejecutan en instancias de Amazon EC2.
- Las aplicaciones que se ejecutan en una instancia EC2 necesitan credenciales para acceder a otros servicios de AWS. Para proporcionar credenciales a la aplicación de forma segura, utilice roles de IAM. Un rol es una entidad que tiene su propio conjunto de permisos, pero no es un usuario ni un grupo de usuarios.
- Los roles tampoco tienen su propio conjunto de credenciales permanentes como los usuarios de IAM. En el caso de Amazon EC2, IAM proporciona credenciales temporales a la instancia EC2 de forma dinámica, y estas credenciales cambian automáticamente sin necesidad de que usted las modifique.

1. Utilice roles para delegar permisos.
- No comparta credenciales de seguridad entre cuentas con el fin de permitir que los usuarios de otra cuenta de AWS accedan a los recursos de su cuenta de AWS. En su lugar, use roles de IAM. Puede definir un rol que especifique qué permisos tienen los usuarios de IAM en la otra cuenta. También puede designar qué cuentas de AWS cuentan con los usuarios de IAM que pueden asumir el rol.

1. No comparta claves de acceso.
- Las claves de acceso proporcionan acceso mediante programación a AWS. No comparta estas credenciales de seguridad entre los usuarios de su cuenta de AWS. En el caso de las aplicaciones que necesitan acceso a AWS, configure el programa para recuperar credenciales de seguridad temporales mediante un rol de IAM.

1. Cambie las credenciales regularmente.
- Cambie sus propias contraseñas y claves de acceso con frecuencia y asegúrese de que todos los usuarios de IAM de su cuenta también lo hagan. De esta forma, si una contraseña o clave de acceso se ve comprometida sin su conocimiento, podrá limitar el tiempo de uso de las credenciales para acceder a sus recursos. Puede aplicar una política de contraseñas a su cuenta para exigir que todos los usuarios de IAM cambien sus contraseñas. También puede elegir con qué frecuencia deben hacerlo.

1. Elimine credenciales innecesarias.
- Elimine las credenciales de usuario de IAM (contraseñas y claves de acceso) que no sean necesarias.

1. Utilice las condiciones de la política para obtener mayor seguridad.
- Defina las condiciones en las que las políticas de IAM permiten el acceso a un recurso. Por ejemplo, puede escribir condiciones para especificar un rango de direcciones IP permitidas desde donde debe proceder una solicitud. También puede especificar que una solicitud solo se permita dentro de un intervalo de fechas o de horas especificado. También puede establecer condiciones que requieran el uso de SSL o MFA (autenticación multifactor). Por ejemplo, puede exigir que un usuario se autentique con un dispositivo MFA para poder terminar una instancia de Amazon EC2.

1. Supervise la actividad de su cuenta de AWS.
- Puede utilizar las funciones de registro de AWS para determinar las acciones que realizaron los usuarios en su cuenta y los recursos que se utilizaron. Los archivos de registro muestran la hora y la fecha de las acciones, la IP de origen de una acción, qué acciones fallaron debido a permisos inadecuados y más.

**Identidades de AWS**

Cuando se piensa en IAM en AWS, hay roles, identidades y grupos, y todos ellos se rigen por políticas.

En el nivel más alto se encuentra el *usuario raíz*. Esta es la identidad que creó la cuenta de AWS. El usuario raíz tiene acceso a todos los aspectos de AWS y actúa como administrador universal. Nunca se deben dar a conocer las credenciales del usuario raíz y tampoco se recomienda que el creador de la cuenta realice tareas cotidianas como usuario raíz. En su lugar, se debe utilizar la cuenta del usuario raíz para crear una cuenta de administrador. Solo se deben realizar pocas tareas como usuario raíz, como cambiar el plan de AWS Support o cerrar una cuenta.

Un *usuario de IAM* es una entidad creada en AWS. Representa a la persona que utiliza los servicios de AWS y permite a los usuarios iniciar sesión en AWS. A un usuario se le asignará un nombre y una contraseña para acceder a la consola de AWS. Al crear un usuario, se considera una práctica recomendada asignarlo a un *grupo* que tenga la *política* de permisos adecuada.

Un *grupo* es un conjunto de *usuarios de IAM*. Puede utilizar grupos con el fin de especificar permisos para un conjunto de usuarios, lo que puede facilitar la administración de esos permisos para esos usuarios. Por ejemplo, puede tener un grupo llamado Administradores y concederle a este los tipos de permisos que normalmente necesitan los administradores. Cualquier usuario de dicho grupo tiene automáticamente los permisos que se asignaron al grupo. Si un nuevo usuario se une a su organización y necesita privilegios de administrador, puede asignar los permisos adecuados agregando el usuario a ese grupo. De manera semejante, si una persona cambia de puesto dentro de la organización, en vez de editar los permisos del usuario, puede quitarlo del grupo anterior y agregarlo al nuevo grupo adecuado.

*Los roles de IAM* son similares a los *usuarios*, ya que son identidades de AWS con políticas de permisos para determinar qué puede o no puede hacer la identidad en AWS. Sin embargo, un rol no tiene asociadas credenciales, como una contraseña o claves de acceso. En vez de estar asociado únicamente a una persona, el rol está pensado para asignarse a cualquiera que lo necesite

.Un usuario de IAM puede asumir un rol y adquirir temporalmente diferentes permisos para una tarea específica. Los roles son útiles en los casos en que una aplicación móvil accede a sus datos de AWS. No es deseable que todas las personas que utilicen esa aplicación tengan credenciales para su cuenta de AWS, aunque sí necesitan algún tipo de acceso a los datos cuando la utilizan. Si se asigna un rol cuando el usuario inicia sesión, se le otorga un acceso temporal con algunos permisos, pero sin credenciales permanentes.

Anteriormente, se mencionó las *políticas* en relación con los permisos que se pueden asignar a un *grupo*. Cuando una política se adjunta a un *usuario*,*rol* o *grupo*, se definen sus permisos. Las políticas se almacenan en AWS como documentos JSON. Es una práctica recomendada asignar *políticas* a los *grupos* y luego asignar cada *usuario* y *rol* a un grupo al crearlos. De esta forma, puede eliminar o cambiar rápidamente los permisos sin tener que modificar cada *usuario* o *rol* individual.

**Laboratorio**

- Las políticas administradas son políticas prediseñadas (que crearon AWS o sus administradores) que se pueden adjuntar a grupos o usuarios de IAM. Cuando la política se actualiza, los cambios se implementan inmediatamente en los usuarios y grupos adjuntos a ella.
- Una política define qué acciones están permitidas o denegadas para recursos concretos de AWS. Esta política concede permiso para *Enumerar* y *Describir* (ver) información sobre Amazon Elastic Compute Cloud (Amazon EC2), Elastic Load Balancing, Amazon CloudWatch y Amazon EC2 Auto Scaling. Esta capacidad para ver recursos, pero no modificarlos, resulta idónea para asignar un rol de soporte.

