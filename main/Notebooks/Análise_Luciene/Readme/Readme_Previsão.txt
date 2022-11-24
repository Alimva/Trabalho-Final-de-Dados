Aplicando um modelo de Regressão Linear simples nos dados de Energia Hidráulica, temos a variável x como o ano (variável preditiva) e  y será nossa variável objetivo, onde será guardado a quantidade de geração de energia hidráulica por ano.

Utilizando o coeficiente de correlação podemos ver que 89,44% dos dados de geração de energia pode ser explicado pelos "anos", ou seja, um algoritmo de regressão linear pode funcionar bem.

Assim, colocamos os dados em formato de Matriz para poder enviar para o algoritmo de regressão liner (requisito da biblioteca sklearning)

Posteriormente fizemos o treinamento, passando os atributos previsores e as respostas esperadas. 
Deste modo, podemos encontrar o parâmetro b0 e também os coeficientes para cada um dos atributos. Que define a localização da linha do gráfico de regressão.

O gráfico de regressão nos permitiu prever pra cada ano a geração de energia hidráulica, utilizando a fórmula y=b_0+b_1*"Ano".
Com isso, trocando a variável novamente para vetor simples, com a função ravel no numpy, o gráfico foi criado para demonstrar essas previsões.

Logo após podemos perceber que aplicando os anos na fórmula, por exemplo 1990, podemos ter o valor exato da variável.

Uma métrica para aplicar quão bom é o algoritmo de regressão, foi passada, dando aproximadamente 0,80, o que é bom pois está próximo a 1.
