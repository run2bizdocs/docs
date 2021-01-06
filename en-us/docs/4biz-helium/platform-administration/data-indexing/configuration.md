Title: Managing content indexing

# Managing Content Indexing

4biz uses Apache SOLR to index content created in the Knowledge Management and makes it available in the Knowledge Portal search system.

## What to do before

In order for Knowledge Indexing to work correctly, it is necessary:

* [x] Install the Apache SOLR component as shown in the [installation manual][1].

## Parametrizing the indexing service

1. Access the main menu Parametrization > 4biz Parameters;
2. Configure parameter 304 by entering the URL of the SOLR component;

    ```sh
    http://localhost:8983/solr/collection_name
    ```

3. Configure parameter 308 stating the number of items to be indexed each time;
4. Configure parameter 332 stating whether synchronization with the Indexing server is active;  
5. Configure Parameter 333 informing the interval in minutes to synchronize knowledge with the index server - Accepted values between 1 and 59;  
6. Access the main menu System > Settings > Knowledge Management (Indexing) and click on "Update the index server".

## Managing content

1. Access the main menu System > Settings > Kowledge Management (Indexing);
2. To index the available knowledge, click on "Index Knowledge Base", or to remove the knowledge already indexed, click on "Remove 
Knowledge Base Indexing".


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020

[1]:/en-us/4biz-helium/get-started/installation-and-upgrade/download-software.html#servidor-de-indexacao-apache-solr_1
