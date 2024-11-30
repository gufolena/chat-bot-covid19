# Chatbot COVID-19 - Artemis

Este projeto é um chatbot interativo, chamado **CovidBot**, que fornece informações sobre dados de COVID-19. A Artemis utiliza uma interface gráfica criada com `customtkinter` para exibir dados globais, de países específicos, histórico de casos e dados de vacinação sobre a COVID-19. O chatbot utiliza a API [disease.sh](https://disease.sh/) para obter informações atualizadas e inclui suporte de áudio para saudar o usuário ao iniciar o aplicativo.

## Funcionalidades

- Exibe dados globais sobre COVID-19.
- Exibe dados de COVID-19 para um país específico.
- Fornece histórico dos últimos 30 dias de casos para um país específico.
- Exibe dados de vacinação para um país.
- Saudação de boas-vindas com síntese de voz ao iniciar o aplicativo.

## Tecnologias Utilizadas

- `customtkinter`: Biblioteca para criar a interface gráfica do chatbot.
- `requests`: Para fazer requisições HTTP à API de dados de COVID-19.
- `pyttsx3`: Para síntese de voz no Python.
- `unicodedata`, `re`: Para normalização e manipulação de strings.
- `pyinstaller`: Para envelopar e criar o arquivo executável.

## Pré-requisitos

- Python 3.7 ou superior instalado.
- `pipenv` instalado para gerenciar o ambiente virtual.

## Configuração do Ambiente

1. Clonar o repositório

- git clone https://github.com/gufolena/chat_bot_covid19.git
- cd chatbot-covid19

2. Instalar o ambiente virtual com pipenv (Windows e Linux)

- pip install pipenv
- pipenv install

3. Ativar o Ambiente Virtual

- pipenv shell

4. Rodar o Executável no Windows

- pipenv run pyinstaller --onefile --windowed --icon=injecao.ico --add-data "injecao.ico;." --hidden-import=customtkinter --hidden-import=requests --hidden-import=pyttsx3 chat_bot_covid19.py

5. Rodar o Executável no Linux

- pipenv run pyinstaller --onefile --windowed --icon=injecao.ico --add-data "injecao.ico:." --hidden-import=customtkinter --hidden-import=requests --hidden-import=pyttsx3 chat_bot_covid19.py



