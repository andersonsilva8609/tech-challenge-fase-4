# Tech Challenge Fase 4
Sistema de Gerenciamento de Pedidos Integrado com Spring e Microsserviços

## TECH CHALLENGE
Tech Challenge é o projeto que englobará os conhecimentos obtidos em todas as disciplinas da fase. Esta é uma atividade que, em princípio, deve ser desenvolvida em grupo. Importante atentar-se ao prazo de entrega, pois trata-se de uma atividade obrigatória, uma vez que vale 60% da nota de todas as disciplinas da fase.

## OBJETIVO:
Seu grupo deverá criar um Sistema de Gerenciamento de Pedidos Integrado com Spring e Microsserviços.
O projeto deverá conter um sistema de gerenciamento de pedidos altamente eficiente, que explore profundamente a arquitetura de microsserviços utilizando o ecossistema Spring. Este sistema deverá abranger desde a gestão de clientes e produtos até o processamento e entrega de pedidos, enfatizando a autonomia dos serviços, comunicação eficaz, e persistência de dados isolada.

### Visão Detalhada do Sistema:
O objetivo é criar um sistema modular onde cada microsserviço desempenha um papel no gerenciamento de pedidos. Este sistema não apenas facilitará a gestão eficiente de pedidos, mas também servirá como um exemplo prático do uso de tecnologias de ponta em um cenário realista de desenvolvimento de software.

## DESCRIÇÃO FUNCIONAL E TÉCNICA:

#### Microsserviço de Gerenciamento de Clientes
Descrição Funcional: este serviço será responsável por todas as operações relacionadas aos clientes, incluindo a criação, leitura, atualização e exclusão de registros de clientes (CRUD).

#### Tecnologias e Abordagens
  • Spring Boot para facilitar a criação do microsserviço.
  • Spring Data JPA para a integração com um banco de dados relacional, simplificando operações CRUD.

##### Microsserviço de Catálogo de Produtos
Descrição Funcional: este microsserviço gerenciará o catálogo de produtos, incluindo informações detalhadas dos produtos e o controle de estoque. Uma característica chave será a funcionalidade de carga de produtos, permitindo a importação em massa de informações de produtos para o sistema.
  • Spring Boot para desenvolvimento e configuração.
  • Spring Data JPA para gerenciamento de dados de produtos em um banco de dados.
  • Spring Batch para implementar a funcionalidade de carga de produtos, automatizando a importação de dados de produtos de fontes externas, como arquivos CSV.
  
#### Funcionalidade de Carga de Produtos
Descrição Funcional: esta funcionalidade específica permitirá a importação em massa de dados de produtos, incluindo descrições, preços e quantidades em estoque. A importação poderá ser agendada ou iniciada manualmente, garantindo que o catálogo de produtos esteja sempre atualizado.

#### Microsserviço de Gestão de Pedidos
Descrição Funcional: centralizará o processamento de todos os pedidos, desde a criação até a conclusão. Isso inclui receber pedidos dos clientes, processar pagamentos (se aplicável), e coordenar com o microsserviço de logística de entrega para garantir a entrega eficiente dos produtos.

#### Tecnologias e Abordagens:
  • Spring Boot para a estrutura do serviço.
  • Spring Data JPA para manipulação de dados dos pedidos.
  • Spring Cloud Stream para comunicação baseada em eventos com outros serviços, melhorando a coordenação de processos de negócios complexos.
##### Microsserviço de Logística de Entrega:
Descrição Funcional: este serviço cuidará de toda a logística relacionada à entrega de pedidos, desde a atribuição de entregadores até o rastreamento das entregas em tempo real. A função inclui calcular as rotas mais eficientes, estimar tempos de entrega e fornecer atualizações de status aos clientes.

##### Tecnologias e Abordagens:
• Spring Boot para a base do microsserviço.
• Spring Data JPA para gerenciar as informações de entrega em um banco de dados.

##### Critérios de Avaliação Técnica:
1. Arquitetura e Design: avaliação da coerência arquitetônica, incluindo a escolha e implementação dos padrões de design, separação de responsabilidades, e a eficácia da comunicação entre serviços.
2. Qualidade do Código: análise da legibilidade, estrutura e uso de práticas de codificação recomendadas, incluindo a implementação de princípios SOLID e padrões de codificação limpa.
3. Funcionalidade e Cobertura de Recursos: avaliação da implementação completa dos requisitos funcionais, incluindo a robustez, a segurança dos dados, e a precisão dos processos de negócio.
4. Integração e Desacoplamento: avaliação da eficácia na integração entre microsserviços, uso de comunicação assíncrona e a habilidade de manter a funcionalidade mesmo diante de falhas parciais.
5. Testes: análise da abrangência e qualidade dos testes automatizados, incluindo testes unitários, de integração e end-to-end, além da implementação de práticas de TDD ou BDD onde aplicável.
6. Documentação: qualidade da documentação do projeto, incluindo a descrição da arquitetura, design dos serviços, endpoints de API e guias de implantação e uso.
7. Demonstração: apresentação eficaz do sistema, demonstrando a funcionalidade através de casos de uso reais, e capacidade de explicar as decisões técnicas tomadas.
