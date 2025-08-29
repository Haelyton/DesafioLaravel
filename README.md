# Gerenciador de Tarefas - Laravel

Projeto de exemplo desenvolvido em **Laravel 12** para gerenciar tarefas, com CRUD completo (Criar, Listar, Editar, Excluir) usando **MVC, Eloquent e Blade Templates**.

---

## 📦 Tecnologias

- PHP 8.x
- Laravel 12.x
- MySQL
- Composer
- Bootstrap 5 (para interface)

---

## 🚀 Instalação

1. Clone o repositório:
```bash
git clone git@github.com:Haelyton/DesafioLaravel.git
cd DesafioLaravel
Instale as dependências do Laravel:

bash
Copiar código
composer install
Copie o arquivo de ambiente:

bash
Copiar código
cp .env.example .env
No Windows PowerShell:

powershell
Copiar código
copy .env.example .env
Configure o banco de dados no .env:

dotenv
Copiar código
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=gerenciador_tarefas
DB_USERNAME=root
DB_PASSWORD=
⚠️ Ajuste DB_DATABASE, DB_USERNAME e DB_PASSWORD de acordo com seu MySQL/XAMPP.

Gere a chave da aplicação:

bash
Copiar código
php artisan key:generate
Crie as tabelas no banco de dados:

bash
Copiar código
php artisan migrate
🎯 Como usar
Suba o servidor local:

bash
Copiar código
php artisan serve
Acesse no navegador:

arduino
Copiar código
http://127.0.0.1:8000/tarefas
Funcionalidades disponíveis:

Listar tarefas

Criar nova tarefa

Editar tarefa existente

Visualizar detalhes da tarefa

Excluir tarefa

🗂 Estrutura do projeto
bash
Copiar código
app/
 └── Models/Tarefa.php
app/Http/Controllers/TarefaController.php
resources/views/layout.blade.php
resources/views/tarefas/
    ├── index.blade.php
    ├── create.blade.php
    ├── edit.blade.php
    └── show.blade.php
routes/web.php
database/migrations/
    └── xxxx_xx_xx_create_tarefas_table.php
📌 Observações
Todas as views usam Blade Templates e Bootstrap 5.

O CRUD utiliza o ORM Eloquent do Laravel.

A página inicial (/) redireciona automaticamente para a lista de tarefas (/tarefas).
