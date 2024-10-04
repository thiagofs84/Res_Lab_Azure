# 🌐 Resumo Laboratório Azure - AZ-900 - Módulo 2️⃣ - Arquitetura e Serviços Azure

## 🏫 Aula: Componentes de Arquitetura do Azure
### 🔖 Conteúdo: Componentes de Arquitetura do Azure

* REGIÕES: Ao criar um recurso no Azure é necessário indicar o local em que ele deve ficar 🗺️
  * Quanto mais perto o recurso estiver do local fisico menor será o delay da informação. 🌩️⏲️
  * As tarifas variam de acordo com a região. 💸
  * Alguns recursos estão disponiveis em determinadas regiões. 🛍️
* O Azure está presente em mais de 60 regiões correspondentes a mais de 140 paises. 🌍
* As regiões são compostas de um ou mais datacenters muito próximos. [zona de disponibilidade]

<h1 align="center"> ☁️🗄️💻 ↔️ ☁️🗄️💻 ↔️ ☁️🗄️💻 </h1>

* Cada datacenter é equipado com alimentação, resfriamento e rede independentes. 🔌 🧊 🕸️
 
### 🔖 Conteúdo: Entendendo Pares de Região e Grupos de Recursos

* PARES DE REGIÃO: Cada região possui uma região par que será acessada caso a região original seja impactada. 🧑‍🤝‍🧑
  * Há cenários com replicação automática para alguns serviços. ⚙️
    * [Regiões Pares](https://aka.ms/PairedRegions-ptb)
   
![Pares de Região](https://github.com/thiagofs84/Res_Lab_Azure/blob/main/Regi%C3%B5es.PNG)

* REGIÕES SOBERANAS DO AZURE: Regiões exclusivas de governos (atualmente EUA e China). 🧑‍🤝‍🧑
  * Inacessíveis para usuários não autorizados.
    * Serviços Governamentais dos EUA - Voltado  às necessidades de segurança e conformidade das agencias federais. 🗽
    * Azure China - A Microsoft é o 1º provedor estrangeiro de serviços de nuvem pública na China. (fisicamente separada dos serviços de nuvem - 21Vinet) 🎖️
   
   * RECURSOS DO AZURE: Componentes como armazenamento, máquinas virtuais e redes disponíveis para soluções de nuvem. ☁️
     * Ao criar uma maquina virtual por exemplo é importante organizar os respectivos recursos - [criar grupo de recursos] 🗃️
       * Os recursos podem existir em apenas um grupo e em diferentes regioes.
       * Podem ser movidos
       * Os aplicativos podem utilizar varios grupos de recurso.
      
### 🔖 Conteúdo: Assinatura da Azure e Grupos de Gerenciamentos

* ASSINATURA DO DESENVOLVIMENTO 🔑⚙️
* ASSINATURA DO TESTE 🔑🧪
* ASSINATURA DA PRODUÇÃO 🔑🕴️

> ❗ Uma conta pode ter diversas assinaturas mas uma assinatura está associada apenas a uma conta.

  * As assinaturas do Azure permitem gerenciar limites de cobrança e controles de acesso

* GRUPOS DE GERENCIAMENTO
  * Regras padrões para gerenciar assinaturas
 
 ## 🏫 Aula: Computação e Rede na Azure
### 🔖 Conteúdo: Serviços de Computação e Máquinas Virtuais do Azure

* SERVIÇOS DE COMPUTAÇÃO DO AZURE: serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rde e sistemas operacionais.
  * Exemplos → Virtual Virtuais, Aplicativo Serviços, Contêiner Instancias  Serviços de Kubernetes do Azure, Area de Trabalho Virtual do Azure.
* MÁQUINAS VIRTUAIS DO AZURE: são emulações de software de computadores fisicos que incluem processador virtual, memória, armazenamento e rede 💻
* CONJUNTOS DE DIMENSIONAMENTO DE VMs: oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente. ⚖️⚙️

### 🔖 Conteúdo: Conjuntos de Disponibilidade de Máquinas Virtuais do Azure

* Estratégia para configurar a VM em racks diferentes.
  * Cada rack é chamado de dominio de falha;
  * As VMs são distribuidas em dominios de atualização.
 
 ### 🔖 Conteúdo: Área de Trabalho Virtual e Contêineres do Azure

* ÁREA DE TRABALHO VIRTUAL: Executa aplicativos completos através da nuvem. ☁️
* SERVIÇOS DE CONTÊINERES DO AZURE: fornecem um ambiente leve e virtual que não exige o gerenciament do sistema operacional e pode responder a alterações sob demanda.
  * Instancias de contêiner - oferta PaaS executado no azure
  * Aplicativos de conteiner - oferta PAaS que pode balancear a carga e escalar.
  * Serviço de Kubernetes do Azure: um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres.
* 
