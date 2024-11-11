# Página de Teste com Docker

Este repositório contém uma página HTML simples com um **Dockerfile** configurado para facilitar a execução da página em um contêiner Docker. O projeto inclui uma interface de blog fictícia sobre Docker, com conceitos básicos e uma seção de comentários.

## Estrutura do Projeto

- **Dockerfile**: Arquivo de configuração Docker para iniciar um servidor web e hospedar a página HTML.
- **index.html**: Página principal com conteúdo informativo sobre Docker.
- **styles.css**: Arquivo CSS para estilizar a página.

## Pré-requisitos

- **Docker**: Certifique-se de ter o Docker instalado no seu sistema. Para instruções de instalação, visite [a documentação oficial do Docker](https://docs.docker.com/get-docker/).

## Como Executar

1. Clone o repositório:
    ```bash
    git clone git@github.com:ruanncaetano/PaginaDocker.git
    cd PaginaDocker
    ```

2. Construa a imagem Docker:
    ```bash
    docker build -t minha-pagina-docker .
    ```

3. Inicie o contêiner:
    ```bash
    docker run -d -p 8080:80 minha-pagina-docker
    ```

4. Acesse a página no navegador em `http://localhost:8080`.

## Funcionalidades

- **Página HTML informativa sobre Docker**: Conteúdo e estilo básico para apresentar o Docker de forma simples.
- **Formulário de Comentário**: Permite que usuários deixem comentários fictícios.
- **Galeria de Fotos**: Espaço para adicionar imagens relacionadas.

## Personalização

- **Adicione ou edite o conteúdo em `index.html`** para personalizar o texto e as seções da página.
- **Atualize o Dockerfile** para ajustar configurações de servidor ou ambiente conforme necessário.

## Tecnologias Utilizadas

- **HTML/CSS**: Estrutura e estilo da página.
- **Docker**: Contêiner para hospedagem local.
