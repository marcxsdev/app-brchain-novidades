# 🩺 Módulo de Novidades - App de Saúde

Este projeto é um módulo de **coleta e exibição de conteúdos sobre saúde**, desenvolvido como parte de um aplicativo mobile voltado ao bem-estar dos usuários. Ele utiliza **web scraping** para buscar informações em sites confiáveis e exibe essas novidades de forma categorizada e cronológica dentro do aplicativo.

---

## 🧠 Objetivo

Criar uma **aba de novidades** que:

- Coleta automaticamente conteúdos (notícias, dicas, artigos) sobre saúde
- Armazena os dados em um banco MySQL
- Exibe essas informações de forma organizada no app
- Permite atualizações periódicas das fontes

---

## ⚙️ Tecnologias Utilizadas

| Camada | Tecnologia |
|--------|------------|
| Scraping | Python, BeautifulSoup |
| Backend/API | Flask |
| Banco de Dados | MySQL |
| Mobile | Flutter |
| Comunicação | API REST |

---

## 📦 Estrutura do Projeto

```
app-saude-novidades/
│
├── backend/
│   ├── scraper/             # Scripts Python para web scraping
│   ├── api/                 # API Flask para servir os dados
│   └── requirements.txt     # Dependências Python
│
├── database/
│   └── estrutura.sql        # Script de criação do banco
│
├── mobile/
│   └── flutter_novidades/   # Projeto Flutter com aba de novidades
│
├── README.md                # Documentação do projeto
└── .gitignore               # Arquivos a serem ignorados pelo Git
```

---

## 🔐 Requisitos Funcionais

- ✅ Coletar dados de sites confiáveis sobre saúde (gov.br, OMS, etc.)
- ✅ Armazenar os dados em um banco de dados
- ✅ Exibir os dados na aba de novidades em ordem cronológica
- ✅ Atualizar os dados periodicamente
- ✅ Categorizar os conteúdos por tipo ou cor

---

## 📡 Como rodar o projeto

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/app-saude-novidades.git
cd app-saude-novidades
```

### 2. Instale as dependências do Python
```bash
cd backend
pip install -r requirements.txt
```

### 3. Configure o banco MySQL
- Crie o banco `saude_app`
- Execute o script `estrutura.sql` na pasta `/database`

### 4. Execute o scraper (opcional para testes)
```bash
cd scraper
python scraper.py
```

### 5. Rode a API Flask
```bash
cd api
python api.py
```

### 6. Rode o app Flutter
```bash
cd mobile/flutter_novidades
flutter pub get
flutter run
```

---

## 📁 API - Endpoints disponíveis

| Método | Rota | Descrição |
|--------|------|-----------|
| GET | `/novidades` | Retorna todas as novidades da base |

---

## 📄 Licença

Este projeto é acadêmico e está sob a licença MIT.
