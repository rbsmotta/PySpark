# Spark SQL

## Spark
- Utiliza o Metastore do Hive
- Não é preciso ter o hive instalado para usar o Spark

<p> Hive é um data warehouse para o Hadoop.
<p> Metastore direciona o local onde os metadados ficam direcionados.

## Tabela
- Persistente (não é volátil como o Dataframe)
- Objeto Tabular que reside em um banco de dados
- Pode ser gerenciado e consultado utilizando SQL
- Totalmente interoperável com Dataframe (podemos transformar um Dataframe em tabela e vice-versa, de forma muito simples)
- Ex.: Um Dataframe importado (Parquet, json, ORC, CSV) pode se transformar em uma tabela

### Tabelas Gerenciadas (Managed)
Spark gerencia dados e metadados
- Armazenadas no warehouse do spark
- Se excluírmos, tudo é apagado (dados e metadados)

### Tabelas Não Gerenciadas (External)
Spark apenas gerencia metadados
- Informamos onde a tabela está (arquivo, por exemplo orc)
- Se excluírmos, Spark só exclui os metadados, dados permanecem onde estavam

## Views
- Mesmo conceito de banco de dados relacionais
- São "alias" para uma tabela
- Não contém dados

### Tipos de Views
- Globais: visíveis em todas as sessões
- Sessão: visível apenas na própria sessão