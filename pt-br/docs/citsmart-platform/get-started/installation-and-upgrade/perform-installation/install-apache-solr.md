Title: Instalando o Apache SOLR

# Instalando o Apache SOLR

A versão homologada do Apache Solr para o CITSmart é a 6.4.2. O download do pacote pode ser feito através do próprio site no URL https://archive.apache.org/dist/lucene/solr/. No caso específico para o CITSmart também será necessário fazer o download dos arquivos de configuração (Knowledge Base Confs) que podem ser baixados na área de relacionamento com o parceiro, no item Installation Components.

## Instalando o SOLR

Faça o download do pacote para o /tmp do servidor

``` shell
[root@server /tmp]# https://archive.apache.org/dist/lucene/solr/6.4.2/solr-6.4.2.tgz
```
Extraia o script de instalação com comando abaixo:

``` shell
[root@server /tmp]# tar -xvf solr-6.4.2.tgz solr-6.4.2/bin/install_solr_service.sh --strip-components=2
solr-6.4.2/bin/install_solr_service.sh
```
Execute o script de instalação da seguinte forma:

``` shell
[root@server /tmp]# ./install_solr_service.sh solr-6.4.2.tgz
id: solr: no such user
Creating new user: solr

Extracting solr-6.4.2.tgz to /opt


Installing symlink /opt/solr -> /opt/solr-6.4.2 ...


Installing /etc/init.d/solr script ...


Installing /etc/default/solr.in.sh ...

Service solr installed.
Customize Solr startup configuration in /etc/default/solr.in.sh
Waiting up to 180 seconds to see Solr running on port 8983 [\]
Started Solr server on port 8983 (pid=23010). Happy searching!

Found 1 Solr nodes:

Solr process 23010 running on port 8983
{
  "solr_home":"/var/solr/data",
  "version":"6.4.2 34a975ca3d4bd7fa121340e5bcbf165929e0542f - ishan - 2017-03-01 23:30:23",
  "startTime":"2019-11-14T17:45:18.589Z",
  "uptime":"0 days, 0 hours, 0 minutes, 7 seconds",
  "memory":"21.5 MB (%4.4) of 490.7 MB"}

[root@server /tmp]#

```
Importe as configurações do CITSmart para o SOLR. Para isso, envie via scp  para o servidor o arquivo base_conhecimento_configs.zip que foi feito download da área de parceiros. Supondo que o arquivo esteja no `/tmp`, e que você tenha o unzip, execute o comando abaixo:

``` shell
[root@server /tmp]# unzip base_conhecimento_configs.zip -d /opt/solr-6.4.2/
```
Faça login com usupário do SOLR:

``` shell
[root@server /tmp]# su - solr -s /bin/bash
```
E execute o comando abaixo:

``` shell
[root@server /tmp]# /opt/solr/bin/solr create -c base_conhecimento -d /opt/solr/base_conhecimento_configs -s 2 -rf 2

Copying configuration to new core instance directory:
/var/solr/data/base_conhecimento

Creating new core 'base_conhecimento' using command:
http://localhost:8983/solr/admin/cores?action=CREATE&name=base_conhecimento&instanceDir=base_conhecimento

{
  "responseHeader":{
    "status":0,
    "QTime":1606},
  "core":"base_conhecimento"}


[root@server /tmp]#

```
Após a mensagem acima, o SOLR está configurado.


## Próximo passo

[Instalando o MongoDB][1]

[1]:/pt-br/citsmart-platform-8/get-started/installation-and-upgrade/perform-installation/install-mongo.html
