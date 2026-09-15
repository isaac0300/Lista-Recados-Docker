# Lista de Recados — Docker

Projeto acadêmico desenvolvido durante a formação técnica em Desenvolvimento Web e Cibersegurança, na disciplina de Segurança e Hospedagem.

A atividade teve como objetivo estudar e praticar conceitos de Docker utilizando uma aplicação de lista de recados previamente disponibilizada pelo professor.

## Sobre o projeto

A aplicação utilizada na atividade possui três partes principais:

- Frontend
- Backend
- Banco de dados MySQL

O foco da atividade não foi o desenvolvimento da aplicação, mas a utilização do Docker para executar e gerenciar seus diferentes serviços.

Durante a aula, foram estudados conceitos de containers, redes Docker, volumes, Docker Compose e persistência de dados.

## O que foi praticado

Durante a atividade, foram realizadas as seguintes práticas:

- Criação e utilização de Docker Volume
- Criação de uma rede Docker
- Configuração do Docker Compose
- Execução de múltiplos containers
- Comunicação entre containers
- Utilização do MySQL em container
- Persistência de dados utilizando volumes
- Verificação dos containers em execução
- Verificação da rede Docker
- Verificação do volume
- Teste de persistência dos dados
- Utilização dos comandos `docker compose up` e `docker compose down`
- Teste da remoção do volume utilizando `docker compose down -v`

## Estrutura da aplicação

A aplicação utilizada na atividade possui a seguinte estrutura:

```text
Frontend
    ↓
Backend
    ↓
MySQL
```

Os serviços foram executados utilizando Docker Compose.

## Containers

- `front-recados` — responsável pelo frontend
- `back-recados` — responsável pelo backend
- `banco-recados` — responsável pelo banco de dados MySQL

## Rede

Foi utilizada a rede Docker:

`rede-recados` - ela permite a comunicação entre os containers da aplicação.

## Volume

`dados_recados` - o volume foi utilizado para armazenar os dados do MySQL de forma persistente.

## Docker Compose

O arquivo `docker-compose.yml` foi utilizado para definir e executar os serviços da aplicação em conjunto.

A configuração inclui:

- Frontend
- Backend
- MySQL
- Rede Docker
- Volume para persistência
- Dependência entre os serviços

A aplicação pode ser executada com:

`docker compose up -d --build` 

Após a inicialização, o frontend pode ser acessado pelo navegador através de:

`http://localhost:8080`

## Persistência dos dados

Um dos objetivos da atividade foi compreender a diferença entre remover os containers e remover também os dados persistidos.

Ao executar:

`docker compose down` - os containers são removidos, mas o volume permanece.

Ao executar:

`docker compose down -v` - os containers e o volume também são removidos.

Esse teste permitiu observar na prática a função dos volumes na persistência de dados.

## Tecnologias presentes na aplicação

- Docker
- Docker Compose
- Docker Volume
- Docker Network
- MySQL
- Node.js
- Express
- NGINX
- HTML
- CSS
- JavaScript

## Contexto acadêmico

A aplicação utilizada neste repositório foi previamente disponibilizada pelo professor para a realização da atividade.

O desenvolvimento do frontend, backend e banco de dados não fez parte da atividade. O foco foi estudar e praticar a utilização do Docker e do Docker Compose sobre uma aplicação já preparada.

Este repositório faz parte do meu histórico de estudos durante a formação técnica.
