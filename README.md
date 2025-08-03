# ⚡ PV Operation — Sistema Completo

Um sistema full stack para importação, processamento e visualização de dados da **ANEEL** usando:
- 🔹 **Backend:** Flask + MongoDB + Redis  
- 🔹 **Frontend:** React  
- 🔹 **Orquestração:** Docker Compose  

---

## 🚀 Como Rodar o Projeto

### 1️⃣ Clone este repositório (com submódulos)
```bash
git clone --recurse-submodules https://github.com/RafaelSteffens/PVOperation_Desafio.git
cd PVOperation_Desafio

⚠️ Se você já clonou sem --recurse-submodules:
git submodule update --init --recursive

2️⃣ Suba os containers
docker-compose up --build


3️⃣ Acesse no navegador
Frontend → http://localhost:3000

Backend (API) → http://localhost:5000

🗂 Estrutura do Projeto
PVOperation_Desafio/
│── BackendPVOperation/       # Flask + MongoDB + Redis
│── FrontendPVOperation/      # React
│── docker-compose.yml
│── README.md


📌 Funcionalidades
✅ Importação massiva de dados CSV da ANEEL
✅ Armazenamento otimizado em MongoDB
✅ Cache em Redis para respostas rápidas
✅ Interface responsiva e moderna em React
✅ Ambiente pronto via Docker Compose

👨‍💻 Autor
Rafael Steffens — LinkedIn