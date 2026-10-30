# manuten-o_celulares

# 📱 Sistema de Gerenciamento – Assistência Técnica de Celulares

<p align="center">
  **Sistema de controle de clientes, aparelhos e agendamentos de reparos**
</p>

---

## 📌 Sobre o projeto

O Sistema de Gerenciamento de Assistência Técnica de Celulares foi desenvolvido com o objetivo de informatizar e facilitar a rotina de uma assistência técnica.

A aplicação busca substituir os controles manuais por um sistema organizado, permitindo gerenciar clientes, registrar aparelhos, controlar agendamentos de reparos e proteger informações pessoais.

O projeto também considera as exigências da Lei Geral de Proteção de Dados (LGPD), implementando mecanismos de segurança para proteger os dados armazenados.

## 🎯 Objetivos

- Organizar os atendimentos da assistência técnica.
- Facilitar o cadastro e gerenciamento de clientes.
- Registrar aparelhos e seus respectivos defeitos.
- Controlar os agendamentos de reparos.
- Garantir a segurança das informações dos usuários.
- Reduzir erros, duplicidade de informações e perda de horários.

## ⚙️ Funcionalidades

### 🔐 1. Login e autenticação
- Autenticação por e-mail e senha.
- Validação das credenciais.
- Controle de sessão com tempo de expiração.
- Opção de sair do sistema.

### 👥 2. Gerenciamento de clientes
- Cadastro de clientes.
- Pesquisa por informações cadastradas.
- Edição de dados existentes.
- Proteção do CPF por criptografia.

### 📱 3. Gerenciamento de aparelhos
- Cadastro de marca e modelo.
- Registro do IMEI.
- Descrição do defeito relatado.
- Associação do aparelho a um cliente cadastrado.

### 📅 4. Gerenciamento de agendamentos
- Cadastro de agendamentos de reparos.
- Listagem organizada por data.
- Exibição dos dados do cliente e aparelho.
- Alteração da data de um agendamento.

### 🏠 5. Página principal
- Exibição do nome do usuário autenticado.
- Acesso aos módulos do sistema.
- Navegação entre as funcionalidades.
- Opção de encerramento da sessão.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Finalidade |
|---|---|
| Python | Linguagem de programação |
| MySQL | Sistema de gerenciamento de banco de dados |
| HTML | Estrutura das páginas |
| CSS | Estilização e layout |
| JavaScript | Interatividade |
| Flask | Desenvolvimento da aplicação web |

## 🗄️ Banco de dados

O banco de dados utilizado é o `assistencia_db`, responsável por armazenar as informações do sistema.

Principais tabelas:

- **usuarios:** armazena os dados de acesso dos usuários.
- **clientes:** armazena os dados dos clientes.
- **aparelhos:** registra os dispositivos recebidos para manutenção.
- **agendamentos:** armazena as datas e informações dos reparos.

Os relacionamentos entre as tabelas são estabelecidos por meio de chaves primárias e estrangeiras.

## 🔒 Segurança e LGPD

O sistema considera boas práticas de segurança da informação:

- Senhas armazenadas utilizando hash seguro.
- CPF armazenado de forma criptografada.
- Controle de acesso por autenticação.
- Expiração automática de sessões.
- Proteção das informações pessoais dos clientes.

## 📂 Estrutura do projeto

```text
assistencia-tecnica/
│
├── sistema/
│   ├── app.py
│   ├── autenticacao.py
│   ├── banco.py
│   ├── clientes.py
│   ├── aparelhos.py
│   ├── agendamentos.py
│   ├── templates/
│   └── static/
│
├── assistencia_db.sql
├── documentacao.pdf
├── der.png
└── README.md
```

*Estrutura de referência, que pode ser adaptada conforme a organização dos arquivos implementados.*

## 🚀 Como executar o projeto

### 1. Requisitos

- Python instalado.
- MySQL Server instalado.
- MySQL Workbench.
- Editor de código, como Visual Studio Code.

### 2. Criar o banco de dados

Abra o MySQL Workbench e execute o arquivo:

```text
assistencia_db.sql
```

### 3. Instalar as dependências

No terminal, dentro da pasta do projeto, execute:

```bash
pip install flask mysql-connector-python bcrypt cryptography
```

### 4. Configurar a conexão

Configure as credenciais de acesso ao MySQL no arquivo responsável pela conexão com o banco de dados.

### 5. Executar o sistema

Na pasta do projeto, execute:

```bash
python app.py
```

Acesse no navegador o endereço local configurado pela aplicação.

## 👨‍💻 Desenvolvedor

**Nome:** SEU NOME COMPLETO

**Curso:** Técnico em Desenvolvimento de Sistemas

**Instituição:** SENAI

## 📚 Considerações finais

O projeto tem como finalidade desenvolver uma solução informatizada para melhorar a organização e a eficiência dos serviços de uma assistência técnica de celulares.

Por meio da integração entre autenticação, gerenciamento de clientes
