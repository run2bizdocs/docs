Title: Configurando el Wildfly

# Configurando el Wildfly

Ingrese en el jboss-cli y ejecute los siguientes comandos:

``` shell
/subsystem=logging/root-logger=ROOT:write-attribute(name=level,value=INFO)
/subsystem=logging/console-handler=CONSOLE:write-attribute(name=level,value=INFO)
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/configuration=filter/rewrite=citsmart:add(target="/citsmart")
/subsystem=undertow/server=default-server/host=default-host/filter-ref=citsmart:add(predicate="regex('\^/?\$') and equals(/citsmart)")
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:add
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:write-attribute(name=pattern, value="%h %l %u [%t] \\"%r\\" %s %b \\"%{i,Referer}\\" \\"%{i,User-Agent}\\"")
/subsystem=messaging-activemq/server=default/jms-queue=filaDocumentoQueue:add(entries=["queue/filaDocumento","java:jboss/exported/jms/queue/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-topic=filaDocumentoTopic:add(entries=["topic/filaDocumento","java:jboss/exported/jms/topic/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-queue=builderInputQueue:add(entries=["queue/builderInputQueue","java:jboss/exported/jms/queue/queue/builderInputQueue"])
/subsystem=messaging-activemq/server=default/jms-queue=builderOutputQueue:add(entries=["queue/builderOutputQueue","java:jboss/exported/jms/queue/queue/builderOutputQueue"])
/subsystem=deployment-scanner/scanner=default:write-attribute(name=deployment-timeout,value=6000000)
```

## Próximo paso

[Configuracines extras de 4biz][1]

[1]:/es-es/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-extras.html
