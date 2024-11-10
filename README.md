# SpinMaster - Sistema de Ranking de Tênis de Mesa 🏓

![Versão](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow.svg)
![Licença](https://img.shields.io/badge/license-MIT-green.svg)

Sistema completo para gerenciamento de rankings e estatísticas de tênis de mesa, permitindo o acompanhamento de jogadores, partidas, torneios e evolução dos atletas.

## 🚀 Tecnologias Utilizadas

### Backend
- Python 3.11+
- FastAPI
- PostgreSQL
- Redis
- Docker

### Frontend
- React + TypeScript
- Next.js
- Material-UI
- Recharts

### Mobile
- React Native
- Expo

## 📋 Pré-requisitos

- Python 3.11+
- Node.js 18+
- Docker e Docker Compose
- PostgreSQL 14+
- Redis 6+

## 🔧 Configuração do Ambiente

1. **Clone o repositório**
```bash
git clone https://github.com/your-org/spinmaster-docs.git
cd spinmaster-docs
```

2. **Configure o ambiente virtual Python**
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
.\venv\Scripts\activate   # Windows
pip install -r requirements.txt
```

3. **Configure as variáveis de ambiente**
```bash
cp .env.example .env
# Edite o arquivo .env com suas configurações
```

4. **Inicie os serviços com Docker**
```bash
docker-compose up -d
```

5. **Execute as migrações do banco**
```bash
alembic upgrade head
```

6. **Inicie o servidor de desenvolvimento**
```bash
uvicorn app.main:app --reload
```

## 🏗️ Arquitetura

```
spinmaster/
├── backend/           # API e lógica de negócio
├── frontend/         # Interface web
├── mobile/           # Aplicativo móvel
└── docs/            # Documentação
```

## 📦 Estrutura do Projeto

### Backend
```
backend/
├── app/
│   ├── api/          # Endpoints da API
│   ├── core/         # Lógica de negócio
│   ├── db/           # Modelos e migrations
│   └── utils/        # Utilitários
├── tests/            # Testes
└── alembic/          # Migrações
```

### Frontend
```
frontend/
├── src/
│   ├── components/   # Componentes React
│   ├── pages/        # Páginas da aplicação
│   ├── hooks/        # Custom hooks
│   └── utils/        # Utilitários
└── public/           # Arquivos estáticos
```

## 🎯 Funcionalidades Principais

- Gestão completa de jogadores
- Sistema de ranking por categorias (F à A)
- Cálculo automático de ELO
- Organização de torneios
- Estatísticas detalhadas
- Dashboard analítico
- App mobile para registro rápido

## 🚀 Deploy

### Produção
```bash
docker-compose -f docker-compose.prod.yml up -d
```

### Staging
```bash
docker-compose -f docker-compose.staging.yml up -d
```

## 🧪 Testes

```bash
# Backend
pytest

# Frontend
npm test

# E2E
npm run cypress
```

## 📚 Documentação Adicional

- [Arquitetura Detalhada](./architecture/README.md)
- [API Reference](./api/README.md)
- [Guia de Contribuição](./CONTRIBUTING.md)
- [Changelog](./CHANGELOG.md)

## 🔐 Segurança

Para reportar vulnerabilidades de segurança, por favor envie um email para security@spinmaster.com

## 🤝 Contribuição

1. Fork o projeto
2. Crie sua branch (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add: amazing feature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🎯 Status do Projeto

- [x] Configuração inicial
- [x] Estrutura base
- [ ] MVP
- [ ] Beta
- [ ] Release 1.0

## 📊 Métricas do Projeto

![GitHub stars](https://img.shields.io/github/stars/your-org/spinmaster)
![GitHub forks](https://img.shields.io/github/forks/your-org/spinmaster)
![GitHub issues](https://img.shields.io/github/issues/your-org/spinmaster)

## 🤝 Time

- Tech Lead - [@techlead](https://github.com/techlead)
- Backend - [@backend](https://github.com/backend)
- Frontend - [@frontend](https://github.com/frontend)
- Mobile - [@mobile](https://github.com/mobile)

## 📞 Suporte

- Email: support@spinmaster.com
- Discord: [SpinMaster Community](https://discord.gg/spinmaster)
- Issues: [GitHub Issues](https://github.com/your-org/spinmaster/issues)

---
Desenvolvido com ❤️ pelo time SpinMaster
