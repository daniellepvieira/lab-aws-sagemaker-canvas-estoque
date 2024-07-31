## Resultados das Previsões de Estoque no SageMaker Canvas

Utilizei como CSV na plataforma de SageMaker Canvas o dataset dataset-1000-com-preco-promocional-e-renovacao-estoque.CSV. 
Após analisar o modelo de previsão de estoque, obtive as seguintes métricas:

### Estatísticas de Erro

- **Avg. wQL (Weighted Quantile Loss)**: 0.060
  - O Average Weighted Quantile Loss indica uma boa precisão do modelo, com valores mais baixos refletindo previsões mais precisas.

- **MAPE (Mean Absolute Percentage Error)**: 14.9%
  - O MAPE mede o erro percentual médio absoluto das previsões. Um MAPE de 14.9% sugere um erro médio de cerca de 15% em relação ao valor real, indicando um desempenho moderado do modelo.

- **WAPE (Weighted Absolute Percentage Error)**: 10.3%
  - O WAPE é uma versão ponderada do MAPE e indica uma precisão razoável, com um erro percentual médio ponderado de 10.3%.

- **RMSE (Root Mean Square Error)**: 5.977
  - O RMSE representa o erro médio das previsões em unidades da variável target. Um RMSE de 5.977 sugere que as previsões têm uma margem de erro média de aproximadamente 5.977 unidades.

- **MASE (Mean Absolute Scaled Error)**: 0.310
  - O MASE compara o desempenho do modelo com um modelo de referência simples. Com um valor de 0.310, o modelo está significativamente melhor do que um modelo de referência básico.

### Outras Métricas

- **Preço**: 9.14%
  - Refere-se ao impacto do preço nas previsões de estoque. O preço contribui com 9.14% para o modelo de previsão.

- **Holiday**: 2.79%
  - Indica a influência dos feriados ou eventos promocionais nas previsões de estoque. O impacto dos feriados é relativamente pequeno, com uma contribuição de 2.79%.
### **Conclusão**
   - O modelo de previsão de estoque analisado fornece uma boa base para previsões, com métricas indicando um desempenho razoável. A análise sugere que o modelo é eficaz em alguns aspectos, mas pode ser otimizado ainda mais para melhorar a precisão das previsões e a inclusão de variáveis relevantes.
