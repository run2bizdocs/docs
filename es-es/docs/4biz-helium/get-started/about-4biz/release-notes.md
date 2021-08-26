Title: Notas de Release
Description: Notas de la versión, corrección de errores y mejoras de 4biz.

# Notas de Release

## Versión Helium 2.1.8 (2021/08/25) 

Bienvenidos a 4Biz Helium Versión 2.1.8. Esta versión presenta las siguientes correcciones:

|Número|Tipo|Descripción| 
|------|----|-----------|
|7644  |Corrección| Permiso para la encuesta de satisfacción mediante cuestionario |
|7655  |Corrección| Alteración del comportamiento de la pantalla de registro de encuestas para evitar que se realicen registros como inactivo |
|12510 |Corrección| Eliminación de la actualización automática de employeecontract_view |
|7685  |Corrección| Filtro por fechas |

La versión Builder compatible con esta versión es 1.3.7.6.


## Versión Helium 2.1.7 (2021/08/11) 

Bienvenidos a 4Biz Helium Versión 2.1.7. Esta versión presenta las siguientes correcciones:

|Número|Tipo|Descripción| 
|------|----|-----------|
|7269  |Corrección| Adición de acción al botón de previsualización en la pantalla de registro de la encuesta |
|7572  |Corrección| Ajuste del filtro de SLA en la pantalla de ticket |

La versión Builder compatible con esta versión es 1.3.7.6.


## Versión Helium 2.1.6 (2021/07/30)

Bienvenidos a 4Biz Helium Versión 2.1.6. Esta versión presenta las siguientes correcciones:

|Número|Tipo|Descripción| 
|------|----|-----------|
|7303   |Corrección| Conversión de JSON respuesta  anuva|
|7428	|Corrección| Permiso de programación sin adjunto |
|11137	|Corrección| Modal de comparación de contratos y actividades <br/> Grabación de dominio de usuario en la pantalla de persona |
|11323	|Corrección| Auditoría de las pantallas de usuario y perfil de acceso |
|11370  |Corrección| Cambios en la arquitectura de audit |
|11373  |Corrección| Inclusión de la auditoría de la pantalla de grupo <br/> Inclusión del registro de usuario en la auditoría |
|11371	|Corrección| Ajuste en el montaje del objeto antiguo - no se estaba guardando los grupos del usuario <br/> Auditoría de la pantalla de persona |
|11372	|Corrección| Auditoría de colaborador <br/> Cambios en Builders |
|11541	|Corrección| Permiso para descargar los archivos en actividad periódica |
|11703	|Corrección| Eliminación de los botones Guardar, Idioma y Acerca de CKEditor |
|11704	|Corrección| Corrección de las palabras en la internacionalización <br/> Permiso de restore de contrato usando queryParms |
|11714  |Corrección| Ajustes en la auditoría de grupo |
|11715  |Corrección| Ajustes en la auditoría de grupo | 
|11716	|Corrección| Ajustes en la auditoría de grupo |
|11778	|Corrección| Ajuste en concat para la base oracle, que no acepta más de 2 argumentos <br/> Ajustes en la auditoría de grupo <br/> Corrección en la auditoría del campo perfil de acceso que no se reflejaba <br/> Corrección en la pantalla de grupo que no estaba guardando correctamente las banderas de envío de e-mail <br/> Mejora en la auditoría del campo timezone concatenando los campos name y timezone para una mejor lectura |
|11833	|Corrección| Adición de la funcionalidad de auditoría sin mostrar los valores cambiados |
|11922	|Corrección| Ajuste en la auditoría de usuario cuando se crea fuera de la pantalla del sistema |
|12019	|Corrección| Verificación de la cantidad de portafolio listado que estaba equivocado |
|12058	|Corrección| Mejora del rendimiento del sistema |
|12076	|Corrección| Corrección en la auditoría del campo tipo de socio |
|12077	|Corrección| Adición de StringComparator.java para evitar casos en los que los campos vacíos y nulos se estaban comparando como "diferentes" <br/> Corrección del problema en el análisis nulo x vacío <br/> Adición de la validación adicional para los casos de nulo x vacío|
|12161	|Corrección| Solicitud de la liberación que duplicaba los IC’s al guardar |
|12213	|Corrección| Permiso para marcar los objetivos del tiempo de servicio |
|12228	|Corrección| Limpieza en el grupo ejecutor de la tarea cuando la delegación es solo para grupo |
|12270	|Corrección| Corrección de error al hacer clic en el enlace de actividades que redirigía a la pantalla equivocada en el detalle de contratos vinculados |
|12272	|Corrección| Adición de texto "no encontrado" para filtros de modal de detalle de contratos |
|12278	|Corrección| Formato del campo de fecha en la auditoría |
|12290	|Corrección| Grabación de los grupos de LDAP que estaban deshaciendo las programaciones en la eliminación de LDAP |
|12292	|Corrección| Cambio del tooltip del button para abrir el modal de filtro de actividades |
|12294	|Corrección| Grabación de los cambios de los usuarios en el registro de personas <br/> Grabación de auditoría en el cambio de persona |
|12301	|Corrección| Corrección de la apertura de enlace de servicios en el detalle de contrato |
|12316	|Corrección| Adición del timeout para los casos de internet lenta |
|12317	|Corrección| Cambio de la validación de mensajes de "notfound" a modal de detalles de contratos |
|12320	|Corrección| Permiso de envío para la revisión de un conocimiento |
|12323	|Corrección| Permiso de registro de conocimiento en el portal |
|12324	|Corrección| Eliminación de la duplicidad en el historial de cambios de comentarios |
|12328	|Corrección| Adición del límite mínimo para el campo de identificador en el filtro de historial de tickets |

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.1.5 (2021/07/07)

