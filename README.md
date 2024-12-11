# Odonto Clinic - Sistema de Gerenciamento de Clínica Odontológica

## Descrição
Odonto Clinic é um sistema completo de gerenciamento para clínicas odontológicas. Ele permite a gestão de pacientes, consultas, prestadores de serviço e fornecedores. O projeto foi desenvolvido com tecnologias web modernas, possui autenticação segura por JWT e pode ser implantado localmente ou em um servidor.

---

## Estrutura do Projeto

```
/odonto_clinic
|
├── /assets
│   ├── logo.png
│   └── user.jpg
│
├── /css
│   └── style.css
│
├── /js
│   └── main.js
│
├── /sql
│   └── odonto_clinic_db.sql
│
├── /controllers
│   ├── pacientes.php
│   ├── prestadores.php
│   ├── consultas.php
│   ├── fornecedores.php
│   └── login.php
│
├── config.php
├── auth.php
├── api.php
├── login.html
├── index.html
└── README.md
```

---

## Funcionalidades

- **Gerenciamento de Pacientes:**
  - Cadastro, edição, visualização e exclusão de pacientes.
- **Gerenciamento de Consultas:**
  - Agendamento, edição, visualização e cancelamento de consultas.
- **Gerenciamento de Prestadores:**
  - Controle de dados de profissionais, como nome, CRO e contato.
- **Gerenciamento de Fornecedores:**
  - Cadastro e consulta de fornecedores de materiais.
- **Autenticação:**
  - Login seguro com JWT (JSON Web Token).
- **Interface Intuitiva:**
  - Design responsivo e fácil de usar.

---

## Tecnologias Utilizadas

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- PHP (com PDO para acesso ao banco de dados)
- MySQL

### Outros
- JWT para autenticação
- XAMPP ou WAMP (para ambiente local)

---

## Requisitos

- Servidor local (XAMPP, WAMP ou similar)
- PHP >= 7.4
- MySQL >= 5.7
- Navegador atualizado (Google Chrome ou Firefox recomendado)

---

## Instalação

### 1. Configurar o Servidor Local

1. Instale o [XAMPP](https://www.apachefriends.org/) ou [WAMP](https://www.wampserver.com/).
2. Copie os arquivos do projeto para o diretório `htdocs` (no XAMPP) ou `www` (no WAMP).

### 2. Configurar o Banco de Dados

1. Abra o phpMyAdmin no seu navegador (exemplo: `http://localhost/phpmyadmin`).
2. Crie um banco de dados chamado `odonto_clinic_db`.
3. Importe o arquivo `odonto_clinic_db.sql` da pasta `/sql`.

### 3. Configurar o Projeto

1. Edite o arquivo `config.php` com as credenciais do seu banco de dados:
   ```php
   $host = 'localhost';
   $dbname = 'odonto_clinic_db';
   $username = 'root';
   $password = '';
   ```

### 4. Iniciar o Servidor

1. Inicie o servidor Apache e MySQL pelo painel do XAMPP ou WAMP.
2. Acesse `http://localhost/odonto_clinic/login.html` no navegador.

---

## Uso

1. **Tela de Login:**
   - Insira o nome de usuário e senha para acessar o sistema.
2. **Dashboard:**
   - Gerencie pacientes, consultas, prestadores e fornecedores.
3. **Logout:**
   - Encerre a sessão de maneira segura.

---

## API

O backend da aplicação possui uma API RESTful para integração com outras aplicações.

### Endpoints Principais

#### Autenticação

- **POST /login**
  - Realiza o login e retorna um token JWT.

#### Pacientes

- **GET /pacientes**: Retorna todos os pacientes.
- **GET /pacientes/{id}**: Retorna um paciente pelo ID.
- **POST /pacientes**: Cadastra um novo paciente.
- **PUT /pacientes/{id}**: Atualiza os dados de um paciente.
- **DELETE /pacientes/{id}**: Exclui um paciente.

#### Consultas

- **GET /consultas**: Retorna todas as consultas.
- **POST /consultas**: Cadastra uma nova consulta.

#### Prestadores

- **GET /prestadores**: Retorna todos os prestadores.
- **POST /prestadores**: Cadastra um novo prestador.

#### Fornecedores

- **GET /fornecedores**: Retorna todos os fornecedores.
- **POST /fornecedores**: Cadastra um novo fornecedor.

---

## Desenvolvimento

### 1. Clonar o Repositório
```bash
git clone https://github.com/usuario/odonto_clinic.git
```

### 2. Configurar o Ambiente
- Siga as etapas de instalação mencionadas acima.

### 3. Contribuições
- Crie um branch para sua contribuição:
  ```bash
  git checkout -b minha-contribuicao
  ```
- Envie um pull request para revisão.

---

## Suporte

Em caso de problemas ou dúvidas, entre em contato:
- **Email:** carlos@crdwebcode.com.br
- **Github Issues:** [https://github.com/crdwebcode/odonto_clinic_project/issues](https://github.com/crdwebcode/odonto_clinic_project/issues)

---

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

