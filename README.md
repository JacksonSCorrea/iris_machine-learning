# iris_machine-learning

Este projeto visa aplicar modelos de classificação e usa como base o dataset 'iris'.

As tarefas propostas são:
* Fazer a Análise Exploratória dos Dados.
* Fazer o Pré-Processamento dos dados
* Criar a Máquina Preditiva.
* Avaliar a Máquina Preditiva.

Foram implementados 6 modelos no exercício de forma que para cada um dos modelos as predições
foram realizadas ao mesmo tempo em que a validação cruzada era aplicada, através do método cross_val_predict, pelos seguintes motivos:
*  O dataset possui poucas instâncias (150). Logo, quanto menos dados forem separados, melhor o aprendizado do modelo.
*  Acredita-se que melhor do que treinar o modelo em 20% dos dados e testar nos 20% restantes, seria predizer os valores já
   na validação cruzada.
*  Como não será discutida a tunagem do modelo com osmelhores hiperparâmetros, o validação cruzada já poderia
   retornar as predições, e não as métricas.

As predições e métricas foram realizados através de iterações em uma lista de modelos.
Ao fim dos cálculos, é gerado um dataset resumo das métricas de cada modelo para cada classe analisada (setosa, virgínica, versicolor)

Foram trabalhadas duas variações do dataset iris: o dataset original e o dataset com duas features excluídas, com o intuito de verificar
o deempenho dos modelos.

Ressaltando novamente, não foram efetuadas otimizações de modelos através de ajuste de hiperparâmetros.
Também não serão aplicadas técnicas de seleção devariáveis.

Enjoy!

