# Configurar atributos de serviço

Todo serviço possui um conjunto de atributos que o caracterizam e o diferencia
dos outros. As características individuais são variadas e podem estar
relacionadas com a prestação do serviço, o seu relacionamento com os diferentes
processos de gerenciamento, a sua relação com outros serviços e com as partes
envolvidas na sua entrega ou operação.

No 4biz, os atributos de serviço são configurados a partir do Portfólio do
Serviço.

## Antes de começar

- [x]   É necessário ter configurado previamente o Funil de Serviços.

## Procedimento

Para acessar a tela de configuração dos atributos de um serviço, siga o
procedimento abaixo.

1.  Acessar o menu principal Processos \> Gerência de Portfólio e Catálogo \>
    Portfólio;

2.  Encontrar o Portfólio de Serviços que possui o serviço a ser detalhado e
    clicar no botão "Avançar";

3.  Encontrar o serviço na lista do Portfólio de Serviços e clicar no botão
    "Avançar';

4.  No lado esquerdo da tela estão apresentados os diferentes temas onde os
    atributos que podem ser configurados estão agrupados.

5.  Clicar no tema do atributo a ser definido para acessar a sua página de
    configuração.

>   A seguir, estão descritos os temas de atributos de serviço disponíveis no 4biz.

## Atributos do Serviço

**Detalhes**

Tema relacionado com os atributos básicos do serviço, como Nome, Status,
Criticidade, Categoria, entre outros.

