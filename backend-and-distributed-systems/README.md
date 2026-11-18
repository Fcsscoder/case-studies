# Estudos de Caso em Backend e Sistemas Distribuídos

Esta categoria reúne estudos de caso focados em rastreamento distribuído, propagação de telemetria, ingestão resiliente de documentos, microsserviços em arquitetura hexagonal e máquinas de estado transacionais seguras para concorrência.

---

## Estudos de Caso nesta Trilha

### 1. [Biblioteca de Rastreamento Distribuído e Logs Estruturados para Node.js](distributed-observability-lib/README.md)
* **Temas Centrais:** Sistemas Distribuídos, Telemetria, Node.js AsyncLocalStorage, Propagação de Contexto HTTP.
* **Principais Desafios:** Preservar identificadores de correlação através de loops de eventos assíncronos e filtrar sondagens rotineiras de health check de contêineres sem omitir diagnósticos de falhas.
* **Tecnologias:** TypeScript, Node.js, Pino, Axios Interceptors, Middlewares Express.

### 2. [Pipeline Tolerante a Falhas para Ingestão de Documentos e Gateway Blindado](fault-tolerant-ingestion-gateway/README.md)
* **Temas Centrais:** Ingestão Automatizada, Extração de Dados em PDF, Supervisor Fail-Fast, Proteção de Gateway com Nginx.
* **Principais Desafios:** Extrair tabelas complexas de PDFs com múltiplas colunas sustentado por 31 baterias de teste de regressão e impedir que rotinas de sincronização sobreponham correções manuais via contratos de posse.
* **Tecnologias:** Python 3, PyPDF, Docker Compose, Nginx, MongoDB.

### 3. [Microsserviço de Gestão de Identidade e Acesso em Arquitetura Hexagonal](hexagonal-auth-service/README.md)
* **Temas Centrais:** Arquitetura Limpa, Ports & Adapters, Segurança Criptográfica de Tokens, Testes de Mutação.
* **Principais Desafios:** Evitar invalidação acidental de sessões durante renovações paralelas de tokens de atualização e verificar matematicamente regras de autorização com testes de mutação.
* **Tecnologias:** TypeScript, Node.js, Express, PostgreSQL, JWT, Jest, Padrões Stryker.

### 4. [Motor de Fluxo Editorial Concorrente com Máquinas de Estado Formais](concurrency-safe-editorial-engine/README.md)
* **Temas Centrais:** Máquinas de Estado Finitas (FSM), Concorrência em Banco de Dados, Travas Transacionais.
* **Principais Desafios:** Eliminar condições de corrida durante aprovações simultâneas de revisores utilizando travas de linha no PostgreSQL com isolamento `READ COMMITTED`.
* **Tecnologias:** TypeScript, Node.js, Express, PostgreSQL (`SELECT FOR UPDATE`), Padrão de Máquina de Estados Finitos.
