# Instituto Atlântico - Desafio Técnico para Cientista de Dados

## Aprendizagem de Máquina, classificação dos incidentes em "Level 1" ou "Level 2"
  A liderança do Departamento de Polícia de Seattle manifestou o interesse em uma aplicação que classifica os incidentes em "Level 1" ou "Level 2" com base em outras colunas da tabela e lhe requisitou um parecer sobre esta proposta. Descreva os desafios envolvidos, enumere fatores que fomentem a criação deste classificador e sugira um modelo estatístico para executar esta tarefa, justificando a sua escolha. P.S.: Sua justificativa deve conter explicação teórica de ao menos dois algoritmos, um benchmark destas soluções candidatas de tempo e performance, os experimentos e análise do bias variance threshold.
* Desafios envolvidos

  1\) Testa vários algoritmos para analisar qual algoritmo consegue um bom desempenho.
  
  2\) Confiabilidade dos dados, usar métodos de treinamento e avaliação de forma que os modelos conseguem generalizar os dados.
  
  3\) Realizar vários testes com a retirada e a substituição de dados faltosos, pode haver efeitos nos desempenhos dos modelos com a retirado ou fazendo a substituição dos dados faltosos.

## Exemplos de resultados obtidos, todos os resultados pode ser encontrado [aqui](https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Aprendizagem_de_Maquina/classification.ipynb):
  ### Classificador Naive Bayes
  
   * Os métodos [Naive Bayes](https://scikit-learn.org/stable/modules/naive_bayes.html) são um conjunto de algoritmos de aprendizagem supervisionada com base na aplicação do teorema de Bayes com a suposição "ingênua" de independência condicional entre cada par de recursos dado o valor da variável de classe. O teorema de Bayes afirma a seguinte relação, dada a variável de classe `y` e o vetor de características dependentes `x_1` a `x_n`. A Variação usada é o [Gaussian Naive Bayes](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html#sklearn.naive_bayes.GaussianNB).
   
   * Resultados 
      <p align="center">
      <a href="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Aprendizagem_de_Maquina/imagens/resut_nava.png"><img src="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Aprendizagem_de_Maquina/imagens/resut_nava.png"></a></p>
    
   <p align="center">
      <a href="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Aprendizagem_de_Maquina/imagens/result_comp.png"><img src="https://github.com/brunoprp/Desafio-Tecnico-para-Cientista-de-Dados/blob/master/Aprendizagem_de_Maquina/imagens/result_comp.png"></a>
    </p>
