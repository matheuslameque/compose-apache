# Provisionamento de um web server Apache utilizando o Docker Compose

Este repositório contém um arquivo _.yml_ com as configurações necessárias para subir um web server Apache simples, com uma aplicação como demonstração (gerada via IA).

## Requisitos do projeto

- ** O projeto necessitava apenas de uma configuração simples de um Docker Compose em _.yml_ de um web server Apache, como: aberturas da porta _http_, configuração do volume, e especificação da versão da imagem;
- ** A aplicação web que funciona no Apache não possui especificação alguma, servindo apenas como teste.

## Como usar

1. Clone o repositório:
   ```
   git clone https://github.com/matheuslameque/compose-apache.git
   ```
   
2. Navegue até o diretório do projeto:
   ```
   cd <seu-repositorio>
   ```

3. Certifique-se de ter o Docker e o Docker Compose instalados, utilizando os comandos abaixo na CLI:
   ```
   sudo apt update && sudo apt install docker-ce docker-compose -y
   ```

4. Execute o comando para subir o contêiner, certificando-se de deixar o arquivo _index.html_ no mesmo diretório do _compose.yml_ ou de fazer as alterações correspondentes no _.yml_, em caso de mudanças:
   ```
   docker-compose up -d
   ```

5. Teste a aplicação, checando o _IP_ da máquina que está rodando o contêiner, em seguida, no seu navegador, digite o primeiro comando caso o contêiner esteja na sua rede local, ou o segundo, caso esteja numa rede separada:
   ```
   localhost:8080
   ```
   ```  
   <seu-ip>:8080
   ```

   
