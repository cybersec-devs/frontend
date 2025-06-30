# 💻 Sistema de Hospital - FRONTEND - Projeto Prático

Este é o frontend desenvolvido para o sistema hospitalar. Ele permite realizar operações de **CRUD** (Criar, Ler, Atualizar e Deletar) para três entidades:

- 👨‍⚕️ Médicos  
- 🧑‍🤝‍🧑 Pacientes  
- 📅 Consultas  

Todo o sistema utiliza **HTML, JavaScript puro (Vanilla JS)** e **Bootstrap 5** para estilização.

---
## Integrantes

- Enrico Carrano  
- Glauber Ariel Magalhães  
- Gregorio Queiroz  
- Eduardo Silva  
- Welther Moraes  

---

## ✅ Requisitos Funcionais (RF)

- **RF001** - Permitir o cadastro de médicos com nome, especialidade e CRM.  
- **RF002** - Permitir o cadastro de pacientes vinculados a um médico.  
- **RF003** - Permitir o cadastro de consultas vinculadas a um paciente, informando data, horário e descrição.  
- **RF004** - Listar todos os médicos cadastrados.  
- **RF005** - Listar todos os pacientes de um médico específico.  
- **RF006** - Listar todas as consultas de um paciente específico.  
- **RF007** - Permitir atualizar os dados de médicos, pacientes e consultas.  
- **RF008** - Permitir excluir médicos, pacientes e consultas.  

---

## ✅ Requisitos Não Funcionais (RNF)

- **RNF001** - Utilizar arquitetura RESTful.  
- **RNF002** - Utilizar banco de dados relacional (ex: PostgreSQL, MySQL, SQLite).  
- **RNF003** - Garantir integridade referencial entre médicos, pacientes e consultas.  
- **RNF004** - Respostas da API em formato JSON.  

---

## ✅ Diagrama de Classes

![Diagrama UML](Classe%20UML.png)

**Relacionamentos:**

- **Médico 1:N Paciente** (um médico pode ter vários pacientes)  
- **Paciente 1:N Consulta** (um paciente pode ter várias consultas)  

---

## ✅ Funcionalidades

- Visualização de registros
- Cadastro com validação
- Atualização e exclusão de dados com confirmação
- Integração via API RESTful com backend Flask

---

## 📁 Estrutura de Arquivos
frontend/
│
├── index.html # Página principal (menu de acesso)
├── medicos/ # Página CRUD de médicos
├── pacientes/ # Página CRUD de pacientes
├── consultas/ # Página CRUD de consultas
└── README.md # Este arquivo

---

## ⚙️ Configuração da API

Todas as páginas usam uma constante chamada **`apiBaseUrl`** para se comunicar com o backend.

### Ambiente Local
```js
const apiBaseUrl = 'http://127.0.0.1:5000'; 
```

### Ambiente de Produção
```js
const apiBaseUrl = 'https://hospital-backend-yeq5.onrender.com';
```

📌 Alterando a URL
Se a sua API estiver hospedada em outro local (como no Render, Railway, ou outro IP), basta alterar essa constante no topo de cada arquivo HTML:


##  ▶️ Como Executar Localmente
Certifique-se de que o backend (Flask) esteja rodando na mesma máquina/local.

Dê duplo clique no index.html para abrir no navegador ou use uma extensão como o Live Server no VSCode para evitar problemas de CORS.

###  Clique em uma das opções do menu:
- Médicos
- Pacientes
- Consultas

## ❗ Importante sobre o CORS
Para que o frontend consiga se comunicar com o backend corretamente:
- O backend deve estar com CORS habilitado:

```python
from flask_cors import CORS
CORS(app)
```

---

**Atenção - Visitar o Projeto em Produção**: 

- Aplicação Backend está disponível em: <https://hospital-backend-yeq5.onrender.com/>
- Aplicação FrontEnd está disponível em: <https://cybersec-devs.github.io/frontend/>


Caso queira executar na sua própria máquina, siga as orientações deste documento.