Bienvenidos a 4Biz Helium Versión 2.1.5. Esta versión presenta las siguientes correcciones:

|Número|Tipo|Descripción| 
|------|----|-----------|
|6928  |Corrección| Corrección del Informe de Cuantitativo de Tickets en el campo Grupo| 
|7054  |Corrección| Implementación de control de acceso interno, del sistema, para el usuario no autorizado| 
|7162  |Corrección| Al abrir el cambio, va a la planificación y después de planificar, va a la aprobación| 
|7268  |Corrección| Permitiendo la ejecución del cambio| 
|12185 |Corrección| El correo electrónico de notificación de cambio de la base de conocimientos está llegando incompleto| 
|12193 |Corrección| Cambio de la contraseña del usuario conectado| 
|12201 |Corrección| Crear claves primarias|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.1.4 (2021/06/23)

Bienvenidos a 4biz Helium Versión 2.1.4. Esta versión presenta las siguientes correcciones:

|Número|Tipo|Descripción|
|------|----|-----------|
|12123| Corrección| Corrección de la carga para países, municipios y ciudades|
|6652| Corrección| Asignar grupo ejecutor, como grupo actual, a WebService /servicerequestincident/create cuando no se especifica|
|7077| Corrección| Mayor disponibilidad del procesamiento batch|
|7164| Corrección| Permitir la ejecución de la expresión del grupo actual|
|7165| Corrección| Key violation – RequestTemplateInfo|
|12117| Corrección| Formulario Builder no funciona en la pantalla de solicitud de cambio en ningún flujo predeterminado del sistema|
|12118| Corrección| La versión generada de la rama hotfix/itsm-7077 del incidente muestra un error de codificación en la ventana emergente "Acerca de 4biz"|

La versión Builder compatible con esta versión es 1.3.7.4.



!!! warning "ATENCIÓN"

    Para más información sobre Builder 1.3.7.6, vea el archivo de [Notas de Release Builder][10]

## Versión Helium 2.1.3 (2021/05/24) 

Bienvenidos a 4biz Helium Versión 2.1.3. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11824	|Corrección	|Corrección de error para permitir la ejecución de la solicitud asignada solo al usuario|
|11937	|Corrección	|Corrección de error para presentar la notificación de informe completada cuando se procesa en segundo plano|
|11952	|Corrección	|Corrección de componentes Builder|
|11353	|Corrección	|Corrección de script de base de datos|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.1.2 (2021/05/14)

Bienvenidos a 4biz Helium Versión 2.1.2. Esta versión incluye las siguientes correcciones:

|Número	|Tipo  	   |Descripción        |
|-------|----------|-------------------|
|11510	|Corrección|	Corrección de error con el usuario invitado en Smart Chat|
|11393	|Corrección|	Corrección de error al iniciar sesión en varios entornos en los que está abriendo la ventana emergente de chat|
|11607	|Corrección|	Corrección de error cuando el usuario inicia una conversación con Helper y luego abre una nueva ventana en el navegador|
|11541	|Corrección|	Corrección de error al intentar descargar una evidencia dentro de una actividad periódica|
|10025	|Corrección|	Error al crear un ticket o sub-ticket con una situación igual a "Resuelto". No es posible que sea creado y cerrado al mismo tiempo|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.1.1 (2021/05/03)

Bienvenidos a 4biz Helium Versión 2.1.1 Esta versión incluye las siguientes correcciones:

|Número	|Tipo  	   |Descripción        |
|-------|----------|-------------------|
|11607	|Corrección|	Corrección de error en el que el usuario que está configurado como usuario invitado no puede acceder al sistema|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.1.0 (2021/04/16)

Bienvenidos a 4biz Helium Versión 2.1.0. Esta versión incluye las siguientes correcciones:

|Número	|Tipo  	   |Descripción        |
|-------|----------|-------------------|
|11235	|Corrección|	Las respuestas al formulario Builder no aparecen en la búsqueda avanzada|
|11348	|Corrección|	Verificar que los formularios Builder se están guardando sin la validación de campos obligatorios|

Y las siguientes mejoras:

|Número	|Tipo	|Descripción        |
|-------|-------|-------------------|
|11155	|Mejora	|Mejora en el mantenimiento del Portafolio|
|11220	|Mejora	|Crear área de configuración para Smart Chat|
|11221	|Mejora	|Permitir la visualización e iteración del usuario con Smart Chat desde la pantalla de inicio del sistema|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.0.5 (2021/04/16)

Bienvenidos a 4biz Helium Versión 2.0.5. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11348	|Corrección	|Validación de campos obligatorios en la página de CRUD de Builder|
|11355	|Corrección	|Cambio para que el sistema no utilice Trigger bpm_itemtrabalhofluxo_mv|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.0.4 (2021/04/16)

Bienvenidos a 4biz Helium Versión 2.0.4. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|10735	|Corrección	|Corrección del filtro de seguridad|
|11235	|Corrección	|Corrección de tratamiento de errors Builder |
|11235	|Corrección	|Las respuestas al formulario Builder no aparecen en la búsqueda avanzada|
|11355	|Corrección	|Cambio para que el sistema no utilice Trigger bpm_itemtrabalhofluxo_mv|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.0.3 (2021/04/16)

