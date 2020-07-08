Title: Integrações

# Integrações

As integrações com o assistente virtual Helper dizem respeito aos canais em que o administrador irá disponibilizar o assistente. Essa funcionalidade permitirá a inserção dos links das plataformas desejadas para haver a integração da assistente virtual com o sistema selecionado.

Veremos adiante que o chatbot pode ser integrado nativamente ao 4biz, além do Facebook ou sistema próprio do usuário através de API Rest.

**Procedimento**

1.  Após acessar a plataforma, acesse o menu “Integrações”;

2.  Serão apresentadas as seguintes opções de integração: Facebook Messenger, 4biz e API Rest;

3.  Selecione qual opção você deseja integrar.

## 4biz

O Helper já se integra nativamente ao 4biz, então é muito fácil adicioná-lo ao seu ambiente.

Para realizar a integração, é necessário que você configure os parâmetros necessários no seu próprio ambiente de produção. Para isso, acesse o sistema e no menu de processos, selecione Parametrização > Parâmetros 4biz.

Localize e preencha os seguintes parâmetros:

|Parâmetro| Valor|
|-|-|
| 402 Helper Assistant - External URL     | http://[nome-servidor].helperassistant.com                                     |
| 441 Helper Assistant - Conversation API | http://[nome-servidor][sigla-idioma].helperassistant.com/webhooks/rest/webhook |
| 442 Helper Assistant - Parameters API   | http://[nome-servidor][sigla-idioma].helperassistant.com/conversations/        |

!!! info "Importante"

    Os valores a serem preenchidos nos parâmetros acima dependerão do valor apresentado na ferramenta Helper. Para isso, acesse o seu assistente virtual e selecione “Integrações”. Para integrar com a plataforma, selecione “4biz” e serão apresentados os valores para copiar e colar no valor na própria plataforma 4biz. Esses parâmetros não podem ser alterados pelo cliente.


## Facebook Messenger

Também é possível de integrar o assistente virtual Helper ao chat do Facebook Messenger. Nesse caso as instruções são fornecidas pelo próprio Facebook e fornecemos as informações necessárias para realizar a integração:

-   Callback URL

-   Verify Token

-   Secret

-   Page Access Token


## API Rest

Nessa funcionalidade o cliente pode customizar o assistente virtual para outro canal. Por exemplo, se o cliente já possuir um site institucional e deseja incluir a assistente virtual para o seu chat. Para isso, basta selecionar a opção de comunicação API Rest.

O API Rest é o protocolo de comunicação do assistente virtual. Nela são apresentadas as seguintes informações para realizar a integração com sucesso:

-   Endpoint

-   Método

-   Media Type

E os formatos necessários para integração:

-   Formato de envio de mensagem ao bot:

!!! exemple "Exemplo"

    {"sender": "joao","message": "conte-me algumas coisas sobre você"}


-   Formato de retorno da mensagem do bot em texto:

!!! exemple "Exemplo"

    {"recipient_id": "joao", "text": "Eu posso ajudá-lo a trabalhar de maneira mais inteligente, em vez de mais"}


-   Formato de retorno da mensagem do bot em botão:

!!! exemple "Exemplo"

    {"recipient_id": "joao", "text": "Você poderia avaliar o meu atendimento?","buttons": [{"title": "Sim", "payload": "sim"},{"title": "Não","payload": "não"}]}



-   Formato de retorno da mensagem do bot em imagem:

!!! exemple "Exemplo"

    {"image": "https://anuvaassistantimages.s3.amazonaws.com/dev/fe711b50-d974-11e9-9622-94de80f33bee.png","recipient_id": "joao"}

    Ou

    {"attachment":"https://anuvaassistantimages.s3.amazonaws.com/dev/fe711b50-d974-11e9-9622-94de80f33bee.png","recipient_id": "joao"}