As guias, os campos do formulário e as ações disponíveis neste tema estão
descritas no documento de [Cadastrar/Editar um
serviço](https://docs.run2biz.com/pt-br/4biz-helium/processes/portfolio-and-catalog/use/register-a-service.html).

### Requisitos de Nível de Serviço

Este tema agrupa os atributos relacionados com o processo de gerenciamento de
nível de serviço, como a utilidade e garantia do serviço. A utilidade do serviço
é o seu propósito pela qual foi criado e quais necessidades dos clientes
pretende atender. Já a garantia do serviço são as condições que determinam que o
serviço está adequado ao uso.

Evidentemente, os requisitos de nível de serviço estão relacionados com o
processo de gerenciamento de nível de serviço. Contudo, eles também podem estar
associados com outros processos, como o gerenciamento de incidentes, problemas e
mudanças.

*Aba de Requisitos de Nível de Serviço*

| Campo                     | Descrição                                            |
|---------------------------|------------------------------------------------------|
| Data de criação (\*)      | Data de criação do serviço.                          |
| Data de início do serviço | Data em que o serviço foi ou será liberado para uso. |
| Dono do serviço           | Indicação do dono do serviço.                        |

(\*) Campo obrigatório

-   UTILIDADE DO SERVIÇO

| Campo                             | Descrição                                                                                                                                        |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| Especificação (\*\*)              | Descreva qual o propósito do serviço, ou seja, porque o serviço existe e o que ele deve realizar para atender as necessidades dos seus clientes. |
| Contexto (\*\*)                   | Descreva o contexto de uso do serviço, ou seja, por quem, quando, onde e como o serviço será utilizado.                                          |
| Funcionalidades essenciais (\*\*) | Liste os recursos essenciais do serviço. São os itens que o serviço depende para funcionar e cuja falha provocaria a sua indisponibilidade.      |

(\*\*) Campos que aceitam anexar arquivos

-   GARANTIA DO SERVIÇO

| Campo                          | Descrição                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Segurança (\*\*)               | Descreva os requisitos de segurança da informação e quais são os mecanismos que o serviço deve possuir para garantir a segurança dos seus dados, como: Armazenamento seguro e descarte de dados, perfis de acesso e permissões, classificação de informação etc.                                                                                                      |
| Disponibilidade (\*\*)         | Descreva os requisitos de disponibilidade e quais são os mecanismos que o serviço deve possuir para garantir a sua disponibilidade de acesso, como: implantação e manutenção de redundâncias de equipamentos, tecnologias de alta-disponibilidade como clusters etc.                                                                                                  |
| Capacidade (\*\*)              | Descreva os requisitos de capacidade e quais são os mecanismos que o serviço deve possuir para garantir a entrega de capacidade adequada, como: Alocação dinâmica de processamento, monitoração do uso do serviço, métricas de mensuração da capacidade e da demanda etc.                                                                                             |
| Continuidade do Negócio (\*\*) | Descreva os requisitos de continuidade do serviço e quais são os mecanismos que o serviço deve possuir para garantir que o serviço pode operar dentro de níveis mínimos aceitáveis, mesmo em uma situação de crise, como: disponibilidade de datacenter redundante, planos de resposta a desastre, testes de recuperação de serviço etc.                              |
| Performance/Desempenho (\*\*)  | Descreva os requisitos de performance e quais são os mecanismos que o serviço deve possuir para garantir que o seu desempenho atenderá as expectativas dos clientes, como: tempos esperados e aceitáveis para conclusão de cada etapa do serviço etc.                                                                                                                 |
| Interrupções planejadas (\*\*) | Descreva os requisitos para interrupções planejadas do serviço e como o gerenciamento do serviço precisa garantir que as regras acordadas serão seguidas, como: Tempo máximo para uma interrupção planejada do serviço, a frequência na qual o serviço pode ser interrompido, mecanismos para solicitação, aprovação e gerenciamento das interrupções planejadas etc. |

(\*\*) Campos que aceitam anexar arquivos

-   SUPORTE DE SERVIÇO

| Campo                       | Descrição                                                                                                                                                                                                                                                                                 |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Gerenciamento de Incidentes | Descreva os requerimentos para o processo de gerenciamento de incidentes. Itens como: Classificação de incidentes, sua gravidade e prioridade, os tempos aceitáveis para identificação de um incidente, o seu registro, a sua investigação e a restauração da operação normal do serviço. |
| Gerenciamento de Problema   | Descreva os requerimentos para o processo de gerenciamento de problemas. Itens como: Tempos esperados para a identificação, registro e a investigação de um problema.                                                                                                                     |
| Gerenciamento de Mudança    | Descreva os requerimentos para o processo de gerenciamento de mudança. Itens como: Tipos de mudanças, procedimentos para registro, análise, aprovação e revisão de mudanças. Também janelas preferenciais para a execução de manutenções e períodos de congelamento de mudanças.          |

-   CONFORMIDADE

| Campo          | Descrição                                                                                                                                                                                                                                                                                                                             |
|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Interna (\*\*) | Descreva os requerimentos internos de governança e risco que devem ser observados e atendidos durante o ciclo de vida do serviço e sua operação. Usualmente estão relacionados com políticas gerenciais determinadas pelo conselho administrativo da organização para preservar os investimentos e a organização de má administração. |
| Externa (\*\*) | Descreva os requerimentos externos de governança e risco que devem ser observados e atendidos durante o ciclo de vida do serviço e sua operação. Normalmente envolve o atendimento a regulamentos, portarias, leis e marcos regulatórios aos quais a organização está submetida.                                                      |

(\*\*) Campos que aceitam anexar arquivos

*Aba de Documentos Anexos*

| Componente                  | Descrição                                            |
|-----------------------------|------------------------------------------------------|
| Selecionar assunto do anexo | Selecione o assunto o qual o anexo está relacionado. |
| Tabela de arquivos          | Lista de arquivos anexados                           |

As seguintes funções estão disponíveis:

| Funções            | Descrição                                                  |
|--------------------|------------------------------------------------------------|
| Adicionar arquivos | Insere o arquivo indicado como um anexo ao tópico indicado |
| Gravar             | Salvar o atributo                                          |
| Limpar             | Limpar os campos                                           |
| Excluir            | Exclui o arquivo                                           |

### Atributos Financeiros

São os atributos que descrevem o relacionamento do processo de gerenciamento
financeiro com o serviço.

Os atributos financeiros indicam o relacionamento do serviço com os Centros de
Resultados, Departamentos e com os valores financeiros de CAPEX, OPEX, Valor
Direto e outros.

Estas informações podem ser usadas para apresentar a situação financeira atual
de um serviço, bem como todo o histórico de variação do custo e preço.

O registro ou alterações nas informações financeiras são realizadas dentro do
processo de Gerência Financeira.

!!! note "Tip"

    O 4biz realiza a diferenciação entre o custo de serviço e o preço de serviço.

!!! note "Nota"

    O 4biz, através do modelo hierárquico de custo, relaciona os itens financeiros
    registrados e calcula os valores correspondentes a cada serviço. Isto permite
    identificar a distribuição do custo entre os diferentes serviços cadastrados.

Além disto, os valores serão vinculados automaticamente ao item de configuração
correspondente apresentando as seguintes informações:

| Campo         | Descrição                                               |
|---------------|---------------------------------------------------------|
| Categoria     | A categoria do registro financeiro.                     |
| Tipo          | Indicação do tipo do registro, isto é, custo ou receita |
| Classificação | A classificação do custo.                               |
| Valor         | O valor do serviço                                      |
| Ciclo         | O ciclo financeiro                                      |

### Casos de Negócios

Nesta seção estão registradas as informações estratégicas relacionadas com os
casos de negócio elaborados para o projeto e desenvolvimento do serviço.

*Guia de Casos de Negócios*

| Campo                        | Descrição                                                                            |
|------------------------------|--------------------------------------------------------------------------------------|
| Caso de Negócio (\*)         | Nome do caso de negócio                                                              |
| Sumário executivo (\*\*)     | Apresente o sumário executivo do caso de negócios                                    |
| Stakeholder/Entidade         | Indique as partes interessadas para o caso de negócios                               |
| Cenários (\*\*)              | Descreva os cenários de negócio considerados no desenvolvimento dos casos de negócio |
| Problema/Oportunidade (\*\*) | Descreva o problema a ser solucionado ou a oportunidade a ser aproveitada            |
| Proposta de solução (\*\*)   | Especifique as soluções propostas                                                    |
| Análise financeira (\*\*)    | Relate sobre a análise financeira realizada                                          |
| Análise de risco (\*\*)      | Descreva sobre os riscos considerados na análise do caso                             |
| Viabilidade técnica (\*\*)   | Indique as considerações técnicas sobre o caso                                       |
| Conclusão (\*\*)             | Especifique a conclusão alcançada pela análise do caso                               |

(\*) Campos obrigatórios

(\*\*) Campos que aceitam anexar arquivos

*Guia de Documentos Anexos*

| Componente                 | Descrição                                           |
|----------------------------|-----------------------------------------------------|
| Selecionar tópico do anexo | Selecione o assunto o qual o anexo está relacionado |
| Tabela de arquivos         | Lista de arquivos anexados                          |

As seguintes funções estão disponíveis:

| Funções            | Descrição                                                  |
|--------------------|------------------------------------------------------------|
| Adicionar arquivos | Insere o arquivo indicado como um anexo ao tópico indicado |
| Gravar             | Salvar o atributo                                          |
| Limpar             | Limpar os campos                                           |

### Itens de Configuração

Nesta seção de atributos é apresentado o mapa de relacionamento dos itens de
configuração que compõe o serviço.

Alterações relacionamento entre os itens de configuração são realizadas dentro
do processo de Gerência de Configuração & ITAM.

### Processos de Negócio

Serviços sempre estão ligados a processos de negócio, seja para operacionalizar,
suportar ou viabilizar a sua execução. É importante compreender esta relação
para avaliar adequadamente os riscos e impactos de indisponibilidades, bem como
as oportunidades de investimentos e negócios.

Nesta seção de atributos, registre e vincule os processos de negócio da
organização com os serviços prestados.

As seguintes funções estão disponíveis:

| Função                        | Descrição                                             |
|-------------------------------|-------------------------------------------------------|
| Vincular processo de negócio  | Associa um registro de processo de negócio ao serviço |
| Novo processo de negócio      | Registra um novo processo de negócio                  |
| Pesquise aqui                 | Pesquisa entre os processos vinculados                |
| Lista de processos de negócio | Permite visualizar detalhes e desvincular             |

### Serviços de Apoio

Serviços podem ser principais, intensificadores ou de apoio.

Serviços principais são aqueles que criados e suportados para entregarem os
resultados esperados. São percebidos diretamente pelos seus clientes através da
interação e obtenção de valor.

Serviços intensificadores, não são essenciais para a entrega de valor ao
cliente, contudo estimulam os clientes a utilizar mais os serviços contratados e
diferencia o provedor de serviços de seus concorrentes.

Serviços de apoio que fornecem suporte para o serviço principal. Não são
utilizados diretamente pelos clientes e usuários, contudo são críticos para a
entrega de valor. Exemplos mais comuns são o backup de dados e a monitoração de
equipamentos.

As seguintes funções estão disponíveis:

| Função           | Descrição                             |
|------------------|---------------------------------------|
| Vincular serviço | Vincule um serviço de apoio.          |
| Pesquise aqui    | Pesquisa entre os serviços vinculados |

### Dono do Negócio

O dono do negócio é a pessoa ou grupo que é responsável pela definição da visão
e do roadmap de negócio que deve ser suportado pelo serviço.

Esta informação é importante para agilizar a negociação de mudanças, escalação
de incidentes, reporte dos níveis de serviço e outras ações de gerenciamento que
envolvem as áreas de negócio.

As seguintes funções estão disponíveis:

| Função            | Descrição                                        |
|-------------------|--------------------------------------------------|
| Vincular usuários | Vincule um indivíduo como dono do negócio        |
| Vincular grupos   | Vincule um grupo como dono do negócio            |
| Pesquise aqui     | Pesquisa entre os indivíduos e grupos vinculados |
| Desvincular       | Desvincule o dono do negócio listado.            |

### Usuário do Negócio

Usuários do negócio são as pessoas que utilizam do serviço durante do seu
trabalho.

Esta informação é relevante para ações, como: a comunicação sobre o
funcionamento do serviço, identificação de oportunidades de melhoria,
compreensão da demanda e outras ações de gerenciamento que envolvem o uso do
serviço.

As seguintes funções estão disponíveis:

| Função            | Descrição                                      |
|-------------------|------------------------------------------------|
| Vincular usuários | Vincule um indivíduo como usuário              |
| Vincular grupos   | Vincule um grupo como usuário                  |
| Pesquise aqui     | Pesquisa entre os usuários e grupos vinculados |
| Desvincular       | Desvincule o usuário ou grupo listado          |

### Requisições

Nesta seção de atributos são vinculadas todas as atividades de requisição que
compõe o serviço. Estas atividades são os principais ponto de contato dos
usuários com o serviço, já que seus pedidos são formalizados através dos seus
registros.

A disponibilidade para registro de uma requisição depende do seu vínculo com o
serviço e da permissão definida.

As seguintes funções estão disponíveis:

| Função                           | Descrição                                                        |
|----------------------------------|------------------------------------------------------------------|
| Nova atividade de requisição     | Registra uma atividade de requisição                             |
| Vincular atividade de requisição | Permite pesquisar e vincular uma atividade registrada ao serviço |
| Pesquise aqui                    | Pesquisa entre as requisições vinculadas                         |
| Desvincular                      | Desvincule a atividade listada                                   |

### Aplicações

Serviços são suportados ou operacionalizados pelo uso de aplicativos ou sistemas
de informação. Nesta seção, são associadas e apresentadas todas as aplicações
relacionadas ao serviço.

As seguintes funções estão disponíveis:

| Função             | Descrição                                             |
|--------------------|-------------------------------------------------------|
| Vincular aplicação | Permite pesquisar e vincular uma aplicação ao serviço |
| Nova aplicação     | Cria um registro para uma aplicação                   |
| Pesquise aqui      | Pesquisa entre as aplicações vinculadas               |
| Desvincular        | Desvincule a aplicação listada                        |

### Pacote de desenho do serviço

Nesta seção está registrada toda documentação técnica do serviço, como os
requisitos de software, modelos de contrato, acordos de nível de serviço,
acordos de nível operacional, planos de transição do serviço, esquema de dados,
topologia de rede de dados etc.

É requerido anotar os detalhes técnicos do serviço e arquivos podem ser
anexados. Como o conteúdo do pacote de desenho do serviço pode variar muito
entre diferentes organizações, cada arquivo anexado pode receber uma descrição
própria.

| Campo         | Descrição                                           |
|---------------|-----------------------------------------------------|
| Detalhes (\*) | Anotação dos detalhes pacote de desenho do serviço. |

(\*) Campo obrigatório

*Documentos Anexos*

As seguintes funções estão disponíveis para anexar documentos:

| Funcionalidade           | Descrição                                |
|--------------------------|------------------------------------------|
| Descrição do anexo       | Indicação do assunto do arquivo anexado. |
| Adicionar arquivo        | Selecione o arquivo a ser anexado.       |
| Lista de arquivos anexos | Abrir e excluir arquivos anexados.       |

### Incidentes

Nesta seção de atributos são vinculadas todas as atividades de incidentes que
compõe o serviço. O registro destas atividades permite o rápido direcionamento
do atendimento do incidente, bem como, sua avaliação, diagnóstico e resolução.

As seguintes funções estão disponíveis:

| Função                          | Descrição                                                        |
|---------------------------------|------------------------------------------------------------------|
| Nova atividade de incidente     | Registra uma atividade de incidente.                             |
| Vincular atividade de incidente | Permite pesquisar e vincular uma atividade registrada ao serviço |
| Pesquise aqui                   | Pesquisa entre os incidentes vinculados                          |
| Desvincular                     | Desvincule atividade listada                                     |
|                                 |                                                                  |

### Procedimentos de continuidade

Os procedimentos de continuidade são usados para responder a uma situação
excepcional que impacta severamente o serviço, como uma crise ou desastre.
Nestes casos, um plano de ação para dar a continuidade a entrega do serviço deve
ser acionado e seguido para uma rápida resposta. Este plano é composto de um
conjunto de procedimentos.

Nesta seção de atributos, são relacionados todos os procedimentos necessários
para o restabelecimento da operação normal do serviço.

As seguintes funções estão disponíveis:

| Função                | Descrição                                               |
|-----------------------|---------------------------------------------------------|
| Novo procedimento     | Registrar novo procedimento                             |
| Vincular procedimento | Permite pesquisar e vincular um procedimento ao serviço |
| Pesquise aqui         | Pesquisa entre os procedimentos vinculados              |
| Desvincular           | Desvincule o procedimento listado                       |

### Contratos

O relacionamento entre serviços e contratos é uma das configurações mais
importantes do 4biz. A flexibilidade para organizar esta relação permite
gerenciar múltiplos contratos e ofertar diferentes níveis de qualidade para o
mesmo serviço, como por exemplo, nível Ouro, Prata e Bronze.

As seguintes funções estão disponíveis:

| Função            | Descrição                                           |
|-------------------|-----------------------------------------------------|
| Novo contrato     | Registrar novo contrato                             |
| Vincular contrato | Permite pesquisar e vincular um contrato ao serviço |
| Pesquise aqui     | Pesquisa entre os contratos vinculados              |
| Desvincular       | Desvincule o contrato listado                       |

### Dono do serviço

Dono do serviço presenta o serviço perante a organização. Possui grande
conhecimento sobre o serviço e participa de decisões estratégicas. O dono também
atua como ponto de contato dentro do processo de escalação para incidente e
requisições.

Nesta seção de atributos, estão relacionados os usuários e grupos que são
indicados como donos do serviço.

As seguintes funções estão disponíveis:

| Função            | Descrição                                      |
|-------------------|------------------------------------------------|
| Vincular usuários | Vincule um indivíduo como dono do serviço      |
| Vincular grupos   | Vincule um grupo como dono do serviço          |
| Pesquise aqui     | Pesquisa entre os usuários e grupos vinculados |
| Desvincular       | Desvincule o usuário ou grupo listado          |

### Base de Conhecimento

Conhecimento é uma ferramenta fundamental para o design, desenvolvimento,
entrega e uso de um serviço. Quanto mais as pessoas forem conhecedoras sobre o
serviço, maiores são as chances de obter valor a partir de seu uso.

Nesta seção estão indicados todos os registros de conhecimento relacionados ao
serviço.

As seguintes funções estão disponíveis:

| Função                | Descrição                                                           |
|-----------------------|---------------------------------------------------------------------|
| Vincular conhecimento | Permite pesquisar e vincular um registro de conhecimento ao serviço |
| Pesquise aqui         | Pesquisa entre os registros de conhecimento vinculados              |
| Desvincular           | Desvincule um registro de conhecimento listado                      |

### Habilidade/Recurso

Para colocar o conhecimento em prática, as pessoas envolvidas no serviço
precisam de habilidades e recursos para executar as ações. Indicar quais são os
requisitos para uso do serviço, facilita o processo de contratação de pessoas,
organização de times e o treinamento e capacitação.

Nesta seção, estão listadas as habilidades e recursos necessários para usar e
manter o serviço.

As seguintes funções estão disponíveis:

| Função              | Descrição                                              |
|---------------------|--------------------------------------------------------|
| Vincular habilidade | Permite pesquisar e vincular uma habilidade ao serviço |
| Nova habilidade     | Registre uma nova habilidade                           |
| Pesquise aqui       | Pesquisa entre as habilidades vinculadas               |
| Desvincular         | Desvincule um registro de habilidade listado           |

### Capacidade Planejada

Ao projetar um serviço, o responsável deve planejar como irá atender as
necessidades atuais e futuras de capacidade. Essa visão de longo prazo para o
serviço permitirá realizar os investimentos adequados e em tempo para assegurar
a disponibilidade de capacidade.

Nesta seção de atributos, estão relacionados os indicadores de capacidade ou
performance do serviço.

As seguintes funções estão disponíveis:

| Função                                         | Descrição                                                                         |
|------------------------------------------------|-----------------------------------------------------------------------------------|
| Vincular indicadores de capacidade/performance | Permite pesquisar e vincular um indicador de capacidade ou performance ao serviço |
| Desvincular                                    | Desvincule um indicador de capacidade ou performance listado                      |

### Atributo de Demanda

A falta de capacidade de um serviço causa indisponibilidades e o excesso é um
desperdício de investimentos. Por isto, a demanda por um serviço precisa ser
compreendida para planejar adequadamente a capacidade para atendê-la.

Nesta seção, os atributos de demanda são relacionados ao serviço.

As seguintes funções estão disponíveis:

| Função                        | Descrição                                                      |
|-------------------------------|----------------------------------------------------------------|
| Vincular atributos de demanda | Permite pesquisar e vincular um atributo de demanda do serviço |
| Desvincular                   | Desvincule um atributo de demanda listado                      |

### Avaliações do Serviço

Nesta seção estão listadas todas as avaliações da entrega do serviço. Para
facilitar a visualização, é possível filtrar os registros utilizando datas para
limitar o período da listagem.

As seguintes funções estão disponíveis:

| Filtro                       | Descrição                                 |
|------------------------------|-------------------------------------------|
| Período de registro - Início | A data inicial para filtrar as avaliações |
| Período de registro - Fim    | A data final para filtrar as avaliações   |

As seguintes funções estão disponíveis:

| Função    | Descrição                                           |
|-----------|-----------------------------------------------------|
| Pesquisar | Listar as avaliações considerando o filtro definido |
| Limpar    | Limpar as datas definidas no filtro                 |

### Auditoria do Serviço

Nesta seção estão apresentadas as ocorrências das ações relacionadas ao serviço.
Estas podem ser a alteração de atributos ou detalhes, o registro de incidentes e
requisições, a configuração de relacionamento com contratos etc.

As seguintes funções estão disponíveis:

| Campo               | Descrição                                     |
|---------------------|-----------------------------------------------|
| Período de abertura | Define a data inicial e final para a listagem |
| Categoria           | Filtra a listagem pela categoria escolhida    |
| Pesquisar           | Pesquisa com filtros definidos                |
| Limpar              | Limpar os filtros                             |
| Expandir            | Mostra mais detalhes                          |

*Aba de Cadastrar ocorrências*

| Objeto         | Descrição                          |
|----------------|------------------------------------|
| Categoria (\*) | Define a categoria para o registro |
| Descrição (\*) | Especifica os detalhes do registro |
| Gravar         | Grava os dados preenchidos         |
| Limpar         | Limpar campos preenchidos          |

(\*) Campo obrigatório
