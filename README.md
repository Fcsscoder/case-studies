# Portfólio de Estudos de Caso de Engenharia

Uma coleção selecionada de estudos de caso em produção detalhando arquitetura de software, engenharia de sistemas e resolução de problemas técnicos em múltiplos domínios de engenharia.

Todos os estudos de caso são devidamente anonimizados para preservar o sigilo institucional e corporativo, focando estritamente em realizações técnicas verificáveis, decisões de arquitetura e soluções de engenharia concretas.

---

## Navegação por Trilha de Engenharia

```
case-studies/
├── backend-and-distributed-systems/   # Rastreamento Distribuído, Microsserviços, IAM Hexagonal e Máquinas de Estado
├── mobile-engineering/                 # React Native, Expo, Interfaces Acessíveis e Barreiras de Privacidade
├── frontend-and-web-apps/              # Next.js 15, Portais Corporativos Multi-Tenant e Aplicações em Camadas
├── 3d-graphics-and-simulation/         # Three.js, Rapier 3D (Wasm), Quatérnions e WebSockets
├── data-engineering-and-privacy/       # Sanitização de PII, Ingestão de CSV em Streaming e Indexação
├── fullstack-and-monorepos/            # Monorepos (npm workspaces), Grafos DAG e Filas de Canvas
└── embedded-systems-and-iot/           # ESP32 C++, Brokers MQTT e Transmissão em Tempo Real com SSE
```

---

### 1. [Backend e Sistemas Distribuídos](backend-and-distributed-systems/README.md)
* **[Biblioteca de Rastreamento Distribuído e Logs Estruturados para Node.js](backend-and-distributed-systems/distributed-observability-lib/README.md)**  
  *Stack:* TypeScript · Node.js · Pino · Axios · AsyncLocalStorage  
  *Destaques:* Biblioteca modular sem dependências externas para propagar contextos de correlação entre microsserviços, filtragem inteligente de logs de health check e telemetria de falhas.

* **[Pipeline Tolerante a Falhas para Ingestão de Documentos e Gateway Blindado](backend-and-distributed-systems/fault-tolerant-ingestion-gateway/README.md)**  
  *Stack:* Python 3 · PyPDF · Node.js · Express · Docker Compose · Nginx · MongoDB  
  *Destaques:* Extração de tabelas PDF com bateria de 31 testes de regressão, supervisor automático orquestrando daemons isolados e gateway com proteção ativa contra abusos.

* **[Microsserviço de Gestão de Identidade e Acesso em Arquitetura Hexagonal](backend-and-distributed-systems/hexagonal-auth-service/README.md)**  
  *Stack:* TypeScript · Node.js · Arquitetura Hexagonal (Ports & Adapters) · PostgreSQL · JWT  
  *Destaques:* Separação estrita entre domínio e infraestrutura, rotação de sessão concorrente, salvaguardas de revogação de tokens e testes de mutação para políticas de autorização.

* **[Motor de Fluxo Editorial Concorrente com Máquinas de Estado Formais](backend-and-distributed-systems/concurrency-safe-editorial-engine/README.md)**  
  *Stack:* TypeScript · Node.js · Express · PostgreSQL (`READ COMMITTED`) · State Machine  
  *Destaques:* Máquina de estados formal para publicação, travas transacionais em nível de linha, artigos com versionamento imutável e testes de mutação.

---

### 2. [Engenharia Mobile](mobile-engineering/README.md)
* **[Aplicativo Mobile de Rastreamento de Frotas com Preservação de Privacidade](mobile-engineering/campus-mobility-transit-app/README.md)**  
  *Stack:* React Native · Expo · TypeScript · NativeWind · Android Exact Alarms · Jest  
  *Destaques:* Linha do tempo em traço único com origem pulsante adaptada a acessibilidade (redução de movimento), barreira técnica de consentimento de privacidade e alarmes exatos no Android.

---

### 3. [Frontend e Aplicações Web](frontend-and-web-apps/README.md)
* **[Portal Corporativo Multi-Tenant com Rastreamento de Erros Cliente-Servidor](frontend-and-web-apps/enterprise-operations-admin-portal/README.md)**  
  *Stack:* Next.js · React · TypeScript · Tailwind CSS · Playwright · Pino  
  *Destaques:* Autorização por departamento, ordenação visual de avisos com drag-and-drop, barreiras de erro no cliente integradas aos logs estruturados do servidor e telas de carregamento planejadas contra layout shift.

