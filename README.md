Azure AI Search – Aisearchsample

Meu processo e conclusões:

Criei minha conta Trial no Microsoft Azure.

Assim que entrei, provisionei meu resource group rg-01. Para esse projeto, criei uma Storage Account, um Azure AI Service e um Azure AI Search.

Para inserir dados na pesquisa cognitiva, é possível utilizar Azure Blob Storage containers, Azure Data Lake Storage Gen2 e Azure Table Storage.
O AI Search oferece suporte a Vision e NLP (Processamento de Linguagem Natural) para ampliar a compreensão dos dados e gerar índices mais precisos.


Na Storage Account stgaisample01, armazenei no container container-ai-sample alguns dados de exemplo em .json e .txt para executar a pesquisa e análise com o AI Search.


![image](https://github.com/user-attachments/assets/e2ea4b92-edf0-4016-91e8-05f9e2d465a6)



Logo depois, importei os dados diretamente no meu recurso azure-ai-searchsample01, selecionando a Connection String do meu container.

Após isso, acessei o Search Explorer e executei alguns métodos para filtrar tipos de dados específicos, como avaliações com notas mais baixas, buscas por título, tema, etc.



Um exemplo de query utilizada:

search=* &$filter=avaliacao eq 5
Essa query retorna apenas documentos cujo campo avaliacao tem valor 5.



Minha estrutura atual nessa Subscription:


![image](https://github.com/user-attachments/assets/957b031e-a3b5-48e3-9977-44170f76cf7c)

