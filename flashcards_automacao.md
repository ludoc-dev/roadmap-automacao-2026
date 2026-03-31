# Automação Flashcards

## Card 1

**Front:** No React Native, qual propriedade deve ser usada exclusivamente para identificação de elementos pelo Appium?

**Back:** A propriedade `testID`.

---

## Card 2

**Front:** Qual propriedade do React Native deve ser reservada apenas para anúncios de leitores de tela?

**Back:** A propriedade `accessibilityLabel`.

---

## Card 3

**Front:** No Android, para qual propriedade nativa o `testID` do React Native é mapeado?

**Back:** View Tag (`view.setTag()`) ou Resource ID.

---

## Card 4

**Front:** No iOS, qual o mapeamento nativo da propriedade `testID` do React Native?

**Back:** A propriedade `accessibilityIdentifier`.

---

## Card 5

**Front:** Qual o risco de usar `accessibilityLabel` como substituto para o `testID` no Android?

**Back:** Isso polui os metadados de acessibilidade com identificadores de teste.

---

## Card 6

**Front:** Como o Appium deve localizar elementos no Android para garantir alta confiabilidade?

**Back:** Usando estratégias de localização customizadas para atingir a View Tag.

---

## Card 7

**Front:** Qual técnica do React Native remove elementos decorativos da árvore de acessibilidade no Android?

**Back:** O uso de `importantForAccessibility="no-hide-descendants"`.

---

## Card 8

**Front:** Qual propriedade do React Native esconde elementos do VoiceOver no iOS?

**Back:** A propriedade `accessibilityElementsHidden={true}`.

---

## Card 9

**Front:** Por que o uso de `FlatList` é preferível ao `ScrollView` em automação de testes?

**Back:** Reduz drasticamente o número de nós no DOM, acelerando as consultas do Appium.

---

## Card 10

**Front:** Qual o impacto de configurar `unmountOnBlur: true` no React Navigation?

**Back:** Reduz o consumo de memória e evita que o Appium encontre elementos em telas ocultas.

---

## Card 11

**Front:** O que a configuração `snapshotMaxDepth` do Appium controla?

**Back:** O valor máximo de profundidade para percorrer os elementos na árvore de origem.

---

## Card 12

**Front:** Qual o efeito de definir `accessible={true}` em um contêiner pai no React Native?

**Back:** Ele achata todos os filhos em um único nó de acessibilidade, escondendo-os do Appium.

---

## Card 13

**Front:** Qual é a recomendação sobre o uso da propriedade `accessible` em listas e coleções?

**Back:** Nunca deve ser definida como `true` no contêiner, para manter os itens filhos testáveis.

---

## Card 14

**Front:** No iOS (XCUITest), o que o framework verifica para garantir que o app está pronto para interação?

**Back:** Verifica se o aplicativo está ocioso (idling) e se todas as animações terminaram.

---

## Card 15

**Front:** Por que a localização de elementos por XPath é lenta no iOS (WDA)?

**Back:** Porque o XPath não é nativo do XCTest e exige um snapshot caro de toda a hierarquia.

---

## Card 16

**Front:** Como acelerar buscas XPath no iOS reduzindo o escopo da árvore?

**Back:** Através da configuração do ajuste `snapshotMaxDepth`.

---

## Card 17

**Front:** Quais atributos de elemento são considerados "caros" para calcular no WebDriverAgent (iOS)?

**Back:** Os atributos `visible` e `accessible`.

---

## Card 18

**Front:** O que são elementos de UI dinâmicos?

**Back:** Componentes cujos atributos ou valores mudam dinamicamente durante a execução.

---

## Card 19

**Front:** Qual estratégia de XPath é útil para lidar com IDs gerados dinamicamente?

**Back:** O uso da função `contains()` para correspondências parciais.

---

## Card 20

**Front:** O que caracteriza um "Explicit Wait" em automação?

**Back:** A espera por condições específicas como visibilidade ou clique, com um tempo limite definido.

---

## Card 21

**Front:** Qual a função do "Fluent Wait" no Selenium?

**Back:** Lidar com atrasos assíncronos permitindo intervalos de sondagem (polling) customizados.

---

## Card 22

**Front:** Como estabilizar o ambiente de teste contra dados dinâmicos de APIs externas?

**Back:** Utilizando servidores de mock para simular respostas estáveis.

---

## Card 23

**Front:** No Liferay, qual a diferença na hospedagem entre IFrame e Custom Element?

