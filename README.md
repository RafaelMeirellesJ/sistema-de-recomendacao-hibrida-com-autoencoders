# Sistema de Recomendação com Autoencoders (SRcA)

Este projeto implementa um sistema de recomendação híbrido utilizando autoencoders e similaridade entre usuários. O objetivo é recomendar conteúdos personalizados para os usuários com base em suas interações anteriores e em usuários similares.

## Estrutura do Projeto

- **`interactions_full_df.csv`**: Arquivo contendo o conjunto de dados de interações entre usuários e conteúdos.
- **`Sh_Games.ipynb`**: Notebook principal com a implementação do sistema de recomendação.
- **`requirements.txt`**: Lista de dependências necessárias para executar o projeto.

## Funcionalidades

1. **Pré-processamento de Dados**:
   - Transformação dos dados utilizando a técnica de Yeo-Johnson.
   - Criação de uma matriz usuário-item escalada.

2. **Modelo de Autoencoder**:
   - Treinamento de um autoencoder para gerar embeddings de usuários.
   - Utilização de EarlyStopping para evitar overfitting.

3. **Recomendações Híbridas**:
   - Combinação de previsões do autoencoder com similaridade entre usuários.
   - Geração de recomendações personalizadas para cada usuário.

4. **Visualização**:
   - Gráficos de desempenho do treinamento (MSE e MAE).

## Como Executar

1. **Instalar Dependências**:
   Certifique-se de ter o Python instalado. Em seguida, instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

2. **Executar o Notebook**:
   Abra o arquivo `Sh_Games.ipynb` em um ambiente Jupyter Notebook ou VS Code e execute as células sequencialmente.

3. **Testar Recomendações**:
   Utilize as funções no notebook para gerar recomendações para usuários específicos.

## Requisitos

- Python 3.8 ou superior
- Bibliotecas listadas em `requirements.txt`

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

Este projeto é distribuído sob a licença MIT. Consulte o arquivo LICENSE para mais informações.
