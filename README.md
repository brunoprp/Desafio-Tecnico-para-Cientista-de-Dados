# Instituto Atlântico - Desafio Técnico para Cientista de Dados

Nesta prova você trabalhará com uma versão levemente modificada dos dados coletados pelo Departamento
de Polícia de Seattle e disponibilizados publicamente em seu próprio
[site](https://www.seattle.gov/police/information-and-data/use-of-force-data/use-of-force-dataset). Os dados
para a prova estão no arquivo `use-of-force.csv`.

## Contexto

Para facilitar a administração, o Departamento de Polícia de Seattle dividiu a cidade em 5 partes, cada uma
com uma delegacia. Cada parte foi subdividida em setores, que por sua vez foram divididos em *beats*,
somando um total de 17 setores e 51 *beats*
([mais detalhes](https://www.seattle.gov/police/information-and-data/tweets-by-beat)).

Suponha que você seja um Cientista de Dados contratado pela prefeitura de Seattle para automatizar o
processo de geração de relatórios. Sua responsabilidade atual é lidar com dados que caracterizam o uso
da força por parte da polícia (pun intended).

## Questões

Para responder aos questionamentos, crie um [Jupyter Notebook](https://ipython.org/notebook.html) e
organize bem as suas ideias. Clareza na lógica e qualidade visual na comunicação de resultados são
características de um bom Cientista de Dados. Sinta-se livre para utilizar quaisquer bibliotecas, tais como
[pandas](https://pandas.pydata.org/), [SciPy](https://www.scipy.org/),
[seaborn](http://seaborn.pydata.org/index.html), [scikit-learn](http://scikit-learn.org/stable/index.html) etc.

A utilização da linguagem Python é preferível, mas se você já é acostumado com R, Julia ou alguma outra,
fique à vontade.

### Análise Exploratória de Dados

Esta seção avalia a sua capacidade de responder perguntas com base em dados e de sumarizar as
informações de modo compreensivo. Você pode utilizar as formas gráficas que achar interessantes para
representar as respostas, tais como gráficos de barra, de pizza, mapas de calor etc.

1. Como é a distribuição do uso de força dentre as delegacias e os setores? Em cada setor, qual o *beat* com
maior número de incidentes? Apresente também o ranking dos setores segundo o percentual de incidentes
"Level 2" em relação ao total de incidentes do respectivo setor.

2. Com relação à distribuição dos incidentes no tempo, é possível encontrar picos ou linhas de tendência
dentro dos dias, dos meses, das semanas ou dos anos?

3. A polícia deseja dar início a uma investigação interna para verificar se existem policiais excessivamente
violentos. No entanto, o prazo para o término desta investigação é bastante limitado. Elabore um script capaz
de elencar os policiais em ordem decrescente de chance de violência excessiva com base no número de
incidentes dos quais eles participaram.

4. Uma métrica interessante para a polícia é o grau de reincidência por parte dos civis. Apresente o percentual
de casos reincidentes em relação ao total de incidentes em cada setor e verifique se há correlação entre esta
métrica e o percentual de incidentes "Level 2" calculado na questão 1. Que interpretação pode ser dada a
este resultado?

### Aprendizagem de Máquina

Esta parte da prova avalia a sua familiaridade com o processo de criação de um modelo estatístico.
Argumente bem em cada uma das fases, desde a etapa de tratamento dos dados até a validação dos
resultados.

5. A liderança do Departamento de Polícia de Seattle manifestou o interesse em uma aplicação que classifica
os incidentes em "Level 1" ou "Level 2" com base em outras colunas da tabela e lhe requisitou um parecer
sobre esta proposta. Descreva os desafios envolvidos, enumere fatores que fomentem a criação deste
classificador e sugira um modelo estatístico para executar esta tarefa, justificando a sua escolha.
P.S.: Sua justificativa deve conter explicação teórica de ao menos dois algoritmos, um benchmark destas
soluções candidatas de tempo e performance, os experimentos e análise do bias variance threshold.

6. Quando os incidentes são reportados, eles vão para uma lista que será avaliada por um inspetor cujo
papel é classificá-los como "Level 1" ou "Level 2", que normalmente é um procedimento demorado. Além
disso, há o interesse por parte da direção do Departamento de Polícia de Seattle que os incidentes "Level 2"
sejam reportados com maior antecedência. Portanto, seu papel é ordenar as listas de incidentes de modo
que o inspetor se depare primeiro com eles. Formalmente, as suas listas ordenadas devem atender ao
seguinte requisito:

* Dado um incidente aleatório A que seria avaliado como "Level 2" e um incidente aleatório B que seria
avaliado como "Level 1", as listas devem elencar A acima de B com probabilidade pelo menos 0.75.