**Back:** IFrames exigem um servidor externo para o markup, enquanto Custom Elements só precisam da URL do código.

---

## Card 24

**Front:** Qual técnica é necessária para garantir que a declaração de um Custom Element rode assim que o código carregar?

**Back:** O uso de uma IIFE (Immediately Invoked Function Expression).

---

## Card 25

**Front:** Qual o método padrão para comunicação segura entre um IFrame e sua página host?

**Back:** O método `window.postMessage()`.

---

## Card 26

**Front:** O que o localizador `page.getByRole()` do Playwright prioriza?

**Back:** Atributos de acessibilidade explícitos e implícitos, como usuários percebem a página.

---

## Card 27

**Front:** Qual localizador do Playwright deve ser usado para campos de formulário com rótulos associados?

**Back:** O método `page.getByLabel()`.

---

## Card 28

**Front:** Como o Playwright lida com o Shadow DOM por padrão?

**Back:** Todos os seus localizadores conseguem penetrar o Shadow DOM automaticamente.

---

## Card 29

**Front:** O que define a "estrita conformidade" (strictness) dos localizadores no Playwright?

**Back:** Operações falham se o localizador encontrar mais de um elemento no DOM.

---

## Card 30

**Front:** Qual a recomendação do Playwright sobre o uso de seletores XPath ou CSS longos?

**Back:** Evitá-los, pois são propensos a quebrar quando a estrutura do DOM muda.

---

## Card 31

**Front:** No GitLab CI, qual a função da palavra-chave `rules:`?

**Back:** Controlar condicionalmente quando um job deve ou não ser executado na pipeline.

---

## Card 32

**Front:** Qual a diferença entre `cache` e `artifacts` no GitLab CI?

**Back:** O cache acelera tarefas repetitivas salvando dependências; os artifacts persistem saídas entre estágios.

---

## Card 33

**Front:** O que é o "Docker-in-Docker" (DinD) em pipelines de CI/CD?

**Back:** Uma técnica que permite executar comandos Docker dentro de um contêiner Docker.

---

## Card 34

**Front:** Qual a vantagem da arquitetura do Playwright sobre a do Selenium?

**Back:** O Playwright comunica-se diretamente via protocolos de browser (CDP), eliminando a latência do WebDriver.

---

## Card 35

**Front:** Qual ferramenta do Playwright permite gerar scripts gravando as ações do usuário?

**Back:** A ferramenta `Codegen`.

---

## Card 36

**Front:** Qual é a principal limitação comum tanto ao Selenium quanto ao Playwright?

**Back:** Ambos funcionam apenas dentro de navegadores web.

---

## Card 37

**Front:** O que caracteriza o "Auto-waiting" no Playwright?

**Back:** O framework espera automaticamente que os elementos existam e estejam clicáveis antes de interagir.

---

## Card 38

**Front:** Em um arquivo `.gitlab-ci.yml` para Android, para que serve o comando `sdkmanager`?

**Back:** Para instalar versões específicas do SDK, ferramentas de build e plataformas Android.

---

## Card 39

**Front:** Por que testes unitários de Android no GitLab CI rodam na JVM sem dispositivos reais?

**Back:** Porque verificam a lógica individual e não dependem do hardware ou do sistema Android completo.

---

## Card 40

**Front:** O que define um teste de regressão "atômico"?

**Back:** Um teste focado em apenas uma unidade testável e independente de outros testes.

---

## Card 41

**Front:** Por que seletores por ID são mais rápidos que XPath no Selenium?

**Back:** IDs são otimizados nativamente pelos navegadores através de `findElementById`.

---

## Card 42

**Front:** Por que o uso de `Thread.sleep` é desencorajado em scripts de automação?

**Back:** Porque bloqueia a thread de execução e aumenta o tempo de teste de forma ineficiente.

---

## Card 43

**Front:** Qual a vantagem de usar o Selenium Grid na nuvem em vez de um grid local?

**Back:** Evita custos de manutenção e oferece acesso instantâneo a múltiplas combinações de OS/Navegador.

---

## Card 44

**Front:** Qual biblioteca Python de parsing de HTML é a mais rápida?

**Back:** A biblioteca `lxml`, pois é baseada em bibliotecas C.

---

## Card 45

**Front:** Qual biblioteca Python é recomendada para iniciantes devido à facilidade de navegar na árvore de parsing?

**Back:** A biblioteca `BeautifulSoup`.

