title: Validar e encerrar o ticket
Description: Após o atendimento do ticket, a execução do mesmo deverá ser validada e o ticket encerrado.

# Validar e encerrar o ticket

Após o atendimento do ticket, a execução do mesmo deverá ser validada e o ticket encerrado.

Antes de começar
----------------

É necessário o cadastro prévio do ticket e possuir permissão para validar o
mesmo.

Procedimento
------------

1.  Acessar a funcionalidade de Gerenciamento de Tickets navegando pelo menu
    principal Processos \> Gerência de Ticket \> Ticket;

2.  Localizar o ticket desejado, pressionar sobre o mesmo e clicar no
    ícone “Abrir”;

3.  Certificar se o atendimento do ticket foi realizado de acordo com o que foi
    solicitado;

4.  Na área “Situação” escolher a opção “Resolvida”, preencher
    os dados para encerrar o ticket;

    - Se o tipo de solicitação for "Incidente":

        * Categoria de Solução: selecionar a categoria de solução do incidente;

        * Detalhamento da Causa: descrever os detalhes da causa do incidente;

        * Solução Resposta: descrever os detalhes da solução que foi realizada 
          para atendimento do incidente;

        * Gravar Solução/Resposta na Base de Conhecimento: para que o checkbox 
          "Gravar Solução/Resposta na Base de Conhecimento" esteja visível,
          verificar a parametrização do processo de Gestão do Conhecimento;
          
        !!! abstract "NOTE"
        
            Para reduzir as opções dos campos "Causa" e "Categoria da Solução", apresentadas ao encerrar o ticket,
            a ferramenta proporciona o vínculo de Causa e Categoria de Solução a serviços específicos.
            Para isso, é necessário a criação de uma "Causa", nela é possível vincular a  causas relacionadas. Também 
            é necessário a criação da "Categoria de solução", nela é possível vincular uma causa e dependendo dela, 
            ela trará todas as causas relacionadas à causa principal.
            Depois, no Portfólio de serviços desejado, você irá vincular as Causas e Categoria da Solução no serviço
            que achar mais apropriado.
            Na hora de execução do ticket, quando for descrever os campos de encerramento, as opções para "Causa" e 
            "Categoria da Solução" serão de acordo ao que foi vinculado ao serviço dentro do Portfólio, reduzindo
            assim as opções disponíveis, com foco apenas no necessário

        !!! Abstract "ATENÇÃO"
            
            Para que a opção “Gravar solução/Resposta na Base de Conhecimento” 
            fique disponível ao marcar a opção “Resolvida” do ticket, é necessário 
            configurar os parâmetros 182 e 192.

        * Justificativa SLA vencido: a visibilidade desse campo está condicionada ao 
          status de SLA vencido para o atendimento em questão;

        * Solução Temporária: indicar se a atividade realizada para atendimento do 
          incidente foi uma solução temporária.


    - Se o tipo de solicitação for "Requisição", preencher o campo "Solução Resposta", 
      descrever o que foi realizado para atendimento da requisição de serviço.

    !!! Abstract "ATENÇÃO"

        Os passos de resolução do Ticket podem ser a sugestão de um novo conhecimento, sendo 
        avaliado previamente para efetivação. É possível sugerir também um nome para este novo 
        conhecimento no campo "Título Base de Conhecimento".

5.  Clicar no botão flutuante “Opções” e definir a etapa seguinte da solicitação:

     -   “Salvar alterações”;

     -   “Enviar ticket”.


Relacionado
-----------

[A área de trabalho da Central de Serviços](/pt-br/4biz-helium/processes/tickets/use/desktop-of-service-desk.html)

[Criar um ticket](/pt-br/4biz-helium/processes/tickets/use/create-ticket.html)

[Cadastrar um grupo](/pt-br/4biz-helium/initial-settings/access-settings/user/register-groups.html)

[Configurar permissão de acesso do gerenciamento de Tickets](/pt-br/4biz-helium/initial-settings/access-settings/profile/access-ticket-management.html)  

<!-- <i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)
-->
!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
