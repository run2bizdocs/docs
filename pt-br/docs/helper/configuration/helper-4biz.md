Title: Disponibilizar Helper na interface 4biz
# Disponibilizar Helper na interface 4biz

A Helper já se integra nativamente ao 4biz, então é muito fácil adicioná-la ao seu ambiente.

## Procedimento

1. Com acesso de Administrador, acesse a tela de parâmetros do 4biz
2. Altere o valor do parâmetro “402 Helper Assistant - External URL” para http://[nome-servidor].helperassistant.com
3. Altere o valor do parâmetro “441 Helper Assistant - Conversation API” para http://[nome-servidor][sigla-idioma].helperassistant.com/webhooks/rest/webhook e clique em “Salvar”
4. Altere o valor do parâmetro “442 Helper Assistant - Parameters API” para http://[nome-servidor][sigla-idioma].helperassistant.com/conversations/
5. Configurar o parâmetro 453 "Mensagem default de Fallback do Helper Assistant", com uma mensagem que o Helper irá responder sempre que não possuir resposta para aquela pergunta
6. Habilitar parâmetro 423 "Habilitar Helper Assistant na área interna do sistema", parâmetro que permite que os analistas tenham iteração com o Helper
7. Habilitar parâmetro 450 "Habilitar Helper Assistant na área externa", parâmetro que permite que os usuários finais tenham iteração com o Helper.    


!!! note "NOTA"

    Para a sigla dos idiomas, use EN (Inglês) e PT (Português-Brasil).
    Se os parâmetros mencionados não estiverem disponíveis, atualizar a versão do 4biz.


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
