# FincAi

Aplicação full stack de inteligência financeira para gestão, previsões e recomendações de orçamento pessoal.

## Descrição

O FincAi é um projeto pensado para ajudar pessoas e pequenas empresas a organizar finanças, controlar receitas e despesas, acompanhar metas e receber recomendações de equilíbrio financeiro com base em dados e regras de negócio.

A proposta da aplicação é unificar gestão financeira, análise de comportamento de gastos e apoio à tomada de decisão em um único ambiente, com foco em usabilidade, organização e clareza na apresentação dos dados.

## Objetivo

Criar uma solução prática para gestão financeira pessoal, combinando front-end, back-end, banco de dados e lógica de análise para melhorar a tomada de decisão sobre orçamento, previsões e controle de despesas.

## Stack

- PHP 8.x
- Laravel
- MySQL / MariaDB
- HTML / CSS / JavaScript
- Bootstrap ou Blade (conforme configuração do projeto)
- Composer
- Git / GitHub

## Funcionalidades

- Cadastro de receitas e despesas
- Organização por categorias
- Controle do saldo e orçamento mensal
- Visualização geral do fluxo financeiro
- Histórico de movimentações
- Sugestões e previsões de gastos
- Estrutura de aplicação full stack
- Organização do código para facilitar manutenção e evolução

## Demonstração

A aplicação pode ser usada localmente em ambiente de desenvolvimento para testar as funcionalidades de cadastro, listagem e análise financeira.

Se houver imagens, GIFs ou um link de deploy, adicione aqui:

- Preview local: `http://localhost`
- Demo em produção: em breve

## Requisitos do ambiente

Antes de começar, certifique-se de ter instalado:

- PHP >= 8.1
- Composer
- Node.js e npm (se o projeto utilizar assets frontend)
- MySQL ou MariaDB
- Git

## Como executar

### 1. Clone o repositório

```bash
git clone https://github.com/LuisFer3251/FincAi.git
cd FincAi
```

### 2. Instale as dependências

```bash
composer install
npm install
```

Se o projeto não utilizar assets front-end, você pode ignorar o passo de `npm install`.

### 3. Configure o ambiente

Copie o arquivo de exemplo:

```bash
cp .env.example .env
```

Edite o arquivo `.env` com as configurações do banco e da aplicação:

```env
APP_NAME="FincAi"
APP_ENV=local
APP_KEY=
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=fincai
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Gere a chave da aplicação

```bash
php artisan key:generate
```

### 5. Execute as migrations

```bash
php artisan migrate
```

Se o projeto tiver seeders para dados de exemplo:

```bash
php artisan db:seed
```

### 6. Inicie a aplicação

```bash
php artisan serve
```

A aplicação ficará disponível em:

```text
http://localhost:8000
```

Se houver build do frontend, rode também:

```bash
npm run dev
```

## Estrutura do projeto

```text
FincAi/
├── app/
├── bootstrap/
├── config/
├── database/
├── public/
├── resources/
├── routes/
├── storage/
├── tests/
├── .env.example
├── composer.json
├── package.json
├── phpunit.xml
├── README.md
└── server.php
```

## Arquitetura

- Front-end: interface da aplicação e interação com o usuário
- Back-end: regras de negócio e lógica da aplicação
- Banco de dados: persistência dos dados financeiros
- Organização: estrutura modular para facilitar manutenç��o da aplicação

## Roadmap

- [ ] Melhorar autenticação e perfis de usuário
- [ ] Adicionar relatórios financeiros mais detalhados
- [ ] Implementar previsões de orçamento com regras inteligentes
- [ ] Melhorar a experiência visual e responsividade
- [ ] Adicionar testes automatizados
- [ ] Preparar deploy em ambiente de produção

## Contribuição

Contribuições são bem-vindas. Para colaborar:

1. Faça um fork do projeto
2. Crie uma branch para sua funcionalidade
3. Faça commit das mudanças
4. Abra um pull request com uma descrição clara

## Status

Projeto em desenvolvimento com foco em evolução funcional, organização da estrutura e melhoria da experiência do usuário.

## Autor

Luis Fernando

## Licença

Este projeto está disponível sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Observação

Este repositório representa uma visão prática de desenvolvimento full stack com foco em aplicações reais de gestão financeira, organização pessoal e análise de comportamento de gastos.