---

## Card 46

**Front:** Qual biblioteca de parsing Python imita o comportamento exato de um navegador ao lidar com HTML quebrado?

**Back:** A biblioteca `html5lib`.

---

## Card 47

**Front:** Qual a principal desvantagem da biblioteca `html5lib`?

**Back:** Ela é muito lenta e consome muita memória.

---

## Card 48

**Front:** O que é o localizador de "cadeia de classe" (Class Chain) no iOS?

**Back:** Uma estratégia nativa do WDA para localizar elementos em hierarquias complexas de forma mais rápida que XPath.

---

## Card 49

**Front:** No React Native, qual a consequência de não limpar o estado de telas antigas na navegação?

**Back:** Causa acúmulo de nós no DOM e risco do Appium interagir com elementos obsoletos (stale elements).

---

## Card 50

**Front:** Como o Appium Inspector ajuda no desenvolvimento de testes para React Native?

**Back:** Permite visualizar a árvore nativa e verificar como `testID` e `accessibilityLabel` foram mapeados.

---

## Card 51

**Front:** O que o termo "flaky test" descreve em automação de testes?

**Back:** Um teste que falha e passa de forma inconsistente, sem alterações no código.

---

## Card 52

**Front:** Qual é a ordem de preferência recomendada para seletores Selenium visando performance?

**Back:** ID > Seletores CSS (class, name) > XPath.

---

## Card 53

**Front:** No GitLab CI, qual a função do executor "Runner"?

**Back:** É o agente que executa os jobs definidos na pipeline em ambientes específicos.

---

## Card 54

**Front:** Qual o benefício de rodar testes em paralelo em uma pipeline de CI/CD?

**Back:** O tempo total da suíte de testes passa a ser igual ao tempo do teste mais lento.

---

## Card 55

**Front:** O que é a análise de causa raiz (RCA) assistida por IA?

**Back:** O uso de agentes de IA para classificar erros e sugerir correções de forma automatizada.

---

## Card 56

**Front:** Qual a utilidade do "Trace Viewer" no Playwright?

**Back:** Analisar falhas de teste através de screencasts, snapshots do DOM e logs de ações.

---

## Card 57

**Front:** No contexto de IFrames no Liferay, o que é a "Same-origin policy"?

**Back:** Uma política de segurança que restringe como documentos de diferentes origens interagem.

---

## Card 58

**Front:** Como as "Quality Gates" ajudam na confiabilidade da pipeline?

**Back:** Estabelecem condições obrigatórias (ex: 100% de sucesso nos testes) antes do deploy.

---

## Card 59

**Front:** O que o localizador `page.getByAltText()` do Playwright busca?

**Back:** Elementos (geralmente imagens) baseando-se no seu texto alternativo descritivo.

---

## Card 60

**Front:** Por que o XPath deve ser evitado para atravessar Shadow Roots no Playwright?

**Back:** Porque o XPath não consegue atravessar as raízes de sombra (shadow roots) por padrão.

---

## Card 61

**Front:** No GitLab CI, para que serve o parâmetro `unmountOnBlur` em apps React Native?

**Back:** Para garantir que telas não visíveis sejam removidas da memória e do DOM.

---

## Card 62

**Front:** Qual a recomendação para lidar com elementos que possuem IDs gerados por frameworks modernos?

**Back:** Usar atributos de dados customizados (ex: `data-testid`) ou localizadores baseados em texto/função.

---

## Card 63

**Front:** No Android, qual o papel do comando `yes | sdkmanager --licenses` no CI?

**Back:** Aceitar automaticamente as licenças do SDK Android para permitir o download sem intervenção humana.

---

## Card 64

**Front:** Qual técnica ajuda a depurar animações infinitas que travam testes XCUITest?

**Back:** Ajustar o `animationCoolOffTimeout` nas capacidades do driver.

---

## Card 65

**Front:** Como filtrar localizadores no Playwright para encontrar um item específico em uma lista?

**Back:** Usando o método `locator.filter()` com texto ou outro localizador interno.

---

## Card 66

**Front:** O que a biblioteca Python `PyQuery` oferece de único?

**Back:** Uma sintaxe inspirada em jQuery para manipular HTML dentro do ecossistema Python.

---

## Card 67

**Front:** Qual a principal vantagem da biblioteca nativa `html.parser` do Python?

**Back:** Ela já vem instalada com o interpretador Python, sem necessidade de dependências externas.

---

## Card 68

