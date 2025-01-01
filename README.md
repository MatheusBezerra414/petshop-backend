# Petshop Backend 🐾

![Go Version](https://img.shields.io/badge/Go-1.20-blue)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14.0-blue)
![Docker](https://img.shields.io/badge/Docker-Compose-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)

**Petshop Backend** é um sistema desenvolvido em **Golang** seguindo os princípios de **Clean Architecture**. Ele utiliza **PostgreSQL** como banco de dados e é containerizado com **Docker** para facilitar a implantação e escalabilidade. Este projeto foi projetado com foco em boas práticas de código, modularidade e desempenho.

## 🚀 Tecnologias Utilizadas

- **[Golang](https://golang.org/):** Linguagem de programação para alta performance e escalabilidade.
- **[PostgreSQL](https://www.postgresql.org/):** Banco de dados relacional robusto e confiável.
- **[Docker](https://www.docker.com/):** Containerização para padronizar o ambiente de desenvolvimento e produção.
- **[Clean Architecture](https://en.wikipedia.org/wiki/Clean_Architecture):** Organização que separa lógica de negócios, casos de uso, e interfaces de entrega.
- **[Air](https://github.com/cosmtrek/air):** Hot reload para desenvolvimento rápido e eficiente.

## 📦 Recursos

- Cadastro e gerenciamento de pets e clientes.
- Integração com APIs RESTful.
- Estrutura modular para fácil manutenção e expansão.
- Suporte a configurações flexíveis com variáveis de ambiente.

## 🛠️ Como Rodar o Projeto

Siga os passos abaixo para configurar e rodar o projeto localmente:

1. **Clone este repositório**:
 ```bash
 git clone https://github.com/MatheusBezerra414/petshop-backend
 ```
   
2. **Navegue até o diretório**:
 ```bash
   cd petshop-backend
```

3. **Inicie os containers com Docker Compose**:
  ```bash
  docker-compose up --build
```

## 📚 Estrutura do Projeto
```plaintext
petshop-backend/
├── cmd/                     # Ponto de entrada da aplicação
├── config/                  # Configurações de ambiente
├── internal/                # Lógica de domínio e casos de uso
│   ├── domain/              # Entidades e interfaces do domínio
│   ├── usecase/             # Casos de uso
│   ├── repository/          # Implementação dos repositórios
│   └── delivery/            # Interfaces de entrega (HTTP, gRPC)
├── migrations/              # Arquivos de migração para o banco de dados
├── pkg/                     # Pacotes reutilizáveis
├── docker-compose.yml       # Configuração do Docker Compose
└── README.md                # Documentação do projeto
```
