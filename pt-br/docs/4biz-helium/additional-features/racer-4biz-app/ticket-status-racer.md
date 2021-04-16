Title: Situação dos Tickets no Racer 4biz  
Description: Nesse documento vamos ver as ações possíveis de realizar no tratamento de um ticket.

# Situação dos Tickets no Racer 4biz  

Nesse documento vamos ver as ações possíveis de realizar no tratamento de um ticket dentro do aplicativo Racer 4Biz. 

## Antes de começar

- [x] Instalar o aplicativo Racer4biz no Android ou no IOS  
- [x] Possuir um usuário cadastrado no sistema através da aplicação

Além disso, é necessário realizar algumas configurações na plataforma 4biz de Webservice, Unidade e Tickets.

**Webservice**

Acessar a funcionalidade através do menu principal Sistema > Webservice > Operação Webservice.  
Na aba Pesquisa de Operações, buscar por cada um dos webservices abaixo, em seguida em cada um clicar no botão "Adicionar grupo" e incluir o(s) grupo(s) que o(s) atendente(s) estão vinculados:

    - request_add_attachments
    - request_updateRequestList
    - request_userLocation
    - request_saveRequest
    - request_uploadAttachment
    - request_getByUser
    - request_saveRequestNote
    - request_updateRequestNoteList
    - request_updateRequestListGroups
    - request_uploadSignature
    - parameter_query
    - registerdevice_query
    
O webservice de request_updateStatus deverá estar configurado com as seguintes informações:
    
    - ID padrão para a justificativa da alteração do chamado;
    - Adicionar os grupos que possuem permissão para modificar o status de um chamado;

Clicar no botão "Gravar" após configurar os grupos em cada webservice.

**Unidade**

Acessar a funcionalidade através do menu principal Cadastros Gerais > Gerência de Pessoal > Unidade.  
Buscar pela unidade na aba Pesquisa de Unidade e selecionar a escolhida.  
Na aba Cadastro de Unidade com a unidade já escolhida, clicar no botão "Obter Coordenadas".  
Clicar em "Gravar".

**Tickets**

É necessário possuir permissão para visualizar, capturar e realizar as ações possíveis dentro do ticket.  
Para reclassificar um ticket o usuário tem que pertencer a um grupo executor, na tela de grupo vincular o Fluxo a opção de "Alterar SLA", além de ter a permissão para "criar" no fluxo da atividade destino, isso quando a reclassificação incluir troca de atividade e se for um cenário de fluxos diferentes.  
O grupo deverá possuir a permissão de suspender no fluxo da atividade.  
O administrador poderá habilitar o parâmetro para envio de e-mail específico:

    - 290 - ID do modelo de e-mail enviado ao suspender uma solicitação de serviço;

O administrador poderá habilitar a obrigatoriedade do campo para complemento da suspensão:

    - 372 - Habilitar complemento obrigatório ao suspender a solicitação

O administrador deverá ter cadastrado as Justificativas de Solicitação para suspender o chamado.  
O administrador deverá habilitar o parâmetro que limita o período para abertura de um chamado, após o seu encerramento:

    - 171 - Limite de dias para a reabertura de Tickets de serviços;

O administrador poderá habilitar o parâmetro para envio de e-mail específico:

    - 291 - ID do modelo de e-mail enviado ao reativar uma solicitação de serviço;

O administrador deverá habilitar os seguintes parâmetros para receber notificações Push:

    - 350 - Habilita o envio de notificações para celulares;
    - 352 - Habilita o envio de notificações para celulares durante a criação de solicitações;
    - 353 - Habilita o envio de notificações para celulares durante a atualização de solicitações informando atendimentos próximos;  
    - 460 - Habilita o envio de notificações para celulares durante a atualização de solicitações.

## Procedimento

Abra o aplicativo Racer4biz no celular. Faça Login no aplicativo e acesse os tickets.

### Detalhes do ticket

