title: Implementar reglas de seguridad de contraseña
Description: Configuración de contraseñas de uso del sistema, ofreciendo mayor nivel de seguridad con uso de diferentes caracteres.

# Implementar reglas de seguridad de contraseña

Esta funcionalidad retrata la configuración de contraseñas de uso del sistema,
ofreciendo mayor nivel de seguridad con el uso de diferentes caracteres.

!!! Abstract "ATENCIÓN"

     Esta política de seguridad no está disponible para los usuarios LDAP.
     

1. Desde la versión Helium 2.1.0, al actualizar la aplicación, el sistema configurará automáticamente los siguientes parámetros de la pantalla de política de privacidad:

       - El campo Habilitar política de contraseña se configurará como habilitado;  
       - El campo Tamaño mínimo se configurará en 8;  
       - El campo Exigir virá com as opções Minúsculas, Maiúsculas, Números e Símbolos setados como habilitados;  
       - El campo La nueva contraseña no puede ser la misma que las anteriores, se configurará en 2;  
       - El campo Requerir cambio de contraseña en el primer inicio de sesión se establecerá como habilitado;  
       - El campo de duración de la contraseña se establecerá en 2 meses.

2. El sistema requerirá cambiar la contraseña en el primer inicio de sesión, después de una actualización o instalación;  
3. Para actualizaciones, si la política de contraseñas ya está habilitada, el sistema respetará la configuración del cliente;  
4. Si la aplicación vuelve a cambiar su versión en menos de 2 meses, establecida en la configuración inicial, el sistema no solicitará un cambio de contraseña para los usuarios locales que ya hayan realizado el cambio;  
5. Esta configuración solo será válida para usuarios locales;  
6. Al habilitar la Política de bloqueo de usuarios, el administrador autoriza el bloqueo de usuarios externos o internos;  
7. El uso de captcha cambia la forma de iniciar sesión, teniendo un método extra de autenticación;  
8. El administrador, si habilita el bloqueo de usuarios, puede enviar un correo electrónico a los responsables de la seguridad del sistema.

Procedimiento
------------

1.  Acceder al menú principal Sistema \> Configuración \> Política de Seguridad;

2.  Habilitar la clave "Habilitar política de contraseña";

3.  En el campo **Complejidad de la contraseña** el administrador debe establecer el número mínimo
    de caracteres de la contraseña (valor mínimo de 8) y si la misma contendrá requisitos
    de: letras mayúsculas, minúsculas, números y símbolos;

4.  Establecer la cantidad de contraseñas anteriores en la que la nueva no puede ser igual, en el limitador **La nueva contraseña no puede ser igual que las anteriores**;

5.  Para nuevos usuarios, el cambio de contraseña se puede definir al hacer clic en la clave
    “Forzar el cambio de contraseña la primera vez que se inicie sesión”

6.  En el campo **Duración de la contraseña** definir el tiempo para caducar la contraseña;

7.  Para usuarios que ya están en operación, es posible forzar el cambio de contraseña de la nueva configuración, desde el siguiente inicio de sesión, haga clic en la clave “Forzar el cambio de contraseña la primera vez que se inicie sesión”;

A partir de la versión 1.2.23 o 2.1.0 de Helium, se han insertado nuevos parámetros:

8.  Habilite la clave "Habilitar política de bloqueo de usuarios":
    
        - Un símbolo con una "i" que indica que: Se considerará para inicios de sesión internos y externos
        
9.  Habilite la clave “Habilitar Captcha al iniciar sesión”: esta funcionalidad habilita una verificación obligatoria de las conexiones de todos los usuarios en el sistema; durante el inicio de sesión;    

10.  En el campo Bloqueo de usuarios, el administrador debe definir el número mínimo de errores sucesivos de credenciales para el bloqueo de usuarios, este bloqueo ocurre tanto para usuarios internos como externos y el desbloqueo se realiza dentro del producto;  

11.  Definir el tiempo de los sucesivos errores de credencial de los últimos minutos para bloquear al usuario: Este campo está vinculado al campo **“Bloquear usuario tras sucesivos errores de credencial”**, porque el sistema necesita un parámetro de tiempo para comparar el error de cantidad en un período de tiempo dado y no considerar al usuario bloqueado si no se encuentra dentro del límite de tiempo definido por haber alcanzado el número de intentos de bloqueo;  

12.  En el campo Notificaciones, debe definir:
        
         1. Enviar alerta de seguridad al grupo: Informar al grupo al que se le enviará el correo electrónico de alerta en caso de bloqueo de usuario por exceder los intentos configurados;
         2. Enviar alerta de seguridad a correos electrónicos: Informar al correo electrónico de posibles colaboradores que deben ser alertados en caso de bloqueo de usuarios. Los correos electrónicos deben estar separados por una coma y sin espacios entre ellos y sin espacios al final;
        
!!! warning "ATENCIÓN"
        
    Si el sistema identifica el correo electrónico del usuario al que se le ha bloqueado el acceso, ese usuario también recibirá un correo electrónico de bloqueo. La plantilla de correo electrónico de bloqueo no está disponible para cambios en esta versión. 

Clicar em “Salvar”.

## Relacionado

[Requisito para desbloqueio de usuário](/es-es/4biz-helium/platform-administration/security/user-unlock-requirement.html)
