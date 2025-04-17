# 🩺 App Saúde - Módulo de Novidades

Este projeto é um módulo de um aplicativo de saúde focado em exibir **notícias, dicas e artigos** atualizados e categorizados. Ele utiliza **Web Scraping com Python**, uma **API Flask**, e um **aplicativo mobile com Flutter** para entregar uma experiência rica e informativa ao usuário.

## 📚 Objetivo

- Coletar dados de fontes confiáveis sobre saúde (como Ministério da Saúde, OMS, etc.);
- Armazenar os dados coletados;
- Exibir os dados de forma cronológica e categorizada no app;
- Atualizar automaticamente as novidades (ex: a cada 12h ou 24h).

---

## 🧪 Tecnologias Utilizadas

| Tecnologia     | Descrição                                   |
|----------------|---------------------------------------------|
| Python         | Web scraping com BeautifulSoup, Scrapy etc. |
| Flask          | API REST para servir os dados               |
| MySQL          | Banco de dados para armazenar os conteúdos  |
| Flutter        | Aplicativo mobile (iOS e Android)           |
| Git/GitHub     | Controle de versão                          |

---

## 📁 Estrutura de Pastas

```
app-saude-novidades/
├── backend/
│
├── scraper/              # Scripts Python de web scraping
│   └── .gitkeep
│
├── api/                  # API Flask para servir os dados
│   └── .gitkeep
│
├── database/
│   ├── estrutura.sql     # Script SQL para criação do banco
│   └── .gitkeep
│
├── mobile/
│   └── flutter_novidades/ # Projeto Flutter
│       └── .gitkeep
│
├── requirements.txt      # Dependências Python
├── README.md             # Este arquivo
└── .gitignore
```

---

## 🚀 Como Executar

### 🔧 1. Clonar o repositório

```bash
git clone https://github.com/marcxsdev/app-saude-novidades.git
cd app-saude-novidades
```

### 🐍 2. Instalar dependências do Python

```bash
cd scraper
pip install -r ../requirements.txt
```

### 🛠️ 3. Rodar a API

```bash
cd ../api
python app.py
```

### 📱 4. Rodar o app Flutter

```bash
cd ../mobile/flutter_novidades
flutter pub get
flutter run
```

---

## 🔖 Categorias de conteúdo

- ✅ **Notícias** – tag verde
- 💡 **Dicas de Saúde** – tag azul
- 📚 **Artigos Científicos** – tag laranja

---

## 👨‍💻 Branches

| Branch                | Descrição                      |
|-----------------------|-------------------------------|
| `main`                | Versão estável                |
| `develop`             | Desenvolvimento geral         |
| `feature/backend-scraper`  | Web scraping com Python       |
| `feature/api-flask`        | API REST com Flask           |
| `feature/flutter-novidades`| App mobile com aba de novidades |

---

## 🧠 Requisitos (Resumo)

### Requisitos Funcionais

- Coleta de dados via web scraping
- Armazenamento em banco de dados
- Exibição ordenada e categorizada no app
- Atualização periódica


## 📌 Licença

Este projeto é de uso educacional e sem fins lucrativos. Consulte a instituição responsável para mais detalhes.