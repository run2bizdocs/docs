
title: Implementar 4biz Inventory

# Implementar 4biz Inventory

4biz Inventory es un componente de la plataforma 4biz que permite recopilar, registrar y administrar información de activos de TI. Permite gestionar el ciclo de vida de los elementos de configuración de su organización desde el proceso de Gestión de Configuración.

![Arquitectura 4biz EVM y INV](images/cloud-arch-inv-evm.png)

Antes de empezar
-------------

El 4biz Inventory trabaja en conjunto con el [Monitor de Eventos 4biz - EVM][1] y como un colector de datos (ej.: paquetes XML) el EVM sirve como repositorios para esta información. Por lo tanto, para activar el inventario, primero debe configurar el EVM.  


## Procedimiento


1. [Instalar][2] el servidor de aplicación Wildfly;
2. Descargar el paquete WAR del componente Inventory;
3. Descomprimir los archivos;  
4. Copiar el paquete a la carpeta de implementación del servidor de aplicaciones Wildfly (ej.: /deployments);  
5. Configurar las [Propriedades del Sistema][3] con los datos de la instancia 4biz.

## Lo que hacer después

Para probar el Inventory, [configurar][4] las conexiones en la instancia 4biz.

## Relacionado

[Implementar 4biz Event Monitor][5]

[Gestión de Configuración y Activos][6]


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

[1]:/es-es/4biz-helium/additional-features/add-ons/event-monitor.html
[2]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation.html
[3]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracion-del-system-properties
[4]:/es-es/4biz-helium/processes/event/configuration/set-inventory-connection.html
[5]:/es-es/4biz-helium/additional-features/add-ons/event-monitor.html
[6]:/es-es/4biz-helium/processes/configuration/overview.html
