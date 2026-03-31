### Comparativo de Ferramentas e Estratégias de Teste e Performance

| Domínio | Ferramenta | Limitação | Estratégia de Alta Performance |
| :--- | :--- | :--- | :--- |
| **Web** | Selenium | Latência HTTP síncrona | Playwright (WebSockets/CDP) |
| **Mobile** | Appium | Pontes IPC lentas | ADB Shell / Testes Instrumentados |
| **Carga** | Locust | Gargalo de CPU (GIL) | FastHttpUser / Modo Distribuído |
| **Infra** | GitLab | Overhead de Virtualização | Runners Bare Metal / Shell |
| **Liferay** | Java Portlets | IDs Dinâmicos | Seletores Estruturais / Data-Attributes |