Ao acessar um ticket, você terá acesso a todos os detalhes, ações e informações para o ticket escolhido. Temos como informações o seguinte:

1. Um Símbolo informando o tipo do ticket;	
2. A situação do ticket;
3. A Prioridade do ticket;
4. A tarefa do ticket;
5. O grupo atual do ticket;
6. O SLA do ticket;
7. O tempo limite para a entrega do ticket;
8. O solicitante do Ticket. Exibido com o seu avatar, o seu nome e o seu telefone. Ao selecionar o solicitante é aberta uma tela com uma seta para voltar e as seguintes informações:

       - O avatar do solicitante;
       - O nome do solicitante;
       - O Símbolo e o nome chamada, que ao ser selecionado redireciona o celular para realizar uma chamada para o número cadastrado;
       - O Símbolo e o nome Mensagem, que ao ser selecionado redireciona o celular para enviar uma mensagem para o número cadastrado;
       - O Símbolo e o nome E-mail, que ao ser selecionado redireciona o celular para enviar um E-mail para o e-mail cadastrado;
       - O Telefone do solicitante;
       - O e-mail do solicitante;
       - O endereço do solicitante.

9. O responsável do Ticket. Exibido com o seu avatar, o seu nome e o seu telefone. Ao selecionar o responsável é aberta uma tela com uma seta para voltar e as seguintes informações:

       - O avatar do responsável;
       - O nome do responsável;
       - O Símbolo e o nome chamada, que ao ser selecionado redireciona o celular para realizar uma chamada para o número cadastrado;
       - O Símbolo e o nome Mensagem, que ao ser selecionado redireciona o celular para enviar uma mensagem para o número cadastrado;
       - O Símbolo e o nome E-mail, que ao ser selecionado redireciona o celular para enviar um E-mail para o e-mail cadastrado;
       - O Telefone do responsável;
       - O e-mail do responsável;
       - O endereço do responsável.

10. A descrição do ticket;
11. Local de destino: Apresenta o nome do local seguido de um mapa com a localização da unidade do solicitante do ticket;
12. Formulário de acompanhamento: Ao ser selecionado é aberta uma tela com uma seta para voltar com o Título: Questionário e o número do ticket aberto. A existência de um questionário será definida pelo administrador na aplicação através da configuração de portfólio ou do fluxo. Caso haja formulário as perguntas serão definidas pelo administrador do contrato e preenchidas durante o atendimento do ticket;

        - Respostas do formulário de criação: Essa função poderá conter as respostas do formulário de criação.

13. Anexo. Ao ser selecionado é aberta uma tela com uma seta para voltar com o Título: Anexos.

    !!! note "NOTE"
    
        Caso ainda não haja nenhum anexo inserido no ticket:  
        
            - Será apresentada uma mensagem: Nenhum anexo foi adicionado;
            - Um botão Adicionar anexo. Que ao ser selecionado abre uma opção para selecionar o arquivo desejado no celular. Ao selecionar o arquivo é apresentada a mensagem: Novo Anexo adicionado com sucesso! E o Botão de Ok.
            
        Caso haja anexo adicionado no ticket:
        
            - O aplicativo apresentará a quantidade de anexos;
            - Ao selecionar a aba Anexos será apresentado o nome do anexo;
            - Um botão com 3 pontinhos que ao ser selecionado apresenta a opção excluir anexo, que ao ser selecionada apresenta uma janela com o Título Excluir anexo, a mensagem Tem certeza de que deseja excluir este documento em anexo?, o botão cancelar (que retorna para a tela anterior) e o botão confirmar (que remova o anexo do ticket).
            
            
