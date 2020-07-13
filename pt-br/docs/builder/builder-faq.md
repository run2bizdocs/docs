Title: FAQ (Builder)
Description: 4biz - FAQ

# FAQ (Builder)

!!! Question "Qual a diferença entre criar um formulário através do menu Formulário e através do menu Objeto de negócio?"

	A criação através do menu Formulário ocorre de forma 100% manual. Através do menu de Objeto de Negócio, é possível gerar o formulário a partir do modelo do banco de dados. O formulário gerado poderá então ser editado no menu Formulário.
    

!!! Question "Como eu crio relacionamentos "muitos para muitos" no objeto de negócio?"
	
	Para criar um relacionamento "muitos para muitos" entre dois objetos de negócio, é necessário criar um terceiro objeto de negócio terceiro que será responsável pelo relacionamento.
	Ex: Vamos criar um relacionamento "muitos para muitos" entre dois objetos A e B, através do objeto de negócio C.
	Tanto o objeto de negócio A quanto o objeto de negócio B terão relacionamentos "um para muitos" com o objeto C.
	No objeto de negócio C existirão dois relacionamentos "muitos para um", sendo um com o objeto de negócio A e outro com o objeto de negócio B.
	Assim, através do objeto de negócio C, consegue-se relacionar um registro do objeto de negócio A com vários registros do objeto de negócio B, e vice-versa.


!!! Question "É possível criar componentes customizados que possam ser utilizados em formulários Builder?"

	Sim, é possível criar seus próprios componentes para serem utilizados em formulários Builder. Para um tutorial completo, vide a documentação técnica.
	

!!! Question "Por onde devo começar a construção de uma aplicação utilizando o Builder?"
	
	Para injetar uma dependência própria, é necessário cadastrá-la antes. Somente dependências do tipo CSS e JavaScript podem ser injetadas em um formulário Builder.
	Cadastre a sua dependência através do menu Builder > Recursos > CSS ou Builder > Recursos > JavaScript.
	Com a dependência adicionada ao sistema, selecione a aba Código compartilhado ou a aba relativa ao tipo da página que deseja injetar a dependência, clique na aba lateral "Dependências" e preencha os campos solicitados.
	Para mais informações à respeito de dependências de formulário, vide a documentação técnica.
	Veja a seção Passos para implementar a Solução Builder.


!!! Question "Como defino as ações que devem estar disponíveis em cada tarefa do workflow?"

	As ações são cadastradas nas abas principais do cadastro do fluxo. Para associar uma ação a uma tarefa específica, ir para o desenho do workflow, abra as propriedades daquele elemento, selecione as ações desejadas e salve as alterações.
	

!!! Question "Como deleto um elemento do workflow?"

	Para deletar um elemento do workflow, selecionar o elemento que deseja deletar e pressionar Ctrl + Del.
	

!!! Question "O que faço quando ocorrer o erro "Processo de negócio não informado"?"

	Este erro ocorre porque o processo de negócio não está referenciado no controller do formulário que inicia o processo de negócio. Para corrigir este problema, acessar o formulário referente ao processo de negócio, e inserir o seguinte comando no controller da Página de processo: 
	$scope.businessProcessName = 'nome_do_processo_de_negocio';

	

!!! Question "Quando eu cadastro um subprocesso, as informações do processo principal são herdadas pelo subprocesso?"

	Não. Ao incluir um novo subprocesso, seja do tipo ESI ou do tipo BPE, em um workflow principal é necessário informar na aba "Atributos, o nome exato do subprocesso que deverá ser criado manualmente no cadastro do workflow.
	Todas as informações, como ações e estados do fluxo principal deverão ser replicados no cadastro do subprocesso.
	Resumindo em passos, recomenda-se seguir a seguinte ordem:
		1.	Cadastrar o fluxo principal;
		2.	Cadastrar o subprocesso;
		3.	Incluir o elemento de subprocesso, referenciando o subprocesso já criado.

	 
