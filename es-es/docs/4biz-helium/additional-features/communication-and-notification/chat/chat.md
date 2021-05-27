Title: Chat
# Chat

La noción de "Chat" se utiliza para aludir al intercambio de mensajes escritos de forma instantánea. En este caso, permite que el usuario tenga el contacto adecuado para el operador del sistema, a fin de aclarar dudas, hacer solicitudes, entre otros. Los parámetros de esta aplicación permiten activar el chat, definir el contrato estándar para la apertura de llamadas y ajustar el grupo predeterminado, además de otras acciones.

El chat se puede usar de tres maneras:

-   Manual: intercambio de mensajes entre varios tipos de usuarios 
    (ej.: solicitante y asistente) en una instancia de 4biz;

-   Automático: utilizado para la mensajería entre el usuario y un 
    asistente virtual - a través de Chatbot, utilizando la inteligencia 
    artificial de Helper;

-   Ambos: se usa para habilitar el contacto entre el solicitante y el asistente, 
    lo que también permite que un usuario interactúe con un chatbot.

!!! Abstract "NOTA"
    
    Para interactuar con un Chatbot, se necesita comprar este servicio. Si tiene alguna pregunta, comuníquese con 4biz.

## Antes de empezar

Para que el chat esté disponible, debe configurar los parámetros de activación de la funcionalidad.

1.	Acceder a la funcionalidad a través de la navegación en el menú principal 
    Parametrización > Chat;

2.	Definir los valores de los parámetros (atributos);

3.	Hacer clic en el botón "Gravar";

4.	La siguiente lista muestra los parámetros de la funcionalidad "Chat" y 
    el propósito de cada uno de ellos.

|#	|Nombre                                                      |Valores posibles|Finalidad                                                   |Directrices adicionales |
|:-:|:----------------------------------------------------------:|:--------------:|:---------------------------------------------------------------:|:-----------------:|
|118|	ID de contrato estándar para la apertura de Tickets      |	              |     ID de contrato estándar para la apertura de Tickets         |   No se aplica    |
|315|	ID de origen de las solicitudes creadas por el chat      |		          |     ID de origen de las solicitudes creadas por el chat         |   No se aplica    |
|316|	Activar Chat	                                         |      S o N	  |     Activar Chat	                                            |   No se aplica    |
|317|	ID de la actividad de las solicitudes creadas por el chat|		          |     ID de la actividad de las solicitudes creadas por el chat   |   No se aplica    |
|388|	ID de usuario predeterminado (Solicitud externa)		 |                |     ID de usuario predeterminado (Solicitud externa)	        |   No se aplica    |
|389|	ID grupo predeterminado (Solicitud externa)		         |                |     ID grupo predeterminado (Solicitud externa)	                |   No se aplica    |
|390|	ID de unidad predeterminado		                         |                |ID de unidad que se asignará al usuario registrado en el perfil	|   No se aplica    |
|447|	ID de plantilla de correo electrónico para la notificación de nuevos mensajes en el chat| |ID de plantilla de correo electrónico para la notificación de nuevos mensajes en el chat|    No se aplica    |
|299|	Activar el intercambio de mensajes                  	 |      S o N	  |Activa un icono de conversación junto al número de ticket en la cola de llamadas|No se aplica|
|448|	Editor de texto utilizado por la aplicación              |		          |     Editor de texto utilizado por la aplicación                 |	No se aplica    |

5.	Los parámetros 315, 316, 317, 447 y 423 deben asignarse manualmente.
6.	Para que el chat se abra integrado al asistente virtual Helper, es necesario habilitar el parámetro 423.


## Procedimiento

### Configurando el Smart Chat

Accede al menú principal > Parametrización > Chat

Se mostrarán los siguientes parámetros:

