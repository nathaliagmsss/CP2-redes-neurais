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
