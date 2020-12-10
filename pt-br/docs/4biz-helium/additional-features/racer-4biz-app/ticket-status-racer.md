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