|Parámetro|Descripción|
|---------|---------|
|Habilitar el modo de invitado| Configure si el Smart Chat se mostrará en la pantalla de inicio de sesión. Las opciones serán Sí o No, por defecto es No. Si el usuario elige "Sí", el sistema solicitará el inicio de sesión del usuario. El inicio de sesión debe seguir el patrón: dominio\\login|
|Modo de invitado - ID del usuario| Es el número de identificación del usuario que iniciará sesión como invitado. Información contenida en la columna UserID de la tabla de usuarios|
|Modo de invitado - clave secreta| La clave secreta es la contraseña del usuario invitado|
|Mensaje de bienvenida| Cambiar o mantener el mensaje de bienvenida predeterminado|
|Empezar abierto| Cuando está activo, significa que Smart Chat siempre estará en el modo esperando por un mensaje. El valor predeterminado será No|
|Acción inicial| Cuando se le informa, se iniciará una acción desde el asistente virtual en la pantalla del Smart Chat|
|Guardar| Botón para guardar la configuración|

Después de guardar, la pantalla de Smart Chat estará disponible en la pantalla de inicio de sesión, así como todos los servicios configurados para Smart Chat o asistente virtual, siguiendo las restricciones, grupo y perfil de acceso, impuestas al usuario invitado.


A continuación hay algunos ejemplos de cómo utilizar el Chat de 4biz en diferentes escenarios:

### Acceso al Smart Chat sin configuración de Helper: Creación de tickets

1. Acceder a la pantalla Smart Portal o Centro de Experiencia;
2. Hacer clic en el icono "Hablar" en la parte inferior de la pantalla para iniciar la conversación;
3. Informar en el chat que desea crear un nuevo ticket y agregar la informaciones necesarias;
4. El sistema devolverá el número del ticket creado;
5. El sistema redirigirá a la pantalla de conversación;
6. Ingrese un nuevo mensaje en la pantalla de chat;
7. La atención puede asumir los siguientes estados:
   a. Esperando asistente (el asistente puede ser el solicitante o analista) - señalado por una bola verde sin llenar
   b. En línea - Ambas partes están activas para conversar - señaladas por una bola verde llena
8. Ambos estando en línea, es posible mantener la conversación;
9. Si una de las partes no está en línea y el parámetro 447 está configurado, el sistema envía un mensaje indicando.

### Acceso al Smart Chat sin configuración de Helper - Creación de tickets mediante la Búsqueda de Actividades

1. Acceder a la pantalla Smart Portal o Centro de Experiencia;
2. Hacer clic en el icono "Hablar" en la parte inferior de la pantalla para iniciar la conversación;
3. Informar el nombre de una Actividad;
4. El sistema devuelve las opciones para crear un nuevo servicio o reanudar la atención;

### Acceso al Smart Chat para búsqueda de Conocimiento

1. Acceder a la pantalla Smart Portal o Centro de Experiencia;
2. Hacer clic en el icono "Hablar" en la parte inferior de la pantalla para iniciar la conversación;
3. Informar el título o parte de un título del conocimiento;
4. El sistema devolverá las opciones de conocimiento encontradas y permitidas para su visualización;
5. Hacer clic en el título del conocimiento y el sistema abrirá la descripción del conocimiento;
6. El sistema presentará el botón de visualización y, al hacerlo clic, se abre el portal de conocimiento;
7. El sistema presentará el botón de cierre y, al hacerlo clic, reduce el conocimiento y regresa al estado original.

### Acceso al Asistente Virtual - Creación de Ticket

1. Hacer clic en el icono en la parte superior de la pantalla llamada "Virtual Assistant" para hablar con Helper;
2. Ingresar su búsqueda o asunto;
3. El asistente virtual puede identificar conocimientos o actividades para abrir;
4. Cuando el asistente virtual da el mensaje de fallback, se muestran inmediatamente las opciones "Hablar con el asistente" o "Reanudar Atención";
5. Hacer clic en el ícono para empezar la conversación;
6. El sistema devolverá el número del ticket creado;
7. La atención puede asumir los siguientes estados:
   a. Esperando asistente (el asistente puede ser el solicitante o analista) - señalado por una bola verde sin llenar
   b. En línea - Ambas partes están activas para conversar - señaladas por una bola verde llena
