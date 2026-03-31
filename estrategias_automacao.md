Este documento técnico apresenta a desconstrução sistemática de frameworks de automação sob a ótica de engenharia de infraestrutura, com foco em performance, escalabilidade e resiliência em ecossistemas complexos.

## 1. Arquitetura de Automação e Primazia Técnica
O Selenium não controla o browser diretamente; ele atua como um cliente que envia comandos via protocolo W3C WebDriver sobre conexões HTTP síncronas. O Playwright utiliza conexões WebSocket persistentes para comunicação bidirecional direta com os protocolos de depuração nativos do browser (CDP).

## 2. MECÂNICA DE PERFORMANCE: Otimização Mobile (Appium)
No Android (UiAutomator2), definir 'waitForIdleTimeout' como zero e usar 'ignoreUnimportantViews' acelera a execução. No iOS (XCUITest), limitar 'snapshotMaxDepth' evita timeouts em telas complexas.

## 3. ESTRATÉGIA LIFERAY: IDs Dinâmicos
Utilizar seletores CSS parciais ou atributos estáveis como 'data-qa-id' para evitar a volatilidade dos IDs namespaced do Liferay.

## 4. Engenharia de Testes de Carga: Locust
Para superar o GIL do Python, usar o modo Master-Worker e o 'FastHttpUser' para aumentar o RPS em até 6x.