14. Artigos de conhecimento. Ao ser selecionado é aberta uma tela com seta para voltar com o Título: Conhecimento e uma Lupa que ao ser selecionada abre um campo de pesquisar que possibilita digitar o nome a ser pesquisado na base de conhecimento.

        - A pesquisa é feita pelo título do anexo ou parte do conteúdo do conhecimento;
        - Para que o aplicativo liste corretamente os conhecimentos garanta que a indexação da base de conhecimento esteja atualizada na aplicação;
        - Caso o ticket não tenha nenhum conhecimento vinculado, será presentada a mensagem: O ticket selecionado não tem nenhum conhecimento vinculado a ele. E o Botão OK.
        - Será apresentado o Título: Base de Conhecimentos e uma lista com os conhecimentos. Cada item da lista terá: O autor; O nome do conhecimento; A descrição do conhecimento; Um botão para Vincular o vincular o conhecimento, caso ele não esteja vinculado ao ticket; Um símbolo de vinculado e um botão de Desvincular, caso ele esteja vinculado ao ticket.

15. Portfólio de serviços e contrato. Ao ser selecionado é aberta uma tela com seta para voltar, com o Título: Portfólio/contrato e as seguintes informações:

        - Uma caixa com o Título: Portfólio e o nome do portfólio;
        - Uma caixa com o Título: Serviço e o nome do serviço;
        - Uma caixa com o Título: Atividade e o nome da atividade;
        - Uma caixa com o Título: Contrato e a descrição do contrato;

16. Comentários. Ao ser selecionado é aberta uma tela com seta para voltar com o Título: Comentários e as seguintes informações:

    1. Caso não haja nenhum comentário será exibida a seguinte mensagem: Não há comentário e o botão Ok;
    
       Na tela será exibida e mensagem: Não há nenhum comentário na lista e um botão: Adicionar comentário. Ao selecionar o botão, Será aberta uma nova tela com seta para voltar, Título Adicionar comentário e as seguintes informações:
       
           - Chave para selecionar se o campo é Público;
           - Ao selecionar essa opção, o autor do comentário permite a visualização por parte do solicitante;
           - Chave para selecionar se é para enviar o comentário por e-mail;
           - O envio de e-mail depende da correta parametrização da aplicação;
           - Caixa para digitar o comentário;
           - Título: Lançar horas (opcional);
           - Campo para selecionar a data, que abre um calendário;
           - Campo para digitar a hora;
           - Botão Enviar;
            Se o campo comentário não for preenchido é exibida uma mensagem: Você deve informar uma descrição para o comentário. E o botão Ok.
            Se tudo estiver correto o comentário é adicionado e apresentada a mensagem: Comentário enviado com sucesso. E o botão Ok que retorna para a tela anterior; 

    2. Caso haja comentário, será exibida a lista de comentários da seguinte maneira:  
    
           - Nome do autor do comentário;
           - O comentário;
           - Data e hora do comentário;
           - Botão Responder, que abre a mesma tele de adicionar comentário;
           - Botão 3 pontinhos, com as opções de editar(abre a mesma tela de adicionar comentário, mas com as informações do comentário preenchidas) e excluir comentário (apresenta uma mensagem: Tem certeza de que deseja excluir este comentário? E uma opção para Cancelar e outra para Confirmar); 
           - Botão com sinal +, que abre a tela de adicionar comentário;
           
17. Histórico do Ticket. Ao ser selecionado é aberta uma tela com seta para voltar, Título: Histórico do ticket e uma lista com as seguintes informações:

        - Data da alteração;
        - Nome de quem fez a alteração;
        - Hora da alteração;
        - Ip da máquina que fez a alteração;
        - A ação que foi executada na alteração;
        - O detalhamento da alteração;

18. Ação. Ao ser selecionado é aberta uma tela com seta para voltar, Título: Ação e as seguintes informações:

    1. Campo para selecionar a Ação, que pode ser: Aprovar Ticket ou Recusar Ticket;
    
           - As ações apresentadas dependem do desenho de fluxo determinado para a atividade criada.
           
