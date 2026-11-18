# Estudos de Caso em Engenharia de Dados e Privacidade

Esta categoria concentra-se em processamento de dados em larga escala, pipelines de ingestão eficientes em memória via streaming e engenharia de privacidade regulatória (sanitização de dados sensíveis e PII) no setor de saúde pública.

---

## Estudos de Caso nesta Trilha

### 1. [Ingestão Escalável de Prontuários Clínicos e Sanitização de Dados Sensíveis (PII)](clinical-record-pii-sanitization/README.md)
* **Temas Centrais:** Engenharia de Dados em Saúde, Sanitização de PII, Ingestão de CSV em Streaming com Memória O(1), Otimização em PostgreSQL.
* **Principais Desafios:**
  - Expurgar completamente números de CPF de rotas de API, parâmetros de busca e logs de acesso de servidores web para atender às normas da LGPD.
  - Eliminar falhas por estouro de memória (Out-Of-Memory) ao processar cadastros municipais de dezenas de milhares de cidadãos, desenvolvendo um leitor iterativo em streaming com pegada estável de memória inferior a 80 MB.
  - Criar rotinas automáticas de estratificação de risco clínico e listas operacionais de visitas para agentes comunitários com paginação no servidor.
* **Tecnologias:** Python, Flask, Gunicorn, PostgreSQL, psycopg2, Docker, Nginx, Shell Scripting.
