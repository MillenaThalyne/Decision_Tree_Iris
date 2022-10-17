# Decision Tree Iris
## Árvore de decisão com o dataset Iris
Esse projeto tem como finalidade a criação de uma árvore de decisão, utilizando o banco de dados Iris, para fazer a predição de características dessa espécie de flor.

> **Data** : 17/10/22 

> **Linguagem utilizada** : Python 

> **Autoria** : Millena Thalyne
---
## Descrição
- Primeiro, fiz a importação das bibliotecas que serão utilizadas para o projeto. Estão descritas Sklearn, Seaborn, Matplotlib e Pandas, com suas função esplicitadas. 
- Para a leitura do dataset, em formato CSV, utilizei a função "read_csv()", uma função da biblioteca Pandas; através desta que podemos fazer a posterior manipulação dos dados.
- Para a visualização dos dados, eu usei a biblioteca Matplotlib, com elas podemos ver que a classe Setosa é a mais distinta entre as demais. 
- Agora, para a fazer os _splits_ (com StratifiedShuffleSplit()) e treinamentos (com fit()), criei as funções "executar_validador" e "executar_classificador", nela também adicionei a predição, através da função "predict()" para retornar nosso _y_pred_. Adicionei uma função para salvarmos nossa árvore utilizando a função "savefig()" do Matplotlib.pyplot.
- Para X temos os valores que serão necessários para fazer a classificação da flor, ou seja,largura e comprimento das pétalas e pedal. Y são as classes em si: Sepala, Versicolor e Virginica. 
- A separação de _x_train_, _x_test_, _y_train_ e _y_test_ foi feita com a função criada anteriormente, portanto será somente necessário a chamada das variáveis para fazê-lo.
- A partir daqui fica mais fácil, uma vez que as funções já estão prontas, é somente necessário a chamada do classificador (DecisionTreeClassifier()) que retornará o _y_pred_arvore_decisao_, o Y de predição para o classificador da árvore de decisão. 
- Agora para a validação da árvore, eu tinha criado anteriormente uma função específica para isso. Nela, contém os _prints_ com as características estatísticas de Acurária, Matriz de Confusão, Score de Precisão e Recall. Vemos que temos de acurácia 96%, que nos diz que a árvore está próxima de realmente fazer predições precisas de qual flor é através de suas características. Ainda fiz um teste de predição criando um _array_ com os valores onde a IA classificou como ['versicolor' 'virginica'].
- Por fim, fiz uma breve classificação do dataset usando Random Forest (RandomForestClassifier()), porém não soube desenvolver e apenas coloquei sua validação, que ficou bem próxima da nossa árvore de decisão.

## Considerações
- A ideia de criar métodos que nos facilite a colocação de somente o classificador para criação dos algoritmos foi tirada do curso que eu fiz na Alura: ÁRVORES DE DECISÃO: APROFUNDANDO EM MODELOS DE MACHINE LEARNING, com a professora Thainá Mariani. 
- Eu achei genial, pois assim fica mais organizado e melhor de se visualizar e quis implementar juntamente com o projeto Iris, onde foi estimulado pela disciplina de Inteligência Artificial da minha faculdade. 
- Se você tiver ideias para melhoria dos algoritmos, estou completamente aberta para estas e ficarei muito grata. 

 Muito obrigada por acompanhar meu projeto! 💕