19. Título: Direcionar para Grupo, seguido de um campo para seleção com o Título: Selecionar grupo, que ao ser selecionada apresenta uma lista com todos os grupos cadastrados;
20. Botão: Salvar e Sair, que ser selecionado apresenta um caixa com o Título: Deseja salvar e sair?, a Mensagem: Todas as alterações serão salvas e você retornará para a tela de listagem. E os botões Voltar e Salvar e Sair;
21. Botão: Salvar e Avançar, que ao ser selecionado apresenta um caixa com o Título: Sucesso, a Mensagem: Avançado para a próxima fase e o botão OK.


## Trabalhando no ticket

Para acessarmos as possibilidades de ações dentro de um ticket no aplicativo, vamos selecionar um dos tickets na fila. Para as ações a seguir iremos abordar o caso de um ticket **em andamento**.

### Capturar ticket

!!! warning "ATENÇÃO"

    Para capturar um ticket, ele deve estar aberto e checado. O usuário pode realizar check-in em mais de um ticket. Mostraremos mais adiante nesse documento como relaizar o check-in.
    
1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Capturar Ticket".  
3. Ao selecionar essa opção, irá abrir um pop-up com a mensagem: Capturar ticket número #0000. Você pode cancelar a captura e voltará para a tela do ticket selecionado, ou você pode confirmar a captura e salvar essa informação. O ticket então estará sob sua responsabilidade.  

!!! note "NOTA"

        O usuário pode realizar a captura de mais de um ticket por vez.

### Suspender ticket

!!!note "NOTA""

        Para efetivar a suspensão o usuário deverá ter permissão para tal ação, além de possuir uma justificativa de suspensão previamente cadastrada.

1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Suspender Ticket".  
3. Ao selecionar a opção de suspender ticket é aberta uma nova tela com os campos:

- Campo para selecionar justificativa;  
- Campo para inserir um comentário.

4. Após preencher os campos necessário, clique em Salvar.

!!! warning "ATENÇÃO"

        - Se o campo justificativa não for preenchido é apresentado um pop-up com o texto: Por favor, você deve selecionar uma justificativa para a suspensão do ticket. ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se o campo comentário não for preenchido é apresentado um pop-up com o texto: Por favor, você deve informar um complemento para a suspensão do ticket. ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se estiver tudo correto e apresentado uma mensagem no final da tela com o texto: Suspensão realizada. Id: 0000000. Botão Ok que volta para a tela do ticket.
        
### Concluir ticket  

1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Concluir Ticket".  
3. Ao selecionar a opção de suspender ticket é aberta uma nova tela com os campos:

- Campo para selecionar a causa;  
- Campo para selecionar a solução. A lista só é carregada após a seleção do campo causa;
- Campo opcional para inserir um comentário.

4. Após preencher os campos necessário, clique em Salvar.

!!! warning "ATENÇÃO"

        - Se o campo causa não for selecionado é apresentado um pop-up com o título: Atenção. Mensagem: Por favor, selecione a Causa e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se o campo solução não for selecionado é apresentado um pop-up com o título: Atenção. Mensagem: Por favor, selecione a solução e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se estiver tudo correto e a ação for concluída, voltamos para a tela de ticket com a situação do ticket como concluída.
        
### Cancelar ticket        

1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Cancelar Ticket".  
3. Ao selecionar a opção de cancelar ticket é aberta uma nova tela com os campos:

- Campo para selecionar causa;
- Campo para selecionar a solução. A lista só é carregada após a seleção do campo causa;
- Campo opcional para inserir um comentário.

4. Após preencher os campos necessário, clique em Salvar.

!!! warning "ATENÇÃO"

        - Se o campo causa não for selecionado é apresentado um pop-up com o título: Atenção. Mensagem: Por favor, selecione a Causa e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.
        - Se o campo solução não for selecionado é apresentado um pop-up com o título: Atenção. Mensagem: Por favor, selecione a solução e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.
        - Se estiver tudo correto e a ação for concluída, voltamos para a tela de ticket com a situação do ticket como cancelada.
        
### Realizar check-in        

