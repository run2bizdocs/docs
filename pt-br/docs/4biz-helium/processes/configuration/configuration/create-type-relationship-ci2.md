Title: Cadastrar tipo de relacionamento de IC

Cadastrar tipo de relacionamento de IC
======================================

O cadastro de tipo relacionamento de IC é necessário para a gestão de Itens de Configuração (ativos e serviços) no CMDB. Com este cadastro será possível, a partir de um IC, definir níveis de relacionamento entre ICs.

O que fazer antes
-----------------

O usuário deverá possuir acesso à tela de Cadastro de Tipo de Relacionamento.

Procedimento
------------

-   Acessar a funcionalidade pelo menu Processos \> Gerência de Configuração \>
    Item de configuração;

-   O sistema apresentará a tela com os Tipo de relacionamento cadastrados com
    filtro de Nome e Status;

-   O usuário podera selecionar a opção "Novo" para inserir um novo tipo de relacionamento ou para cada registro rio poderá selecionar as opções:

    1. Editar - alterar um tipo de relacionamento;

    2. Excluir - excluir um tipo de relacionamento;

Campos 
-------

| Campo        | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|--------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nome (*)    | Descrição do tipo de relacionamento                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Status (*)  | Indica disponibilidade para uso <br>   - Ativo <br>   - Inativo                                                                                                                                                                                                                                                                                                                                                                                                        |
| Posição (*) | Define no desenho de mapa em qual posição ficará a cardinalidade do item de configuração: <br>- "Mesmo nível" - do ponto selecionado para o desenho do mapa de IC, significa que o IC ficará no mesmo nível(se “Ligado” não será pedido os níveis); <br>- "Nível Superior" – Descrição do ponto selecionado para o desenho do mapa de IC, que ficará acima; <br>- "Nível Inferior" - Descrição do ponto selecionado para o desenho do mapa de IC, que ficará abaixo; |

(*) Indica Obrigatoriedade

Ações
-----

| Ação   | Descrição                                            |
|--------|------------------------------------------------------|
| Gravar | Insere / Altera o tipo de relacionamento.            |
| Limpar | Retorna os campos de cadastro ao seu estado default. |


!!! warning "ATENÇÃO" 
    Caso um Tipo de relacionamento esteja sendo utilizado em um desenho de Mapa, então, o sistema não permitirá a edição da posição Mesmo Nível.

!!! note "GRAVAÇÃO" 
    Sempre será gravado o usuário que realizou a gravação, a data e a hora da criação.

Relacionado
-----------

[Relacionar Item de Configuração a um serviço](/pt-br/4biz-helium/processes/configuration/use/create-ic-relationship.html)

