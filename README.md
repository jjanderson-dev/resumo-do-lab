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


-------------------------------------------------------------------------------------------------------------------------------------------

### Módulo 2: Componentes de Arquitetura do Azure

#### **Regiões:**
- As regiões do Azure são locais estratégicos onde os recursos são alocados, garantindo melhor desempenho e custo otimizado ao estar próximo do usuário.
- Cada região é composta por um ou mais datacenters interconectados, proporcionando escalabilidade e flexibilidade.
- As regiões ajudam a reduzir a latência, melhorando a experiência do cliente.
- As regiões também garantem a conformidade com normas, preservando a residência dos dados de acordo com regulamentações locais.
- Não há um preço fixo para todos os recursos, e nem todos estão disponíveis em todas as regiões.
- O Azure tem uma abrangência global, possibilitando alcance mundial.
- É importante verificar a LGPD para garantir que os dados não sejam transferidos para fora do Brasil sem conformidade.

#### **Zona de Disponibilidade:**
- Ambientes com alta disponibilidade tendem a ser mais caros, mas oferecem maior resiliência.
- Caso ocorra uma falha em uma única zona de disponibilidade, a rede pode ficar indisponível.
- É possível implementar redundância por meio de datacenters ou outros métodos de segurança (como hacks).

#### **Assinaturas:**
- O Azure permite múltiplas assinaturas, divididas em categorias como desenvolvimento, teste e produção.
- Uma única conta pode ter diversas assinaturas, mas cada assinatura está vinculada a uma única conta.
- Uma estratégia recomendada é criar assinaturas separadas para cada projeto, facilitando o controle financeiro e o gerenciamento de recursos.
- Todas as assinaturas de uma conta respondem a um único proprietário.

#### **Grupos de Gerenciamento:**
- Grupos de gerenciamento permitem a aplicação de regras e políticas uniformes para várias assinaturas ao mesmo tempo, facilitando a administração.

#### **Recapitulando:**
- As regiões e pares de regiões do Azure garantem disponibilidade global.
- As zonas de disponibilidade e datacenters garantem resiliência.
- Recursos e grupos de recursos organizam a infraestrutura.
- Assinaturas e grupos de gerenciamento estruturam e facilitam a administração dos ambientes.

---

### Materiais Complementares:
Nossos materiais de apoio visam complementar seu aprendizado, oferecendo recursos como slides, repositórios e links para páginas oficiais. Além disso, incluímos dicas sobre como se destacar na DIO e no mercado de TI. 😎

