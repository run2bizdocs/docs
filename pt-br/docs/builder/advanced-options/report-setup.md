Title: Configuração de relatório    
Description:Em Configuração de relatório é onde são realizadas, se necessário, as configurações de execução dos relatórios cadastrados no sistema através da opção Arquivo de Relatório.  

# Configuração de relatório   

Em Configuração de relatório é onde são realizadas, se necessário, as configurações de execução dos relatórios cadastrados no sistema através da opção Arquivo de Relatório.     

## Como acessar 

Acesse a funcionalidade através do menu Builder > Gerenciamento > Relatório.

## Pré-requisitos

O relatório a ser configurado deve ter sido previamente cadastrado no menu Builder > Recursos > Upload de relatório.

## Configurando um relatório 

1. Escolher um item da lista de relatórios e clicar no botão “Editar”.  

## Dados do relatório

1.	Os valores de Aplicação, Nome, Descrição e Pasta são preenchidos com base no cadastro do arquivo de relatório e podem ser alterados nessa tela. 

## Data source

1.	**Data source** refere-se à fonte de dados para a execução do relatório. Informe o **Tipo** da fonte de dados, dentre as opções:
    •	**Nenhum**: caso o relatório não realize buscas no banco de dados.
    •	**Conexão de dados:** caso a fonte de informações esteja em banco de dados. Neste caso, informe também a respectiva Conexão de Banco (cadastrada no menu Builder > Configuração > Conexão de Banco de Dados).
    •	**Objeto de dados**: caso a fonte de informações seja um objeto de banco de dados cadastrado na aplicação Builder.
    •	**Fluxo ESI:** caso a fonte de informações seja um fluxo de integração cadastrado na aplicação Builder. Neste caso, informe também o nome do Fluxo (cadastrado no menu Builder > Gerenciamento > Fluxo de Integração).
    •	**Script:** caso a fonte de dados seja um script, codifique o script Rhino a ser utilizando.


## Parâmetros

1. Esta aba refere-se ao cadastro de parâmetros necessários à execução do relatório.
    •	Clique em "Adicionar" para incluir um novo parâmetro;
    •	Informe o **Nome** do parâmetro, o **Tipo** e os dados relativos ao tipo;
    •	Clique em "Salvar" para incluir o parâmetro na lista;
    •	Para editar um parâmetro da lista, clique em "Editar";
    •	Para remover um parâmetro da lista, clique em "Remover".
 
## Formulário

Esta aba representa o formulário a ser exibido quando o usuário for gerar o relatório.

1.	Informe o Título do Formulário e se deverão ser exibidas abas;

2.	Se desejado, faça alterações nos códigos HTML e Javascript do formulário.



!!! tip "About"
    <b>Updated:</b>11/03/2021
