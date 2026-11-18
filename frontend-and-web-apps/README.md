# Estudos de Caso em Frontend e Aplicações Web

Esta categoria apresenta arquiteturas web desenvolvidas com React, Next.js e TypeScript, com foco em observabilidade de erros do cliente para o servidor, administração multi-tenant com controle de acesso, arquiteturas estritamente em camadas e métricas financeiras adaptadas para mobile.

---

## Estudos de Caso nesta Trilha

### 1. [Portal Corporativo Multi-Tenant com Rastreamento de Erros Cliente-Servidor](enterprise-operations-admin-portal/README.md)
* **Temas Centrais:** Next.js, Observabilidade de Cliente, RBAC Departamental, Otimização de Layout Shift.
* **Principais Desafios:** Conectar barreiras de erro do React diretamente aos logs estruturados do servidor preservando o ID de correlação do proxy reverso, e eliminar saltos de interface (CLS) com telas de carregamento sob medida.
* **Tecnologias:** Next.js (App Router), React, TypeScript, Tailwind CSS, Playwright, Pino.

### 2. [Plataforma Comercial com Arquitetura em Camadas e Análise de Faturamento](retail-inventory-analytics-platform/README.md)
* **Temas Centrais:** Arquitetura em Camadas, Serviços de Domínio Desacoplados, Conectividade Dupla com Banco de Dados.
* **Principais Desafios:** Aplicar separação rigorosa em quatro níveis (UI → Route Handlers → Serviços de Domínio → Prisma) e criar uma fábrica de conexões que suporta SQLite local e Turso em nuvem sem alterar código.
* **Tecnologias:** Next.js 15 (App Router), React 19, TypeScript, Prisma ORM, SQLite / Turso libSQL.

### 3. [Sistema Full-Stack para Gestão de Adoções e Bem-Estar Comunitário](community-welfare-adoption-platform/README.md)
* **Temas Centrais:** Arquitetura Full-Stack, CORS Dinâmico para Múltiplas Origens, Publicação em Nuvem com Contêineres.
* **Principais Desafios:** Lidar com origens dinâmicas de CORS entre ambientes locais e de produção, além de gerenciar volumes persistentes de fotos com cache no Nginx em servidores Linux.
* **Tecnologias:** React, Node.js, Express, MongoDB, Mongoose, Docker, Nginx, GitHub Actions.
