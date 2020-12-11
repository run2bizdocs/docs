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








