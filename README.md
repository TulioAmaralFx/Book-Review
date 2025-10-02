Guia de Configuração e Inicialização do Projeto

Este projeto utiliza Laravel como framework e SQLite como banco de dados. Para configurar e iniciar o projeto, siga estes passos:

Passo 1: Clonar o Projeto

Clone o repositório do projeto para sua máquina local usando o Git:
```bash
git clone https://github.com/your-username/project-name.git
```
Passo 2: Instalar Dependências

Navegue até o diretório do projeto e instale as dependências necessárias usando o Composer:
```bash
composer install
```
Passo 3: Configurar Variáveis de Ambiente

Copie o arquivo .env.example para .env e atualize as configurações do banco de dados para usar SQLite:
```bash
cp .env.example .env
```
No arquivo .env, defina DB_CONNECTION como sqlite e DB_DATABASE como o caminho onde você deseja armazenar o arquivo do banco de dados SQLite.

Passo 4: Gerar a Chave da Aplicação

Gere uma nova chave de aplicação com o seguinte comando:
```bash
php artisan key:generate
```
Passo 5: Executar as Migrações

Execute as migrações para configurar o esquema do banco de dados:
```bash
php artisan migrate
```
Passo 6: Popular o Banco de Dados (Opcional)

Se quiser preencher o banco de dados com alguns dados iniciais, execute o seguinte comando:
```bash
php artisan db:seed
```
Passo 7: Iniciar o Servidor de Desenvolvimento

Inicie o servidor de desenvolvimento com o seguinte comando:
```bash
php artisan serve
```
Abra o navegador e acesse http://localhost:8000 para visualizar o projeto.

Pronto! Agora você deve ter o projeto configurado e rodando na sua máquina local.
