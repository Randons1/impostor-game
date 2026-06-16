<p align="center">
  <img src="public/logo.png" alt="Logo Descubra o Impostor" height="120">
</p>

<h1 align="center">Descubra o Impostor</h1>

<p align="center">
  Um jogo multiplayer local de dedução, blefe e criatividade desenvolvido com React.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-000?style=for-the-badge&logo=react&logoColor=61DAFB">
  <img src="https://img.shields.io/badge/JavaScript-000?style=for-the-badge&logo=javascript&logoColor=F7DF1E">
  <img src="https://img.shields.io/badge/CSS3-000?style=for-the-badge&logo=css&logoColor=1572B6">
  <img src="https://img.shields.io/badge/Docker-000?style=for-the-badge&logo=docker&logoColor=2496ED">
  <img src="https://img.shields.io/badge/licença-MIT-000?style=for-the-badge">
</p>

---

## 📌 Sobre o projeto

**Descubra o Impostor** é um jogo multiplayer local desenvolvido em React, criado para ser jogado com amigos usando o mesmo dispositivo.

Durante cada rodada, a maioria dos jogadores recebe a mesma pergunta — mas um deles recebe uma pergunta parecida, porém diferente. Esse jogador é o **impostor**.

O desafio dos jogadores normais é analisar as respostas e descobrir quem está tentando se misturar ao grupo. Já o impostor precisa responder de forma convincente para não ser descoberto.

Ideal para encontros, festas ou qualquer momento que peça um jogo de dedução, blefe e criatividade.

---

## 📸 Screenshots

<div align="center">

### 🌑 Tema Escuro

|                           Mobile                            |                           Desktop                            |
| :---------------------------------------------------------: | :----------------------------------------------------------: |
|  <img src="screenshots/mobile-dark-setup.png" width="200">  |  <img src="screenshots/desktop-dark-setup.png" width="780">  |
| <img src="screenshots/mobile-dark-players.png" width="200"> | <img src="screenshots/desktop-dark-players.png" width="780"> |

### ☀️ Tema Claro

|                            Mobile                            |                            Desktop                            |
| :----------------------------------------------------------: | :-----------------------------------------------------------: |
|  <img src="screenshots/mobile-light-setup.png" width="200">  |  <img src="screenshots/desktop-light-setup.png" width="780">  |
| <img src="screenshots/mobile-light-players.png" width="200"> | <img src="screenshots/desktop-light-players.png" width="780"> |

## </div>

## 🎯 Objetivo do jogo

**Jogadores normais** — observar as respostas exibidas na rodada e identificar quem recebeu uma pergunta diferente.

**Impostor** — disfarçar sua resposta e parecer que recebeu a mesma pergunta dos demais.

---

## 🕹️ Como funciona

1. Os jogadores definem a quantidade de participantes e informam seus nomes
2. O jogo sorteia automaticamente quem será o impostor e qual pergunta será usada
3. Cada jogador visualiza sua pergunta individualmente na tela
4. Todos respondem sem revelar qual pergunta receberam
5. As respostas aparecem embaralhadas e de forma anônima
6. Os jogadores votam em quem acreditam ser o impostor
7. O resultado final revela o impostor e exibe os votos recebidos

---

## ✨ Funcionalidades

- Sorteio automático do impostor e das perguntas a cada rodada
- Tela individual por jogador para visualizar a pergunta e enviar a resposta
- Respostas exibidas de forma anônima e embaralhada
- Sistema de votação entre os jogadores
- Tela de resultado com revelação do impostor e placar de votos
- Timer opcional por rodada
- Tema escuro como padrão, com suporte a tema claro
- Interface responsiva

---

## 🚀 Como rodar localmente

**Pré-requisitos:** Node.js 18+

```bash
git clone https://github.com/VitorNorton/impostor-game
cd impostor-game
npm install
npm start
```

Acesse [http://localhost:3000](http://localhost:3000) no navegador.

---

## 🐳 Rodando com Docker

```bash
docker build -t impostor-game .
docker run -p 80:80 impostor-game
```

Acesse [http://localhost](http://localhost) no navegador.

---

## 🗂️ Estrutura do projeto

```
src/
├── components/
│   ├── SetupGame.jsx       # Configuração de jogadores
│   ├── PlayerScreen.jsx    # Tela individual de pergunta
│   ├── AnswerInput.jsx     # Campo de resposta
│   ├── ResultsScreen.jsx   # Exibição anônima das respostas
│   ├── VotingScreen.jsx    # Sistema de votação
│   ├── FinalScreen.jsx     # Resultado final
│   └── TopBar.jsx          # Barra de navegação
├── context/
│   └── GameContext.jsx     # Estado global do jogo
├── data/
│   └── perguntas.js        # Banco de perguntas
├── hooks/
│   └── useTimer.js         # Hook do timer
└── utils/
    └── gameUtils.js        # Funções auxiliares
```

---

👨‍💻 Desenvolvedores
|                  |                                                |
| ---------------- | ---------------------------------------------- |
| Vitor Norton | @VitorNorton |
| Vitor Braga  | @Randons1
---

## 📄 Licença

Este projeto está sob a licença MIT.
