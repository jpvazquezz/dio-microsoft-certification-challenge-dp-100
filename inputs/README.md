# Utilizando o Azure Machine Learning no trabalho

No meu trabalho, construí um pipeline job no Azure Machine Learning para gerar previsão para meu modelo de série temporal. O modelo consiste num algoritmo Prophet treinado com regressores. No pipeline job, recupero a base de dados histórica, registrada como data asset, e também o modelo treinado e registrado com MLflow. Em seguida, a previsão é realizada por meio da invocação de um batch endpoin que possui o deploy do modelo mais recentemente treinado. O resultado é um csv com o resultado das previsões do modelo Prophet. 
