Clonando o repositório

    git clone git@github.com:hugomatheuss/projeto-pos-docker.git

Entrando no diretório do projeto

    cd projeto-pos-docker

Para construir a imagem baseada no Dockerfile
    
    docker build -t hugomatheuss/projeto-pos-docker:1.0.0 .
    
Para executar a imagem da aplicação na porta 8080

    docker run -p 8080:80 hugomatheuss/projeto-pos-docker:1.0.0


Acessando em http://localhost:8080/


Para subir a imagem para o docker hub
    
    docker login -u CONTA_DOCKER_HUB

    docker image push CONTA_DOCKER_HUB/NOME_REPOSITORIO:TAG_VERSAO