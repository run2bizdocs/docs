title: Cadastrar gerente Global
Description: Tem como objetivo criar regras para monitorar vários tipos de eventos.
# Cadastrar gerente Global

Esta funcionalidade tem como objetivo criar regras para monitorar vários tipos
de eventos.

Cada gerente de eventos global contém uma EPL para *Information* (informação),
*Warning* (advertência) e/ou *Exception* (exceção). EPL é uma linguagem de
correlação de eventos utilizada pelo Esper (Espertech). Na inicialização do
4biz Event Monitor, estes EPL são importados para a engine do Esper, de modo
que um novo evento correlacionado será criado toda vez que a condição definida
na EPL for satisfeita. 

Eventos e alertas relacionados a 

- Processo de Negócios, Requisitos de Nível de Serviço, 

- Consciência de eventos semelhantes e múltiplos por IC ou Serviço, 

- Conexão com códigos e categorizações de priorização de Incidentes,

- Ação de controle, 

- Acesso a informações sobre ICs dependentes e de suporte, programação de alterações e informações de erro conhecidas de fornecedores

Exemplo de uma EPL que faz correlação entre os eventos do
4biz Inventory e Nagios: \@Description ('Para qualquer evento do Nagios que
ocorrer depois de um evento qualquer do Inventory, nos últimos 10 minutos)
select \* from pattern [every a=EventoCheckInventory-\>b=EventoServicoNagios
where timer:within(10minutes)].

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir um gerente Global.

Antes de começar
--------------------

Para cadastrar o gerente Global é necessário cadastrar previamente a conexão do
4biz Event Monitor, o horário, a categoria de ocorrência, a ação automática
e a conexão do 4biz Inventory.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Processos \>
    Gerência de Evento \> Gerente Global;

2.  Preencher os campos disponibilizados em cada área:

    -   Informe os dados da **Ação para Information**:

         -   Selecionar a ação que será disparada quando houver uma ocorrência de
             evento do tipo *information*, o grau de urgência e impacto. As regras para
             essa ação, são definidas utilizando a Linguagem de Processamento de
             Eventos - EPL. Clicar no botão "Validar EPL de Information" para validar
             a EPL informada.

    -   Informe os dados da **Ação para Warning**:

        -   Selecionar a ação que será disparada quando houver uma ocorrência de
            evento do tipo *warning*, o grau de urgência e impacto. As regras para
            essa ação, são definidas utilizando a Linguagem de Processamento de
            Eventos - EPL. Clicar no botão "Validar EPL de Warning" para validar a
            EPL informada.

    -   Informe os dados da **Ação para Exception**:

        -   Selecionar a ação que será disparada quando houver uma ocorrência de
            evento do tipo *exception*, o grau de urgência e impacto. As regras para
            essa ação, são definidas utilizando a Linguagem de Processamento de
            Eventos - EPL. Clicar no botão "Validar EPL de Exception" para validar a
            EPL informada.

3.  Clicar no botão "Gravar".



Relacionado
-----------

[Cadastrar categoria de ocorrência](/pt-br/4biz-helium/processes/event/configuration/register-occurence-category.html)

[Cadastrar Conexão Event Monitor](/pt-br/4biz-helium/processes/event/configuration/register-event-monitor-connection.html)

[Cadastrar horário](/pt-br/4biz-helium/processes/event/configuration/register-time.html)

[Configurar Conexão Inventory](/pt-br/4biz-helium/processes/event/configuration/set-inventory-connection.html)

[Cadastrar ação automática](/pt-br/4biz-helium/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
 
