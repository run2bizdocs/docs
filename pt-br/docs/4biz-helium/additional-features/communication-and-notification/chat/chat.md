Title: Chat
# Chat

A noção de "Chat" é usada para troca de mensagens escritas de forma instantânea.
Permite que o usuário tenha contato com o atendente do sistema, a fim de
esclarecer dúvidas, fazer solicitações, entre outros. Os parâmetros deste
aplicativo permitem ativar o chat, definir o contrato padrão para abertura de
chamados e ajustar o grupo padrão, além de outras ações.

O chat pode ser usado de três modos:

-   Manual: troca de mensagens entre diversos tipos de usuários (ex: solicitante
    e atendente) em uma instância 4biz;

-   Automático: utilizado para a troca de mensagens entre usuário e um
    assistente virtual – por meio de um Chatbot, usando a inteligência
    artificial Helper;

-   Ambos: utilizado para viabilizar o contato entre o solicitante e o
    atendente, possibilitando também que um usuário interaja com um chatbot.

!!! Abstract "NOTA"
    
    Para interação com um Chatbot é necessário ter adquirido este serviço. Em caso de dúvidas, entrar em contato com a             4biz.

## Antes de começar

Para que o chat esteja disponível é preciso configurar os parâmetros de ativação da funcionalidade.

•	Uso Manual: 299, 315, 316, 317, 447 e 423.

•	Integração com o Helper: 423

Ao habilitar o parâmetro 423 o chat será aberto integrado ao assistente virtual Helper.

## Procedimento

### Configurando o Smart Chat

Acesse o menu principal > Parametrização > Chat

Serão apresentados os seguintes parâmetros:

|Parâmetro|Descrição|
|---------|---------|
|Ativar modo convidado| Configurar se o Smart Chat será visualizado na tela de login. As opções serão Sim ou Não, default Não. Caso o usuário escolha "Sim", o sistema solicitará o login do usuário. O login deverá seguir o padrão: domínio\\login|
|Modo convidado - ID Usuário| É o número identificador do usuário que iniciará sessão como convidado. Informação contida na coluna idUsuario da tabela usuário|
|Modo convidado - Chave secreta| A chave secreta é a senha de acesso do usuário convidado|
|Mensagem de boas-vindas| Alterar ou manter a mensagem padrão de boas-vindas|
|Iniciar aberto| Quando ativo significa que o Smart Chat vai sempre estar no modo aguardando mensagem. O default será Não|
|Ação inicial| Quando informado iniciará uma ação vinda do assistente virtual na tela de Smart Chat|
|Salvar| Botão para salvar as configurações|

Após salvar, a tela do Smart Chat estará disponível na tela de login, assim como todos os serviços configurados para Smart Chat ou assistente virtual, seguindo as restrições, de grupo e perfil de acesso, impostas ao usuário convidado.


A seguir apresentamos alguns exemplos de como utilizar o Chat do 4biz em cenários diferentes:

### Acesso ao Smart Chat sem configuração de Helper - Criação de ticket

1. Acesse a tela de Smart Portal ou Centro de Experiência;
2. Clique no ícone "Falar" no canto inferior da tela para iniciar a conversa;
3. Informe no chat que você deseja criar um novo ticket e adicione as informações necessárias;
4. O sistema retornará o número do ticket criado;
5. O sistema redirecionará para a tela de conversação;
6. Digite uma nova mensagem na tela de conversação;
7. O atendimento poderá assumir os seguintes status:
   a. Aguardando atendente (o atendente pode ser o solicitante ou o Analista) - sinalizado por uma bola verde não preenchida
   b. Online - Ambos os interlocutores estão ativos para conversa - sinalizado por uma bola verde preenchida
8. Ambos estando online é possível manter a conversa;
9. Se um dos interlocutores não estiver online e o parâmetro 447 - estiver configurado, então o sistema envia mensagem informando.

### Acesso ao Smart Chat sem configuração de Helper - Criação de ticket por meio de Pesquisa de Atividades

1. Acesse a tela de Smart Portal ou Centro de Experiência;
2. Clique no ícone "Falar" no canto inferior da tela para iniciar a conversa;
3. Informe o nome de uma Atividade;
4. O sistema retornará as opções para criar novo atendimento ou retomar um atendimento;

### Acesso ao Smart Chat para pesquisa de Conhecimento

