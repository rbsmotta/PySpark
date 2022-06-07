## Instalação
- sudo apt update
- sudo apt upgrade
- sudo apt install curl mlocate default-jdk -y
- pesquisar "spark download", entrar no site do Spark e procurar a versão mais atual. Copiar o link.
- Fazer o download do arquivo. No terminal digitar: wget (colar o link)
- extrair arquivos: 
<p>tar xvf (nome_do_arquivo)

- mover pasta extraida para pasta opt: 
<p>sudo mv (pasta_extraida)/ /opt/spark

- definir variáveis de ambiente: 
<p>sudo nano ~/.bashrc

- acrescentar as duas linhas abaixo:
<p>export SPARK_HOME=/opt/spark
<p>export PATH=$PATH:$SPARK_HOME bin:$SPARK_HOME/sbin

- verificar se o arquivo foi atualizado:
<p>source ~/.bashrc

- inicializa o nó master stand alone do spark:
<p>start-master.sh

- no navegador, digitar:
<p>localhost:8080

- inicializar o working process do Spark:
<p>/opt/spark/sbin/start-slave.sh spark://localhost:7077

- entrar no shell do Spark:
<p>pyspark