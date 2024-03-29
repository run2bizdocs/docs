title: Aprovar um ticket
Description: Em alguns casos, os tickets do tipo "Requisição" irão passar por uma fase de aprovação para execução dos mesmos. Isso irá depender do fluxo de trabalho do ticket, o qual está vinculado a atividade de requisição do serviço. 
# Aprovar um ticket

Quando um ticket possuir uma atividade de aprovação é possível confirmar ou
rejeitar este pedido utilizando o recurso para esta finalidade. Neste sentido, o
fluxo de trabalho do ticket deve conter uma tarefa de usuário (aba Identificação
\> Botão   "É uma tarefa de aprovação? = SIM"), o qual está vinculado a
atividade.

!!! Abstract "ATENÇÃO"

    Para aprovação de forma simplificada do ticket é preciso que o fluxo da
    solicitação de serviço possua uma tarefa do tipo aprovação, assim, o botão de
    aprovação rápida estará visível.


Antes de começar
----------------

É necessário o cadastro prévio do ticket e possuir permissão para aprovar o
mesmo.

Procedimento 
-------------


1.  Acessar a funcionalidade Ticket navegando pelo menu principal Processos \>
    Gerência de Requisição e Incidente \> Ticket;

2.  Localizar o ticket desejado, pressionar sobre o mesmo e clicar no
    ícone “Abrir”;

3.  Verificar o ticket e registrar as informações necessárias referente a
    aprovação do mesmo;

4.  Marcar umas das opções de aprovação: **Aprovada** ou **Não aprovada**:

    -   Se marcar "Aprovada", descrever as observações, se achar necessário;

    -   Se marcar "Não aprovada", descrever as observações, informar a
        justificativa e o complemento da justificativa.

5.  Se a tarefa do ticket for do tipo aprovação o sistema irá apresentar abaixo do campo Direcionar para Grupo o Botão: "Ver aprovações". Ao clicar em Ver Aprovações,  será apresentado o Histórico de aprovações da tarefa;

6.  No histórico de aprovações da tarefa é apresentado 3 abas com informações:

- Aba **Executadas**, onde serão apresentadas as seguintes colunas

|Coluna|Descrição|
|------|---------|
|Responsável| Será apresentado o nome do usuário que votou|
|Resultado| Será apresentado o voto do usuário|
|Comentário| Será apresentado, se houver, o comentário do usuário|
|Data/Hora| Será apresentado a Data e a Hora do voto|
|Quantidade de aprovações| Será apresentada a quantidade de votos positivos da aprovação|
|Quantidade de abstenções| Será apresentado a quantidade de votos em abstenção|
|Quantidade de rejeições| Será apresentado a quantidade de votos negativos para aprovação|
|Aprovações pendentes| Será apresentado quantas usuários antes faltam votar|

- Aba **Pendentes** com o campo:

|Coluna|Descrição|
|------|---------|
|Responsável| Será apresentado o nome dos usuários que ainda não votaram|

- Aba **Histórico** com os campos:

|Campo|Descrição|
|-----|---------|
|Responsável| Será apresentado o nome do usuário que mudou o voto|
|Resultado| Será apresentado o voto anterior do usuário|
|Comentário| Será apresentado, se houver, o comentário do usuário|
|Data/Hora| Será apresentado a Data e a Hora da mudança do voto|


7.  Clicar no botão de “Opções” e logo em seguida clicar no botão “Gravar e
    avançar fluxo” para gravar e avançar o fluxo. Feito isso, se o ticket
    estiver sido aprovado, o mesmo será encaminhado para a fase de execução, ou
    seja, para o atendimento do mesmo. Mas, caso o ticket não seja aprovado, o
    mesmo será encerrado.

Relacionado
-----------

[Criar um ticket](/pt-br/4biz-helium/processes/tickets/use/create-ticket.html)

[Cadastrar um grupo](/pt-br/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Configurar permissão de acesso do gerenciamento de requisições/incidentes](/pt-br/4biz-helium/processes/tickets/configuration/access-ticket-management.html)

[Criar um fluxo de trabalho](/pt-br/4biz-helium/tracker/use/create-flow.html)

[Configurar tarefa de usuário](/pt-br/4biz-helium/tracker/use/user-task-configure.html)

<!-- <i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)'
-->
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021
