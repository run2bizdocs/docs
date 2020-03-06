Title: Configuring the Wildfly

# Configuring the Wildfly

Enter the jboss-cli and run the commands below:

``` shell
/subsystem=logging/root-logger=ROOT:write-attribute(name=level,value=INFO)
/subsystem=logging/console-handler=CONSOLE:write-attribute(name=level,value=INFO)
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/configuration=filter/rewrite=4biz:add(target="/4biz")
/subsystem=undertow/server=default-server/host=default-host/filter-ref=4biz:add(predicate="regex('\^/?\$') and equals(/4biz)")
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:add
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:write-attribute(name=pattern, value="%h %l %u [%t] \\"%r\\" %s %b \\"%{i,Referer}\\" \\"%{i,User-Agent}\\"")
/subsystem=messaging-activemq/server=default/jms-queue=filaDocumentoQueue:add(entries=["queue/filaDocumento","java:jboss/exported/jms/queue/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-topic=filaDocumentoTopic:add(entries=["topic/filaDocumento","java:jboss/exported/jms/topic/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-queue=BuilderInputQueue:add(entries=["queuebuilderInputQueue","java:jboss/exported/jms/queue/queuebuilderInputQueue"])
/subsystem=messaging-activemq/server=default/jms-queue=BuilderOutputQueue:add(entries=["queuebuilderOutputQueue","java:jboss/exported/jms/queue/queuebuilderOutputQueue"])
/subsystem=deployment-scanner/scanner=default:write-attribute(name=deployment-timeout,value=6000000)
```

## Next step

[4biz extra settings][1]

[1]:/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation/conf-extras.html
