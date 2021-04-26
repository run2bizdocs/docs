Title: Requisito de Desbloqueo de Usuario

# Requisito de Desbloqueo de Usuario

En este documento veremos los requisitos necesarios para desbloquear un usuario.

## Antes de empezar

- [x]	El administrador debe haber habilitado la regla de bloqueo de usuarios, contenida en el registro de Políticas de Seguridad;
- [x]	Se debe impedir que el usuario acceda a la aplicación debido al uso de la regla de bloqueo de usuarios.

## Procedimiento

A partir de la versión Helium 1.2.24, se introdujeron nuevas reglas de seguridad que llevaron a la inclusión de esta funcionalidad.

1. Acceder al menú principal Sistema \> La Seguridad \> Usuarios Bloqueados;

2. Al acceder a la funcionalidad, aparecerá una pantalla con el campo: Nombre de usuario - Campo de tipo de texto para buscar el nombre de usuario bloqueado;

3. Además de este campo, aparecerá una lista con la siguiente información:

|Lista|Descripción|
|-----|---------|
|Usuarios bloqueados|Presenta la información del contexto/inicio de sesión del usuario bloqueado|
|Fecha de bloqueo|Presenta la información de fecha/hora en la que el sistema realizó el bloqueo|

4. Aquí, también existe la acción Eliminar, que permite la eliminación del bloqueo inmediato del usuario.

## Relacionado

[Implementar reglas de seguridad de contraseña](/es-es/4biz-helium/platform-administration/security/implement-password-security-rules.html)
