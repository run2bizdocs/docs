title: Passos para implementar a Solução Builder
Description: Passos para implementar a Solução Builder
#Passos para implementar a Solução Builder


![create builder app](images/builder-1.png)

Figura 1 - Criar aplicação Builder


![business](images/builder-2.png)

Figure 2 - Objeto de negócios


!!! Abstract "ATENÇÃO"

    Os passos podem ser encontrados na documentação 4biz (docs.run2biz.com).

## Desenhar App


Para um melhor desenvolvimento das aplicações Builder, é necessário o **desenho anterior das necessidades, requisitos que a aplicação atenderá**, além de incluir o modelo de entidades dos dados que percorrerão a aplicação.

Uma pesquisa das **interfaces desejadas** e, se o Builder for a opção de usar dados para serviços, o **desenho dos serviços** que serão automatizados.

## Configuração Builder


Depois de Desenhar a Aplicação reunindo as informações referentes às entidades de dados de sua Aplicação Builder, você irá:

1.  Criar sua BASE DE DADOS DE CONEXÃO e sua entrada APLICAÇÃO Builder;

2.  Verificar se você vai usar qualquer DOMÍNIO comum para sua instalação e criar um se necessário;

3.  Você também verificará as REGRAS DE NEGÓCIO para o registro, atualização ou exclusão de registros na entidade de dados... você os vinculará ao Objeto de Negócio;

4.  Se você tiver formulários que usarão vários idiomas, você criará as CHAVES DE INTERNACIONALIZAÇÃO, labels que serão usadas para todos os campos em seus formulários.

## Desenvolvimento Builder


A etapa de configuração nos preparará para desenvolver a aplicação:

1.  Criar os OBJETOS DE NEGÓCIO, contendo a estrutura de dados da entidade, nesta etapa você poderá criar as colunas, PK's e FK's (atribuir relações), vincular Regras de Negócio e Domínios, além de poder criar Formulários CRUD e outros recursos;

2.  Criar FORMULÁRIOS relacionados ao seu Negócio.

## Conexão Experience


Depois de ter criado seus Objetos de Negócio e Formulários, você poderá:

1.  VINCULAR O FORMULÁRIO A UM SERVIÇO como necessário, ou

2.  VINCULAR O FORMULÁRIO AO MENU EXPERIENCE OU A UM CENTRO DE EXPERIÊNCIA, isso fará com que você consiga manter tabelas e dados adicionais que não serão usados na abertura de um ticket.



!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021 
