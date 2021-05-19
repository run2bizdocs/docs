Title: Autenticação Oauth2 usando Keycloack
Description:

# Autenticação Oauth2 usando Keycloack


## Antes de começar

- [x] Possuir um servidor de autenticação com protocolo OAUTH2, exemplo Keycloack  
- [x] Conectar ao servidor de autenticação ao sistema  
- [x] Após leitura de um novo usuário, o sistema atribuirá as seguintes permissões contidas nos seguintes parâmetros: 

      - Parâmetro 45 - LDAP – ID Grupo Padrão  
      - Parâmetro 39 - LDAP - Id do perfil de acesso que será setado automaticamente caso o usuário não possua nenhum


## Procedimento

1. Acessar o menu principal Parametrização > Método de Autenticação > Oauth2;  
2. Será apresentado a tela de Mètodo de Autenticação Oauth2 com duas opções "Filtros" e "Método de Autenticação";
3. A partir da versão Helium 1.2.24 houve alterações na interface descritas abaixo;  
4. A opção "Filtros" é uma tela de pesquisa com 4 opções:

|Opção|Descrição|
|-----|---------|
|Tipo| Onde será escolhido o tipo de autenticação. Existem dois tipos: interno ou externo. Se a opção for externa o sistema poderá ter 3 tipos de autenticação: Interno, Oauth2 ou Ambos.  
1. Se a opção estiver como ambos o sistema irá apresentar a tela de login com a área para: "autenticação", a opção de "esqueceu sua senha" e "acesse a sua conta" que poderá ser através do Google, Facebook ou Run2biz Keycloack;  
2. Se a opção for ambos mas não tiver nenhum provedor externo cadastrado, o sistema não irá mostrar as opções de autenticação por Google, Facebook ou Run2biz Keycloack;  
3. Se a opção for Oauth2 e não tiver um provedor cadastrado ele não irá mostrar a tela com vários provedores, mostrando direto a tela de login da Run2biz"|
|Provider| Onde será escolhido se será do tipo Google, Facebook ou outros|
|Domínio| Informar o domínio da autenticação|
|Nome do cliente| Informar o nome do cliente da autenticação|


5. Após preencher as informações em "Filtros", caso exista algum cadastro com o campo informado, ele será apresentado na tabela exibida logo abaixo em "Método de Autenticação";  
6. Caso não haja nenhum método autenticação cadastrado ou você deseja criar um novo, clicar em "Novo";  
7. Ao clicar em "Novo" será apresentado a tela para cadastro de um novo método de autenticação com 2 abas para serem preenchidas: "Identificação" e "Mapeamento de Campos";  
8. Para a aba de "Identificação", preencher:

|Campo|Descrição|
|-----|---------|
|Tipo de Autenticação| Existem duas opções para selecionar "Oauth2 - Interna" e "Oauth2
    
    












## Relacionado
