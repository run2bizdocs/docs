Title: Gerenciar a indexação de conteúdo

# Gerenciar a indexação de conteúdo

O 4biz usa o Apache SOLR para indexar o conteúdo criado na Gerência de Conhecimento e o disponibiliza no sistema de busca do Portal de Conhecimento.

## O que fazer antes

Para que a Indexação de conhecimento funcione corretamente é necessário:

* [x] Instalar o componente Apache SOLR como apresentado no [manual de instalação][1].

## Parametrizar o serviço de indexação

1. Acessar o menu principal Parametrização > Parâmetros 4biz;
2. Configurar o Parâmetro 333 informando o intervalo em minutos para sincronizar os conhecimentos com o servidor de indexação – Valores aceitos entre 1 e 59;
3. Configurar o parâmetro 304 informando a URL do componente SOLR;

    ```sh
    http://localhost:8983/solr/collection_name
    ```

4. Configurar o parâmetro 308 informando a quantidade de itens a serem indexados por vez;
5. Configurar o parâmetro 332 informando se a sincronização com o servidor de Indexação está ativa;
6. Acessar o menu principal Sistema > Configurações > Gerência do Conhecimento (Indexação) e clicar em "Atualizar o servidor de indexação".

## Gerenciar conteúdo

1. Acessar o menu principal Sistema > Configurações > Gerência do Conhecimento (Indexação);
2. Para indexar os conhecimentos disponíveis, clicar em "Indexar base de conhecimento", ou para remover os conhecimentos já indexados, clicar em "Remover indexação base conhecimento".


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

[1]:/pt-br/4biz-helium/get-started/installation-and-upgrade/download-software.html#servidor-de-indexacao-apache-solr_1
