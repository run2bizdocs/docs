Title: Disponer Helper en la interfaz 4biz
# Disponer Helper en la interfaz 4biz

Helper ya se integra nativamente al 4biz, entonces es muy fácil añadirla a su entorno.

## Procedimiento

1. Con acceso de administrador, acceda a la pantalla de parámetros del 4biz;
2. Cambiar el valor del parámetro “402 Helper Assistant - External URL” para http://[nombre-servidor].helperassistant.com
3. Cambiar el valor del parámetro “441 Helper Assistant - Conversation API” para http://[nombre-servidor][sigla-idioma].helperassistant.com/webhooks/rest/webhook y hacer clic en "Guardar"
4. Cambiar el valor del parámetro “442 Helper Assistant - Parameters API” para http://[nombre-servidor][sigla-idioma].helperassistant.com/conversations/
5. Configurar el parámetro 453 "Mensaje predeterminada de Fallback de la Helper Assistant", con un mensaje que Helper responderá cuando no tenga respuesta a esa pregunta.
6. Habilitar el parámetro 423 "Habilitar Helper Assistant en el área interna del sistema", un parámetro que permite a los analistas iterar con ANUVA
7. Habilitar el parámetro 450 "Habilitar Helper Assistant en el área externa del sistema", parámetro que permite a los usuarios finales iterar con ANUVA.    

!!! note "NOTA"
    
    Para la abreviatura de los idiomas, utilice EN (Inglés) y PT (Portugués-Brasil).
    Si estos parámetros no están disponibles, actualice su versión de 4biz.
   
 
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
