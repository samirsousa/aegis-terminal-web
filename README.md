# ⚡ KRYPTON AI — Multi-Agent Decision Support System (DSS)

[![Flutter](https://img.shields.io/badge/Flutter-3.22+-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev/)
[![Bloc](https://img.shields.io/badge/State_Management-BLoC-8B5CF6?style=for-the-badge)](https://bloclibrary.dev/)

O **Krypton AI** é um Sistema de Apoio à Decisão (*Decision Support System - DSS*) fundamentado em uma arquitetura de **Enxame de Agentes Autônomos de Inteligência Artificial (*Swarm Intelligence*)** focado no monitoramento, análise de risco e simulação de operações no mercado financeiro e de criptoativos em tempo real.

O projeto combina telemetria de alta frequência, processamento sintético de sinais e execução automatizada (*Paper Trading*) via WebSocket para oferecer relatórios analíticos de alta precisão.

---

## 🧠 Arquitetura do Enxame de Agentes (Swarm Intelligence)

O núcleo de tomada de decisão é composto por **4 Agentes Especializados** que trabalham de forma colaborativa e paralela para gerar um **Consenso Global** e calcular o **DSS Risk Score**:

<img width="923" height="298" alt="image (1)" src="https://github.com/user-attachments/assets/19b31e2a-e5f9-4c86-8d0c-ba15cabd4955" />

### 🤖 Atribuições dos Agentes:
* **AG-1 (Technical Analyst):** Avalia indicadores técnicos clássicos, suporte, resistência e momento de preço. Subtítulos: *(MÉDIAS/RSI/MACD) | Analista Gráfico*.
* **AG-2 (Sentiment Agent):** Analisa a pressão do livro de ofertas e sentimento de mercado sintético. Subtítulos: *(ORDERBOOK/PNL) | Análise de Mercado/Livro*.
* **AG-3 (Risk Manager):** Calcula o **DSS Risk Score** (0 a 100), define o limite máximo de exposição e valida o *Stop Loss*. Subtítulos: *(PONTUAÇÃO DE RISCO 0-100) | Gerente de Riscos*.
* **AG-4 (Macro Trend & Execution):** Avalia a tendência macro, consolida o consenso e autoriza a execução das ordens. Subtítulos: *(TENDÊNCIA/EXEC) | Analista Macro/Execução*.

---

## ✨ Principais Funcionalidades

* 📊 **Terminal DSS de Alta Frequência:** Gráficos interativos em tempo real para os pares `BTCUSDT`, `ETHUSDT` e `SOLUSDT`.
* 🛡️ **DSS Risk Score Panel:** Métrica precisa de risco de 0 a 100, nível de confiança global e porcentagem recomendada de alocação por operação.
* 💼 **Paper Trading & Auto-Pilot:** Corretora simulada com saldo inicial de **$10,000 USDT** e robô de execução autônoma orientado pelo consenso do enxame.
* 📊 **Portfolio Risk Copilot:** Módulo de simulação e rebalanceamento de carteira com balanceamento dinâmico de caixa em USDT.
* 📜 **Audit Log System:** Rastreabilidade e logs em tempo real de todas as decisões tomadas pelos agentes, com suporte à exportação em formato `.CSV`.
* 💬 **Krypton AI Support:** Chatbot inteligente integrado focado no auxílio operacional e explicação de parâmetros de risco.
* 🌓 **Suporte a Dark & Light Mode:** Interface responsiva adaptável otimizada para desktops e dispositivos móveis.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** [Dart 3.x](https://dart.dev/)
* **Framework Frontend:** [Flutter 3.22+](https://flutter.dev/)
* **Gerenciamento de Estado:** `flutter_bloc`
* **Comunicação em Tempo Real:** WebSockets (`web_socket_channel`)
* **Design & Temas:** CustomPainter para logos geométricas, Google Fonts (`JetBrains Mono`), suporte a temas dinâmicos via `ValueNotifier`.

---

## 🚀 Como Executar o Projeto Localmente

### Pré-requisitos
* Flutter SDK instalado (versão `>=3.22.0`)
* Git instalado
* Navegador Google Chrome (para execução Flutter Web)

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/krypton-ai.git](https://github.com/seu-usuario/krypton-ai.git)
   cd krypton-ai

2. Instale as dependências do projeto:

flutter pub get

3. Execute a aplicação no navegador (Flutter Web):

flutter run -d chrome

💡 Dica de Desenvolvimento: Para evitar re-renderizações pesadas do CanvasKit durante Hot Restarts no Chrome, execute utilizando o modo HTML:

flutter run -d chrome --web-renderer html
