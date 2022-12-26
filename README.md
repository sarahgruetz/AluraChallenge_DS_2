# Alura Challenge Data Science 2

Analise dos dados de imóveis para venda localizados em bairros do Rio de Janeiro, criação de modelo de regressão para precificação dos imóveis 
e criação de um sistema de recomendação de imóveis utilizando PySpark.

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **Modelos de regressão e recomendação**
| :label: Tecnologias | python, pyspark
| :rocket: URL         | -
| :fire: Desafio     | https://www.alura.com.br/challenges/data-science-2?host=https://cursos.alura.com.br

<!-- Inserir imagem com a #vitrinedev ao final do link -->
![](https://media.istockphoto.com/id/868891198/vector/house-selection-magnifying-glass-with-house-concept-for-web-banners-websites-infographics.jpg?s=612x612&w=0&k=20&c=2L1-eSTQtYdKlEwXQ11H6M7vU1pVQ4b8Z3It6e7alEw=#vitrinedev)

## Detalhes do projeto

Esse projeto foca na utilização do PySpark para a análise dos dados de imóveis localizados em alguns bairros do Rio de Janeiro. A imobiliaria está com dificuldades
na venda e aluguel desses imóveis devido a seu métodos de precificação e recomendação.

O desafio foi separado em 3 etapas, cada etapa possui um notebook correspondente. Segue uma descrição do conteúdo de cada arquivo:

### Etapa 1 
**Transformação dos dados com Pyspark** 

`tratamento-dados.ipynb`
- exploração e tratamento inicial dos dados que serão utilizados nos modelos
- seleção das colunas relevantes
- correção dos tipos de algumas variáveis

### Etapa 2
**Tratamento dos dados e criação de um modelo de regressão com PySpark** 

`modelo-regressao.ipynb`
- seleção de variáveis
- correção dos tipos das variáveis
- tratamento dos dados faltantes
- criação de variáveis dummy
- vetorização dos dados para entrada nos modelos
- análise de correlação
- regressão linear
- regression decision tree
- random forest regressor
- GBT regressor
- Grid Search e Cross Validation

### Etapa 3
**Criação de um modelo de recomendação com PySpark**

`sistema-recomendacao.ipynb`
- vetorização dos dados
- padronização (Standard Scaler)
- redução de dimensionalidade com PCA
- KMeans
- criação de uma função recomendadora

[Base de dados - InsightPlaces](https://caelum-online-public.s3.amazonaws.com/challenge-spark/semana-1.zip)

### Dicionário de Dados - Anuncio

| Colunas         | Descrição                                                      |
|-----------------|----------------------------------------------------------------|
| id              | Código de identificação do anúncio no sistema da InsightPlaces |
| tipo_unidade    | Tipo de imóvel (apartamento, casa e outros)                    |
| tipo_uso        | Tipo de uso do imóvel (residencial ou comercial)               |
| area_total      | Área total do imóvel (construção e terreno)                    |
| area_util       | Área construída do imóvel                                      |
| quartos         | Quantidade de quartos do imóvel                                |
| suites          | Quantidade de suítes do imóvel                                 |
| banheiros       | Quantidade de banheiros do imóvel                              |
| vaga            | Quantidade de vagas de garagem do imóvel                       |
| caracteristicas | Listagem de características do imóvel                          |
| andar           | Número do andar do imóvel                                      |
| endereco        | Informações sobre o endereço do imóvel                         |
| valores         | Informações sobre valores de venda e locação dos imóveis       |
