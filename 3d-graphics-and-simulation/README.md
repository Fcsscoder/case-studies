# Estudos de Caso em Computação Gráfica 3D, WebGL e Simulação

Esta categoria reúne estudos de engenharia gráfica e simulações interativas, abordando renderização em WebGL2 em tempo real, física de corpos rígidos determinística com WebAssembly, matemática de rotação com quatérnions sem travamento de cardan e renderização procedural puramente vetorial.

---

## Estudos de Caso nesta Trilha

### 1. [Laboratório Clínico Virtual 3D em WebGL com Simulação Física em Primeira Pessoa](clinical-lab-webgl-physics-simulation/README.md)
* **Temas Centrais:** WebGL2, Three.js, React Three Fiber, Rapier 3D (Wasm), Matemática de Quatérnions.
* **Principais Desafios:** Formular rotações com quatérnions alinhadas à câmera para manipulação tátil de frascos sem deriva angular, somado a efeitos de profundidade de campo bokeh e máquinas de estado para equipamentos clínicos.
* **Tecnologias:** Three.js, React Three Fiber, Rapier 3D (Wasm), TypeScript, Vite, Playwright E2E.

### 2. [Motor de Simulação Espacial Cooperativa Multiusuário em Tempo Real](multiplayer-space-flight-simulation/README.md)
* **Temas Centrais:** Modo Multijogador Cooperativo, WebSockets, Calibração de Telemetria, Cenas Tridimensionais.
* **Principais Desafios:** Sincronizar transições de estado e efeitos sonoros entre clientes conectados via Socket.IO, calibrando mecânicas de sobrevivência com dados científicos reais de radiação espacial.
* **Tecnologias:** React 19, TypeScript, Three.js, Socket.IO, Neon PostgreSQL, Drizzle ORM.

### 3. [Simulação Educacional Isométrica 2D sem Dependência de Imagens Externas](procedural-2d-isometric-health-sim/README.md)
* **Temas Centrais:** Gráficos Procedurais, HTML5 Canvas 2D, Web Audio API, Arquitetura sem Recursos Externos.
* **Principais Desafios:** Eliminar o download de imagens e áudios para viabilizar carregamento instantâneo em conexões de baixa velocidade, utilizando geometria vetorial pura e osciladores sintetizados em tempo real.
* **Tecnologias:** JavaScript, React, HTML5 Canvas 2D, Web Audio API.