* **[Plataforma Comercial com Arquitetura em Camadas e Análise de Faturamento](frontend-and-web-apps/retail-inventory-analytics-platform/README.md)**  
  *Stack:* Next.js 15 (App Router) · React 19 · TypeScript · Prisma ORM · SQLite / Turso libSQL  
  *Destaques:* Arquitetura em quatro camadas desacopladas (UI → Route Handlers → Serviços de Domínio → Prisma), alternância transparente entre SQLite local e Turso em produção, e métricas financeiras adaptadas para mobile.

* **[Sistema Full-Stack para Gestão de Adoções e Bem-Estar Comunitário](frontend-and-web-apps/community-welfare-adoption-platform/README.md)**  
  *Stack:* React · Node.js · Express · MongoDB · Docker · Nginx · GitHub Actions  
  *Destaques:* Arquitetura full-stack desacoplada, configuração dinâmica de CORS para múltiplos domínios, fluxos de aprovação por papéis e publicação automatizada em servidores Linux.

---

### 4. [Computação Gráfica 3D, WebGL e Simulação](3d-graphics-and-simulation/README.md)
* **[Laboratório Clínico Virtual 3D em WebGL com Simulação Física em Primeira Pessoa](3d-graphics-and-simulation/clinical-lab-webgl-physics-simulation/README.md)**  
  *Stack:* Three.js · React Three Fiber · Rapier 3D (Wasm) · TypeScript · Vite · Playwright E2E  
  *Destaques:* Interação física tridimensional, inspeção de amostras com quatérnions 1:1 sem travamento de cardan (gimbal lock), profundidade de campo com desfoque bokeh e máquinas de estado para centrífugas e incubadoras.

* **[Motor de Simulação Espacial Cooperativa Multiusuário em Tempo Real](3d-graphics-and-simulation/multiplayer-space-flight-simulation/README.md)**  
  *Stack:* React 19 · TypeScript · Vite · Three.js · Socket.IO · Neon PostgreSQL · Drizzle ORM  
  *Destaques:* Simulação cooperativa de sobrevivência planetária, sequência de lançamento interativa e telemetria de radiação calibrada com dados espaciais reais.

* **[Simulação Educacional Isométrica 2D sem Dependência de Imagens Externas](3d-graphics-and-simulation/procedural-2d-isometric-health-sim/README.md)**  
  *Stack:* JavaScript · React · HTML5 Canvas 2D · Web Audio API  
  *Destaques:* Renderização isométrica totalmente procedural em vetor sem arquivos externos de imagem, síntese sonora em tempo real via osciladores da Web Audio API e navegação territorial de saúde comunitária.

---

### 5. [Engenharia de Dados e Privacidade](data-engineering-and-privacy/README.md)
* **[Ingestão Escalável de Prontuários Clínicos e Sanitização de Dados Sensíveis (PII)](data-engineering-and-privacy/clinical-record-pii-sanitization/README.md)**  
  *Stack:* Python · Flask · PostgreSQL · Docker · Nginx  
  *Destaques:* Expurgamento completo de CPFs de URLs e logs de servidores, leitor de CSV em streaming com consumo constante O(1) de memória para cadastros volumosos e algoritmos de estratificação de risco epidemiológico.

---

### 6. [Full-Stack e Monorepos](fullstack-and-monorepos/README.md)
* **[Motor Gráfico de Matrizes Curriculares e Quadro Branco Colaborativo](fullstack-and-monorepos/academic-curriculum-dag-whiteboard/README.md)**  
  *Stack:* TypeScript · Node.js · Express · React 19 · Vite · Prisma · PostgreSQL · MinIO · Docker · Zod  
  *Destaques:* Estrutura em monorepo, pipeline de eventos idempotente para analytics, controle de concorrência em tela de desenho digital e memoização de grafos curriculares.

---

### 7. [Sistemas Embarcados e IoT](embedded-systems-and-iot/README.md)
* **[Firmware para Telemetria Ambiental e Painel em Tempo Real Orientado a Eventos](embedded-systems-and-iot/real-time-air-quality-iot-telemetry/README.md)**  
  *Stack:* C++ · ESP32 · Eclipse Mosquitto MQTT · Node.js · Express · EJS · Server-Sent Events (SSE)  
  *Destaques:* Firmware em C++ com amostragem de sensores a 1 Hz e envio a cada 30 segundos, integrado a painel web com Server-Sent Events eliminando polling constante.
