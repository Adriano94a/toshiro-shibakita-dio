# 🐳 Projeto Docker: Cluster Swarm com MySQL, NGINX e PHP

> Projeto desenvolvido durante o Bootcamp de Linux da [DIO](https://www.dio.me/) com o professor **Denilson Bonatti**.  
> O foco principal foi a criação de um ambiente containerizado e escalável utilizando **Docker Swarm**, integrando **NGINX**, **PHP** e **MySQL**.

---

## 🛠️ Tecnologias Utilizadas

- [Docker](https://www.docker.com/)
- [Docker Swarm](https://docs.docker.com/engine/swarm/)
- [MySQL](https://www.mysql.com/)
- [NGINX](https://www.nginx.com/)
- [PHP](https://www.php.net/)
- Linux (Ambiente base)

---

## 📝 Descrição

Este projeto tem como objetivo principal simular um ambiente de produção com múltiplos containers orquestrados via Docker Swarm, onde:

- 🐋 **Docker e Docker Swarm** são usados para orquestrar os containers e garantir alta disponibilidade
- 🗃️ **MySQL** roda em um container dedicado para persistência de dados
- 🔄 **NGINX** atua como um **proxy reverso** e balanceador de carga para a aplicação
- 🖥️ Uma **aplicação PHP** se comunica com o banco de dados MySQL para exibir conteúdo dinâmico
- ⚡ Foram realizados **testes de performance e escalabilidade** para simular acessos simultâneos

---

## 📦 Estrutura do Projeto

```bash
.
├── docker-compose.yml         # Configuração para ambiente de testes local
├── swarm-setup/               # Scripts e configurações para deploy no Swarm
│   ├── php/                   # Código da aplicação PHP
│   ├── nginx/                 # Configurações do NGINX
│   └── mysql/                 # Volume e init do banco de dados
├── README.md                  # Este arquivo
└── ...
