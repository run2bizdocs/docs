
title: Implementar o Event Monitor
Description: Módulo que pretende ser un intermediario entre 4biz y soluciones de los clientes.

# Implementar o Event Monitor

Event Monitor - EVM - es un módulo que pretende ser un intermediario entre 4biz y soluciones de los clientes (por ejemplo, Nagios, 4biz Inventory), sirviendo como un repositorio de informaciones de eventos, generado por herramientas de monitoreo o proceso de inventario.

Para activarlo en una instancia del 4biz, es necesario descargar el paquete WAR y ejecutar la implementación en el servidor de aplicaciones Wildfly, que puede ser el mismo que el 4biz. Es importante observar que el EVM debe estar disponible en un puerto diferente de la aplicación 4biz. Además, notamos que el EVM no posee su propia interfaz, porque la gestión es hecha a través de la aplicación 4biz.

Procedimiento
----------

1. Descargar el paquete war del component EVM;
2. Descomprimir los archivos;
3. Copiar el paquete a la carpeta de implementación del servidor de la aplicación Wildfly;
4. Configurar [Propriedades del Sistema][1] con los datos de acceso del Mongo y de la instancia del 4biz;

Lo que hacer después
---------

Para probar el EVM, [configurar][2] las conexiones en la instancia del 4biz.

[1]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation.html
[2]:/es-es/4biz-helium/processes/event/configuration/register-event-monitor-connection.html
