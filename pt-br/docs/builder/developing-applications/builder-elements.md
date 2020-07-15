Title: Elementos Builder

# Elementos Builder

Uma aplicação Builder é construída com uma combinação dos seguintes elementos.

## Objeto de Negócio

Um Objetos de Negócios Builder são abstrações para as entidades de dados das aplicações. Cada Objeto de Negócio representa o modelo de dados e está vinculado a uma tabela ou view de em um banco de dados relacional.

## Regra de Negócio

As Regras de Negócio do Builder servem para realizar validações que reflitam as regras de negócio das aplicações. Podem ser usadas para validação de formulários e/ou associadas a operações de inclusão, alteração e exclusão de objetos de negócio.

## Formulário

É através do Formulário Builder que o usuário interage com a aplicação, executando operações de consulta, inclusão, alteração e remoção de dados nos Objetos de Negócio ou fornecendo informações para a execução de fluxos.

## Fluxo de Integração

Os Fluxos de Integração permitem integrar aplicações Builder a sistemas externos, sejam eles do ambiente 4Biz ou de terceiros. É uma ótima alternativa para integração com sistemas legados.

## Processo de Negócio

O Processo de Negócio permite a execução de Fluxos de Integração de forma rotineira e automatizada.
Interação entre elementos Builder

 
De uma maneira simples, podemos definir a interação entre elementos Builder como:

1.	Objeto de Negócio interage diretamente com Formulários e sistemas externos (via API REST), fazendo uso de  Domínios e Regras de Negócio para validação de dados;

2.	Formulários interagem nativamente com o Objetos de Negócio e com sistemas externos, através de programação JavaScript/AngularJS.  A interface com usuários e as regras de negócio aplicadas ao formulários podem ser enriquecidas com uso de recursos compartilhados tais como código JavaScript, CSS e HTML;

3.	Formulários também se conectam a Fluxos de Integração e Fluxos de Serviço ITSM fazendo, respectivamente, interface com sistemas e bancos de dados legados e com o Gerenciamento de Ticket do 4Biz.
