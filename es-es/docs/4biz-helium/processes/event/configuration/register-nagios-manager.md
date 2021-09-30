title: Registrar gerente Nagios
Description: Registrar y mantener a los gerentes que serán responsables de monitorear los elementos de configuración y ocurrencia de eventos capturados desde el Nagios.
# Registrar gerente Nagios


Nagios es una herramienta de monitoreo de red. Él puede monitorear tanto hosts
como los servicios, alertando cuando ocurren problemas y también cuando los
problemas se resuelven. Los Hosts son los equipos y los Servicios son los
recursos ofrecidos por los equipos.

El objetivo de esta funcionalidad es registrar y mantener a los gerentes que
serán responsables de monitorear los elementos de configuración y ocurrencia de
eventos capturados desde el Nagios. Permite al usuario informar la frecuencia
que se procesará el Gerente, qué elementos de configuración va a administrar y
qué acciones se deben tomar automáticamente.

Esta funcionalidad ofrece diversas acciones, como, incluir, cambiar y borrar un
gerente de Nagios.

Antes de empezar
--------------------

Para registrar el gerente Nagios, es necesario registrar previamente la conexión
del 4biz Event Monitor, horario, categoría de ocurrencia, acción automática
y la conexión del 4biz Inventory.

Procedimiento
-----------------

1.  Acceder al menú principal Procesos \> Gestión de Evento \> Monitor Nagios \>
    Gerente Nagios;

2.  Completar los campos disponibles en cada area;

3.  En el área Ítem de Configuración Padre, es posible registrar el EC en
    4biz, con los datos del Host seleccionado. Hacer clic en "Crear EC". Es
    importante recordar que este registro sólo puede ser realizado si no hay un
    EC con la misma identificación del Host:

    -   Informar los datos del elemento de configuración hijo;

    -   Hacer relación entre el servicio Host y el elemento de configuración hijo.
        Cada servicio del host debe estar relacionado con su elemento de configuración hijo;

4.  Hacer clic en "Guardar".


Relacionado
-----------

[Registrar categoría de ocurencia](/es-es/4biz-helium/processes/event/configuration/register-occurence-category.html)

[Registar Conexión Event Monitor](/es-es/4biz-helium/processes/event/configuration/register-event-monitor-connection.html)

[Registrar conexión Nagios/Zabbix](/es-es/4biz-helium/processes/event/configuration/register-nagios-zabbix-connection.html)

[Registrar horario](/es-es/4biz-helium/processes/event/configuration/register-time.html)

[Registrar acción automatica](/es-es/4biz-helium/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
