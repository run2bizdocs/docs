Title: Requisitos do sistema

# Requisitos do sistema

Para execução da plataforma e aplicações, os requisitos recomendados do sistema podem variar de acordo com o cenário de instalação.

## Aplicação e banco de dados no mesmo servidor

Caso instale todos os programas, e o banco de dados relacional no mesmo servidor, recomendamos que o servidor tenha no mínimo `32GB` de memória para ambientes de produção. Caso deseje apenas realizar algum teste, ou ambientes de homologação e desenvolvimento, um servidor com `16GB` é o suficiente. Quanto ao tamanho do disco, recomendamos ter no mínimo `30GB` de espaço disponível.

## Aplicação e banco de dados desmembrados

Caso já tenha um servidor de banco relacional em seu ambiente, você pode fazer utilização dele para instalação do 4biz. Nesse caso, o servidor de aplicação deverá ter no mínimo `16GB` de memória. Para o servidor de banco, recomendamos no mínimo `4GB` para um ambiente de produção.

!!! Warning "ATENÇÃO"

    Qualquer que seja o caso, esses serão os  valores mínimos recomendados. Lembre-se que a plataforma do 4biz é composta por outros aplicativos, como o Builder por exemplo, que permite integrações com a s mais diversas finalidades. Essas integrações podem levar a consumos e cargas de processamento diferentes das normais, portanto os valores dos requisitos de sistema podem variar de ambiente para ambiente.   

# Versões recomendadas dos pacotes

A partir da versão Helium 1.2.23 a tabela Versões recomendadas dos pacotes deverá ser alterada para os Bancos de dados homologados:

|Aplicação         | Versão   |
-------------- | ------ |
|Wildfly | `12.x` |
|Java JDK | `8.x` |
|PostgreSQL | `12` |
|Driver JDBC |`Depende da versão do banco. No documento usaremos a versão 9.3 pois o postgreSQL será nesta versão.` |
|SOLR | `6.4.2` |
|Sistema Operacional| Embora possa ser instalado em qualquer distribuição e versão, o documento considera a distribuição `Linux CentOS 7.x.`   |
MongoDB   | `3.4.15`|
|Microsoft SQL Server|`2019`|
|Oracle| `12c`|



