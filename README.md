<p><img width=100%  src= "https://i.ibb.co/rskykxr/Projeto-recomendador-de-musica.png" alt="logo"></p>

<p align="center">
    <!-- Python -->
    <img alt="python" src="https://img.shields.io/badge/python-FFFFFF?style=flat&labelColor=000000&color=FFFFFF&logo=python&logoColor=1ED760&">
    <!-- Pandas -->
    <img alt="pandas" src="https://img.shields.io/badge/pandas-FFFFFF?style=flat&labelColor=000000&color=FFFFFF&logo=pandas&logoColor=1ED760&">
    <!-- Numpy -->
    <img alt="numpy" src="https://img.shields.io/badge/numpy-FFFFFF?style=flat&labelColor=000000&color=FFFFFF&logo=numpy&logoColor=1ED760&">
    <!-- Plotly -->
    <img alt="plotly" src="https://img.shields.io/badge/plotly-FFFFFF?style=flat&labelColor=000000&color=FFFFFF&logo=plotly&logoColor=1ED760&">
    <!-- Scikit-learn -->
    <img alt="scikit-learn" src="https://img.shields.io/badge/sklearn-FFFFFF?style=flat&labelColor=000000&color=FFFFFF&logo=scikitlearn&logoColor=1ED760&">
    <!-- Status -->
    <img alt="status" src="https://img.shields.io/badge/Status-Concluído-FFFFFF?style=flat&logoColor=1ED760&labelColor=000000">
</p>

# Projeto: Recomendador de música utilizando API do Spotify
Este projeto é um recomendador de música baseado em clustering utilizando o algoritmo K-means. Ele tem como objetivo recomendar músicas similares com base nas preferências do usuário.

# Índice 

* [Descrição do Projeto](#descrição-do-projeto)
* [Funcionalidades](#funcionalidades)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Acesso ao Projeto](#acesso-ao-projeto)
* [Licença](#licença)


# Descrição do projeto
O projeto "Recomendador de música utilizando API do Spotify" foi desenvolvido com o objetivo de aplicar técnicas de Clustering, utilizando o algoritmo K-Means, para recomendar músicas com base em uma referência utilizando distância euclidiana. O projeto visa proporcionar uma experiência de aprendizagem sobre clustering e aplicação de algoritmos de recomendação.

# Funcionalidades

- Recomendação de músicas similares com base nas preferências do usuário
- Clustering de músicas utilizando o algoritmo K-means

# Tecnologias utilizadas
- Linguagem: Python 3.11.5
- Bibliotecas: 
Pandas (2.1.1), Numpy (1.24.3), Plotly (5.9.0), Matplotlib (3.8.0), Scikit-learn (1.3.0)

# Acesso ao Projeto
Para acessar e executar o projeto, seguir os seguintes passos:
1. Clonar o projeto em sua máquina local.
2. Fazer uma conta na API do Spotify e gerar suas próprias client_id e client_secret no site [Spotify for Developers](https://developer.spotify.com/documentation/web-api)
3. Inserir suas client_id e client_secret nos parâmetros localizados na célula 52 do Notebook.
 ```python
# Autenticando na API do Spotify.
scope = 'user-library-read playlist-modify-private'
OAuth = SpotifyOAuth(
        scope=scope, 
        client_id=client_id, 
        client_secret=client_secret, 
        redirect_uri='http://localhost:8080')

client_credentials_manager = SpotifyClientCredentials(client_id=client_id, client_secret=client_secret)
 ```
4. Executar os scripts em ordem.

# Licença
[MIT License](https://opensource.org/license/mit/)