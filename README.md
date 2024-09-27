# 🌐 Resumo Laboratório Azure - AZ-900 - Módulo 1️⃣

## 🏫 Aula: Localizando Serviços por Categoria
### 🔖 Conteúdo: Computação em Nuvem

* Os recursos da conta de "usuário" são os mesmos disponíveis para contas "corporativas" 🔄
* O portal possui configurações básicas, como, por exemplo, personalização de idioma e aparência 🎨.

#### 📊 Opções do Painel (barra lateral esquerda)
* Seleção de todos os serviços disponíveis no Azure, separados por categorias:
  * ☁️ Exemplos: Computação, Armazenamento, Rede

> ⚠️ Serviços marcados com versão prévia são versões de teste que estão em avaliação para se manterem efetivamente na plataforma. (não são garantidos)

 
### <p align="center"> 📚 A computação em nuvem é uma matéria mandatória para um bom profissional de TI!</p>



## 🏫 Aula: Benefícios da Nuvem Azure

### 🔖 Conteúdo: Disponibilidade

#### ALTA DISPONIBILIDADE - Serviços sempre funcionando quando necessário (SLA). 🤝
* Caso não atendido, o cliente recebe um crédito correspondente a uma indenização. 💰
* Em casos de indisponibilidade, as organizações contratantes do serviço não podem atuar, apenas recebem uma previsão para regularização da situação. ⏲️

### 🔖 Conteúdo: Escalabilidade e Elasticidade

#### ESCALABILIDADE - Possibilidade de adicionar mais recursos para atender ao aumento de demandas. ⛰️
* Paga-se apenas pelo necessário. 🐖 💸
* Se a demanda diminui, os recursos podem ser reduzidos. ⤵️

#### ELASTICIDADE - Possibilidade de adicionar recursos automaticamente ou manualmente em caso de crescimento repentino e acentuado de demanda. 🏔️
* Solicitação de aumento de recursos por envio de requisições condicionais. 🛒 🧠
* Em contrapartida, os recursos podem ser desativados quando há queda na demanda. 🔽

### 🔖 Conteúdo: Confiabilidade, Previsibilidade e Segurança

#### CONFIABILIDADE - Resiliência devido ao design descentralizado. 🗺️
* A nuvem permite que os recursos sejam implantados em várias regiões do mundo. 🌎 🌍 🌏

#### PREVISIBILIDADE - Permite avançar com confiança no desempenho e/ou no custo (Microsoft Azure Well-Architected Framework). 🦸‍♂️
* Casos de sucesso. 🏆

#### SEGURANÇA - A nuvem oferece as ferramentas, mas o cliente deve saber como implementá-las. 🦺
* No nível máximo de segurança, a infraestrutura fornecerá os recursos físicos, mas o usuário poderá gerenciar os sistemas instalados. ⚙️
* Para a aplicação de patches e manutenção automática, plataformas ou software como serviço podem ser as melhores estratégias. 🤖

### 🔖 Conteúdo: Governança e Gerenciabilidade

#### GOVERNANÇA - Auditoria de nuvem que sinaliza inconformidades com os padrões da organização. 🔎
* Fornece estratégias de mitigação. 🧰
* Patches de software, aplicados automaticamente, também ajudam nesse quesito. 💁‍♂️

#### GERENCIABILIDADE - Opções de capacidade de gerenciamento. 👨‍💼
* Exemplos:
  * Utilizar modelo pré-configurado do portal, removendo a necessidade de configuração manual; 🎛️
  * Utilização de APIs; 🔌
  * Utilização do PowerShell. ⚙️💻
  * 
  ## 🏫 Aula: Criando Máquinas Virtuais na Azure

### 🔖 Conteúdo: Beneficios da Nuvem - Laboratório

#### SLAs 🤝
* 99% = 1,68 horas de inatividade por semana.
* 99,9% = 10,1 minutos de inatividade por semana.
* 99,95% = 5 minutos de inatividade por semana.
* 99,99% = 1,01 minutos de inatividade por semana.
* 99,999% = 6 segundos de inatividade por semana.
> Caso não atendido, o cliente recebe um voucher com crédito correspondente a uma indenização.

> Recursos criados com mais 'noves' possuem menos tempo de inatividade.
 
> As opções de gerenciamentam e outras configurações refletem no percentual do SLA.
> 
## 🏫 Aula: Tipos de Serviço de Nuvem na Azure

### 🔖 Conteúdos: IaaS, PaaS e Saas na Azure | Modelo de Responsabilidade Compartilhada

#### IaaS - Infraestrutura como serviço. 💻
* Muito utilizado. 🎆
* Entre os recursos temos: Servidores e armazenamento, Firewalls/segurança de rede, Planta fisica/data center. 🏗️
* O cliente tem mais responsabilidade de acessos. ↗️⚙️
* Mais flexibilidade para personalizar o recurso final. 🔆

#### PaaS - Plataforma como serviço. 🧰
* Engloba os recursos de infraestrutura somados à: Sistemas operacionais e Ferramentas para desenvolvedores, Analise de Negócios de gerenciamento de database. 💻💻💻🔆
* Nesse cenário o cliente está focado nas aplicações. O servidor e maquinas não são importantes. 👀
* Fornece um ambiente sem focar no gerenciamento da infraestrutura subjacente. 🌴
* O gerenciamento de plataforma é realizado pelo provedor de nuvem. 🌩️

#### SaaS - Software como serviço. 💿
* Engloba os recursos de infraestrutura e plataforma somados à: Aplicativos e Apps hospedados. ☁️ 📱 ☁️
* O cliente tem menos responsabilidade de acessos. ↙️⚙️
* O que determina os acessos são os modelos de licenciamento. 🥇 🥈 🥉
* Modelo de preço de pagamento conforme o uso. 💸

#### Modelo de Responsabilidade Compartilhada.
![Modelo](https://github.com/thiagofs84/Res_Lab_Azure/blob/main/Capturar.JPG)


> As nomenclaturas Iaas, PaaS e Saas não são exclusivos da Azure, são contextos genéricos de núvem.
