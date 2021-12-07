# Módulo 1 - Descrever os principais conceitos do Azure

# O que aprenderemos?
Depois de concluir este roteiro, aprenderemos sobre:
* Os benefícios da computação em nuvem no Azure e como ela pode poupar tempo e dinheiro
* Conceitos de nuvem, como alta disponibilidade, escalabilidade, elasticidade, agilidade e recuperação de desastre
* Descrever os principais componentes da arquitetura do Azure, como assinaturas, grupos de gerenciamento, recursos e grupos de recursos
* Resumir conceitos de distribuição geográfica, como regiões do Azure, pares de regiões e zonas de disponibilidade

## Áreas de estudo
Os tópicos abaixo são definidos pela própria Microsoft. A porcentagem indica o peso de cada área no exame, assim, quanto maior a porcentagem, maior será a quantidade de questões sobre esse tema.

![image](https://user-images.githubusercontent.com/60825497/145120030-8e49d6ee-61b7-450f-aa10-98985be03607.png)

**Observação:** Para conseguir a certificação, é necessário acertar 70% das questões

# Introdução
O Azure é uma plataforma de computação em nuvem com um conjunto de serviços em constante expansão, projetado para ajudar você a criar soluções e cumprir suas metas de negócios. Os serviços do Azure variam desde serviços Web simples para hospedar a presença de negócios na nuvem, até a execução de computadores totalmente virtualizados para que você execute suas soluções de software personalizadas. O Azure fornece serviços, como: armazenamento remoto, hospedagem de banco de dados e gerenciamento de conta centralizado. O Azure também oferece novas funcionalidades, como a IA e a IoT (Internet das Coisas).

# O que é nuvem?
Computação em nuvem é a entrega de serviços de computação por meio da internet – servidores, armazenamento, banco de dados, redes, software, analytics, inteligência artificial e muito mais. Possibilitando uma inovação mais rápida, recursos flexíveis e economia de escala (O custo unitário tende a ficar mais barato dependendo do volume do negócio – Mais barato se levar mais).

#	Modelos de nuvem
Há três modelos de implantação para a computação em nuvem: nuvem pública, nuvem privada e nuvem híbrida. Cada modelo de implantação tem aspectos diferentes que você deve considerar ao migrar para a nuvem. 
## Nuvem pública - Não significa que é grátis
A nuvem pública pertence ao provedor, e ele é responsável por fornecer recursos e serviços para organizações e usuários. Os serviços são oferecidos pela Internet pública e ficam disponíveis para qualquer pessoa que deseje comprá-los. Alguns recursos de nuvem são: servidores e armazenamento, são de propriedade e operados por um provedor de serviços de nuvem de terceiros e entregues pela Internet.
##	Nuvem privada
Uma nuvem privada consiste em recursos de computação usados exclusivamente por usuários de uma empresa ou organização. Uma nuvem privada pode estar localizada fisicamente no datacenter (local) da organização ou ser hospedada por um provedor de serviços de terceiros.

**Resumidamente:** A nuvem privada pertence e é operada pela organização que utiliza os recursos da nuvem. Para isso, é necessário que a empresa crie um ambiente nuvem em seu datacenter.
##	Nuvem híbrida
É a combinação da nuvem pública e da privada para garantir que a aplicação seja executada no local mais apropriado.

## Em tópicos teríamos:
* Nuvem Pública
    * Fornece recursos e serviços para várias organizações e usuários.
    * Recursos compartilhados entre cliente.
    * Acesso via conexão de rede segura (geralmente pela internet).
    * Cada cliente tem acesso exclusivamente a sua informação, mas o hardware é compartilhado. 
* Nuvem Privada
    * Pertecente e operado pela organização que utiliza os recursos da nuvem.
    * Recursos somente da organização, assim, ela diferencia.
    * As organizações criam um ambiente de nuvem em seus datacenter.
    * Acesso de autoatendimento para calcular recursos fornecidos aos usuários dentro da organização.
    * Organizações responsáveis pela operação dos serviços que prestam.
* Nuvem Híbrida
    * Interliga rede on-promise com a Azure
    * Combina nuvens públicas e privadas para permitir que os aplicativos sejam executados no local mais apropriado
    
## Comparação dos modelos de nuvem
### Nuvem Pública - Opex
*	Nenhuma despesa de capital para escalar verticalmente.
*	Os aplicativos podem ser provisionados e desprovisionados rapidamente.
*	As organizações pagam apenas pelo que utilizam.
*	Não possui completo controle (Controle físico)
*	hardware shared between clients, Azure, Office 365

### Nuvem privada
*	O hardware deve ser comprado para inicialização e manutenção.
*	As organizações têm controle total sobre os recursos e a segurança.
*	As organizações são responsáveis pela manutenção e pelas atualizações de hardware.
*	Controle completo
*	Azure Stack, looks like data center model, hardware used by a single company (company responsible), no access to users outside of the organization

### Nuvem Híbrida
* Fornece a maior flexibilidade (usa pública ou privada)
* As organizações determinam onde executar seus aplicativos.
* As organizações controlam os requisitos de segurança, conformidade ou jurídicos


# Benefícios da nuvem
![alt text](Imagens/CloudBenefits.jpg "Benefícios da nuvem")
## High Avaibility (Alta disponibilidade)
Provedores de nuvem oferecem um Service-level agreement (SLA) isso garante um certo nível de disponibilidade como porcentagem. 
Um SLA geralmente garante um uptime próximo de 100%, mas isso só se aplica a sistemas gerenciados pelo provedor de nuvem.
Dependendo do SLA (Contrato de Nível de Serviço) que você escolher, seus aplicativos baseados em nuvem poderão oferecer uma experiência de usuário contínua, sem tempo de inatividade aparente, mesmo quando as coisas derem errado.	

## Scalability (Escalabilidade)
* Escalabilidade vertical
* Escalabilidade horizontal

## Elasticity (Elasticidade)
## Agility (Agilidade)
## Disaster Recovery (Recuperação de desastre)
## Fault Tolerance - Redundância
## Global Reach (Alcance global)
## Security (Segurança)
## Predictive cost considerations (Considerações de custo preditivo)

# CapEx e OpEx
## Capital Expenditure (CapEx) - Compra de Hardware - On-premises
Gastar com inraestrutura física antecipadamente. Alto custo inicial, o valor de investimento reduz com o tempo.
Alto custo inicial, o valor do investimento reduz com o tempo.

## Operational Expenditure (OpEx)
Gastar em serviços ou produtos, conforme necessário.
Sem custo inicial, pague conforme o uso.

## No Azure usamos somente OpEx?
* Tem pontos particulares, como a instância reservada que pode ser definida por contrato, que é CapEx. 
* Pouquíssimos recursos usam CapEx.
      
Disaster Recovery vs. High Availability vs. Fault Tolerance
 
Elasticity X Scalability: https://www.geeksforgeeks.org/scalability-and-elasticity-in-cloud-computing/

# Serviços da nuvem
## Infraestructure as a Service (IaaS)
* A categoria mais básica de serviços de computação em Nuvem
* Construa infraestrutura de TI paga como você utilizar servidores, máquinas virtuais, armazenamento, redes e sistemas
operacionais de um provedor de nuvem.
* Infraestrutura de computação instantânea, provisionada e gerenciada pela internet.
Modelo onde tem a maior mão de obra, onde você é responsável por grande parte dos itens de manutenção:
* Instalar updates
* Configuração
* Atualização
* Manutenção
* Firewall
* Antivirus
* Backup do SO
IaaS - Menor responsabilidade para o Provedor.

## Plataform as a Service (PaaS)
* Fornece ambiente para construção, testes e implementação de aplicativos de software.
* Ajuda a criar aplicativos rapidamente, sem se concentrar no gerenciamento de infraestrutura subjacente.
Exemplo: Imagine que desejamos utilizar um banco de dados.

  Em IaaS:
    * Podemos usar SQL Server, para isso, instalamos o SQL no Windows Server. Nesse modo, somos responsáveis por 
todo o gerenciamento do SO.

  Em PaaS:
    * Podemos configurar um SQL Database, assim, iremos gerenciar apenas o banco de dados (Acesso, dados). O provedor irá cuidar da 
infraestrutura e questões de disponibilidade.

## Software as a Service (SaaS)
* Software hospedado centralmente e gerenciado para usuários finais. Os usuários se conectam e usam aplicativos baseados em nuvem pela internet.
Por exemplo: Microsoft Office 365, e-mail e calendários.
* Onde há o mínimo possível de responsabilidade, só cuidamos dos dados, licença e acesso. 

# Modelo baseado em consumo
* Sem custos iniciais
* Não há necessidade de comprar e gerenciar infraestrutura dispendisiosa
* Capacidade de pagar por recursos adicionais, conforme necessário
* Capacidade de parar de pagar por recursos que não são mais necessários.

**Observação:** Existem recursos que ao darmos stop, podemos parar de pagar. Contudo, também há recursos
que mesmo quando parados, ainda continuamos pagando. Exemplo: 
Após a criação e a utilização de uma máquina virtual, se desprovisinarmos/deletarmos ela. Ainda continuamos pagando pelo disco. 
Não é possível desprovisionar o disco porque as informações seriam perdidas. Assim, é necessário deletar o disco separadamente. 

# Modelo de responsabilidade compartilhada
	A tabela abaixo mostra a responsabilidade:
**On-Premises: Tudo é sua responsabilidade**
## IaaS: 
* Não possui responsabilidade sobre Compute, Networking e Storage - Componentes físicos (Hardware *  Switch, Datacenter e discos). 
* Você é responsável pelo gerenciamento da máquina virtual, se tem update, aplicações instaladas, acesso e dados (backup).
## PaaS: 
* Não se preocupa com VM nem com SO. Somente com a aplicação, o acesso e os dados.
## SaaS:
* Só se preocupa com o Uso da aplicação (licenciamento e informações)

# Contas do Azure