Bienvenidos a 4biz Helium Versión 2.0.3. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11344	|Corrección	|Tratamiento de nuevas etiquetas SQL Injection|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 2.0.2 (2021/04/14)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 2.0.2][9]

Bienvenidos a 4biz Helium Versión 2.0.2. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|10975	|Corrección	|[PostgreSQL / Sql Server] Corrección de error al agregar una imagen en el contenido del conocimiento para la visualización de los usuarios visitantes.|
|11190	|Corrección	|[G. Ticket] Corrección de error en el que al suspender un ticket, desaparecía de la lista.|
|10979	|Corrección	|[G. Conocimiento] Corrección de error para el versionamiento de conocimiento.|
|11092	|Corrección	|[G. Ticket] Corrección de error en el que al editar un comentario en la pantalla de ticket no se podía guardar el ticket.|
|11160	|Corrección	|[G. Ticket] Corrección de error que impedía la creación de un ticket a través de un token.|
|11105	|Corrección	|[Centro de Experiencia] Corrección de error en el que al abrir un ticket por el centro de experiencia, añadía en el campo descripción el nombre de la actividad del portafolio.|
|11106	|Corrección	|[Centro de Experiencia] Corrección de error en el que no se muestra el botón Cancelar ticket dentro del ticket seleccionado en el centro de experiencia.|
|11109	|Corrección	|[G. Conocimiento] Corrección de error en el que al agregar una imagen en una categoría de imagen o en un contenido de conocimiento, era redirigido a la pantalla de inicio de sesión.|
|11110	|Corrección	|[G. Ticket] Corrección de error en el que al suspender un ticket a través del smart portal o de la pantalla del ticket se cancelaba, pero seguía apareciendo en la lista principal.|
|11269	|Corrección	|[Webservice] Corrección de error al mostrar la ocurrencia en tickets cerrados.|
|11195	|Corrección	|[G. Ticket] Corrección de error en el campo dirigir a grupos, que cargaba todos los grupos registrados.|
|10928	|Corrección	|[Webservice] Corrección de error al utilizar los WebServices Save y Next definiendo los campos que se van a cambiar en el ticket, no estaban siendo alterados en el Front End y mostraba el cambio solo en el historial del ticket.|
|11287	|Corrección	|[G. Ticket] Corrección de error al rechazar un ticket con flujo de aprobación a través de token por correo electrónico.|
|11197	|Corrección	|[G. Ticket] Corrección de error en el que un ticket que fue capturado en la tarea de dirigir el servicio, al delegar el ticket, no estaba mostrando la información en la tabla 'capturecontrolservicerequest'.|
|10929	|Corrección	|[Sistema] Corrección de error en el que el icono 'bandera' para cambiar el idioma no funcionaba en la pantalla 'Términos de servicio' en una instalación desde cero.|
|11231	|Corrección	|[G. Ticket] Corrección de error en el que la encuesta de satisfacción no funcionaba correctamente, cuando el usuario hacía clic en el enlace del correo electrónico para responder. La aplicación redireccionaba a la url del sistema, pero se quedaba solo en espera. |
|11260	|Corrección	|[G. Ticket] Corrección de error en el que al realizar la validación de un ticket que tenía más de un grupo en la asignación del flujo, con flujo aprobación vía token configurando en la tarea de usuario ejecutor "Aprobar" con más de un grupo, al aprobar o rechazar por correo electrónico en la tabla bpm_itemtrabalhofluxo no establecía el campo executor_grupo_id.|
|11263	|Corrección	|[Webservice] Corrección de fallo en el webservice del empleado.|
|11258	|Corrección	|[G. Ticket] Corrección de error cuando teníamos un ticket de origen vinculado a un ticket relacionado, al cerrar, el ticket de origen y el ticket relacionado también estaban cerrados. Sin embargo, en la tabla bpm_itemtrabalho no estaba registrado el grupo ejecutor del ticket relacionado.|
|11261	|Corrección	|[Webservice] Corrección de error en el webservice de check-in.|
|11196	|Corrección	|[G. Ticket] Corrección de error en el componente de flujo que no se podía mover en Chrome.|
|11189	|Corrección	|[G. Ticket] Corrección de error al crear un ticket que contenía solamente una imagen en el campo descripción el sistema no mostraba la imagen después de la creación.|
|10476	|Corrección	|[CMDB] Corrección de error en el que en la pantalla de 'Midia' al vincular un conocimiento y guardar, al entrar dentro de él nuevamente, el conocimiento se replicaba.|
|11239	|Corrección	|[G. Ticket] Corrección de error en el comportamiento del sistema cuando el usuario no seleccionaba ningún grupo al capturar un ticket y hacía clic en siguiente.|
|11223	|Corrección	|[G. Liberación] Corrección de error cuando intentábamos guardar y avanzar una liberación que estaba con la tarea actual igual 'liberación' y esa liberación contenía un cambio que tenía un IC vinculado en la misma solicitud de liberación, no guardaba y muestraba un mensaje de error.|
|10971	|Corrección	|[Correctiva] Corrección de error de key violation, remanente de la corrección de Sequence_Block.|
|11199	|Corrección	|[G. Ticket] Corrección de error al delegar un ticket dentro de la llamada.|
|10487	|Corrección	|[Webservice] Corrección de error en el que al reclasificar, por el webservice, no quedaba la justificación correcta.|
|10546	|Corrección	|[G. Portafolio] Corrección de error en el que, en el portafolio, al editar cualquier campo de pop-up "Vincular Servicio de Solicitud o Incidente" presentaba el error de SQL en el log y no guardaba la edición. El botón de "Guardar" estaba sin acción.|
|11217	|Corrección	|[G. Problemas] Corrección de error en el que no se podía crear un problema de tipo 'Reactivo', ya que no podíamos vincular un ticket al problema.|
|11188	|Corrección	|[G. Ticket] Corrección de error al suspender un ticket dentro de la llamada.|
|11010	|Corrección	|[Webservice] Corrección de error en el que no estaba creando un ticket con el viejo webservice create.|
|11011	|Corrección	|[G. Ticket] Corrección de error en el que al suspender un ticket, la aplicación no se suspendía y presentaba deadlock.|
|11290	|Corrección	|[Webservice] Corrección de error que estaba ocurriendo cuando se utiliza el webservice para listar portafolios. El mismo no estaba presentando correctamente los portafolios del usuario conectado, cuyo el mismo es el usuario proporcionado en el body del webservice cuando el parámetro 293 está habilitado.|
|11291	|Corrección	|[Usuarios] Corrección de error cuando registrábamos a un usuario a través de la aplicación no estaba recibiendo el dominio local, por ejemplo, 4biz.local re.|
|11288	|Corrección	|[G. Ticket] Corrección de error donde al intentar reabrir un ticket que tenía un flujo de aprobación a través de token, la aplicación mostraba un mensaje de error.|
|11293	|Corrección	|[Webservice] Corrección de error en el que al intentar capturar un ticket a través del webservice, con un usuario conectado y con permiso en el flujo para dos grupos, no se permitía capturar el ticket y se mostraba un mensaje de error.|
|11216	|Corrección	|[Sistema] Corrección de vulnerabilidad en el sistema.|
|10503	|Corrección	|[G. Ticket] Corrección de error al validar llamados cerrados que seguían apareciendo en la lista de llamados en curso.|
|10649	|Corrección	|[Sistema] Corrección de error porque el campo "useremail" de la tabla "chatusers" no aceptaba null. Al iniciar sesión con los usuarios de LDAP, que no tenía correo electrónico registrado, presentaba un error.|
|10930	|Corrección	|[Usuario] Corrección de error en la tabla perfil de acceso.|
|10931	|Corrección	|[Sistema] Corrección de errores presentados en el log al realizar una nueva instalación.|
|10944	|Corrección	|[Sistema] Corrección de error al crear un flujo.|
|10314	|Corrección	|[G. Liberación] Corrección de error en el que no se mostraban las ocurrencias de "creación y finalización" en la búsqueda avanzada y en el nombre de la persona que realizó la ocurrencia estaba descrito el inicio de sesión del usuario y no su nombre completo.|
|10867	|Corrección	|[Webservices] Corrección de error al guardar un ticket con un conocimiento vinculado el sistema limpiaba el conocimiento.|
|10921	|Corrección	|[Webservices] Corrección de error en el webservice location/last.|
|10554	|Corrección	|[Smart Portal] Corrección de error cuando el parámetro id 293 = Sí, la aplicación estaba mostrando error al abrir la pantalla de Smart portal.|
|10866	|Corrección	|[G. Problema] Corrección de error en la que al crear una petición de problema se presentaba, en la pantalla para el usuario y en el log, un error de SQL.|
|10865	|Corrección	|[G. Cambio] Corrección de error del cambio al insertar IC y guardar.|
|10861	|Corrección	|[G. Cambio] Corrección de error en Java en el que la tabla "RequisicaoMudancaServiceEjb" no estaba trayendo la cantidad de solicitudes de aprobación en la pantalla de cambio.|
|10788	|Corrección	|[Sistema] Corrección de error en el que al actualizar la versión de 1.2.24 a 2.0.1-Snapshot-02, la aplicación presentaba error en los parámetros corpore del sistema.|
|10922	|Corrección	|[Webservice] Corrección de error en el que la notificación push no estaba llegando a la aplicación.|
|10891	|Corrección	|[Sistema] Corrección de error para eliminar una programación, cuando un procesamiento batch se desactiva automáticamente.|
|10902	|Corrección	|[Sistema] Corrección de error en la secuencia de la tabla "Rest_operation" que estaba con valor equivalente a "Restoperation_seq.nextval" para la clave primaria.|