O check-in é o meio utilizado para identificar o caminho percorrido para o atendimento de um ticket aberto de Requisição/Incidente. Para utilizá-lo é necessário que o usuário tenha habilitado a opção disponível para atendimento.

!!! note "NOTA"

       O check-in não é obrigatório para o atendimento do ticket pelo agente 

Ao selecionar a opção realizar check-in é apresentado um Pop-up com a mensagem: "Tem certeza que deseja realizar check-in neste ticket?". Caso queira continuar com o check-in, clique em "Salvar". Caso queira cancelar o check-in, clique em "Cancelar".

### Realizar checkout

O check-out é o meio utilizado para identificar o encerramento do caminho percorrido para o atendimento de um ticket aberto de Requisição/Incidente. Para utilizá-lo é necessário que o agente possua permissão de execução no ticket.

!!! note "NOTA"

        O checkout (desbloqueio) não é obrigatório para o encerramento do atendimento do ticket pelo agente
        
!!! note "NOTA"

        Caso seja necessário, um atendente com acesso à aplicação web poderá realizar o checkout (desbloqueio) do atendimento
        
 Ao selecionar a opção realizar checkout é apresentado um Pop-up com a mensagem: "Tem certeza que deseja realizar checkout neste ticket?". Caso queira continuar com o checkout, clique em "Salvar". Caso queira cancelar o checkout, clique em "Cancelar".
 
### Atribuit ticket

1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Atribuir Ticket".  
3. Ao selecionar a opção de cancelar ticket é aberta uma nova tela com os campos:

- Campo para selecionar a usuário;  
- Campo para selecionar o grupo;  
- Campo para inserir uma justificativa.

4. Após preencher os campos necessário, clique em Salvar.

!!! warning "ATENÇÃO"

        - Se o campo solução não for selecionado, é apresentado um pop-up com o Texto: Por favor, selecione o grupo para a atribuição do ticket e o botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se o campo justificativa não for preenchido é apresentado um pop-up com o Texto: Por favor, informe uma justificativa para a atribuição do ticket e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela
        - Se estiver tudo correto e apresentado uma mensagem no final da tela com o texto: Atribuição realizada com sucesso. Botão Ok que volta para a tela do ticket.
        
### Reclassificar ticket

1. Quandro clicar em um ticket da lista, irá apresentar a tela com os detalhes dessa requisição. No topo da tela, existe um botão com 3 pontinhos onde serão apresentados as opções do ticket.  
2. Selecione "Reclassificar Ticket".  
3. Ao selecionar a opção de reclassificar ticket é aberta uma nova tela com os campos:

- Campo para selecionar portfólio;  
- Campo para selecionar serviço. A lista só é carregada após a seleção do campo portfólio;  
- Campo para selecionar atividade. A lista só é carregada após a seleção do campo serviço;  
- Campo para selecionar contrato. A lista só é carregada após a seleção do campo atividade;  
- Campo para inserir justificativa.

!!! note "NOTA"

        - Se um dos campos não estiver preenchido, é apresentado um pop-up com o Texto: Atenção! A Atividade e o Contrato devem ser selecionados e o botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se o campo justificativa não for preenchido é apresentado um pop-up com o Texto: Por favor, você deve informar uma justificativa para a Reclassificação do ticket e botão ok. Não permitindo salvar a ação e permanecendo na mesma tela.  
        - Se estiver tudo correto, é apresentado o pop-up com o Texto: Deseja se manter como responsável pelo ticket? E os Botões Não e Sim. Se o botão Não for selecionado o aplicativo permanece na mesma tela.  
        - Se o botão Sim for selecionado, é apresentada uma mensagem no final da tela com o texto: Ticket reclassificado com sucesso. Botão Ok que volta para a tela do ticket.
        
!!! warning "ATENÇÃO"

        - O grupo do usuário deverá possuir a permissão de reclassificar no fluxo da atividade;  
        - O ticket a ser reclassificado deverá estar na situação Aberto ou Em Andamento.
        
### Reabrir ticket

