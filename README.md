#Título

KNN Classifier

#Descrição

Este projeto implementa um classificador KNN (K-Nearest Neighbors) em Python. Ele pode ser utilizado para classificar dados com base nos **k** vizinhos mais próximos. A classe `KNNClassifier` também inclui a opção de normalização dos dados, utilizando o método de escalonamento **min-max**, para garantir que todas as características (features) tenham o mesmo peso no cálculo das distâncias.

Além disso, o projeto inclui a geração de dados sintéticos com duas ou três classes e exibe gráficos dos dados gerados, da fronteira de decisão do modelo KNN e de previsões para novos pontos.

#Funcionalidades

- Implementação do algoritmo **KNN** para classificação de dados.
- Normalização opcional dos dados (min-max scaling) antes da classificação.
- Geração de dados sintéticos com **duas** ou **três** classes.
- Visualização dos dados gerados e da fronteira de decisão do modelo.
- Exemplo adicional de previsão para novos pontos.

#Estrutura do Código

- **KNNClassifier**: Classe que implementa o algoritmo KNN.
  - `fit(X, y)`: Treina o modelo com os dados de entrada `X` (dados) e `y` (rótulos).
  - `predict(X)`: Faz a previsão dos rótulos para os dados de entrada `X` com base nos k vizinhos mais próximos.
  
- **Funções auxiliares**:
  - `generate_two_class_data(n_points)`: Gera dados sintéticos com duas classes.
  - `generate_three_class_data(n_points)`: Gera dados sintéticos com três classes.
  - `plot_data(X, y, title)`: Plota os dados gerados em um gráfico de dispersão.
  - `plot_decision_boundary(knn, X, y, title)`: Plota a fronteira de decisão do modelo KNN.

#Como instalar

Este projeto utiliza as bibliotecas **NumPy** e **Matplotlib**. Para instalá-las, execute:

```bash
pip install numpy matplotlib

#Como usar
- Clonar este repositório para sua máquina local

git clone https://github.com/seuusuario/knn-classifier.git
cd knn-classifier

- Executar o script knn_classifier.py

python knn_classifier.py

O script irá solicitar os seguintes parâmetros:

Número de pontos para cada classe: Define a quantidade de pontos a serem gerados para cada classe.
Número de vizinhos (k): Define o número de vizinhos a serem considerados no KNN.
Normalizar dados?: Se yes, os dados serão normalizados.
Escolha do exemplo: Se 1, gera dados com duas classes; se 2, gera dados com três classes.

#Exemplo de Saída

Gráficos Gerados:
Dados Gerados: Gráfico com a distribuição dos pontos de cada classe.
Fronteira de Decisão: Gráfico mostrando a fronteira de decisão do modelo KNN.
Previsões para Novos Pontos: Visualização das previsões do modelo para novos pontos.

Exemplo de previsões:

Previsões para novos pontos: [0 1 0 1]

#Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo LICENSE para mais detalhes.

#Contribuição

Para contribuir, siga estas etapas:

Faça um fork deste repositório.
Crie uma branch com suas alterações: git checkout -b feature/nova-funcionalidade.
Faça commit das suas alterações: git commit -am 'Adiciona nova funcionalidade'.
Envie para o repositório remoto: git push origin feature/nova-funcionalidade.
Abra um pull request para a branch principal.
