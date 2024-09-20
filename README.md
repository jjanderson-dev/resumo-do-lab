# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO - Janderson

# 🚀 Aula sobre **Microsoft Azure - Localizando Serviços por Categoria**

### 👩‍🏫 **Instrutora**: Valéria Baptista

---

## 📋 **Tópicos abordados**:

### 1. **Visão Geral dos Serviços do Azure**
- Introdução aos principais **serviços disponíveis** na plataforma **Microsoft Azure**.
- Diferenças entre os tipos de conta:
  - **Conta Free**: Acesso gratuito com limitações.
  - **Pay-As-You-Go**: Modelo pago baseado no consumo dos recursos.

### 2. **Personalização da Plataforma**
- Demonstração prática sobre como **alterar o esquema de cores** e **personalizar a interface**.
- Exploração detalhada de **todos os serviços** oferecidos no **Azure**.

### 3. **Acordo de Nível de Serviço (SLA)**
- Explicação sobre o **SLA (Service Level Agreement)**:
  - Definição e importância dos **níveis de serviço garantidos** pela Microsoft.
  - Como o SLA impacta a **disponibilidade** e a **confiabilidade** dos serviços.

---

## 📝 **Plataforma Microsoft Azure**
- **Criação de uma conta no portal do Microsoft Azure**:
  - Passo a passo para configurar uma conta e começar a utilizar os serviços do Azure.
  
---

> **💡 Dica**: Utilize a conta gratuita para explorar os serviços antes de migrar para um plano pago, aproveitando os benefícios iniciais sem custo.

---

