Objetivo :  Previsão do valor do aluguel  em 4 cidades do brasil 


este é um data frame do Kaggle : https://www.kaggle.com/code/juniorbueno/brazilian-houses-rent-various-regressions


Neste projeto vou fazer a predição do valor do aluguel em 4 cidades do Brasil , retirei do data frame o símbolo de cifrão que estava nas features com valores monetários, então meu data frame ficou desta forma .
entendendo um pouco dos dados : 

 ![Captura de tela 2024-09-10 164516](https://github.com/user-attachments/assets/f5c3d7cc-09b7-4896-a62b-4dada9a35368)


Fiz uma verificação dos dados para verificar o tipo de dado que temos como tipo e se temos dados nulos :

 ![Captura de tela 2024-09-10 164833](https://github.com/user-attachments/assets/efeec12e-e07b-47eb-9957-4e7cf1e733b8)


Neste data frame não temos dados nulos , deixarei as categorias como object , depois disso fiz algumas analises diretamente no dataframe. 

primeiro verifiquei qual cidade tem o total, entenda total como o valor de todas as despesas para alugar um apartamento , não somente o aluguel   mais caro : 

![cidada valo de aluguel](https://github.com/user-attachments/assets/2a20534f-eee3-4d1c-8d75-5e1cae90e38d)



 sendo São Paulo e Belo Horizonte as cidades mais caras. 
Agora comparando o quanto a mobília impacta no valor do aluguel: 

![aluguel mobilia](https://github.com/user-attachments/assets/45c34c7d-189c-49b1-bebd-ca4d2fed38f9)

 
O valor do aluguel aumenta praticamente R$ 1.500 a mais se ele é mobiliado.

Depois fiz uma contagem de valores que são outliers (outliers são valores em um conjunto de dados que se distanciam significativamente da maioria dos outros pontos.) para não alterar os dados do primeiro data frame após fazer a limpeza dos outliers.
criei um segundo data frame.
Ficamos assim depois que tratarei os outliers: 

![outliers](https://github.com/user-attachments/assets/6cc63d28-20eb-4a14-970d-8732855f56ad)


Tudo pronto para os treinos dos modelos , treinei 4 modelos e dei 2 tunning  no modelos e ficamos assim. 
3 dos modelos infelizmente deu  overfitting , mostrando as métricas : 

Gradient Boosting Regressor:
•	R² (treino): 99.80%
•	MAE: 3.59%
•	MSE: 454.50%
Random Forest Regressor:
•	R² (treino): 99.33%
•	MAE: 6.41%
•	MSE: 1477.87%

HistGradientBoosting Regressor:
•	R² (teste): 99.85%
•	MAE: 2.48%
•	MSE: 162.89%





![previsão x reais](https://github.com/user-attachments/assets/1225e6c7-64c8-45d7-82ae-e0f1ac2522fc)



O melhor modelo escolhido para predição de preço neste dataframe é o Ada boosting :
Gradient Boosting Regressor:
•	R² (treino): 99.80%
•	MAE: 3.59%
•	MSE: 454.50%
