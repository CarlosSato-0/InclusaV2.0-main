# InclusaV2-main

# InclusaV2-main
<div align="center">

# 🚀 Inclusa Vision — Mobilidade sem Barreiras

[![Acessar Site Oficial](https://img.shields.io/badge/🌐_ACESSAR_SITE_OFICIAL-blue?style=for-the-badge)](https://inclusavision.com.br)

Este projeto é uma solução tecnológica focada em acessibilidade real no transporte público. O Inclusa Vision atua como um guia autônomo, integrando radiofrequência (RF) e comunicação NFC para oferecer navegação independente, feedback sonoro em tempo real e resposta tátil a pessoas com deficiência visual.

</div>

---

## 🛠️ Stack Tecnológica & Status da Aplicação

<div align="center">

![STATUS](https://img.shields.io/badge/STATUS-EM_PRODUÇÃO-success?style=flat-square)
![REACT](https://img.shields.io/badge/REACT-18.3-61DAFB?style=flat-square&logo=react&logoColor=black)
![VITE](https://img.shields.io/badge/VITE-5.x-646CFF?style=flat-square&logo=vite&logoColor=white)
![TAILWIND CSS](https://img.shields.io/badge/TAILWIND_CSS-3.x-38BDF8?style=flat-square&logo=tailwind-css&logoColor=white)
![FRAMER MOTION](https://img.shields.io/badge/FRAMER_MOTION-11.x-0055FF?style=flat-square&logo=framer&logoColor=white)

[![DEPLOY](https://img.shields.io/badge/DEPLOY-GITHUB_PAGES-181717?style=flat-square&logo=github)](https://github.com)

</div>

---

## 💡 Arquitetura & Conceitos de Engenharia

O sistema foi arquitetado combinando design inclusivo de alto nível com tecnologias de processamento local, garantindo que o usuário nunca fique desamparado por falta de conexão.

* **Acessibilidade Nativa (WCAG 2.1 AA):** interface desenvolvida especificamente para ser lida por leitores como VoiceOver e TalkBack, com áreas de toque ampliadas e alto contraste.
* **Processamento Edge (Offline-first):** Algoritmos de decisão executam diretamente no dispositivo do usuário, eliminando a dependência de um servidor central e garantindo resposta imediata.
* **Integração Hardware/Software:** Comunicação direta com transmissores de Radiofrequência (433 MHz) nas paradas e Tags NFC (ISO 14443) nos veículos.
* **UI/UX Cromográfica:** Utilização do `framer-motion` para criar feedbacks visuais fluidos e animações baseadas em scroll (Parallax) que não prejudicam a performance.
* **Deploy Contínuo (CI/CD):** Pipeline automatizada com GitHub Actions para publicação direta na nuvem.

---

## 📋 Funcionalidades Principais

### 📍 Rastreamento e Rede RF Local
Posicionamento em tempo real através da rede de transportes. Transmissores nas paradas formam uma rede de baixo consumo garantindo operação contínua mesmo em zonas "cegas" de operadoras móveis.

### 🔊 Feedback Sonoro & Tátil
* **Áudio:** Síntese de voz ativa notifica a chegada de veículos, número de paradas e alertas de rota.
* **Háptico:** Padrões de vibração codificados comunicam informações críticas (ex: pulsos curtos para aproximação, pulsos longos confirmando embarque).

### 📱 Leitura NFC Instantânea
Ao encostar o smartphone nas tags dos veículos ou estações, o sistema captura o ID da linha, destino final e lotação sem necessidade de internet.

---

## 📁 Estrutura do Projeto

```text
InclusaV2/
├── public/                      # Assets estáticos globais (favicons, imagens otimizadas)
│   ├── app.png                  # Mockup da interface
│   └── logo-inclusar.png        # Identidade visual
│
├── src/                         # Código-fonte principal
│   ├── assets/                  # Ícones em SVG e assets vetoriais
│   ├── App.jsx                  # Componentização principal e seções da Landing Page
│   ├── main.jsx                 # Ponto de entrada do React
│   └── index.css                # Configurações globais do Tailwind
│
├── .github/workflows/           # Automação de deploy (GitHub Actions)
├── tailwind.config.js           # Diretrizes de estilização
└── vite.config.js               # Configurações de build e roteamento
