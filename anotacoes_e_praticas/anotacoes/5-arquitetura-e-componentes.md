# Arquitetura e Componentes

- Machine Learning (MLlib)
- SQL (SparkSQL)
- Processamento de Streaming (dados que precisam ser processados em tempo real ou próximo ao tempo real)
- Processamento de Grafos (GraphX)

## Tungsten (motor de execução)
<p> O foco da eficiência do Tungsten é a eficiência da CPU, por que as cargas de trabalho do Spark são em memória, dando foco à otimização da CPU.

## Transformações: Narrow e Wide
<p> Na Transformação Narrow, os dados necessários estão em uma mesma partição.
<p> Na Transformação Wide, os dados necessários estão em mais de uma partição.

## Componentes
- Job: tarefa
- Stage: divisão do Job
- Task: menor unidade de trabalho. Uma por núcleo e por partição