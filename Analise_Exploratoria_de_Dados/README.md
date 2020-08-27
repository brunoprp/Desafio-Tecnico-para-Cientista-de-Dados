# Instituto Atlântico - Desafio Técnico para Cientista de Dados

## Análise Exploratória de Dados
  Esta seção avalia a sua capacidade de responder perguntas com base em dados e de sumarizar as informações de modo compreensivo. Você pode utilizar as formas   gráficas que achar interessantes para representar as respostas, tais como gráficos de barra, de pizza, mapas de calor etc.

  1\) Como é a distribuição do uso de força dentre as delegacias e os setores? Em cada setor, qual o beat com maior número de incidentes? Apresente também o     ranking dos setores segundo o percentual de incidentes "Level 2" em relação ao total de incidentes do respectivo setor.

  2\) Com relação à distribuição dos incidentes no tempo, é possível encontrar picos ou linhas de tendência dentro dos dias, dos meses, das semanas ou dos anos?

  3\) A polícia deseja dar início a uma investigação interna para verificar se existem policiais excessivamente violentos. No entanto, o prazo para o término desta investigação é bastante limitado. Elabore um script capaz de elencar os policiais em ordem decrescente de chance de violência excessiva com base no número de incidentes dos quais eles participaram.

  4\) Uma métrica interessante para a polícia é o grau de reincidência por parte dos civis. Apresente o percentual de casos reincidentes em relação ao total de   incidentes em cada setor e verifique se há correlação entre esta métrica e o percentual de incidentes "Level 2" calculado na questão 1. Que interpretação pode ser dada a este resultado?

## Exemplos de resultados obtidos, todos os resultados podem ser encontrados [aqui](https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Analise_Exploratoria_de_Dados/Analise_Exploratoria_de_Dados.ipynb)
  ### Análise de Dados
  
   * No gráfico abaixo é possível analisar a quantidade de incidentes por delegacia e também o tipo do incidente. Como pode se observar a delegacia que possui mais incidentes é a West, também é possível notar que a quantidade de incidentes de nível 2 é bem menor que os incidentes nível 1.
   
   * Resultados 
      <p align="center">
      <a href="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Analise_Exploratoria_de_Dados/imagens/img1.png"><img src="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Analise_Exploratoria_de_Dados/imagens/img1.png"></a></p>
   
   * Assim como no gráfico anterior é possível notar que o policial 456 é o que tem o percentual maior, mas vale notar que os policiais 1697 e 1562 possui uma tendência maior de incidentes de nível 2, ambos os policiais tem um percentual de incidentes nível 2 bem maior que incidentes de nível 1. 
   
   * Resultados  
   <p align="center">
      <a href="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Analise_Exploratoria_de_Dados/imagens/img2.png?"><img src="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Analise_Exploratoria_de_Dados/imagens/img2.png?"></a>
    </p>