**Slides:**
- [Componentes de arquitetura do Azure](#)
- [Componentes de arquitetura do Azure - Revisão](#)

### Dicas/Links Úteis:
- **Artigos/Fórum:** Compartilhe seus conhecimentos técnicos em artigos, visíveis globalmente na plataforma da DIO, ou use os fóruns para esclarecer dúvidas específicas de experiências como bootcamps.
- **Rooms:** Se você está inscrito em uma experiência como bootcamp, pode participar dos Rooms, um espaço de bate-papo em tempo real onde os inscritos trocam informações, dicas e até mesmo código.
- **Pesquisa na Web:** Utilizar motores de busca, como o Google, pode ser essencial para solucionar problemas e aprofundar conhecimentos. Plataformas como o StackOverflow são fontes valiosas para esclarecer dúvidas técnicas.

-------------------------------------------------------------------------------------------------------------

## Computação e Rede
- Tipos de computação
- Hospedagem de aplicativos
- Redes Virtuais

## Serviços de Computação
- O Azure oferece serviços de computação sob demanda, fornecendo recursos como discos, processadores, memórias, armazenamento e sistemas operacionais.

## Máquinas Virtuais no Azure
- As VMs (Virtual Machines) são emulações de computadores físicos.
- Incluem processador virtual, memória, armazenamento e rede.
- Oferecem IaaS (Infraestrutura como Serviço) com personalização e controle total.

## Conjuntos de Dimensionamento de VMs
- Permitem o balanceamento de carga e o dimensionamento automático dos recursos.

## Conjuntos de Disponibilidade de VMs
- Dentro de um Data Center, há vários racks, e em cada rack, diversas VMs.

## Área de Trabalho do Azure
- A virtualização da área de trabalho e dos aplicativos é executada na nuvem.
- Reduz os riscos de ambientes legados.
- Cria um ambiente completo de virtualização da área de trabalho sem necessidade de servidores adicionais de gateway.
- Suporta várias sessões reais simultaneamente.

## Serviços de Contêineres do Azure
- Os contêineres oferecem um ambiente leve e virtualizado que não requer gerenciamento do sistema operacional e se adapta a alterações sob demanda.
- O Azure é compatível com Docker e fornece diversos serviços de contêineres.

### Ofertas Relacionadas:
- **Instâncias de Contêiner do Azure**: Um serviço de PaaS (Plataforma como Serviço) que executa contêineres ou PODs.
- **Aplicativos de Contêiner do Azure**: Outro serviço PaaS que facilita o balanceamento de carga e escalabilidade.
- **Serviço de Kubernetes do Azure**: Gerenciamento e orquestração de grandes volumes de contêineres em uma arquitetura distribuída.
- **Azure Functions**: PaaS para operações de computação sem servidor, executando código sob demanda sem infraestrutura contínua.

## Comparações de Computação no Azure
- **Máquinas Virtuais (VMs)**
  - Suportam ambientes Windows e Linux.
  - Adequadas para migrações "lift-and-shift", levando sistemas off-line diretamente para a nuvem.
  
- **Área de Trabalho Virtual**
  - Fornece uma experiência de desktop Windows na nuvem, com aplicativos acessíveis de navegadores modernos.
  - Suporta logon de múltiplos usuários no mesmo sistema simultaneamente.

- **Contêineres**
  - Ambientes leves, ideais para execução de microserviços.
  - Projetados para escalabilidade e resiliência por meio de orquestração.
  - Vários contêineres podem ser executados em um único sistema operacional host.

- **Serviços de Aplicativos do Azure**
  - Plataforma gerenciada para criar, implantar e escalar aplicativos web e APIs.
  - Suporta .NET, Node.js, Java, Python e PHP.
  - Oferece desempenho, segurança e conformidade de nível corporativo.

## Serviços de Rede do Azure
- A rede virtual do Azure, chamada **VNet**, permite a comunicação entre recursos do Azure, internet e redes locais.
- Possui pontos de extremidade públicos (acessíveis pela internet) e privados (acessíveis apenas internamente).
- VNETs são isoladas por padrão, mas podem ser configuradas para comunicação entre si.
- Sub-redes virtuais permitem segmentação da rede conforme necessário.
- Emparelhamento de rede conecta redes privadas diretamente.

### Gateway de VPN
- Envia tráfego criptografado entre uma rede virtual do Azure e uma rede local pela internet pública.
- **ExpressRoute**: Extensão de redes locais ao Azure por meio de uma conexão privada fornecida por um provedor de conectividade.

### DNS do Azure
- Aproveita uma rede global de servidores para fornecer serviços DNS confiáveis com suporte à rede **Anycast**.
- A segurança do DNS é gerenciada por controle de acesso baseado em função, com monitoramento e registro.
- O serviço DNS do Azure facilita o gerenciamento de recursos internos e externos.
- Redes virtuais podem ter domínios privados e totalmente personalizáveis.
- Suporta registros de alias para apontar diretamente para recursos no Azure.

## Resumo do Módulo:
- Tipos de computação, instâncias de contêiner, máquinas virtuais e funções.
- Hospedagem de aplicativos, incluindo aplicativos web, contêineres e VMs no Azure.
- Redes virtuais, sub-redes, emparelhamento de rede, DNS, Gateway de VPN e ExpressRoute.

---

## Materiais Complementares
Nossos materiais complementares e de apoio têm como objetivo apresentar informações para facilitar e enriquecer a sua jornada de aprendizado. Para isso, links úteis (como slides, repositórios e páginas oficiais) serão disponibilizados, além de dicas sobre como se destacar na DIO e no mercado de trabalho 😉.

### Slides
- [Computação e rede](#)
- [Computação e rede - Revisão.pptx](#)

### Dicas/Links Úteis

Por fim, disponibilizamos alguns links úteis para que você possa se desenvolver ainda mais através de referências oficiais das tecnologias, páginas de documentação e/ou fóruns de discussão relevantes. Nesse contexto, seguem algumas sugestões:

- **Artigos/Fórum**: você pode compartilhar conteúdos técnicos através de Artigos (visíveis globalmente na plataforma da DIO). Por outro lado, você também pode compartilhar suas conquistas e dúvidas usando os Fóruns (que são específicos para cada experiência educacional na DIO, como um Bootcamp por exemplo).
  
- **Rooms**: caso você esteja inscrito(a) em uma experiência educacional na DIO (como um Bootcamp, por exemplo) você terá acesso ao Rooms. O Rooms é uma ferramenta de bate-papo em tempo real onde todos os inscritos podem interagir, compartilhando dúvidas e dicas (que podem conter imagens e snippets de código-fonte).

- **Pesquise na Web**: pode parecer óbvio, mas é importante frisar a importância das engines de busca no dia-a-dia de um profissional de TI. Caso não encontre o que procura dentro da DIO, pesquise sobre o assunto (conceito, dúvida, erro etc) na Internet (dê um Google), pois na maioria das vezes você será levado à páginas incríveis como o StackOverflow que salvarão o seu dia 😎.

-----------------------------------------------------------------------------------------------------


## Contas de Armazenamento

- O nome da conta deve ser globalmente exclusivo.
- Oferece acesso à internet em escala mundial.
- Define os serviços de armazenamento e as opções de redundância.

## Redundância e Serviços de Armazenamento

- **LRS (Locally Redundant Storage)**: Armazenamento com redundância local.
- **ZRS (Zone-Redundant Storage)**: Armazenamento com redundância de zona.
- **GRS (Geo-Redundant Storage)**: Armazenamento com redundância geográfica.
- **GZRS (Geo-Zone Redundant Storage)**: Armazenamento com redundância de zona geográfica.

## Serviços de Armazenamento do Azure

- **Blob do Azure**: Otimizado para o armazenamento de grandes volumes de dados não estruturados, como texto e dados binários.
- **Disco do Azure**: Fornece discos para uso por máquinas virtuais, aplicativos e outros serviços.
- **Fila do Azure**: Serviço de armazenamento de mensagens que permite o armazenamento e a recuperação de grandes volumes de mensagens, com tamanho de até 64 KB por mensagem.
- **Arquivos do Azure**: Configura um compartilhamento de arquivos de rede altamente disponível, acessível via protocolo SMB (Server Message Block).
- **Tabelas do Azure**: Oferece uma solução para armazenamento de dados estruturados não relacionais, com um design flexível e sem esquema.

## Pontos de Extremidade Públicos dos Serviços de Armazenamento

Os pontos de extremidade públicos são URLs que permitem acessar os serviços de armazenamento do Azure pela internet. Cada serviço de armazenamento disponibiliza um ponto de extremidade público específico, permitindo que aplicativos e usuários se conectem diretamente ao recurso de armazenamento via HTTP ou HTTPS. Abaixo estão os principais tipos de pontos de extremidade disponíveis no Azure:

- **Armazenamento de Blobs**: O ponto de extremidade público para o serviço de blobs permite armazenar e recuperar dados não estruturados, como imagens, vídeos ou arquivos de log. É ideal para o armazenamento de grandes volumes de dados e pode ser acessado globalmente.
  - Exemplo de ponto de extremidade: `https://<nome-da-conta>.blob.core.windows.net`

- **Data Lake Storage Gen2**: Fornece armazenamento otimizado para grandes volumes de dados analíticos. O ponto de extremidade para o Data Lake Storage Gen2 suporta fluxos de dados altamente paralelizados e grandes conjuntos de dados para fins de análise avançada.
  - Exemplo de ponto de extremidade: `https://<nome-da-conta>.dfs.core.windows.net`

- **Arquivos do Azure**: Este ponto de extremidade oferece acesso a um compartilhamento de arquivos em nuvem que pode ser montado localmente ou na nuvem usando o protocolo SMB. É uma solução excelente para migrar ou compartilhar arquivos entre diferentes sistemas.
  - Exemplo de ponto de extremidade: `https://<nome-da-conta>.file.core.windows.net`

- **Armazenamento de Filas**: O ponto de extremidade para o armazenamento de filas é utilizado para processar grandes volumes de mensagens de forma assíncrona. Cada mensagem pode ter até 64 KB de tamanho, e as filas são acessíveis de maneira segura via internet.
  - Exemplo de ponto de extremidade: `https://<nome-da-conta>.queue.core.windows.net`

- **Armazenamento de Tabelas**: O ponto de extremidade para o armazenamento de tabelas é usado para armazenar grandes quantidades de dados estruturados não relacionais. Ele permite o acesso rápido a dados organizados no formato chave-atributo, ideal para aplicativos com alto desempenho e escalabilidade.
  - Exemplo de ponto de extremidade: `https://<nome-da-conta>.table.core.windows.net`

### Considerações de Segurança para Pontos de Extremidade Públicos

Embora os pontos de extremidade públicos ofereçam grande flexibilidade e acessibilidade, é fundamental garantir que o acesso a eles seja seguro. A seguir estão algumas recomendações:

- **Autenticação e Autorização**: Utilize os mecanismos de autenticação do Azure, como SAS (Shared Access Signatures) e Azure Active Directory (Azure AD), para controlar quem pode acessar os dados.
- **Protocolo HTTPS**: Sempre que possível, utilize HTTPS para proteger os dados em trânsito e evitar interceptações.
- **Firewall e Rede Virtual**: Configure regras de firewall e redes virtuais no Azure para restringir o acesso aos pontos de extremidade a IPs confiáveis ou locais específicos.
- **Azure Private Link**: Para cenários que exigem mais segurança, você pode configurar o **Azure Private Link** para limitar o acesso aos serviços de armazenamento exclusivamente através da rede privada, evitando a exposição à internet pública.

## Camadas de Acesso ao Armazenamento no Azure

- **Frequente**: Para dados acessados regularmente.
- **Esporádico**: Para dados acessados ocasionalmente.
- **Frio**: Para dados raramente acessados, mas que precisam estar disponíveis.
- **Arquivo Morto**: Para dados que precisam ser arquivados por longos períodos com acesso mínimo.

## Migração para o Azure

- Plataforma de migração unificada.
- Conjunto de ferramentas integradas e autônomas.
- Avaliação e migração de dados.

## Azure Data Box

- Serviço de migração física para transferência de grandes volumes de dados, com capacidade de até 80 TB.
- Ideal para mover backups de recuperação de desastres para o Azure.
- Protege os dados em trânsito em um invólucro robusto.
- Facilita a migração de dados para atender a requisitos de conformidade ou regulamentação.
- Permite a migração de dados para o Azure a partir de locais remotos, com conectividade limitada ou inexistente.

## Opções de Gerenciamento de Arquivos

- **AzCopy**: Utilitário de linha de comando para copiar blobs ou arquivos de ou para a conta de armazenamento, com suporte para sincronização unidirecional.

## Gerenciamento de Armazenamento do Azure

- Interface de usuário semelhante ao Windows Explorer.
- Compatível com Windows, MacOS e Linux.

## Sincronização de Arquivos do Azure

- Sincroniza arquivos locais e do Azure bidirecionalmente.
- A camada de nuvem mantém os arquivos acessados com frequência no local, liberando espaço de armazenamento.

---

## Materiais Complementares

Nossos materiais complementares e de apoio têm como objetivo apresentar informações para facilitar e enriquecer a sua jornada de aprendizado. Para isso, links úteis (como slides, repositórios e páginas oficiais) serão disponibilizados, além de dicas sobre como se destacar na DIO e no mercado de trabalho 😉.

### Slides

- Armazenamento
- Armazenamento - Revisão

### Dicas/Links Úteis

Por fim, disponibilizamos alguns links úteis para que você possa se desenvolver ainda mais através de referências oficiais das tecnologias, páginas de documentação e/ou fóruns de discussão relevantes. Nesse contexto, seguem algumas sugestões:

- **Artigos/Fórum**: Você pode compartilhar conteúdos técnicos através de artigos (visíveis globalmente na plataforma da DIO). Por outro lado, também pode compartilhar suas conquistas e dúvidas usando os fóruns, que são específicos para cada experiência educacional na DIO, como um bootcamp, por exemplo.
- **Rooms**: Caso você esteja inscrito(a) em uma experiência educacional na DIO (como um bootcamp, por exemplo), terá acesso ao Rooms. O Rooms é uma ferramenta de bate-papo em tempo real onde todos os inscritos podem interagir, compartilhando dúvidas e dicas (que podem conter imagens e snippets de código-fonte).
- **Pesquise na Web**: Pode parecer óbvio, mas é importante frisar a importância das ferramentas de busca no dia a dia de um profissional de TI. Caso não encontre o que procura dentro da DIO, pesquise sobre o assunto (conceito, dúvida, erro etc.) na Internet. Use o Google, pois muitas vezes você será levado a páginas como o StackOverflow, que podem salvar o seu dia 😎.


-------------------------------------------------------------------------------------------------------------------




