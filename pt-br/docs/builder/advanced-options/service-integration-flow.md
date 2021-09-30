Title: Fluxo de integração de serviços  
Description:Os fluxos de integração de serviços, como o próprio nome diz, envolvem workflows executados com base em serviços de sistema, como integrações e conversões, por exemplo.   


# Fluxo de integração de serviços 

Os fluxos de integração de serviços permitem integrar aplicações Builder a sistemas externos, sejam eles do ambiente 4Biz ou de terceiros. É uma ótima alternativa para integração com sistemas legados.  

## Como acessar    

1.	Acesse a funcionalidade através do menu Builder > Gerenciamento > Fluxo de Integração ou menu Tracker > Fluxo de Integração;    

## Pré-requisitos    

1. Não se aplica.   

## Cadastro de um novo fluxo de integração

Para cadastrar um novo fluxo de integração, clique no botão "Cadastrar.

## Dados do fluxo

1.	Na guia Dados de fluxo preencha Nome e Descrição do fluxo de integração e informe a Aplicação Builder a qual ele será associado. Marque a caixa de seleção Exibe como componente se o fluxo de integração deve ser disponibilizado com componente para os fluxos 4Biz Tracker.

## Variáveis

Nesta aba são configuradas as variáveis que serão utilizadas no fluxo de integração. Variáveis são objetos capazes de reter e representar um valor ou expressão durante o tempo de execução do fluxo.

1.	Para adicionar uma variável clique no botão "Adicionar". A seguinte tela será apresentada:

2.	Preencha os campos:
    •	Nome da variável
    •	Descrição
    •	Armazena no banco de dados: se a variável deve ser armazenada internamente, no modelo de dados do Builder.
    •	Variável de retorno: se a variável deve ser incluída no objeto JSON de saída retornado ao final da execução do fluxo.
    •	Lista de valores: Se a variável contém uma lista de valores.
    •	Variável de entrada obrigatória na execução: essa opção deve ser selecionada caso a execução do fluxo dependa da existência da variável antes do início da execução.
    •	Tipo da variável
    •	Valor inicial da variável, que pode ser uma constante ou um valor retornado pela execução de script.

3.	Clique no botão “Incluir” para incluir a variável.

!!! Abstract "Atenção"
    
    Para salvar as alterações definitivamente é necessário clicar no botão “Salvar” na barra superior.

## Ações

Ações são rotinas escritas em Rhino que implementam as regras e lógicas de negócio no fluxo de integração. 

1.	Para adicionar uma variável clique no botão "Adicionar". A seguinte tela será apresentada:

2.	Preencha os campos:
    •	Identificador: como a ação será associada ao diagrama do fluxo.
    •	Nome:  nome pelo qual a ação será referenciada no diagrama do fluxo.
    •	Script Rhino a ser executado quando a ação for acionada.

3.	Clique no botão “Incluir” para incluir a ação.

!!! Abstract "Atenção"

    Para salvar as alterações definitivamente é necessário clicar no botão “Salvar” na barra superior.

## Diagrama

O diagrama é a modelagem do processo de integração sendo implementado pelo fluxo de integração.

1.	Para editar o diagrama clique no clique na aba correspondente. A seguinte tela será apresentada:

2.	Os elementos que podem ser adicionados ao fluxo, se encontram na paleta no canto esquerdo da tela. Para incluir um elemento no fluxo, selecione-o e arraste-o para a página de desenho. Uma janela pop-up com as propriedades do elemento será exibido na tela. Preencha as informações de acordo com o elemento escolhido;

3.	Ao término da edição do diagrama, clique no botão “Salvar” na barra superior.



!!! tip "About"
    <b>Updated:</b>11/03/2021