Y las siguientes mejoras:

|Número	|Tipo	|Descripción        |
|-------|-------|-------------------|
|11214	|Mejora	|[Usuarios] Mejora en el cambio del algoritmo de cifrado de contraseña y forzar el cambio de contraseña en el siguiente inicio de sesión.|
|11159	|Mejora	|[Webservice] Mejora en el webservice de inicio de sesión de 4biz para un nuevo usuario LDAP.|
|11158	|Mejora	|[Webservice] Mejora en el webservice de autenticación – Builder.|
|10665	|Mejora	|[G. Ticket] Mejora en tickets que tenían más de un grupo en la asignación del flujo.|
|- 	|Mejora	|[Usuarios] Mejora en la inclusión del método de autenticación Keycloack.|
|-	|Mejora	|[Usuarios] Mejora en la inclusión del método de autenticación a través de redes sociales.|
|10502	|Mejora	|[G. Ticket] Mejora de las consultas de BI.|
|10081	|Mejora	|[Webservice] Mejora donde se ha creado un webservice que le permite ver los detalles del cambio.|


Bienvenido a Builder 1.3.7.4.

La versión presentada tiene las siguientes correcciones: 

|Número	|Tipo	   |Descripción        |
|-------|----------|-------------------|
|11320	|Corrección|	Corrección de mensaje de error|
|11353	|Corrección|	Corrección de la creación de flujos en el entorno Oracle|
|11353	|Corrección|	Corrección de query componente|

