Title: Implementar o 4biz Inventory

# Implementar o 4biz Inventory

O 4biz Inventory é um componente da Plataforma 4biz que permite coletar, registrar e gerenciar informações de ativos de T.I. Ele possibilita gerenciar o ciclo de vida dos itens de configuração de sua organização a partir do processo de Gerenciamento de Configuração.

![Arquitetura EVM e INV](images/cloud-arch-inv-evm.png)

Antes de começar
------------

O 4biz Inventory trabalha em conjunto com o [Monitor de Eventos 4biz - EVM][1], pois este serve como um orquestrador de dados. Portanto, para utilizar o Inventory, deve-se primeiro configurar o EVM.


## Procedimento

1. [Instalar][2] o servidor de aplicação Wildfly;
2. Fazer download do pacote WAR do componente Inventory;  
3. Descompactar os arquivos;  
4. Copiar o pacote para a pasta de implantação do servidor de aplicativos Wildfly (ex. /deployments);  
5. Configurar as [Propriedades do Sistema][3] com os dados da instância 4biz.

## O que fazer depois  

Para testar o Inventory, [configurar][4] as conexões na instância 4biz.

## Relacionado

[Implementar o 4biz Event Monitor][5]

[Gerenciamento de Configuração e Ativo][6]


[1]:/pt-br/4biz-helium/additional-features/add-ons/event-monitor.html
[2]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation.html
[3]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
[4]:/pt-br/4biz-helium/processes/event/configuration/set-inventory-connection.html
[5]:/pt-br/4biz-helium/additional-features/add-ons/event-monitor.html
[6]:/pt-br/4biz-helium/processes/configuration/overview.html



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021  
	
