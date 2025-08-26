# 🎮 Tap Game - Código do Road to Meridian

> **Código fonte do workshop Stellar - React, Python, Rust**

Este repositório contém o **código fonte** do workshop **"Road to Meridian"** da NearX. Para documentação completa, slides, roteiros e recursos adicionais, consulte o [repositório principal](https://github.com/danielgorgonha/road-to-meridian).

## 🎯 Sobre o Road to Meridian

**Meridian** é o maior evento global da Stellar, combinando hackathon + conferência. O evento acontecerá nos dias **17-18 de setembro de 2025** no **Copacabana Palace, Rio de Janeiro**.

## 📚 Estrutura do Workshop

### **Contratos Inteligentes**
- **Localização**: `web3/`
- **Tecnologias**: Rust + Soroban
- **Abordagem**: **Compartilhado** - usado por ambas as aulas seguintes
- **Objetivo**: Lógica de negócio na blockchain

### **Frontend Descentralizado**
- **Localização**: `frontend/`
- **Tecnologias**: React + TypeScript + Stellar SDK
- **Abordagem**: **Descentralizada** - frontend se conecta diretamente aos contratos
- **Objetivo**: Criar interface do usuário que interage diretamente com a blockchain

### **Backend Educacional**
- **Localização**: `backend/`
- **Tecnologias**: Python + Stellar SDK
- **Abordagem**: **Demonstração** - mostra as mesmas operações em Python
- **Objetivo**: Entender como fazer as mesmas operações usando Python

## 🏗️ Arquitetura do Projeto

```
nearx-tap-game/
├── frontend/          # 🎯 Aula 2: React + Stellar SDK
│   ├── src/
│   │   ├── blockchain/    # Hooks para interação com Stellar
│   │   ├── components/    # Componentes React do jogo
│   │   └── App.tsx        # Aplicação principal
│   └── README.md          # Documentação do frontend
├── backend/           # 🐍 Aula 3: Python + Stellar SDK
│   ├── contract/      # Operações com contratos Soroban
│   │   ├── old/       # Métodos tradicionais
│   │   └── new/       # ContractClient (recomendado)
│   ├── wallet/        # Operações de wallet
│   ├── tx/            # Transações Stellar
│   ├── main.py        # Script principal
│   └── README.md      # Documentação do backend
├── web3/              # 🔧 Aula 1: Contratos Rust + Soroban
│   ├── contracts/
│   │   └── tap-game/  # Contrato do jogo
│   └── README.md      # Documentação dos contratos
└── README.md          # Este arquivo
```

## 🎯 Funcionalidades do Jogo

### **Contratos (Rust + Soroban)**
- ✅ Inicialização do ranking
- ✅ Criação de novos jogos
- ✅ Consulta do ranking de pontuações

### **Frontend (React + Stellar SDK)**
- ✅ Interface do usuário 8-bit
- ✅ Conexão com wallet Stellar
- ✅ Interação direta com contratos
- ✅ Sistema de pontuação em tempo real

### **Backend (Python + Stellar SDK)**
- ✅ Operações de wallet
- ✅ Criação de contas
- ✅ Pagamentos XLM
- ✅ Invocação de contratos Soroban
- ✅ Logging detalhado

## 🔄 Fluxo de Aprendizado

### **Contratos Inteligentes**
1. **Desenvolve** contratos em Rust
2. **Testa** funcionalidades
3. **Deploy** na blockchain
4. **Prepara** base para frontend/backend

### **Frontend Descentralizado**
1. **Conecta wallet** Stellar
2. **Joga** o Tap Game (10 segundos)
3. **Salva pontuação** diretamente no contrato
4. **Visualiza ranking** em tempo real

### **Backend Educacional**
1. **Executa scripts** Python
2. **Demonstra** as mesmas operações
3. **Mostra logs** detalhados do processo
4. **Compara** com implementação frontend

## 🚀 Como Executar

### **Aula 1: Contratos**
```bash
cd web3
cargo build
stellar contract build
stellar contract deploy --wasm target/wasm32-unknown-unknown/release/tap_game.wasm --source alice --network testnet
```

### **Aula 2: Frontend**
```bash
cd frontend
npm install
npm run dev
# Acesse: http://localhost:5173
```

### **Aula 3: Backend**
```bash
cd backend
pip install -r requirements.txt
python main.py
```

## 🎮 Projeto: Tap Game

Jogo de cliques onde o usuário tem 10 segundos para clicar o máximo possível. A pontuação é salva na blockchain Stellar e exibida em um ranking global.

### **Funcionalidades**
- ✅ Jogo de cliques com timer
- ✅ Ranking salvo na blockchain
- ✅ Interface 8-bit minimalista
- ✅ Conexão com wallet Stellar
- ✅ Operações backend em Python

## 🛠️ Tecnologias

### **Blockchain**
- **Stellar Network**: Rede blockchain principal
- **Soroban**: Plataforma de contratos inteligentes
- **Stellar SDK**: SDK oficial para integração

### **Frontend**
- **React 18**: Framework JavaScript
- **TypeScript**: Tipagem estática
- **Vite**: Build tool
- **Tailwind CSS**: Estilização
- **Shadcn/ui**: Componentes UI

### **Backend**
- **Python**: Linguagem principal
- **Stellar SDK**: Integração com blockchain
- **Coloredlogs**: Logging colorido

### **Contratos**
- **Rust**: Linguagem dos contratos
- **Soroban SDK**: SDK para contratos inteligentes

## 🎓 Conceitos Aprendidos

### **Smart Contracts**
- Desenvolvimento em Rust
- Deploy na blockchain
- Invocação de funções
- Gerenciamento de estado

### **Web3 Frontend**
- Integração direta com blockchain
- Gerenciamento de transações
- UX para aplicações descentralizadas
- Conexão com wallets

### **Web3 Backend**
- Operações blockchain via Python
- Logging e monitoramento
- Tratamento de erros
- Demonstração educacional

## 📖 Documentação Completa

Para documentação completa do workshop, incluindo:
- Slides das aulas
- Roteiros detalhados
- Conceitos teóricos
- Recursos adicionais
- Desafios e exercícios

Consulte o **[repositório principal do Road to Meridian](https://github.com/danielgorgonha/road-to-meridian)**.

## 🏆 Hackathon Meridian

### **Evento**
- **Local**: Copacabana Palace, Rio de Janeiro
- **Data**: 17-18 de setembro de 2025
- **Tipo**: Hackathon + Conferência
- **Organização**: Stellar Foundation

### **Preparação**
Este workshop prepara você para:
- ✅ Desenvolvimento completo de DApps Stellar
- ✅ Integração frontend/backend
- ✅ Smart contracts em Rust
- ✅ Operações avançadas de blockchain

## 🔗 Links Úteis

- **[Road to Meridian - Repositório Principal](https://github.com/danielgorgonha/road-to-meridian)**
- **Stellar Documentation**: https://developers.stellar.org/
- **Soroban Documentation**: https://soroban.stellar.org/
- **Stellar SDK Python**: https://stellar-sdk.readthedocs.io/
- **Stellar SDK JavaScript**: https://stellar.github.io/js-stellar-sdk/

---

**Código fonte do Road to Meridian - NearX**  
*Preparando desenvolvedores para o Hackathon Meridian 2025*