1. Acesse a tela de Smart Portal ou Centro de Experiência
2. Clique no ícone "Falar" no canto inferior da tela para iniciar a conversa;
3. Informe o título ou parte do título de um conhecimento;
4. O sistema retornará as opções de conhecimento encontradas e permitidas para visualização;
5. Clique sobre o título do conhecimento e o sistema abrirá a descrição do conhecimento para visualização;
6. O sistema apresentará o botão de visualizar e, quando clicado, abre o portal de conhecimento;
7. O sistema apresentará o botão de fechar e, quando clicado, reduz o conhecimento, retornando ao estado original.

### Acesso ao Assistente Virtual - Criação de Ticket

1. Clique no sinalizador no topo da tela chamado "Virtual Assistant" para falar com o Helper;
2. Digite sua pesquisa ou assunto;
3. O assistente virtual poderá identificar conhecimentos ou atividades a serem abertas;
4. Quando o assistente virtual der a mensagem de fallback, imediatamente será apresentada as opções "Falar com Atendente" ou "Retomar Atendimento";
5. Clique no ícone para iniciar a conversa;
6. O sistema retornará o número do ticket criado;
7. O atendimento poderá assumir os seguintes status:
   a. Aguardando atendente (o atendente pode ser o solicitante ou o Analista) - sinalizado por uma bola verde não preenchida
   b. Online - Ambos os interlocutores estão ativos para conversa - sinalizado por uma bola verde preenchida
8. Ambos estando online é possível manter a conversa;
9. Se um dos interlocutores não estiver online e o parâmetro 447 - estiver configurado, então o sistema envia mensagem informando.

### Acesso ao Assistente Virtual- Criação de ticket por meio de Pesquisa de Atividades

1. Acessa a tela de Smart Portal ou Centro de Experiência;
2. Clique no ícone "Falar" no canto inferior da tela para iniciar a conversa;
3. Informe o nome de uma Atividade;
4. O sistema retornará as opções para criar novo atendimento ou retomar um atendimento;

### Acesso ao Assistente virtual para pesquisa de Conhecimento

1. Acesse a tela de Smart Portal ou Centro de Experiência;
2. Clique no ícone "Falar" no canto inferior da tela para iniciar a conversa;
3. Informe o título ou parte do título de um conhecimento;
4. O sistema retornará as opções de conhecimento encontradas e permitidas para visualização;
5. Clique sobre o título do conhecimento e o sistema abrirá a descrição do conhecimento para visualização;
6. O sistema apresentará o botão de visualizar e, quando clicado, abre o portal de conhecimento;
7. O sistema apresentará o botão de fechar e, quando clicado, reduz o conhecimento, retornando ao estado original.

### Conversa do Smart Chat entre atendentes

1. Os analistas devem estar com a tela de ticket aberta;
2. Os analistas devem vincular os contatos para conversar pela Aba Atendentes;
3. O analista envolvido na interlocução também deve vincular o contato para receber a conversa;
4. O analista abre a aba Atendentes, seleciona um contato e inicia uma conversa;
5. Caso o outro interlocutor possua em seus contatos esse analista, então é possível manter a comunicação;
6. Caso o outro interlocutor não possua em seus contatos esse analista, não é possível manter contato;
7. O atendimento poderá assumir os seguintes status:
   a. Aguardando atendente (o atendente pode ser o solicitante ou o Analista) - sinalizado por uma bola verde não preenchida
   b. Online - Ambos os interlocutores estão ativos para conversa - sinalizado por uma bola verde preenchida
8. Ambos estando online e vinculados é possível manter a conversa;

### Conversa do Smart Chat entre solicitante e atendente

1. O analista deve estar com a tela de ticket aberta;
2. O solicitante ao enviar uma mensagem o sistema enviará ao atendente, independente se o analista estiver com o ticket em questão aberto ou não, o sistema exibe no ícone do SmartChat um ponto de exclamação;
3. Na aba atendimentos aparecerá uma bola azul informando que existem novas mensagens no chat;
4. Quando o atendente abre a tela com a lista de atendimento, essa tela possui os seguintes campos:
   a. Busca pelo número do ticket;
   b. Atendimentos na Fila - São atendimentos que não foi feito captura do chamado
   c. Atendimentos em Andamento -São atendimentos que já foram capturados e estão sendo atendidos

## Relacionado

[Configurar parametrização - chat](/pt-br/4biz-helium/platform-administration/parameters-list/configure-parametrization-chat.html)


!!! tip "About"

    <b>Product/Version:</b> 4biz ESP | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
