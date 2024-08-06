# Teste_previs-es_de_aluguel_2022
Treino de previsões 



Claro! Aqui está o texto revisado sem emoticons:

---

**Explorando o Mercado de Aluguéis com Dados Reais: Um Novo Projeto!**

Olá, pessoal!

Estou empolgado em compartilhar meu mais recente projeto de análise de dados! Utilizando um dataset do Kaggle, explorei a previsão de preços de aluguel em cinco cidades brasileiras: São Paulo, Belo Horizonte, Campinas, Porto Alegre e Rio de Janeiro.

**O que explorei:**
- **Entendimento dos Dados:** Realizei uma análise detalhada das colunas, melhorei a nomenclatura para facilitar a manipulação e confirmei que não havia valores nulos. Fiz uma análise descritiva para entender estatísticas básicas, como média, quartis e valores extremos.

- **Análise de Aluguel:** Descobri que São Paulo e Belo Horizonte têm os aluguéis totais mais altos. A relação entre o número de vagas de estacionamento e o valor total do aluguel mostrou que manter até duas vagas pode ser vantajoso. 

- **Insights Interessantes:** São Paulo tem o aluguel mais caro, com valores podendo ultrapassar R$ 4.000, seguido por Belo Horizonte, com um máximo de R$ 3.500. Analisei outliers usando gráficos Boxplot e identifiquei que, embora eles influenciem as estatísticas, não devem ser descartados sem uma análise cuidadosa.

- **Modelagem e Previsões:** Utilizei `df.query()` para agrupar dados e criei um gráfico de correlação para entender melhor as relações entre variáveis. Por exemplo, o valor total do aluguel tem uma forte correlação com o valor do seguro de incêndio e o número de banheiros. 

**Modelos de Machine Learning:**
Treinei três modelos para previsões de aluguel:
- **Gradient Boosting:** R² = 99,36%
- **Random Forest:** R² = 99,85%
- **AdaBoost:** R² = 96,79%

Todos os modelos mostraram desempenho impressionante, mas o **AdaBoost** se destacou por sua capacidade de evitar exageros, refletindo um R² de 96% que oferece uma avaliação mais equilibrada e realista.

**Conclusão:** A variável mais impactante para o valor do aluguel é o seguro de incêndio. A abordagem com AdaBoost foi a mais eficaz, oferecendo uma perspectiva equilibrada sem superestimar o desempenho do modelo.

**Curioso para saber mais?** Confira o vídeo anexado para visualizar gráficos e análises detalhadas.

Estou animado para ouvir suas opiniões e responder a qualquer pergunta. Vamos discutir como a análise de dados pode transformar a compreensão do mercado de aluguéis!

---

Espero que isso funcione bem para você!
