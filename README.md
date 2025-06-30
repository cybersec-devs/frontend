# 💻 Sistema de Hospital - FRONTEND - Projeto Prático

Atenção: 
Aplicação Backend está disponível em: <https://hospital-backend-yeq5.onrender.com/>
Aplicação FrontEnd está disponível em: <https://cybersec-devs.github.io/frontend/>

Caso queira executar na sua própria máquina, siga as orientações deste documento.
  

Este é o frontend desenvolvido para o sistema hospitalar. Ele permite realizar operações de **CRUD** (Criar, Ler, Atualizar e Deletar) para três entidades:

- 👨‍⚕️ Médicos  
- 🧑‍🤝‍🧑 Pacientes  
- 📅 Consultas  

Todo o sistema utiliza **HTML, JavaScript puro (Vanilla JS)** e **Bootstrap 5** para estilização.

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
├── medicos.html # Página CRUD de médicos
├── pacientes.html # Página CRUD de pacientes
├── consultas.html # Página CRUD de consultas
└── README.md # Este arquivo



---

## ⚙️ Configuração da API

Todas as páginas usam uma constante chamada `apiBaseUrl` para se comunicar com o backend:

```js
const apiBaseUrl = 'http://127.0.0.1:5000'; 
ou

const apiBaseUrl = 'https://hospital-backend-yeq5.onrender.com';



📌 Alterando a URL
Se a sua API estiver hospedada em outro local (como no Render, Railway, ou outro IP), basta alterar essa constante no topo de cada arquivo HTML:

Exemplo:


const apiBaseUrl = 'https://api-hospital.onrender.com'; // exemplo em produção


##  ▶️ Como Executar Localmente
Certifique-se de que o backend (Flask) esteja rodando na mesma máquina/local.

Dê duplo clique no index.html para abrir no navegador ou use uma extensão como o Live Server no VSCode para evitar problemas de CORS.

###  Clique em uma das opções:
- Médicos
- Pacientes
- Consultas

## ❗ Importante sobre o CORS
Para que o frontend consiga se comunicar com o backend corretamente:

O backend deve estar com CORS habilitado:


from flask_cors import CORS
CORS(app)


## 👨‍🏫 Desenvolvido por
Enrico Carrano
Glauber Ariel Magalhães
Gregorio Queiroz
Eduardo Silva
Welther Moraes




