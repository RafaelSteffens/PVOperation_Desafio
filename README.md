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

# 📌 Desafio Proposto

### Parte 1 – Backend (Python / Flask)
- Importar **CSV** e salvar em **MongoDB**.  
- Criar **API REST** com endpoints:
  - `/usinas`: listar empreendimentos (**paginação + filtros**).
  - `/estatisticas`: potência total por **estado** e **distribuidora**.  
- Utilizar **boas práticas em Python** e suportar **grandes volumes de dados**.

### Parte 2 – Frontend (React)
- Consumir a API do backend.  
- Exibir **tabela paginada** com filtros dinâmicos (*estado, município, distribuidora, titular*).  
- Criar **dashboard** com gráficos de **barras** e **pizza**.  
- Exibir **mapa interativo** com coordenadas dos empreendimentos.

### Parte 3 – Extra (DevOps)
- Criar **Dockerfile** para backend e frontend.  
- Configurar **docker-compose.yml** para rodar tudo junto.  
- Elaborar **README** com instruções de uso.


👨‍💻 Autor
Rafael Steffens — LinkedIn