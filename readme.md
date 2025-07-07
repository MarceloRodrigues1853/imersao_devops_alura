# 🚀 Imersão DevOps - Alura Google Cloud

![GitHub repo size](https://img.shields.io/github/repo-size/MarceloRodrigues1853/imersao_decops_alura)
![GitHub last commit](https://img.shields.io/github/last-commit/MarceloRodrigues1853/imersao_decops_alura)
![Python version](https://img.shields.io/badge/python-3.10%2B-blue)
![Cloud Run](https://img.shields.io/badge/Cloud_Run-Deployed-brightgreen)

Este projeto que faz parte da Imersão DevOps da Alura, é uma API desenvolvida com **FastAPI** para gerenciar **alunos, cursos e matrículas** de uma instituição de ensino.

---

## ✅ Execução realizada por mim

Abaixo estão os registros que comprovam a execução e deploy pessoal do projeto:

### 1️⃣ Autenticação no Google Cloud e ativação de APIs
![Autenticação Google Cloud](imgs_ex/imersao_ex1.PNG)

### 2️⃣ Fazendo teste de Restrito na API
![teste de resgito na API](imgs_ex/imersao_ex2.PNG)

### 3️⃣ Deploy da API via Cloud Run
![Deploy Cloud Run](imgs_ex/imersao_ex3.PNG)
---

## ⚙️ Pré-requisitos

- [Python 3.10+](https://www.python.org/downloads/)
- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/)

---

## 🛠️ Executando o projeto localmente

```bash
# Criar ambiente virtual
python3 -m venv venv

# Ativar ambiente virtual
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows

# Instalar dependências
pip install -r requirements.txt

# Executar aplicação
uvicorn app:app --reload
Acesse a documentação interativa: 👉 http://127.0.0.1:8000/docs

````
---

## 🚀 Deploy na Nuvem (Google Cloud)
````bash
gcloud auth login
gcloud config set project alura-imersao-465123
gcloud run deploy --port=8000
````
---

## 🌐 API publicada
A API está hospedada via Google Cloud Run: 
🔗 [imersao-app](https://imersaoo-app-935614443201.southamerica-east1.run.app/docs)

---

## 🔎 Exemplo de resposta do endpoint /alunos
````json
[
  {
    "nome": "Marcelo Rodrigues",
    "email": "marcelo@example.com",
    "telefone": "51999990000"
  }
]
````
---

## 📁 Estrutura do Projeto
````css
imersao-devops-main/
├── app.py
├── database.py
├── models.py
├── routers/
│   ├── alunos.py
│   ├── cursos.py
│   └── matriculas.py
├── schemas.py
├── escola.db
├── Dockerfile
├── requirements.txt
├── .gitignore
├── .dockerignore
├── imgs_ex/
│   ├── imersao_ex1.PNG
│   ├── imersao_ex2.PNG
│   └── imersao_ex3.PNG
└── README.md 

````
---
## 📄 Licença
Este projeto está sob a licença MIT.