**Front:** Por que o uso de localizadores baseados em posição (ex: `.nth(2)`) é perigoso?

**Back:** Porque mudanças na ordem dos elementos na página podem fazer o teste interagir com o elemento errado.

---

## Card 69

**Front:** No GitLab CI, o que é o estágio de "Packaging"?

**Back:** O estágio onde artefatos como APKs, binários ou imagens Docker são criados.

---

## Card 70

**Front:** O que é a técnica de "Canary Release" em automação de deployment?

**Back:** Lançar a nova versão para um grupo pequeno de usuários reais antes do lançamento global.

---

## Card 71

**Front:** Qual ferramenta do Playwright permite depurar o DOM em tempo real e inspecionar elementos?

**Back:** O `Playwright Inspector`.

---

## Card 72

**Front:** Qual a diferença de performance entre XPath e Seletores CSS em dispositivos móveis modernos?

**Back:** Seletores CSS geralmente apresentam performance superior ao XPath.

---

## Card 73

**Front:** O que define a estratégia de "Wait for AJAX" em testes web?

**Back:** Garantir que todas as requisições assíncronas do navegador foram finalizadas antes de prosseguir.

---

## Card 74

**Front:** Como o WebDriverAgent (iOS) é distribuído no ecossistema Appium?

**Back:** Como um pacote NPM (`appium-webdriveragent`) contendo o código-fonte em Objective-C.

---

## Card 75

**Front:** No React Native, como garantir que leitores de tela e Appium convivam bem?

**Back:** Usando `testID` para automação e `accessibilityLabel` para acessibilidade humana de forma separada.

---

## Card 76

**Front:** Qual ajuste do Appium ajuda a evitar erros de timeout ao obter a árvore XML de páginas enormes?

**Back:** Aumentar o valor de `customSnapshotTimeout`.

---

## Card 77

**Front:** O que é a orquestração inteligente de testes?

**Back:** O uso de IA para otimizar fluxos de trabalho, prever gargalos e gerenciar falhas de forma autônoma.

---

## Card 78

**Front:** No GitLab CI para Android, por que é necessário definir `ANDROID_HOME`?

**Back:** Para informar ao Gradle e às ferramentas de build onde o SDK Android está localizado.

---

## Card 79

**Front:** Qual a importância de usar versões fixas (pinned versions) de dependências em CI?

**Back:** Evita o problema do "funciona na minha máquina" e garante builds consistentes em qualquer ambiente.

---

## Card 80

**Front:** No Playwright, o que faz o método `locator.and()`?

**Back:** Refina um localizador existente exigindo que ele também corresponda a um localizador adicional.

---

## Card 81

**Front:** O que é a análise estática de código (SAST) integrada na pipeline?

**Back:** A verificação automática de vulnerabilidades de segurança no código-fonte sem executá-lo.

---

## Card 82

**Front:** Como o Appium lida com animações que impedem que o app fique ocioso?

**Back:** Tenta continuar após o timeout usando uma estratégia de "melhor esforço" (best effort).

---

## Card 83

**Front:** O que é a visibilidade do estado do sistema em pipelines de DevOps?

**Back:** O uso de dashboards e métricas (como duração de jobs) para identificar gargalos e melhorar a performance.

---

## Card 84

**Front:** No Playwright, qual a diferença entre `getByText` e localizadores de papel (role)?

**Back:** Role foca na função semântica (botão, link); text foca apenas no conteúdo da string.

---

## Card 85

**Front:** Qual a vantagem de usar imagens Docker leves (ex: Alpine) em CI/CD?

**Back:** Acelera o tempo de download da imagem e o início da execução dos jobs.

---

## Card 86

**Front:** Como o Selenium WebDriver se comunica com os navegadores?

**Back:** Através de APIs nativas de automação dos navegadores usando o protocolo W3C WebDriver.

---

## Card 87

**Front:** Qual biblioteca Python de parsing não constrói uma árvore de parsing por padrão?

**Back:** A biblioteca `html.parser`, que utiliza parsing orientado a eventos.

---

## Card 88

**Front:** No React Native, qual o efeito colateral de ter um DOM muito aninhado para o Appium?

**Back:** Torna as consultas XPath extremamente lentas e pode causar truncamento na inspeção de elementos.

---

## Card 89

**Front:** O que é o teste de regressão visual?

**Back:** A comparação automática de imagens para detectar bugs visuais e mudanças inesperadas na interface.

---