Caso o ticket já esteja fechado, você terá a opção de reabri-lo através do botão de 3 pontinhos do ticket, onde aparecerá a opção "Reabrir ticket.

!!! note "NOTA"

    - O aplicativo não exibe a opção de reabertura em dois casos: quando o usuário não possui permissão no fluxo para reabrir o ticket e quando o prazo limite para reabertura do chamado estiver expirado.  
    - O ticket deverá estar fechado.  
    - Não é permitido reabrir um ticket com situação Cancelado.
    
Ao selecionar a opção de reabrir ticket é aberta uma nova tela com:  

- Campo para inserir motivo da reabertura;  
- Botão de "Reabrir".

!!! note "NOTA"

    - Se o campo não for preenchido é apresentado um Pop-up com o Texto: Você deve informar um motivo para a Reabertura do ticket e botão ok.  
    - Se estiver tudo correto e apresentado é apresentada uma mensagem no final da tela com o texto: Reabertura realizada. ID 0000. Botão Ok que volta para a tela do ticket.
    
### Avaliar atendimento    

Caso o ticket já esteja fechado, você pode avaliar o atendimento do serviço requisitado.

!!! note "NOTA"

    - O ticket deverá estar fechado;  
    - O ticket não poderá ter sido cancelado.
    
Existem dois tipos de avaliação de atendimento:  
1. Padrão – Configurando no serviço x contrato o campo E-mail de Finalização = Solicitação Atendida (ID2 do modelo de e-mail).  
   - A opção Padrão permite que se reabra o ticket pela pesquisa de satisfação, configurando o parâmetro: 295 - Reabrir Solicitação Pela Pesquisa de Satisfação (Valores possíveis: S ou N, Default: N);  
   - Configurar o parâmetro 139 - Prazo em dias para responder pesquisa de satisfação referente às solicitações de serviço (Ex.: 7) com a quantidade de dias para responder a pesquisa de satisfação após o encerramento do atendimento.  
   
2. Pelo cadastro de pesquisa – Cadastrando uma pesquisa do tipo Atividade/Satisfação e vinculando a pesquisa a uma atividade. O cadastro da pesquisa possui data de finalização, portanto, o parâmetro 139 é desconsiderado nesse caso.    

Ao selecionar a opção de avaliar atendimento é aberta uma nova tela com:  
-  4 carinhas que representam uma escala de muito insatisfeito até muito satisfeito. As carinhas são do tipo botões para serem selecionados e, ao clicar, cada uma apresenta um nome;  
- Campo para inserir comentário.  
    
Se estiver tudo correto, clique em "Enviar avaliação". A avaliação é enviada e volta para a tela do ticket.  

### Reativar ticket

Caso um ticket esteja suspenso, você pode reativa-lo para poder ralizar as ações normais de um ticket.  
Para isso, encontre o ticket e aperte no botão com 3 pontinhos e selecione a opção "Reativar ticket".  
Ao selecionar a opção reativar ticket é apresentado um Pop-up com o Título: R'eativar ticket #00000". Você tem a opção de confirmar ou cancelar a reativação.  
Uma vez reativado, você terá as ações disponíveis para tratamento da requisição em questão.


## Relacionado

[Filtros – todos os tickets](/pt-br/4biz-helium/additional-features/racer-4biz-app/all-tickets-filter.html)

[Filtros - meus tickets](/pt-br/4biz-helium/additional-features/racer-4biz-app/my-tickets-filters.html)

[Racer 4biz – tela inicial do aplicativo](/pt-br/4biz-helium/additional-features/racer-4biz-app/racer-homescreen.html)

[Criar Ticket no Aplicativo Racer 4biz](/pt-br/4biz-helium/additional-features/racer-4biz-app/create-ticket-racer.html)

[Configurar instância para uso do aplicativo Racer4Biz e Mobile GO](/pt-br/4biz-helium/additional-features/mobile-and-field-service/configuration/configure-field-service-application.html)
