Title: Implementar Event Monitor  

# Implementar o Event Monitor

Event Monitor - EVM - é um módulo que visa ser um intermediário entre o 4biz e soluções de clientes (por exemplo, Nagios, 4biz Inventory), servindo como um repositório de informações de eventos, gerado por ferramentas de monitoramento ou processo de inventário.

Para ativá-lo em uma instância do 4biz, é necessário fazer o download do pacote WAR e executar a implementação no servidor de aplicativos Wildfly, que pode ser o mesmo que o 4biz. É importante observar que o EVM deve estar disponível em uma porta diferente da instância 4biz. Lembramos que o EVM não possui sua própria interface, porque o gerenciamento é feito através da instância 4biz.

## Procedimento

1. Baixar o pacote .war do componente EVM;  
2. Descomprimir os arquivos;  
3. Copiar o pacote para a pasta de implementação do servidor de aplicação Wildfly;  
4. Configurar [Propriedades do Sistema][2] com dados de acesso do Mongo e a instância do 4biz.

## O que fazer a seguir  

Para testar o EVM, [configurar][1] as conexões na instância do 4biz.  

[1]:/pt-br/4biz-helium/processes/event/configuration/register-event-monitor-connection.html  
[2]:/pt-br/4biz-helium/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
