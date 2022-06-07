# Context e Session
<p> Podemos rodar um script Spark no shell (pyspark). O Spark cria uma sessão automaticamente chamada spark.
<p> Se criarmos uma aplicação spark (em um programa .py, por exemplo), precisamos criar a sessão:

<p>spark = (SparkSession
<p>.builder
<p>.appName("Meuapp")
<p>.getOrCreate() )