Bienvenido a Builder 1.3.7.3.

La versión presentada tiene la siguiente corrección: 

|Número	|Tipo	   |Descripción        |
|-------|----------|-------------------|
|11320	|Corrección|	Corrección de la visualización de componentes|

Bienvenido a Builder 1.3.7.2.

The version presented has the following correction(s):

|Número	|Tipo	   |Descripción        |
|-------|----------|-------------------|
|10735	|Corrección|	Corrección de scripts|

Bienvenido a Builder 1.3.7.1.

La versión presentada tiene las siguientes correcciones: 

|Número	|Tipo	   |Descripción        |
|-------|----------|-------------------|
|10538	|Corrección|	Corrección de directivas Builder|
|11320	|Corrección|	Mostrar propiedades del componente al crear el formulario por el objeto de negocio|


Bienvenido a Builder 1.3.7.0 

La versión presentada tiene las siguientes correcciones: 

|Número	|Tipo	   |Descripción        |
|-------|----------|-------------------|
|10735	|Correctiva|	Corrección de la autenticación de usuarios|
|10735	|Correctiva|	Inicio de sesión con usuario LDAP y Oauth2|
|10735	|Correctiva|	Tratamiento de contraseña en la autenticación Builder|
|11025	|Correctiva|	Corrección de null pointer|
|11025	|Correctiva|	Refactoring en la autenticación|
|11196	|Correctiva|	Corrección del mouse move del diseño de flujo en Chrome|
|11214	|Correctiva|	Cambio del algoritmo de cifrado de contraseña de usuario|
|11214	|Correctiva|	Retiro de constantes de usuario admin|
|11216	|Correctiva|	Corrección de la vulnerabilidad del filtro de autocomplete|
|11214	|Correctiva|	Cambio del algoritmo de cifrado de contraseña y forzar el cambio de contraseña en el siguiente inicio de sesión.|

!!! warning "ATENCIÓN"

    Para más información sobre Builder 1.3.7.0, vea el archivo de [Notas de Release Builder][8]

## Versión Helium 1.2.31 (2021/05/12)

Bienvenidos a 4biz Helium Versión 1.2.31. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|10025	|Corrección	|Registro del grupo ejecutor, en la tarea de finalización de la solicitud, que fue lanzada y ya resuelta|
|11541	|Corrección	|Permite descargar archivos en la pantalla de actividad periódica|

La versión Builder compatible con esta versión es 1.3.7.4.

## Versión Helium 1.2.30 (2021/05/03)

Bienvenidos a 4biz Helium Versión 1.2.30. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11365	|Corrección	|Cambio en el método de eliminación de etiquetas|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 1.2.29 (2021/04/14)

Bienvenidos a 4biz Helium Versión 1.2.29. Esta versión incluye las siguientes correcciones:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11344	|Corrección	|Correctiva de seguridad|

La versión Builder compatible con esta versión es 1.3.7.4.


## Versión Helium 1.2.28 (2021/03/24)

Bienvenido a 4biz Helium Versión 1.2.28. Esta versión incluye las siguientes mejoras:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11216	|Correctiva	|Corrección de la vulnerabilidad del filtro de autocomplete|
|11214	|Mejora		|Cambio del algoritmo de cifrado de contraseña y forzar el cambio de contraseña en el siguiente inicio de sesión|
|6588	|Correctiva	|Incidente en el informe de control de SLA que devuelve fechas fuera del período solicitado|
|6607	|Correctiva	|Incidente en el informe de Controle de SLA atrasado que muestra fechas fuera del período seleccionado|
|6527	|Correctiva	|Incidente al responder una encuesta de satisfacción, el sistema no carga la encuesta|

La versión Builder compatible con esta versión es 1.3.6.6.


## Versión Helium 1.2.27 (2021/03/23)

Bienvenido a 4biz Helium Versión 1.2.27. Esta versión incluye las siguientes mejoras:

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11094	|Correctiva	|Corrección de la autenticación LDAP a través del webservice|
|11094	|Correctiva	|Corrección de null pointer y mensajes|
|11094	|Correctiva	|No continuar usando la contraseña de usuario de LDAP|
|11094	|Correctiva	|Gestión de errores LDAP|

Bienvenido a Builder 1.3.6.6 

La versión presentada tiene la siguiente corrección: 

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11025	|Correctiva	|Corrección de redirección para la pantalla de inicio de sesión cuando se utiliza el webservice del mismo nombre|

!!! warning "ATENCIÓN"

    Para más información sobre Builder 1.3.6.6, vea el archivo de [Notas de Release Builder][7]


## Versión Helium 1.2.26 (2021/03/23)

Bienvenido a 4biz Helium Versión 1.2.26. Esta versión incluye las siguientes mejoras:

|Número		|Tipo		|Descripción        |
|---------------|---------------|-------------------|
|ITSM 6396	|Correctiva	|Sintaxis SQL incorrecta al crear o abrir un problema |

Bienvenido a Builder 1.3.6.6 

La versión presentada tiene la siguiente corrección: 

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|11025	|Correctiva	|Corrección de redirección para la pantalla de inicio de sesión cuando se utiliza el webservice del mismo nombre|

!!! warning "ATENCIÓN"

    Para más información sobre Builder 1.3.6.6, vea el archivo de [Notas de Release Builder][7]


