# Sistema de Feedback para Cursos Livres - Parte 2

> **Evolução Arquitetural:**  
> Este repositório contém a versão evoluída do sistema de feedback. A aplicação foi refatorada a partir da primeira versão (monolítica) para adotar uma arquitetura modularizada, separando o projeto em três serviços orquestrados via Docker Compose:
> * **API:** Backend para manipulação da regra de negócio.
> * **Dashboard:** Interface gráfica consumindo os dados da API.
> * **Banco de Dados:** Instância PostgreSQL utilizando scripts SQL automatizados (`init.sql`).

**Autores e Desenvolvedores:**  
Gabriel Bezerra, Paulo Augusto de Moura Neto, Felipe Batista de Oliveira Nascimento, Guilherme de Souza Ferraz, Kaique Luccas Dias Rosa.

---

## 🚀 Como Executar o Projeto

Para garantir que o ambiente seja idêntico ao de desenvolvimento (evitando erros de compilação como o que ocorreu com o `numpy` no seu sistema local), utilize o **Docker Compose**.

### Pré-requisitos
* **Docker Desktop** instalado e rodando.

### 1. Preparação dos Arquivos
Certifique-se de que todos os arquivos estejam na mesma pasta:
* `app.py`
* `requirements.txt`
* `Dockerfile`
* `docker-compose.yml`
* `.python-version` (Opcional, mas recomendado)

### 2. Execução (Via Docker Compose)
Abra o terminal (PowerShell, CMD, ou terminal Linux/Mac) na pasta raiz do projeto e execute o seguinte comando:

```bash
docker compose up --build


Endereço para testar: http://localhost:8501
