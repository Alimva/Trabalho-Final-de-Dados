Na aplicação de Machine Leaning nos dados de Energia Hidrálica, primeiro transformamos os dados em np.array, posteriormente escalonamos os dados e assim padronizamos as variáveis na mesma escala.

Deste modo, aplicamos a técnica wcss que é o método para definir o número de clusters.

Então, podemos perceber que, aproximadamente, na escala com um cluster tivemos 40.00; com dois tivemos 8.09; e com três 1.58. 
O que pôde ser melhor visualizado em um gráfico de linha, ferramenta que serviu para a decisão de que os dados seriam dividos em quatro clusters, 
já que não houve muito declínio na escala quando passamos de quatro para cinco clusters e assim, se fizermos com mais clusters a queda não seria muito significativa.

Portanto, criamos o algoritmo final, para de fato fazer o agrupamento, onde aplicamos a função fit_predict que serviu para fazer os treinamento e obter os resultados com os valores dos clusters para cada registro.

No gráfico gerado podemos perceber:

- Os países em azul são aqueles que não geram quase nada de energia hidráulica e quase nada de energia renovável em geral.

- Os países em amarelo são os países medianos, que geram uma quantidade significativa de energia hidráulica e também energia renovável em geral

- O país em lilás é o país que gera muita energia hidraulica e também gera muita energia renovável em geral (O caso da China).

Por fim, para mais informações foi feita a lista dos paises por cluster, e foram ordenamos do cluster zero ao 2.


___________________________________________________________________________________________________________________________________________________________________________________________________________________________

O mesmo foi feito com os dados de Energia por Biocombustível, porém, foi decidido através da análise wcss que esses dados poderiam ser dividos melhor em quatro clusters,
uma vez que os Estados Unidos produz quase a mesma quantidade de Energia por biocombustível do que China, porém, produz bem menos Energia Renovável em geral.

____________________________________________________________________________________________________________________________________________________________________________________________________________________________

A utilidade da análise desses dados se dar, por conseguir ajudar empresas que trabalham com esses tipos de Energia Renovável, a escolher em qual país investir seus respectivos serviços.