## Versión Helium 1.2.25 (2021/02/16)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.25][6]

Bienvenido a 4biz Helium Versión 1.2.25. Esta versión incluye los siguientes elementos:

La versión Builder compatible con esta versión es 1.3.5.5.

|Número	|Tipo		|Descripción        |
|-------|---------------|-------------------|
|6231	|Correctiva	|Error al enumerar el historial de un ticket delegado mediante la búsqueda avanzada|
|10670	|Correctiva	|El sistema no presenta el conocimiento externo y público|
|10802	|Correctiva	|Error de charset en las palabras acentuadas en los informes smart|
|10892	|Correctiva	|Mejora del rendimiento de las consultas de auditoría|


## Versión Helium 1.2.24 (2021/01/16)

!!! warning "ATENCIÓN"
	
    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.24][5]

Bienvenido a 4biz Helium Versión 1.2.24. Esta versión incluye los siguientes elementos:

La versión Builder compatible con esta versión es 1.3.5.5.

|Número	|Tipo	|Descripción        |
|-------|-------|-------------------|
|10619	|Mejora	|Bloqueo de usuarios después de sucesivos errores de acceso	|
|10620	|Mejora	|Envío de notificación de bloqueo de usuario	|
|10617	|Mejora	|Inclusión de captcha al acceder al sistema	|
|10663	|Mejora	|Corrección de acceso a usuarios registrados a través de LDAP	|
|10618	|Mejora	|Configuración de los mensajes de autenticación del sistema |
|10628	|Mejora	|Inclusión de autenticación de keycloack con gestión de acceso e identidad	|
|10624	|Mejora	|Revisión de los criterios de seguridad	|

|Errores conocidos	|Descripción		|
|-----------------------|-----------------------|
|10670			|La pantalla de acceso para la visualización de conocimientos externos no permite el acceso sin iniciar sesión en el sistema|

Bienvenido a Builder 1.3.5.5 

La versión presentada tiene la siguiente corrección: 

|Correctiva	|Descripción	|
|---------------|---------------|
|		|Corrección de error intermitente ocasionado en Scripts Rhino|
	

## Versión Helium 1.2.23 (2021/01/05)

!!! warning "ATENCIÓN" 

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.23][4]

Bienvenido a 4biz Helium Versión 1.2.23. Esta versión incluye los siguientes elementos:

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|Incidente 5929 |Correctiva |Corrección de seguridad del producto evitando aceptar LDAP Injection, caracteres especiales en el inicio de sesión de usuario y tamaño de inicio de sesión|

Bienvenido a Builder 1.3.5.4 

La versión presentada tiene las siguientes correcciones: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10280          |Corrección |Recuperación del valor default de las columnas del objeto de negocio|


## Versión Helium 1.2.22 (2020/12/03)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.22][3]

Bienvenido a 4biz Helium Versión 1.2.22. Esta versión incluye los siguientes elementos: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10176          |Correctiva |Corrección de componente lookup|
|Incidente 5800 |Correctiva |Corrección de error al limitar un select con comando TOP|
		
Bienvenido a Builder 1.3.6.1 

La versión presentada tiene la siguiente corrección: 

|Número         |Tipo       |Descripción        |
|---------------|-----------|-------------------|
|10476          |Corrección |[My 5802] - Menús laterales de Builder no funcionan correctamente|

## Versión Helium 1.2.13 (2021/01/05)

!!! warning "ATENCIÓN"

    Antes de descargar esta versión, consulte las orientaciones en el documento [Guía de orientaciones del 4biz Helium versión 1.2.13][2]

