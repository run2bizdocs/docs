title: Regras de negócio    
Description: As regras de negócio definem como o seu negócio funciona, e podem abranger diversos assuntos como suas políticas, interesses, objetivos, compromissos éticos e sociais, obrigações contratuais, decisões estratégicas, leis e regulamentações entre outros.   

# Regras de negócio  

As Regras de Negócio do Builder servem para realizar validações que reflitam as regras de negócio das aplicações. Podem ser usadas para validação de formulários e/ou associadas a operações de inclusão, alteração e exclusão de objetos de negócio.      

## Como acessar  

1.	1.	Acesse a funcionalidade através da navegação no menu principal Builder > Gerenciamento > Regra de Negócio.    

## Pré-requisitos

1.	Não se aplica.    

## Cadastrar uma nova regra de negócio

1.	Para criar uma nova regra de negócio, clique no botão "Cadastrar";

2.	As Regras de Negócio são construídas através de desenho de um fluxo ou script Rhino.

## Criar regras de negócio tipo Fluxo

1.	Na aba Dados básicos, preencha o **Nome** e a **Descrição** da regra de negócio, a **Aplicação** a qual ela está associada e escolha o **Tipo** Fluxo;

2.	Na aba Variáveis clique em "Adicionar". A seguinte tela será apresentada:

3.	Preencha os campos da seção Variável:
  •	Nome da variável
  •	Descrição
  •	Armazena no banco de dados: se a variável deve ser armazenada internamente, no modelo de dados do Builder.
  •	Variável de retorno: se a variável deve ser incluída no objeto JSON de saída retornado ao final da execução do fluxo da regra de negócio.
  •	Lista de valores: Se a variável contém uma lista de valores.
  •	Variável de entrada obrigatória na execução: essa opção deve ser selecionada caso a execução do fluxo da regra de negócio dependa da existência da variável antes do início da execução.
  •	Tipo da variável
  •	Valor inicial da variável, que pode ser uma constante ou um valor retornado pela execução de script.

4.	Clique no botão “Incluir” para incluir a variável;

5.	Na aba Ações clique em "Adicionar". A seguinte tela será apresentada:

6.	Preencha os campos da seção Ação:

  •	Identificador: como a ação será associada ao diagrama do fluxo.
  •	Nome:  nome pelo qual a ação será referenciada no diagrama do fluxo.
  •	Script Rhino a ser executado quando a ação for acionada.

7.	Clique no botão “Incluir” para incluir a ação;

8.	Para editar o diagrama clique na aba correspondente. A seguinte tela será apresentada:

9.	Os elementos que podem ser adicionados ao fluxo, se encontram na paleta no canto esquerdo da tela. Para incluir um elemento no fluxo, selecione-o e arraste-o para a página de desenho. Uma janela pop-up com as propriedades do elemento será exibido na tela. Preencha as informações de acordo com o elemento escolhido;

10.	Ao término da edição do diagrama, clique no botão “Salvar” na barra superior.

## Criar regras de negócio tipo Script

1.	Na aba Dados básicos, preencha o **Nome** e a **Descrição** da regra de negócio, a **Aplicação** a qual ela está associada e escolha o **Tipo** Script:

2.	Codifique o script Rhino que implementa a regra de negócio e, se necessário, adicione variáveis conforme explicado na seção Variáveis do tipo Fluxo. 

3.	Ao término da edição do script, clique no botão “Salvar” na barra superior.

!!! info "Atenção"

  As regras de negócio criadas são bloqueadas por padrão. Isso significa que a regra não poderá ser utilizada a menos que seja desbloqueada. Para desbloquear selecione a regra desejada e clique na opção Desbloquear. 

!!! tip "About"
    <b>Updated:</b>11/03/2020