### 🔗 **Referências**
- [Portal do Microsoft Azure](https://portal.azure.com)
- [SLA no Azure](https://azure.microsoft.com/en-us/support/legal/sla/)

  -----------------------------------------------------------------------------------------------------------------------------------------------------

  # Benefícios para a Nuvem

Precisamos entender quais são os benefícios da nuvem e como eles são aplicados, para que possamos explicar ao cliente e ele compre a ideia.

## Benefícios da Nuvem Azure

- **Alta disponibilidade**: Recursos que estarão sempre disponíveis, vinculados a um SLA.
- **Autenticação global**: Serviços como o AD (Active Directory), que são nativos da nuvem, garantem a autenticação do usuário. Em caso de indisponibilidade além do SLA acordado, o cliente recebe vouchers para compensar o tempo de inatividade.

## Escalabilidade e Elasticidade

- **Escalabilidade**: Ajusta a capacidade do ambiente para atender a demanda. Se o uso for baixo, ajusta-se para reduzir custos.
- **Elasticidade**: Permite expandir os recursos conforme necessário, como em eventos sazonais ou promoções (ex: DIO), podendo adicionar servidores, máquinas virtuais, memória, etc.

## Confiabilidade, Previsibilidade e Segurança

- **Confiabilidade**: Sistemas que continuam funcionando mesmo em caso de falhas. A Microsoft disponibiliza esses recursos em várias localizações.
- **Previsibilidade**: Está diretamente ligada à confiança, permitindo que os clientes confiem no ambiente da Microsoft.
- **Segurança**: A Microsoft oferece várias ferramentas de segurança, mas a responsabilidade sobre a segurança final não é dela. O provedor deve fornecer um modelo claro de quem faz o quê no ambiente Azure, cabendo ao cliente aplicar os recursos corretamente.

## Governança e Gerenciabilidade

- **Governança**: Ferramentas de auditoria de nuvem permitem corrigir irregularidades. Há regras corporativas e governamentais que precisam ser seguidas.
- **Gerenciabilidade**: Um dos maiores benefícios da nuvem é a capacidade de gerenciar recursos de forma eficiente. O Terraform, por exemplo, é uma ferramenta muito utilizada, embora não seja da Microsoft, e auxilia na criação de implantações em larga escala. A automação de recursos é fundamental para otimizar operações.

# Revisão dos Benefícios da Nuvem Azure

Revisamos os seguintes pontos:

- Alta disponibilidade e escalabilidade.
- Confiabilidade e previsibilidade.
- Segurança e governança.
- Capacidade de gerenciamento.

# Materiais Complementares

Os materiais complementares têm o objetivo de fornecer informações que facilitam o aprendizado. Links úteis (como slides, repositórios e páginas oficiais) serão disponibilizados, além de dicas sobre como se destacar na DIO e no mercado de trabalho.

# Dicas/Links Úteis

Disponibilizamos alguns links para que você possa se aprofundar nas tecnologias e participar de fóruns de discussão relevantes:

- **Artigos/Fóruns**: Compartilhe seus conhecimentos técnicos ou suas dúvidas na plataforma da DIO.
- **Rooms**: Em Bootcamps, você pode acessar o Rooms, um chat em tempo real para discutir dúvidas e compartilhar dicas.
- **Pesquisa na Web**: Se não encontrar algo na DIO, busque em outras fontes, como o Google ou StackOverflow, que podem ajudar a solucionar dúvidas.

-------------------------------------------------------------------------------

## Criando Máquinas Virtuais no Azure

- Foram explicados os benefícios de utilizar a nuvem, com uma tabela ilustrando os SLAs disponíveis.
- Ao criar uma máquina virtual (VM), é essencial definir o escopo e determinar o tempo que o recurso pode ficar indisponível, para escolher o SLA adequado.
- Foi apresentada uma estratégia para entender o tempo de inatividade de um recurso: quanto maior o nome do SLA, menor será o tempo de indisponibilidade, e quanto menor o nome, maior será esse tempo.
- Detalhou-se a importância de explorar as opções e entender melhor cada uma delas.
- Além disso, foi explicado como a replicação de VMs afeta o SLA, a disponibilidade e outros fatores importantes.

  ------------------------------------------------------------------------------

  # Tipos de Serviço de Nuvem na Azure

## IaaS, PaaS e SaaS na Azure

### IaaS - Infraestrutura como Serviço:
- Administradores têm acesso amplo e executam uma variedade de serviços.
- Responsáveis por configurar e manter toda a infraestrutura.

### PaaS - Plataforma como Serviço:
- Os administradores focam apenas no software; a Microsoft cuida do hardware.
- Ambiente otimizado para desenvolvimento, teste e implantação de aplicações, sem a necessidade de gerenciar a infraestrutura subjacente.

### SaaS - Software como Serviço:
- Exemplo: Microsoft Teams e Office 365.
- Usuários acessam aplicativos via subscrição, com o provedor de serviços gerenciando toda a infraestrutura e plataforma.

## Modelo de Responsabilidade Compartilhada

- **On-premise:** O cliente é responsável por tudo.
- **SaaS:** O oposto de IaaS, com mínima responsabilidade do cliente sobre a infraestrutura.

### IaaS:
- Mais flexível entre os serviços de nuvem.
- Permite aos usuários configurar e gerenciar o hardware necessário para suas aplicações.

### PaaS:
- Concentra-se no desenvolvimento de aplicativos.
- Gerenciamento da plataforma realizado pelo provedor de nuvem.

### SaaS:
- Modelo de pagamento baseado no uso.
- Os usuários pagam pelo software que utilizam, geralmente através de uma assinatura.

## Revisão dos Tipos de Serviço de Nuvem
Recapitulação do que foi ensinado nos módulos anteriores, consolidando o entendimento sobre a infraestrutura, plataforma e software como serviços na nuvem.

# Materiais Complementares

Nossos materiais complementares e de apoio têm como objetivo apresentar informações para facilitar e enriquecer a sua jornada de aprendizado. Para isso, links úteis (como slides, repositórios e páginas oficiais) serão disponibilizados, além de dicas sobre como se destacar na DIO e no mercado de trabalho 😉.

## Slides

- Tipos de serviço de nuvem
- Tipos de serviço de nuvem - Revisão

## Dicas/Links Úteis

Por fim, disponibilizamos alguns links úteis para que você possa se desenvolver ainda mais através de referências oficiais das tecnologias, páginas de documentação e/ou fóruns de discussão relevantes. Nesse contexto, seguem algumas sugestões:

- **Artigos/Fórum:** você pode compartilhar conteúdos técnicos através de Artigos (visíveis globalmente na plataforma da DIO). Por outro lado, você também pode compartilhar suas conquistas e dúvidas usando os Fóruns (que são específicos para cada experiência educacional na DIO, como um Bootcamp por exemplo).
- **Rooms:** caso você esteja inscrito(a) em uma experiência educacional na DIO (como um Bootcamp, por exemplo), você terá acesso ao Rooms. O Rooms é uma ferramenta de bate-papo em tempo real onde todos os inscritos podem interagir, compartilhando dúvidas e dicas (que podem conter imagens e snippets de código-fonte).
- **Pesquise na Web:** pode parecer óbvio, mas é importante frisar a importância das engines de busca no dia-a-dia de um profissional de TI. Caso não encontre o que procura dentro da DIO, pesquise sobre o assunto (conceito, dúvida, erro etc) na Internet (dê um Google), pois na maioria das vezes você será levado a páginas incríveis como o StackOverflow que salvarão o seu dia 😎.