Bienvenido a 4biz Helium Versión 1.2.13. Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|10005|Corrección|Sistema|Correcciones en la Auditoría|
|10008|Corrección|G. de Ticket|Corrección en la visualización del SLA a combinar|
|10011|Corrección|Webservice|Mejora en el webservice de telefonía en cuanto a la sesión del usuario|
|10012|Corrección|G. de Ticket|Corrección en la representación de formularios Builder|
|10013|Corrección|G. de Ticket|Corrección en la visualización de un ticket|
|10019|Corrección|G. de Ticket|Corrección al actualizar la lista Sin Responsable|
|10022|Corrección|G. de Ticket|Corrección en la recuperación de tickets para comentarios|
|10023|Corrección|Webservice|Corrección del mecanismo de telefonía websocket con Builder|
|10031|Corrección|G. de Ticket|Corrección en registros de comentarios reclasificados|
|10034|Corrección|G. de Ticket|Corrección en la visualización de la información del solicitante del ticket|
|10035|Corrección|Webservice|Incluir información sobre el ticket creado en el nuevo modal de telefonía|
|10044|Corrección|Chat|Corrección para avanzar el flujo de chatcall de ticket cancelado/cerrado|
|10047|Corrección|G. de Ticket|[My 5540] – Corrección en el envío de correo electrónico al finalizar el servicio|
|10051|Corrección|G. de Ticket|[My 5317] - Problema con la consulta que no se filtra por grupo|
|10052|Corrección|G. de Ticket|No se esta enumerando los tickets para el usuario que solo tiene el permiso "Puedo comentar"|
|10056|Corrección|G. de Ticket|[My 5405] - Error intermitente al intentar la aprobación vía token|
|10057|Corrección|G. de Portafolio|[My 5351] - Problema con el botón de grabación al editar un Portafolio|
|10058|Corrección|G. de Ticket|[My 5339] - Error al crear ticket mediante la lectura de correo electrónico|
|10061|Corrección|Chat|[My 5450] - Error al iniciar una conversación vía chat|
|10065|Corrección|G. de Ticket|Compruebe si hay errores al buscar por la búsqueda avanzada|
|10083|Corrección|G. de Ticket|Corrección cde clave internacionalizada de tipo SLA en caso de solicitud|
|10093|Corrección|G. de Ticket|Manejar transacciones de cierre en transacitionControlerIMPL|
|10097|Corrección|G. de Ticket|Corrección del mensaje "Espere, cargando ..." en la auditoría|
|10098|Corrección|G. de Ticket|Tratar null pointer en la clase OcorrenciaSolicitacaoBuilder|
|10178|Corrección|Flujo|Creación de campos para programar ejecuciones de Rhino Script|
|10204|Corrección|G. de Portafolio|Corrección en la exclusión de Causa Incidente en el Portafolio|
|10211|Corrección|Sistema|Corrección al agregar una imagen a la galería de imágenes|
|10216|Corrección|G. de Portafolio|Corrección en el campo obligatorio del Portafolio|
|8542|Corrección|G. de Ticket|Visualización de respuestas a comentarios en la exportación CSV|
|8589|Corrección|G. de Ticket|Mostrar los nombres de los archivos adjuntos en el historial de creación de tickets|
|9320|Corrección|G. de Ticket|Incluir en las ocurrencias información sobre inclusión y exclusión de los procesos de negocio|
|9826|Corrección|Sistema|Eliminación del SequenceBlock|
|9839|Corrección|G. de Problema|[My 5160] - Error al agregar el Portafolio de Problema|
|9890|Corrección|G. de Ticket|[My 5408] - Corrección de error al mostrar el nombre del contrato al ver el ticket|
|9915|Corrección|G. de Problema|Error al desvincular el contrato del Portafolio de Problema|
|9955|Corrección|G. de Ticket|[My 5403] -Verifique la falla de auditoría al informar la reclasificación de tickets|
|9949|Corrección|G. de Ticket|[MY 5352] - Verificar el historial de delegación que no se muestra en la pestaña del historial de ticket|
|9965|Corrección|G. de Ticket|Verificar que no muestra el motivo de la reclasificación en el historial|
|9968|Corrección|Sistema|[My 5338] - Entorno VNS lento al enumerar la cola de tickets|
|9957|Corrección|G. de Ticket|[My 5121- 5180 - 5163] Error al insertar el adjunto en el subticket creado por copia|
|9959|Corrección|G. de Ticket|[My 5172]- La paginación de la pantalla del ticket va a cero|   

Bienvenido a Builder 1.3.5.1

La versión presentada tiene las siguientes correcciones:

|Número|Tipo|Descrição|
|--------|---------|---------|
|100175|Corrección|Corrección en la internacionalización en un ambiente clusterizado|
|10049|Corrección|[My 5357]- No se pudieron validar los permisos del botón, incluso con el usuario con permiso|
|9751|Corrección|[My 5153] - Verifique que los archivos que tienen nombres con caracteres especiales no se cargan|

