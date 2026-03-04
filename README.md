# Support Ticket API

API to manage technical support tickets, allowing the creation of a support request ticket, updating ticket information, listing tickets with status filtering, and updating a ticket status to closed.

## Project Description
This project was developed during Node.js studies to understand the core of the technology without the use of high-level frameworks like Express. It focuses on the use of native modules to handle HTTP requests, data streams, and file system persistence.

## Features
- Create Ticket: Generates a new support request with equipment, description, and username.
- List Tickets: Retrieves all tickets from the database with optional filtering by status (open/closed).
- Update Ticket: Allows modification of equipment and description for an existing ticket.
- Update Status: Specifically updates the status to closed and adds a solution description.
- Delete Ticket: Removes a ticket record from the system.

## Technologies Used
- Node.js: Runtime environment.
- Native HTTP Module: Server creation and request handling.
- File System (fs/promises): To persist data in a JSON file (db.json).
- Crypto: To generate unique identifiers (UUID).
- Regex: For dynamic route handling and parameter extraction.

## API Endpoints
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| POST | /tickets | Create a new ticket |
| GET | /tickets | List all tickets (Optional: ?status=open) |
| PUT | /tickets/:id | Update ticket information |
| PATCH | /tickets/:id/close | Close a ticket and add a solution |
| DELETE | /tickets/:id | Remove a ticket |

---

# API Support Ticket (Versão em Português)

API para gerenciar ticket de suporte técnico, permitindo criar um ticket solicitando suporte, atualizar as informações do ticket, listar os tickets podendo filtrar pelo status e atualizar o status de um ticket para fechado.

## Descrição do Projeto
Este projeto foi desenvolvido durante os estudos de Node.js para compreender o núcleo da tecnologia sem o uso de frameworks de alto nível como o Express. O foco está no uso de módulos nativos para lidar com requisições HTTP, fluxos de dados e persistência em sistema de arquivos.

## Funcionalidades
- Criar Ticket: Gera uma nova solicitação de suporte com equipamento, descrição e nome de usuário.
- Listar Tickets: Recupera todos os tickets do banco de dados com filtragem opcional por status (aberto/fechado).
- Atualizar Ticket: Permite a modificação do equipamento e descrição de um ticket existente.
- Atualizar Status: Atualiza especificamente o status para fechado e adiciona a descrição da solução.
- Remover Ticket: Exclui o registro de um ticket do sistema.

## Tecnologias Utilizadas
- Node.js: Ambiente de execução.
- Módulo HTTP Nativo: Para criação do servidor e manipulação de requisições.
- File System (fs/promises): Para persistir dados em um arquivo JSON (db.json).
- Crypto: Para geração de identificadores únicos (UUID).
- Regex: Para manipulação de rotas dinâmicas e extração de parâmetros.

## Rotas da API
| Método | Rota | Descrição |
| :--- | :--- | :--- |
| POST | /tickets | Cria um novo ticket |
| GET | /tickets | Lista todos os tickets (Opcional: ?status=open) |
| PUT | /tickets/:id | Atualiza informações do ticket |
| PATCH | /tickets/:id/close | Fecha um ticket e adiciona a solução |
| DELETE | /tickets/:id | Remove um ticket |