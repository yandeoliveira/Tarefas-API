# Tarefas API

Esta é uma API desenvolvida em Python usando FastAPI para a criação, exclusão e gerenciamento de tarefas. A API permite que os usuários criem, leiam, atualizem e excluam tarefas de forma simples e eficiente.

## Funcionalidades

- **Criar Tarefa**: Adicione uma nova tarefa ao banco de dados.
- **Ler Tarefas**: Recupere uma lista de todas as tarefas ou uma tarefa específica.
- **Atualizar Tarefa**: Modifique os detalhes de uma tarefa existente.
- **Deletar Tarefa**: Remova uma tarefa do banco de dados.

## Tecnologias Utilizadas

- [FastAPI](https://fastapi.tiangolo.com/)
- [SQLAlchemy](https://www.sqlalchemy.org/)
- [SQLite](https://www.sqlite.org/index.html) (banco de dados)

## Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/Tarefas_API.git
   cd Tarefas_API
Crie um ambiente virtual e ative-o:
```
python -m venv venv
source venv/bin/activate  # Para Linux/Mac
venv\Scripts\activate  # Para Windows
```
Instale as dependências:

```
pip install fastapi[all] sqlalchemy
```
## Uso
Execute a aplicação:

```
uvicorn main:app --reload
```
Acesse a documentação interativa da API em http://localhost:8000/docs.

## Endpoints

**Criar Tarefa**      

- **Método:** POST
- **URL:** /tasks/

Corpo da Requisição:
```
{
  "title": "Título da Tarefa",
  "description": "Descrição da Tarefa"
}
```
**Ler Todas as Tarefas**

- **Método:** GET
- **URL:** /tasks/
- **Parâmetros:**
   - **skip:** Número de tarefas a serem puladas (opcional).
   - **limit:** Número máximo de tarefas a serem retornadas (opcional).

**Ler Tarefa Específica**

- **Método:** GET
- **URL:** /tasks/{task_id}

**Atualizar Tarefa**

- **Método:** PUT
- **URL:** /tasks/{task_id}
  
Corpo da Requisição:

```
{
  "title": "Novo Título",
  "description": "Nova Descrição"
}
```
**Deletar Tarefa**

- **Método:** DELETE
- **URL:** /tasks/{task_id}
  
## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir um problema ou enviar um pull request.

## Licença
Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE para mais detalhes.

## Contato
Para mais informações entre em contato [yansantos2410@gmail.com]
Desenvolvedor: Yan de Oliveira

## Informações adicionais
Código fonte do aplicativo e executavel se encontram em outra branch do repositório.


