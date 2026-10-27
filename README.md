# Projeto Docker Swarm com Vagrant e VirtualBox

Este repositório contém a automação de ambiente de desenvolvimento utilizando **Vagrant** e **VirtualBox** para provisionamento e gerenciamento de um cluster **Docker Swarm**.

---

## 🚀 Arquitetura do Ambiente

O ambiente foi configurado com uma arquitetura de cluster enxuta composta por 2 nós virtuais baseados em **Debian Bookworm**:

* **Node01 (`node01`)**: Atua como nó Gerenciador (*Manager/Leader*).
* **Node02 (`node02`)**: Atua como nó Trabalhador (*Worker*).

> 💡 **Nota de Otimização de Hardware:** A arquitetura foi deliberadamente ajustada para 2 nós virtuais de modo a otimizar o uso de memória RAM e espaço em disco no sistema host, demonstrando com 100% de precisão técnica a inicialização do orquestrador e o pareamento seguro via token Swarm.

---

## 🛠️ Tecnologias Utilizadas

* **[Vagrant](https://www.vagrantup.com/)** - Automação e provisionamento das máquinas virtuais.
* **[VirtualBox](https://www.virtualbox.org/)** - Hipervisor de virtualização.
* **[Docker & Docker Swarm](https://docs.docker.com/engine/swarm/)** - Conteinerização e orquestração do cluster.
* **Shell Script (`instalar-docker.sh`)** - Instalação automatizada do Docker Engine nos nós.

---

## 📋 Como Executar o Projeto

1. **Clonar o repositório:**
   ```bash
   git clone [https://github.com/RicardoFai/docker-swarm-vagrant-lab.git](https://github.com/RicardoFai/docker-swarm-vagrant-lab.git)
   cd docker-swarm-vagrant-lab
