Title: Deploying 4biz

# Deploying 4biz

Download the 4biz and Builder WAR package from the partner portal. Send to server using scp to the folder /tmp. 4biz installation consists of the following steps:

1. Deploy 4biz Tracker package
2. Deploy Builder package
3. Start 4Biz setup

Unzip the 4biz Platform package if it's in .zip format:

``` shell
[root@server /tmp]# unzip 4bizITSM-Enterprise-8.0.2.0.war.zip
```

Copy to the application server in the folder `standalone/deployments`:

``` shell
[root@server /tmp]# cp 4bizITSM-Enterprise-8.0.2.0.war /opt/wildfly/standalone/deployments/
```
Note the log `/opt/wildfly/standalone/log/server.log` with the option `tail -f` until the message below appears:

``` shell
2019-11-14 17:20:37,731 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 1) WFLYSRV0010: Deployed "4bizITSM-Enterprise-8.0.2.0.war" (runtime-name : "4bizITSM-Enterprise-8.0.2.0.war")
```

The above message confirms that the deployment was performed. The same applies to the Builder package. Copy Builder to the folder `standalone/deployments`:

``` shell
[root@server /tmp]# cp 4biz-builder-web-1.3.2.1.war /opt/wildfly/standalone/deployments/
```

Note the log `/opt/wildfly/standalone/log/server.log` with the option `tail -f` until the message below appears:

``` shell
2019-11-14 17:37:43,647 INFO  [org.jboss.as.server] (DeploymentScanner-threads - 2) WFLYSRV0010: Deployed "4biz-builder-web-1.3.2.1.war" (runtime-name : "4biz-builder-web-1.3.2.1.war")
```

## Accessing 4biz for the first time

After deploying, access 4biz through the URL: if a domain has been set, go to https://DOMAIN/4biz, If you have configured via IP, access https://IP_ADDRESS/4biz.

!!! info "Supported Browsers"
    For the proper functioning of the system, you should use the following minimum versions of the main browsers: **Microsoft EDGE** (Edge 42.17134.0 / Microsoft EdgeHTML 17.17134 or higher); **Google Chrome** (version 76.0.3809.132 or higher); **Mozila Firefox** (version 69.0 or higher).

## Next step

[Completing the installation][1]

[1]:/en-us/4biz-helium/get-started/installation-and-upgrade/perform-installation/setup-4biz.html
