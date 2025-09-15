# CP2-redes-neurais

# Classificação de Vinhos - Wine Dataset (UCI)

## Descrição
Este projeto utiliza o **Wine Dataset** (UCI Machine Learning Repository) para treinar e comparar diferentes modelos de classificação.  
O objetivo é prever a classe de um vinho com base em suas características físico-químicas.

## Modelos Utilizados
1. **Rede Neural (Keras/TensorFlow)**
   - 2 camadas ocultas, 32 neurônios cada, função de ativação ReLU.
   - Camada de saída com 3 neurônios, função de ativação Softmax.
   - Função de perda: categorical_crossentropy.
   - Otimizador: Adam.
   - Métrica: Acurácia.

2. **Random Forest (Scikit-learn)**
   - 100 árvores.
   - Random state fixo para reprodutibilidade.

3. **Regressão Logística (Scikit-learn)**
   - Modelo linear base para comparação.

## Resultados
- **Rede Neural:** ~0.97 de acurácia no conjunto de teste.  
- **Random Forest:** 1.00 de acurácia no conjunto de teste (média de 0.97 na validação cruzada).  
- **Regressão Logística:** ~0.95 de acurácia no conjunto de teste.  

## Conclusão
- O **Random Forest** apresentou o melhor desempenho, atingindo 100% no conjunto de teste e cerca de 97% em validação cruzada.  
- A **Rede Neural** também obteve desempenho elevado, próxima de 97%.  
- A **Regressão Logística** foi competitiva, mas inferior aos outros modelos, como esperado por ser linear.  

## Como Executar
1. Clone o repositório:
   ```bash
   git clone https://github.com/nathaliagmsss/CP2-redes-neurais.git
   cd CP2-redes-neurais


# Atividade 2 - REGRESSÃO

Para rodar o notebook no Jupyter, basta abrir o arquivo e executar as células na ordem, de cima para baixo. O notebook utiliza a biblioteca Keras para treinar uma rede neural. Primeiro, importa as bibliotecas necessárias e carrega os dados. Depois, prepara os dados para o treinamento, definindo a estrutura da rede neural com camadas densas, função de ativação e outras configurações.

Após definir o modelo, ele é treinado com os dados de entrada e depois testado para ver sua precisão. O notebook calcula métricas como o erro médio quadrático (MSE) e o erro absoluto médio (MAE), que indicam a qualidade das previsões da rede. No resultado mostrado, a rede neural teve desempenho pior que um modelo Random Forest, que apresentou erros menores.

Resumindo, o notebook mostra como criar, treinar e avaliar um modelo Keras para regressão e compara seu desempenho com outro modelo clássico. Para rodar os experimentos, basta executar as células sequencialmente em um ambiente com Python, Keras e demais bibliotecas instaladas.
