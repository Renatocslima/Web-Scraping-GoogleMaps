# Buscar Locais com a API do Google Maps

Este código Python demonstra como usar a API do Google Maps Places para buscar locais e salvar os resultados em um arquivo Excel.

## Funcionalidades

* Busca de locais por consulta de texto (ex: "hotel em Aracaju")
* Busca de locais próximos a uma localização (ex: restaurantes próximos a Aracaju)
* Salva os resultados da busca em um arquivo Excel (nome do arquivo baseado na consulta)
* Faz o download do arquivo Excel

## Uso

1. **Obtenha uma chave de API do Google Maps.**
2. **Substitua a chave de API no código (`api_key`).**
3. **Modifique as consultas de pesquisa conforme necessário.**
    * Modifique as variáveis `cidade`, `tipo_de_negocio`, `lista_negocios`, `lista_bairro` para ajustar as consultas.
4. **Execute o código.**
5. **Os arquivos Excel serão baixados automaticamente.**

## Observações

* O código usa as bibliotecas `pandas`, `requests`, `json`, `time` e `google.colab`.
* A função `search_places` realiza a busca de texto.
* A função `search_places_nearby` realiza a busca próxima.
* A função `save_to_excel` salva os dados em um arquivo Excel.
* O código inclui um loop para lidar com a paginação de resultados (next_page_token).
* O código inclui uma pausa de 10 segundos entre as solicitações para evitar exceder os limites da API.
