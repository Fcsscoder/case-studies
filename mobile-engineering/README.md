# Estudos de Caso em Engenharia Mobile

Esta categoria destaca o desenvolvimento de aplicações móveis com React Native e Expo, priorizando desempenho multiplataforma, eficiência energética no rastreamento de frotas, acessibilidade em animações, conformidade regulatória de privacidade e integração nativa com o sistema Android.

---

## Estudos de Caso nesta Trilha

### 1. [Aplicativo Mobile de Rastreamento de Frotas com Preservação de Privacidade](campus-mobility-transit-app/README.md)
* **Temas Centrais:** React Native, Expo, Geolocalização e Transporte, Acessibilidade, Barreiras Regulatórias de Privacidade.
* **Principais Desafios:**
  - Criação de linha do tempo de paradas em SVG animada com indicador pulsante que desativa dinamicamente sob a configuração de redução de movimento do sistema operacional (`prefers-reduced-motion`).
  - Aplicação de barreira técnica de consentimento que bloqueia qualquer tráfego de rede ou telemetria em segundo plano antes da aceitação formal dos termos.
  - Agendamento de notificações de partidas com horário exato utilizando permissões nativas `SCHEDULE_EXACT_ALARM` no Android.
* **Tecnologias:** React Native, Expo, TypeScript, NativeWind (Tailwind CSS), Bridge Nativa Android, Jest.