## Versión Helium 1.1.1 (2020/09/14)
Bienvenido a 4biz Helium Versión 1.1.1. Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|9635|Corrección|G. Liberación|Se corrigió la visualización del icono de reapertura en la pantalla de búsqueda avanzada de la liberación|
|9594|Corrección|G. Cambio|Error en la lista de cambios debido a la flag Active creada en la tabla de itemtrabajo|
|9607|Corrección|G. Ticket|Error al recuperar la búsqueda avanzada|
|5089|Corrección|G. Ticket|Error en la lectura del correo electrónico del solicitante|
|5002|Corrección|Registro Proyecto|Error al buscar los documentos de registro del proyecto|
|9579|Corrección|G. Problema|Error al resolver un Problema|
|9570|Corrección|G. Ticket|Error al ver el flujo en un ticket|
|4930|Corrección|G. Ticket|Verificar si hay error de cálculo de SLA|
|9408|Corrección|G. Conocimiento|Al acceder al portal de conocimiento con un usuario externo, el visitante intenta cargar el archivo que se encuentra en el conocimiento, la carga no se realiza|
|9412|Corrección|Chat|El chat muestra un error solo en el log al capturar y avanzar el flujo|
|4997|Corrección|G. Ticket|Corrección de duplicación de buzones de correo|
|9378|Corrección|G. Ticket|En el Smart Portal, en el historial de un ticket al buscar el Identificador, el campo no es del tamaño correcto y no se puede digitar. Además presenta el error "No se pudo cargar recurso: el servidor respondió con un estado de 403 ()"|
|9287|Corrección|Registro de Grupo|Error al acceder a la pantalla de Grupo|
|9289|Corrección|Registro de Persona|Pantalla de búsqueda de empleados con un error de Front End al buscar un empleado con un estado igual a "Inactivo"|
|9218|Corrección|G. Conocimiento|El registro de conocimientos no se abre|
|4875|Corrección|Tasker|Se ajustó la vista de sprint vencida|
|9219|Corrección|G. Ticket|Subir archivo adjunto de ticket congelando en la pantalla|
|9221|Corrección|Smart Portal|Corrección del botón de cierre que permanece inerte después de grabar un ticket|
|9282|Corrección|Flujo|Error de flujo al vincular un cuestionario de "Seguimiento", ya sea obligatorio o no|
|4633|Corrección|G. Ticket|El sistema no está creando un ticket con el usuario existente en el sistema|
|9126|Corrección|Webservice|Presentar el cuestionario en la aplicación|
|9217|Corrección|G. Cambio|Portafolio de Cambio no se abre|
|4861|Corrección|G. Ticket|Duplicación de ticket reclasificado|
|4668|Corrección|G. Ticket|Duplicación de la tarea de flujo en la delegación|

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|9201|Mejora|G. Ticket|Inclusión de flag en el elemento de trabajo de flujo para aumentar el rendimiento de la aplicación|
|9583|Mejora|G. Ticket|Cambiar al buscar permisos en la lista de ticket|
|9434|Mejora|Sistema|Eliminar la pantalla de acceso de las herramientas de datos de la aplicación|
|9584|Mejora|G. Ticket|Cambiar cuándo buscar grupos en ejecución en la lista de tickets|
|9427|Mejora|Webservice|Permitir responder cuestionario de creación por la aplicación|
|9440|Mejora|Webservice|Permitir filtrar tickets a través de la aplicación|
|8837|Mejora|Webservice|Crear un servicio web que enumere los grupos que se dirigirán a un ticket|
|9342|Mejora|Webservice|Reclasificar ticket por la aplicación|
|9429|Mejora|Webservice|Aumentar la capacidad del campo Extensión de registro de empleados|
|9428|Mejora|Webservice|Identificar el tipo de cuestionario presentado para la identificación de la aplicación|
|9333|Mejora|Webservice|Presentar información extraída de las acciones del usuario en la aplicación|
|9011|Mejora|Webservice|Permitir opciones de flujo en la aplicación|
|8840|Mejora|Webservice|Crear un servicio web que enumere las razones para suspender un ticket|
|8834|Mejora|Webservice|Crear un servicio web que enumere las Unidades para su selección|
|8839|Mejora|Webservice|Cree un servicio web que enumere las categorías de soluciones para resolver un ticket en la aplicación|
|8832|Mejora|Webservice|Presentar información de cierre y responsable de consumo de la aplicación|
|9297|Mejora|G. Ticket|Eliminación de tickets innecesarios en el método filterContract de la clase ServiceResquestIncident - Se eliminó la restauración de proveedores y clientes dentro de la iteración del contrato|
|9010|Mejora|Webservice|Eliminar el archivo adjunto de la aplicación|
|8413|Mejora|Registro de Persona|Crear y Buscar Persona|
|8838|Mejora|Webservice|Crear un servicio web que enumere las causas para resolver un ticket|
|9313|Mejora|G. Ticket|Incluir la gestión de colas para la extracción de datos en "Búsqueda avanzada"|
|8833|Mejora|Webservice|Servicio web que le permite delegar un ticket a un analista|
|9222|Mejora|G. Ticket|Performance - Reemplazar employeecontract con materialized view|
|8855|Mejora|Webservice|Permitir enumerar usuarios y grupos que se pueden delegar en un ticket|
|8836|Mejora|Webservice|Crear un servicio web que enumere la ubicación de una unidad del ticket|
|8835|Mejora|Webservice|Crear un servicio web que enumere la fuente de contacto del ticket|
|8426|Mejora||Colocar el nombre del cliente que ha obtenido la licencia del entorno al final de la página|

Bienvenido a Builder 1.3.5.0. La versión presentada tiene las siguientes correcciones:

|Número|Tipo|Descripción|
|--------|---------|---------|
|7814|Corrección|Refactoría de integración con ITSM para permitir la flexibilidad de la URL externa del Builder|
|8416|Corrección|Corrección del error al utilizar el flujo ESI como componente en el flujo de trabajo|

|Número|Tipo|Descripción|
|--------|---------|---------|
|7751|Mejora|Ajustar los nombres de las propiedades de los componentes del portugués al inglés|
|7774|Mejora|Error de traducción en el BUILDER --> ESI|


## Versión Helium 1.0.2 (2020/04/27)
Bienvenido a 4biz Helium Versión 1.0.2 Esta versión incluye los siguientes elementos:

|Número|Tipo|Funcionalidad|Descripción|
|--------|---------|---------|---------|
|8968|Corrección|Center|Corrección en la devolución de la lista de Portafolios cuando se habilita el parámetro 293 que filtra el portafolio por grupos de acceso|
|4818|Corretiva|Tiempo de Atención|Corrección en la programación de una actividad para vincular al SLA registrado|

[2]:/es-es/4biz-helium/get-started/about-4biz/Guidance-4biz-Helium1213.zip
[3]:/es-es/4biz-helium/get-started/about-4biz/Guía-de-orientaciones-4biz-Helium-versión-2.0.0.zip
[4]:/es-es/4biz-helium/get-started/about-4biz/Paquete-Actualización-1.2.23.zip
[5]:/es-es/4biz-helium/get-started/about-4biz/Paquete-Actualización-1.2.24.zip
[6]:/es-es/4biz-helium/get-started/about-4biz/Orientaciones-sobre-la-versión-4biz-Helium-1.2.25.zip
[7]:/es-es/4biz-helium/get-started/about-4biz/Notas-de-Release-Builder-1.3.6.6.docx
[8]:/es-es/4biz-helium/get-started/about-4biz/Notas-de-Release-Builder-1.3.7.0.docx
[9]:/es-es/4biz-helium/get-started/about-4biz/Paquete-Actualización-2.0.2.zip
[10]:/es-es/4biz-helium/get-started/about-4biz/Notas-de-Release-Builder-1.3.7.6.docx