8. Ambos estando en línea, es posible mantener la conversación;
9. Si una de las partes no está en línea y el parámetro 447 está configurado, el sistema envía un mensaje indicandolo.

### Acceso al Asistente Virtual - Creación de ticket mediante Búsqueda de Actividad

1. Acceder a la pantalla Smart Portal o Centro de Experiencia;
2. Hacer clic en el icono "Hablar" en la parte inferior de la pantalla para iniciar la conversación;
3. Informar el nombre de una Actividad;
4. El sistema devuelve las opciones para crear un nuevo servicio o reanudar la atención;

### Acceso al Asistente virtual para búsqueda de Conocimiento

1. Acceder a la pantalla Smart Portal o Centro de Experiencia;
2. Hacer clic en el icono "Hablar" en la parte inferior de la pantalla para iniciar la conversación;
3. Informar el título o parte de un título del conocimiento;
4. El sistema devolverá las opciones de conocimiento encontradas y permitidas para su visualización;
5. Hacer clic en el título del conocimiento y el sistema abrirá su descripción;
6. El sistema presentará el botón de visualización y, al hacerlo clic, se abre el portal de conocimiento;
7. El sistema presentará el botón de cierre y, al hacerlo clic, reduce el conocimiento y regresa al estado original.

### Conversación del Smart Chat entre asistentes

1. Los analistas deben tener abierta la pantalla de ticket;
2. Los analistas deben vincular contactos para hablar a través de la pestaña Asistentes;
3. El analista involucrado en la conversación también debe vincular el contacto para recibir la conversación;
4. El analista abre la pestaña Asistentes, selecciona un contacto e inicia la conversación;
5. Si la otra parte tiene este analista en sus contactos, entonces puede mantener la comunicación;
6. Si la otra parte no tiene este analista en sus contactos, no puede mantenerse en contacto;
7. La atención puede asumir los siguientes estados:
   a. Esperando asistente (el asistente puede ser el solicitante o analista) - señalado por una bola verde sin llenar
   b. En línea - Ambas partes están activas para conversar - señaladas por una bola verde llena
8. Ambos estando en línea, es posible mantener la conversación.

### Conversación del Smart Chat entre solicitante y asistente

1. Los analistas deben tener abierta la pantalla de ticket;
2. El solicitante, al enviar un mensaje que el sistema enviará al asistente, independientemente de si el analista tiene el ticket abierto o no, el sistema muestra un signo de exclamación en el icono del SmartChat;
3. En la pestaña de atención aparecerá una bola azul informándole que hay nuevos mensajes en el chat;
4. Cuando el asistente abre la pantalla de la lista de atención, esta pantalla tiene los siguientes campos:
   a. Búsqueda por el número del ticket;
   b. Llamadas en cola - son atenciones que no capturaron el llamado
   c. Asistencia en curso - estas son llamadas que ya se han capturado y se están respondiendo.
   
### Conversación entre ambos canales - Chat y Helper

1. Para tener integración entre ambos canales, los parámetros deben estar habilitados: 402, 423, 441, 442, 450 3453;  
2. El parámetro 453 debe contener la información en formato <b>menú</b>. Ej.: Estimado, no entendí muy bien lo que pediste. Escriba <b>menú</b> para que pueda mostrarle las formas en que puedo ayudarlo;  
3. Ítem 1: el usuario hablará con el Helper;  
4. Ítem 2: el asistente virtual enviará varios mensajes de fallback;  
5. Ítem 3: El asistente virtual enviará opciones para hablar con el asistente o para abrir una nueva solicitud/incidente;  
6. Ítem 4: el usuario selecciona hablar con el asistente;  
7. Ítem 5: El asistente virtual abre un nuevo ticket y si hay un agente en el lado del ticket, el ticket se creará con una alerta;  
8. Ítem ​​6: En ese momento puede ocurrir interacción entre el usuario y el asistente.   

## Relacionado

[Configurar parametrización - chat](/es-es/4biz-helium/platform-administration/parameters-list/configure-parametrization-chat.html)


