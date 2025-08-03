# ⚡ PV Operation — Sistema Completo

Este projeto foi desenvolvido como parte do **Desafio Fullstack – Usinas Fotovoltaicas (ANEEL)** para a vaga de **Desenvolvedor(a) Fullstack**.  
O objetivo é demonstrar competências práticas em **Python (Flask)**, **React**, **APIs REST**, **MongoDB**, **Redis** e **Docker**, entregando uma aplicação completa para importação, processamento e análise de dados de usinas fotovoltaicas da ANEEL (~1.3GB).  
O projeto contempla **integração entre frontend e backend**, **modelagem de dados**, **consumo de APIs**, **filtros dinâmicos**, **gráficos interativos** e **mapas georreferenciados**, alinhado aos requisitos técnicos da vaga.

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
✅ Importação massiva de dados CSV (~1.3GB) da ANEEL
✅ Armazenamento otimizado em MongoDB
✅ Cache em Redis para respostas rápidas
✅ API REST em Flask com filtros dinâmicos
✅ Tabela paginada e responsiva no Frontend React
✅ Gráficos interativos (potência por estado, usinas por distribuidora)
✅ Mapa georreferenciado das usinas (Leaflet)
✅ Orquestração completa via Docker Compose

📌 Desafio Proposto
Parte 1 – Backend (Python / Flask)

Importar CSV e salvar em MongoDB.

API REST com endpoints:

/usinas: listar empreendimentos (paginações + filtros).

/estatisticas: potência total por estado e distribuidora.

Boas práticas em Python e manipulação de grandes volumes de dados.

Parte 2 – Frontend (React)

Consumir API do backend.

Tabela paginada com filtros dinâmicos (estado, município, distribuidora, titular).

Dashboard com gráficos (barras e pizza).

Mapa interativo com coordenadas dos empreendimentos.

Parte 3 – Extra (DevOps)

Dockerfile para backend e frontend.

docker-compose.yml para rodar tudo junto.

README com instruções.

👨‍💻 Autor
Rafael Steffens — LinkedIn