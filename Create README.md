# 📌 Django RESTful API - Gerenciamento de Tarefas

Este projeto é uma API RESTful desenvolvida em Django e Django Rest Framework (DRF) para o gerenciamento de tarefas. Ele permite criar, listar, buscar, atualizar e deletar tarefas, além de filtrar por status.

## 🚀 Funcionalidades

- Criar uma tarefa (`POST /api/tarefas/`)
- Listar todas as tarefas (`GET /api/tarefas/`)
- Buscar uma tarefa por ID (`GET /api/tarefas/{id}/`)
- Atualizar uma tarefa (`PUT /api/tarefas/{id}/`)
- Excluir uma tarefa (`DELETE /api/tarefas/{id}/`)
- Filtrar tarefas por status (`GET /api/tarefas?status=pendente`)

## 🛠️ Tecnologias Utilizadas

- **Linguagem**: Python 3
- **Framework**: Django + Django Rest Framework (DRF)
- **Banco de Dados**: SQLite (padrão, mas pode ser alterado para PostgreSQL ou MySQL)
- **Ferramentas**: Postman/Insomnia para testes, GitHub para versionamento

## 🏗️ Como Instalar e Rodar o Projeto

### 1️⃣ Clonar o Repositório
```sh
git clone https://github.com/seu-usuario/django_restful_api.git
cd django_restful_api
```

### 2️⃣ Criar e Ativar o Ambiente Virtual
```sh
python -m venv venv
# Ativar no Windows:
venv\Scripts\Activate
# Ativar no macOS/Linux:
source venv/bin/activate
```

### 3️⃣ Instalar Dependências
```sh
pip install -r requirements.txt
```

### 4️⃣ Criar o Banco de Dados e Aplicar Migrações
```sh
python manage.py migrate
```

### 5️⃣ Criar um Superusuário (Opcional, para acessar o admin Django)
```sh
python manage.py createsuperuser
```

### 6️⃣ Rodar o Servidor
```sh
python manage.py runserver
```
Acesse a API em: [http://127.0.0.1:8000/api/tarefas/](http://127.0.0.1:8000/api/tarefas/)

## 🔄 Testando a API

### Criar uma Tarefa (POST)
```json
{
  "titulo": "Estudar Django",
  "descricao": "Criar uma API RESTful",
  "status": "pendente",
  "data_vencimento": "2024-12-31"
}
```

### Listar Todas as Tarefas (GET)
```sh
GET /api/tarefas/
```

### Buscar uma Tarefa por ID (GET)
```sh
GET /api/tarefas/1/
```

### Atualizar uma Tarefa (PUT)
```json
{
  "titulo": "Estudar Django Avançado",
  "descricao": "Explorar Django Rest Framework",
  "status": "realizando",
  "data_vencimento": "2024-12-30"
}
```

### Excluir uma Tarefa (DELETE)
```sh
DELETE /api/tarefas/1/
```

