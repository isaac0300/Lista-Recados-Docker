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

Os serviços foram executados utilizando Docker Compose.
```
## Containers
- `front-recados` — responsável pelo frontend
- `back-recados` — responsável pelo backend
- `banco-recados` — responsável pelo banco de dados MySQL
