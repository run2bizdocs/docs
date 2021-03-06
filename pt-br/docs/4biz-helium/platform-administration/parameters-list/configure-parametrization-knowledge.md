title: Configurar parametrização - conhecimento
Description: permitir a execução/uso deste processo, podendo ser possível, definir a pasta para armazenamento do conhecimento criado a partir de eventos, definir o diretório para armazenar a descrição da resposta da solicitação de serviço/incidente para ser gravada na base de conhecimento, dentre outras ações.
# Configurar parametrização - conhecimento

O sistema de gerenciamento de conhecimento de serviço inclui ferramentas para
coletar, armazenar, gerenciar, atualizar, analisar e apresentar todos os
conhecimentos, informações e dados que um provedor de serviço de TI precisa para
gerenciar o ciclo de vida completo dos serviços de TI.

A parametrização de "Conhecimento" deve ser realizada para permitir a
execução/uso deste processo, podendo ser possível, definir a pasta para
armazenamento do conhecimento criado a partir de eventos, definir o diretório
para armazenar a descrição da resposta da solicitação de serviço/incidente para
ser gravada na base de conhecimento, dentre outras ações.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Gerência de conhecimento;

2.  Definir os valores dos parâmetros (atributos);

3.  Clicar no botão "Gravar" para efetuar a operação;

4.  A lista abaixo apresenta os parâmetros do "Conhecimento" e a finalidade de
    cada um deles:

