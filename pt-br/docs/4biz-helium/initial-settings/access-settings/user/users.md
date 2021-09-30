title: Cadastrar usuário
Description: Disponibiliza ações diversas, tais como, incluir, alterar e excluir um usuário.

# Cadastro de usuário

Alguns colaboradores podem precisar acessar o sistema e nesse caso é necessário criar uma conta de usuário. Esta conta permitirá o acesso do colaborador através de um login, uma senha e um perfil de acesso que consolida os seus direitos e permissões no sistema.

Note que o colaborador precisa estar cadastrado anteriormente, o que torna este procedimento simplificado.

A manutenção do cadastro do usuário envolve a inclusão, alteração e exclusão. Em particular, o administrador do sistema pode alterar o login e a senha de um colaborador.


## Antes de começar

Para cadastrar um usuário é necessário:

- [X] Registrar previamente o colaborador;

- [X] Relacionar um Perfil de Acesso;

Na criação ou alteração dos dados de um usuário, o sistema verifica se envio de e-mail com os dados de acesso está configurado. Os seguintes parâmetros precisam estar configurados para ativar essa funcionalidade:

- [X] Configurar o parâmetro 33 e indicar corretamente a URL de acesso a plataforma 4biz;

- [X] Configurar o parâmetro 455 com o ID do modelo de e-mail criado para enviar os dados de acesso. O modelo escolhido precisa conter as chaves ${LOGIN} e ${NOVASENHA}.

!!! note "EXEMPLO"

    Modelo de e-mail: "Prezado usuário, seguem os dados de acesso. Usuário: ${LOGIN} e Senha: ${NOVASENHA}"

!!! warning "ATENÇÃO"

    Não é possível enviar o login e a senha ao cadastrar usuários importados do Microsoft Active Directory® ou LDAP.


## Procedimento

1.	Acessar a funcionalidade através do Menu de Navegação > Cadastros Gerais > Gerência de Pessoal > Usuário;

2.	Indicar o colaborador através da caixa de pesquisa apresentada ao clicar na caixa de texto “Colaborador”;

3.	Preencher login e senha, repetindo a senha na caixa de confirmação de senha;

4.	Selecionar o Perfil de Acesso para o usuário;

5.	Se necessário, adicionar Grupos de Usuário correspondentes;

6.	Clicar em "Gravar".


!!! info "INFORMAÇÃO"
   Para concluir uma operação de criação, alteração ou exclusão de um cadastro de usuário, o sistema verifica se há uma política de senha implementada e o se usuário foi importado de um diretório LDAP.
    Desta forma, a conclusão da operação pode ser impedida. Pois não é possível alterar a senha um usuário importado de um diretório LDAP. Assim como, a senha deve seguir a política de complexidade definida.


Active Directory é uma marca registrada da Microsoft Corporation.


## Relacionado

[Cadastrar um colaborador](/pt-br/4biz-helium/initial-settings/access-settings/user/register-employee.html)

[Criar perfil de acesso](/pt-br/4biz-helium/initial-settings/access-settings/profile/create-profile-access.html)

!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2021

