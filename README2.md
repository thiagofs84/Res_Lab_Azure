# 🌐 Resumo Laboratório Azure - AZ-900 - Módulo 2️⃣ - Arquitetura e Serviços Azure

## 🏫 Aula: Componentes de Arquitetura do Azure
### 🔖 Conteúdo: Componentes de Arquitetura do Azure

* REGIÕES: Ao criar um recurso no Azure, é necessário indicar o local em que ele deve ficar 🗺️.
  * Quanto mais perto o recurso estiver do local físico, menor será o delay da informação. 🌩️⏲️
  * As tarifas variam de acordo com a região. 💸
  * Alguns recursos estão disponíveis em determinadas regiões. 🛍️
* O Azure está presente em mais de 60 regiões correspondentes a mais de 140 países. 🌍
* As regiões são compostas de um ou mais datacenters muito próximos. 🏢💻 [Zona de Disponibilidade]

<h1 align="center"> ☁️🗄️💻 ↔️ ☁️🗄️💻 ↔️ ☁️🗄️💻 </h1>

* Cada datacenter é equipado com alimentação, resfriamento e rede independentes. 🔌🧊🕸️

### 🔖 Conteúdo: Entendendo Pares de Região e Grupos de Recursos

* PARES DE REGIÃO: Cada região possui uma região par que será acessada caso a região original seja impactada. 🌍🤝
  * Há cenários com replicação automática para alguns serviços. 🔄⚙️
    * [Regiões Pares](https://aka.ms/PairedRegions-ptb)

![Pares de Região](https://github.com/thiagofs84/Res_Lab_Azure/blob/main/Regi%C3%B5es.PNG)

* REGIÕES SOBERANAS DO AZURE: Regiões exclusivas de governos (atualmente EUA e China). 🛡️🌐
  * Inacessíveis para usuários não autorizados. 🚫
    * Serviços Governamentais dos EUA - Voltado às necessidades de segurança e conformidade das agências federais. 🗽🛡️
    * Azure China - A Microsoft é o 1º provedor estrangeiro de serviços de nuvem pública na China, fisicamente separado dos serviços de nuvem. (21Vinet) 🇨🇳🎖️

   * RECURSOS DO AZURE: Componentes como armazenamento, máquinas virtuais e redes disponíveis para soluções de nuvem. ☁️💾
     * Ao criar uma máquina virtual, por exemplo, é importante organizar os respectivos recursos - [criar grupo de recursos] 🗃️
       * Os recursos podem existir em apenas um grupo e em diferentes regiões. 🌐
       * Podem ser movidos 🔀
       * Os aplicativos podem utilizar vários grupos de recurso. 📦

### 🔖 Conteúdo: Assinatura da Azure e Grupos de Gerenciamentos

* ASSINATURA DO DESENVOLVIMENTO 🔑⚙️
* ASSINATURA DO TESTE 🔑🧪
* ASSINATURA DA PRODUÇÃO 🔑🕴️

> ❗ Uma conta pode ter diversas assinaturas, mas uma assinatura está associada apenas a uma conta. 🧾

  * As assinaturas do Azure permitem gerenciar limites de cobrança e controles de acesso. 🧑‍💻🔐

* GRUPOS DE GERENCIAMENTO
  * Regras padrões para gerenciar assinaturas. 📑⚙️

## 🏫 Aula: Computação e Rede na Azure
* TIPOS DE COMPUTAÇÃO: 🖱️💻
* HOSPEDAGEM DE APLICATIVOS: 🏨🖥️
* REDES VIRTUAIS: 🕸️☁️

### 🔖 Conteúdo: Serviços de Computação e Máquinas Virtuais do Azure

* SERVIÇOS DE COMPUTAÇÃO DO AZURE: Serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais. 🖥️⚡
  * Exemplos → Máquinas Virtuais, Serviços de Aplicativos, Instâncias de Contêineres, Serviços de Kubernetes, Área de Trabalho Virtual. 💻☁️
* MÁQUINAS VIRTUAIS DO AZURE: São emulações de software de computadores físicos que incluem processador virtual, memória, armazenamento e rede. 💻💾
* CONJUNTOS DE DIMENSIONAMENTO DE VMs: Oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente. ⚖️🤖

### 🔖 Conteúdo: Conjuntos de Disponibilidade de Máquinas Virtuais do Azure

* Estratégia para configurar a VM em racks diferentes.
  * Cada rack é chamado de domínio de falha. 🖥️🔧
  * As VMs são distribuídas em domínios de atualização. 🔄💡

### 🔖 Conteúdo: Área de Trabalho Virtual e Contêineres do Azure

* ÁREA DE TRABALHO VIRTUAL: Executa aplicativos completos através da nuvem. ☁️💻
* SERVIÇOS DE CONTÊINERES DO AZURE: Fornecem um ambiente leve e virtual que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda. 🧑‍💻🛠️
  * Instâncias de Contêiner - Oferta PaaS executado no Azure. 🛳️☁️
  * Aplicativos de Contêiner - Oferta PaaS que pode balancear a carga e escalar. ⚖️🚀
  * Serviço de Kubernetes do Azure: Um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres. 🧩🐳

### 🔖 Conteúdo: Azure Functions e Serviços de Aplicativo do Azure

* AZURE FUNCTIONS: Oferta PaaS que dá suporte a operações de computação sem servidor. 🖥️🎛️
  * Baseado em eventos, não exige infraestrutura de servidor durante períodos inativos. 😴
    * As 'Azure Functions' são modelos de execução baseados em eventos e são dimensionadas automaticamente com base na demanda. 🤖🔄

#### Comparação de opções de computação do Azure

> **MÁQUINAS VIRTUAIS**
> * Servidor baseado em nuvem que dá suporte a ambientes Windows ou Linux. 💻
> * Útil para migrações de "lift-and-shift" para a nuvem. ☁️
>   * Exemplo: levar um data center para o ambiente de nuvem exatamente como está configurado no ambiente físico.
> * Pacote completo do sistema operacional. 📦
>
> **ÁREA DE TRABALHO VIRTUAL**
> * Fornece uma experiência de área de trabalho do Windows baseada em nuvem. 🖥️💨
> * Aplicativos dedicados para conexão ou acessíveis de qualquer navegador moderno. 🌐
>
> **CONTÊINERES**
> * Ambiente leve, adequado para microsserviços. 🧩
> * Projetado para escalabilidade e resiliência com orquestração (AKS-Azure Kubernets Service). ⚙️
>
> **SERVIÇOS DE APLICATIVOS**
> * Plataforma totalmente gerenciada para criar e implantar rapidamente aplicativos web e APIs. 🌐🚀
> * Suporta .NET, ,NET Core, Node.js, Java, Python ou php. 💻🔧

* **SERVIÇOS DE REDE DO AZURE**
  * A REDE VIRTUAL do AZURE (VNet) permite que os recursos do Azure se comuniquem entre si, com a Internet e redes locais. 🌐💬
    * As sub-redes virtuais segmentam a rede conforme as necessidades. 🕸️📶
    * O emparelhamento de rede conecta redes privadas diretamente. 🔗
      * Ao criar uma máquina virtual, ela precisa ter um IP, o IP vai ser de uma sub-rede que responde para uma VNet.
  * **GATEWAY DE VPN**: Usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela Internet pública. 🔒🌍
  * **EXPRESSROUTE**: Comunicação direta, via cabo, ligando o data center da empresa até o da Microsoft, proporcionando mais performance e segurança. 🚀🔗
  * **DNS DO AZURE**: Baseado no gerenciador de recursos do Azure, permite controle de acesso baseado em função e monitoramento de logs. 🛠️📝
    * Suporta nomes de domínio privados e personalizados nas redes virtuais. 🌐🔧