|#|Nome|Finalidade|Orientações complementares|
|-|-|-|-|
|78| Avisar, com antecedência, a quantidade de dias que restam para a expiração do conhecimento. (Default: 90 dias)|Definir com quantos dias de antecedência da data de expiração do conhecimento, o autor e aprovador serão notificados. Na criação de um conhecimento na tela “Base de Conhecimento”, deve ser informada a data de expiração, ou seja, a data em que o conhecimento irá expirar. Será notificado ao autor e aprovador do conhecimento, com antecedência de N dias (definido neste parâmetro) da data de expiração do conhecimento| Não se aplica|
|79|ID do modelo de e-mail para envio de notificação de criação de pasta|Informar o número de identificação (ID) do modelo de e-mail de notificação de criação de pasta. Ao criar uma pasta na tela de “Cadastro de Pasta”, será utilizado para o envio da notificação de criação da pasta o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à pasta. Esse ID do modelo de e-mail é definido na tela de “Modelo de E-mail”.|Caso não informe o número de identificação (ID) do modelo de e-mail, há possiblidade de não enviar o e-mail correto.|
|80|ID do modelo de e-mail para envio de notificação de atualização de pasta|Informar o número de identificação (ID) do modelo de e-mail de notificação de atualização de pasta. Ao alterar uma pasta na tela de “Cadastro de Pasta”, será utilizado para o envio da notificação de atualização da pasta o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à pasta. Esse ID do modelo de e-mail é definido na tela de “Modelo de E-mail”.|Caso não informe o número de identificação (ID) do modelo de e-mail, há possiblidade de não enviar o e-mail correto.|
|81|ID do modelo de e-mail para envio de notificação de exclusão de pasta |Informar o número de identificação (ID) do modelo de e-mail de notificação de exclusão de pasta. Ao excluir uma pasta na tela de “Cadastro de Pasta”, será utilizado para o envio da notificação de exclusão da pasta o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à pasta. Esse ID do modelo de e-mail é definido na tela de “Modelo de E-mail”.|Caso não informe o número de identificação (ID) do Modelo de E-mail, há possiblidade de não enviar o e-mail correto.|
|82|ID do modelo de e-mail para envio de notificação de criação de conhecimento (Ex: 11)| Informar o número de identificação (ID) do Modelo de E-mail de notificação de criação de conhecimento. Ao cadastrar um conhecimento na tela de “Base de Conhecimento”, será utilizado para o envio da notificação de criação do conhecimento o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à base de conhecimento. Esse ID do modelo de e-mail é cadastrado na tela de “Modelo de E-mail”|Caso não informe o número de identificação (ID) do modelo de e-mail, há possiblidade de não enviar o e-mail correto. |
|83|ID do modelo de e-mail para envio de notificação de atualização de conhecimento (Ex: 12 )|Informar o número de identificação (ID) do modelo de e-mail de notificação de atualização de conhecimento. Ao atualizar um conhecimento na tela de “Base de Conhecimento”, será utilizado para o envio da notificação de atualização do conhecimento o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à base de conhecimento. Esse ID do modelo de e-mail é definido na tela de “Modelo de E-mail”| Caso não informe o número de identificação r (ID) do modelo de e-mail, há possiblidade de não enviar o e-mail correto. |
|84|ID do modelo de e-mail para envio de notificação de exclusão de conhecimento (Ex: 13)|Informar o número de identificação (ID) do modelo de e-mail de notificação de exclusão de conhecimento. Ao excluir um conhecimento na tela de “Base de Conhecimento”, será utilizado para o envio da notificação de exclusão do conhecimento o modelo de e-mail definido neste parâmetro. Essa notificação será enviada para o grupo e/ou usuário associado à base de conhecimento. Esse ID do modelo de e-mail é definido na tela de “Modelo de E-mail”|Caso não informe o número de identificação (ID) do modelo de e-mail, há possiblidade de não enviar o e-mail correto.|
|182| Pasta para ser salvo a Descrição e a solução da solicitação de serviço na Base de Conhecimento. (Ex: Windows - Descrição_Resposta_Para_BaseConhecimento)| Definir o diretório para armazenar a descrição da resposta da solicitação de serviço/incidente para ser gravada na base de conhecimento. Na tela de Solicitação de Serviço/Incidente é apresentada o campo “Gravar Solução/Resposta na Base de Conhecimento”. Ao atender uma solicitação de serviço/incidente e caso queira gravar a descrição da Solução Resposta na base conhecimento, basta selecionar o campo e informar o título, feito isso, ao gravar e avançar o fluxo, a descrição da solução resposta da solicitação será armazenada na pasta definida no parâmetro. |Não se aplica|
|273|Pasta padrão para os conhecimentos criados a partir de ocorrências de eventos|Definir a pasta para armazenamento do conhecimento criado a partir das ocorrências de eventos|Não se aplica|
|304|URL do servidor do SOLR (Ex: http://localhost:8983/solr/collection_name)|Configurar a URL da coleção do Apache Solr que será usada pelo 4biz para indexar os conhecimentos|Não se aplica|
|305|URL do servidor do Apache Tika (Ex: http://localhost:9998/tika)|Configurar a URL do Apache Tika para fazer OCR dos anexos do conhecimento no momento da indexação|Não se aplica|
|308|Total de itens a serem importados por vez ao indexar documentos no Solr (Ex: 1000)|Configurar a quantidade de itens que serão indexados por vez no Apache Solr|Não se aplica|
|313|Id da Pasta para cadastrar Conhecimentos criados pelo usuário final|Pasta default para cadastrar Conhecimentos criados pelo usuário final|Não se aplica|
|314|d da origem dos Conhecimentos criados pelo usuário final|Origem default que será usado nos conhecimentos criados pelo usuário final| Não se aplica|
|332|Ativar sincronização com o servidor de indexação|Quando é realizado uma indexação de conhecimento no Solr, seja por exclusão, atualização ou criação de um novo conhecimento. Se o Solr estiver parado e este parâmetro estiver ativo, é iniciado uma sincronização automática com o Solr até que este seja ativo novamente. Assim que ele voltar a funcionar todos os conhecimentos que estão pendentes de indexação são indexados e a sincronização automática é finalizada.|Não se aplica|
|333|Informe o intervalo em minutos para sincronizar os conhecimentos com o servidor de indexação|Se a sincronização automática estiver ativa (parâmetro 332). Este parâmetro determina de quanto em quanto tempo a sincronização automática de conhecimentos será executada.|Não se aplica|
|354|URL da logo (Portal do conhecimento) (Ex:./4biz/imagens/logo/logo-header-icon.png)|Parâmetro de uso restrito à 4biz Corporation, indica a URL da logo do Portal do conhecimento.|Não se aplica|
|355|URL do fundo do cabeçalho (Portal do conhecimento)(Ex.:/4biz/imagens/background-header.png)|Ex.:/4biz/imagens/background-header.png   |Parâmetro que personaliza a aparência do Portal do Conhecimento.|Não se aplica|
|356|Cor de fundo do cabeçalho (Portal do Conhecimento)(Default::#e6e6e6)||Parâmetro que personaliza a aparência do Portal do Conhecimento.|Não se aplica|
|357| Cor de fonte do cabeçalho (Portal do conhecimento) (Default : #333333)| Parâmetro que personaliza a aparência do Portal do Conhecimento.|Não se aplica|
|358|Habilitar ranking de pesquisas da base de conhecimento (Ex: S ou N - Default 'N')|A não configuração desta informação, ou a atribuição de "N" impede a criação de relatórios gerenciais que tratam do assunto.|Não se aplica|
|359|Armazenar registros de pesquisas por quantos dias? (Ex: 30)|A não configuração deste limitador pode acumular quantidade excessiva de dados desnecessariamente ao longo do tempo causando lentidões no processamento da aplicação, principalmente em relatórios que tratarem do assunto.| Não se aplica|
|360|Cor da fonte dos favoritos (Portal do Conhecimento) (Default : #f1a21f)|Personalizar a aparência do quadro "Favoritos" que fica na tela inicial tanto do Portal do Conhecimento quanto do Guia do Usuário.|Não se aplica|
|361|Cor da fonte dos curtidos (Portal do Conhecimento) (Default : #6c8ebe)|Personalizar a aparência do quadro "Curtidos" que fica na tela inicial tanto do Portal do Conhecimento quanto do Guia do Usuário.|Não se aplica|
|362|Cor da fonte dos indicados (Portal do Conhecimento) (Default : #67c15e)|Personalizar a aparência do quadro "Indicados" que fica na tela inicial do Portal do Conhecimento.|Não se aplica|
|363|URL do Help (Ex: https://help.cloud4biz.com/4biz)|O parâmetro é usado para informar a URL do Guia do Usuário|Não se aplica|
|364|URL da logo (Guia do usuário) (Ex.: /4biz/imagens/logo/logo-header-icon.png)|Parâmetro de uso restrito à 4biz Corporation, indica a URL da logo do Guia do Usuário.|Não se aplica|
|365|URL do fundo do cabeçalho (Guia do usuário) (Ex.: /4biz/imagens/background-header.png)|Parâmetro de uso restrito à 4biz Corporation, indica a URL da imagem de fundo do Guia do Usuário.|Não se aplica|
|366|Cor do fundo do cabeçalho (Guia do usuário) (Default : #e6e6e6)|Parâmetro de uso restrito à 4biz Corporation, personaliza a aparência do Guia do Usuário.|Não se aplica|
|367|Cor da fonte do cabeçalho (Guia do usuário) (Default : #333333)|Parâmetro de uso restrito à 4biz Corporation, personaliza a aparência do Guia do Usuário.|Não se aplica|
|368|URL para login do parceiro (Ex.: https://example.com/4biz)|Parâmetro de uso restrito à 4biz Corporation, personaliza o link para onde é direcionada a solução quando clicar em "Sou Agente" no Guia do Usuário.|Não se aplica|
|410|Exibir título da tela de Portal do Conhecimento (Default: S)|Informa se é para apresentar o título do conhecimento na tela de Pesquisa de Base de Conhecimento|Não se aplica|

Tabela 1 - Lista de parâmetros

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
