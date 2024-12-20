# Resumo dos laboratórios

## Dois primeiros cursos:
Nos dois primeiros cursos foi possível ter uma ideia geral da computação em nuvem da Microsoft, dando uma noção de como é essa plataforma. Também foi ensinado a criar uma conta para acessar o portal da azure para poder fazer os laboratórios e ter um primeiro contato com a plataforma.

## Cursos sobre códigos
Nos outros 3 cursos foi apresentado sobre o versionamento de código, que foi uma problema encontrado no desenvolvimento do Linux perante as comunidades que efetuam os desenvolovimento.
Apresentando as teorias sobre o Git e GitHub bem como o acesso a essa plataforma para verificar a documentação oficial. A Elidiana ensinou a instalação do GitHub no windows e Linux, configuração de alguns opções e vários comandos para criar repositórios, cloná-los, elaborar o arquivo readme com extensão md, puxar e enviar alterações para o repositório local e para a web, dentro muitas outras tarefas. Também apresentou o material de apoio.
E até o momento tivemos que fazer um portifólio para disponibilizar no GitHub da DIO que o curso disponibilizou.

## Benefícios da nuvem
São muitos os benefícios de se usar a nuvem nuvem, porém tem que se ter cuidado com os custos deles, se mal planejados podem ser bem altos.
Alguns dos benefícios:

1. Curso Alta disponibilidade
Consiste em deixar os serviços disponíveis na maior parte de tempo e também acessíveis.
Ela esta ligada ao tempo de SLA que varia dependendo do serviço e consequentemente no custo.

2. Escalabilidade
Ajustes automáticos ou manuais para atender a uma demanda específica. Esse ajustes podem ser diminuídos quandos não estiverem mais sendo usados, retornando ao estado que era antes.
Se divide em dimensionamento certical e horizontal.

2.1 Dimensionamento vertical
Quando precisamos de mais recurso da máquina como por exemplo, processador e memória.

2.2 Dimensionamento horizontal
Quando devido a algum evento ou necessidados a empresa precisa de um aumento dos recursos de forma repentina, por exemplo, mais máquina virtuais.
Nesse caso esse aumento podeser feito de forma automática.

3. Confiabilidade
Os recursos da nuvem podem estar implantados em vários locais no mundo, ou seja, algum recurso pode esta num local que por algum motivo não esteja funcionando e outro local como e mesmo recurso estaja em perfeito funcionamento não deixando o cliente com o serviço sem funcionar.

4. Previsibilidade
É previsível que seja possível aumentar os recursos rapidamente, estando atendo com os custos que podem demandar.

5. Desempenho
Os recursos da nuvem podem fornecer um alto desempenho, pois são recursos que estão em vários data centers e cobertos por balanceamento de carga e alta disponibilidade, por exemplo. Sendo possível a realização de dimensionamento conforme a necessidade do cliente.

6. Custos
Se paga pelo que é usado, ou seja, todo o recurso tem seu respectivo custo que podem varias de região, zonas, entre outros.

7. Segurança e governança.
Por serem acessados por vários clientes diferentes, armazenamento de informações, dentre outras coisas, a preocupação e melhorais com a segurança são constantes nos provedores de nuvem. Essa segurança pode ser fornecida para que o cliente tenhao o controle máximo dos seus serviços bem como a parte do provedor da nuvem.
Sobre a governança, os serviços são gerenciados por pessoas que atendem a padrões regulatórios e corporativos, dependendo da área que a empresa trabalha.

## Curso tipos de serviços de Nuvem

São conceitos e padrões que são adotados por vários provedores de nuvem do mercado.

IaaS - Infraestrutura como serviço
Nesse tipo o cliente gerencia a administrada a maioria dos recursos que ele tem contratado com o provedor de nuvem, ou seja, grande parte das configurações, administração, segurança, entre outro são de responsabilidade do cliente. Ele possui um gerenciamento mais amplo dos recursos que ele tem. O provedor disponibiliza o hardware, conexão de rede e a segurança física o resto fica por conta do cliente.
É o modelo que a responsabilidade compartilhada fica a cargo do cliente porque ele é responsável pela infraestrutura que ele utiliza.

PaaS - Plataforma como serviço
No PaaS o provedor de nuvem disponibiliza a plataforma para que o cliente possa, por exemplo, realizar o desenvolvimento da aplicação junto com as configurações do banco de dados. Nesse cenário o cliente não se preocupa com as configurações da máquina, como instalação, administração e gerenciamento, ele recebe a máquina pronta e realiza as configurações necessária para ter ambiente de desenvolimento completo da sua aplicação.
A responsabilidade é dividia entre o provedor e o cliente.

SaaS - Software como serviço
O provedor possui uma plataforma que abrange várias aplicações e o cliente adquire as licenças das aplicações que são necessárias para a sua necessidade. Esse tipo é mais voltado para a questão de licenciamento e é o que menos precisa de conhecimento técnico.
Aqui a maior responsabilide fica por conta do provedor, pos ele que fornece os serviços de toda a plataforma. O cliente fica por conta dos acessos dos usuários, pelos dados inseridos, tipos de acesso entre outros, por exemplo.

## Curso componentes da arquitetura do azure

Regiões - São locais onde estão os datacenters da Microsoft. Eles estão próximos um dos outros, interligados através de redes de alta velocidade com baixa latência formando zonas de disponibilidade. Essas regiões geralmente possuem três datacenters e armazenam os dados nos três, ou seja, replicam as informações entre eles ficando todos com as mesas informações, caso um ou dois deles falharem por algum motivo, tem o terceiro que ainda consegue deixar os serviços disponíveis. Também é possível fazer a cópia de algumas informções para regiões diferentes, porém é necessário verificar a legislação de cada país permite elas saiam dele.

Pares de regiões - É quando uma região tem outra como par, ou seja, caso ocorra alguma interrupção com a região original ela possui a sua região para que será a primeira a replicar alguma serviço para que ele não fique indisponível. Essa replicação pode ser automática, dependendo do serviço. Também consideramos essa região para como o serviço de disaster recovery da região original.

Regiões Soberanas - São regiões isoladas que não são disponibilizadas para os clientes em geral, geralmente seu acesso fica específico para o governo.

Recursos em nuvem - São todos os recursos que o provedor oferece para que seja criado, como redes privadas, máquinas, banco de dados, entre outros, podendo criar toda a infraestrutura que uma empresa precisa na nuvem. Esses recursos são criados dentro dos grupos de recursos para um melhor gerenciamento e controle. É possível mover os recursos em grupos de recursos diferentes e criar mais de uma grupo de recurso. Porém os recursos podem existir em somente um grupo de recursos e esses grupos podem ser criados em regiões diferentes.

Assinaturas e grupos de gerenciamento no azure - Permite que uma conta possua várias assinaturas, ou seja, essa conta pode ter uma assinatura de teste, outra para produção, outra para homologação e assim por diante. Uma assinatura só pode ser associada a uma conta. Cada assinatura terá uma fatura de pagamento para ela. Nessa assinatura tem os controles de acesso, limite de cobrança, autenticação a autorização nas contas do azure. Os grupos de gerenciamento podes trabalhar padrões para mais de uma assinatura, eles estão hierarquicamente acima das assinatura e gerenciam elas.

## Curso Computação e rede na Azure

Máquinas virtuais - é um recurso disponibilizado pela Azure que disponibilizado para o cliente ciarem elas conforme a sua necessidade. A plataforma também oferece máquinas virtuais com determinados padrões para atender a certas demandas, como por exemplo para ambientes de teste. Elas podem ser criadas e configuradas para atender a uma demanda específica. Vários são os parâmetros que se tem que definir na criação delas, como por exemplo a processamento, quantidade de memória, configurações de rede, local em que elas srão criadas, entre outros. É uma excelente opção de flexibilização.

Conjuntos de disponibilidade - oferecem mais segurança para as máquinas virtuais, pois colocam elas em agrupamentos lógicos que reduz as chances de falhas. Elas ficam em diferentes domínios para maior confiabilidade. Elas são alocadas em maior proximidade oferecendo latência menores entre elas.

Contêiner do azure - contêiner virtualiza o sistema operacional e faz com que o aplicativo conteinerizado detecto que o sistema operacional esta totalmente a sua disposição. Ele pode ser implantando e executado em qualquer local, são muito mais eficientes, leves e portáteis. Eles fornecem agilidade porque ele empacota um aplicativo e encmainha para a TI para execução em uma plataforma padronizada, fornecem um formato padronizado de todos os componentes necessários para executar o aplicativo e possibilitam cenários em que possam escalar e reduzir verticalmente rapidamente.

Azure functions - não requer a manutenção de máquinas virtuais ou contêineres. Um evento ativa a função, sem a necessidade de manter os recursos provisionados quando não tem eventos. O time de desenvolvimento não precisa se preocupar com a infraestrutura, apenas com o desenvolvimento da aplicação que executa o serviço. O azure functions é ideal para utilização sobre demandas, ou seja, conforme a demanda ela aloca mais recursos e desaloca quando necessário, sendo cobrado somente o tempo de uso enquanto a função foi usada.

Azure ExpressRoute - são conexões realizadas diretamente na nuvem da Microsoft, podendo ser feita via VPN, conexão privada via provedor de conectividade, uma rede ponto a ponto ou via através de uma conexão crizada virtual numa instalação de colocalização. Também é possível fazer conexões diretas entre escritórios, centro de dados ou outras instalações a nuvem da Microsoft. A ligação expressRoute não utiliza a internet pública. 

## Armazenamento do Azure

Redundância - entre vários data centers para que as informações e serviços fiquem ativos e protegidos de eventos como falhas, problemas de hardwares e energia. E também para cópias de segurança garantindo disponibilidade e durabilidade. A nuvem da Microsoft oferece alguma opções que podem atender aos clientes dependendo do que ele necessita.
LRS - Armazenamento com redundância local
ZRS - Armazenamento com redundância de zona
GRS - Armazenamento com redundância geográfica
GZRS - Armazenamento com redundância de zona geográfica

LRS - nessa redundância os dados estão armazenados em um único datacenter na mesma região e estão replicados três vezes dentro desse data center.  Protege os dados contra falhas de rack e drive do servidor. É uma redundância de menor custo.

ZRS - armazena os dados em 3 datacenters diferentes da mesma região primária. Mesmo que um data center fique indisponível, os dados ficam com acesso de leitura e gravação porque estão em outro zona. Se um data center dicar indisponível, é realizada atualizações de rede para que os clientes continuem acessando. Esse cenários é recomendado para situações que deve ser atendido aos requisitos de governança de dados.

GRS - armazena os dados em um único data center da mesma região e replica de forma assíncrona para a região par da região principal usando o LRS. Nesse caso os dados podem estar armazenados a quilômetros de distância oferecendo uma alta segurança para perda e acesso. 

GZRS - Nesse caso as informações ficam armazenadas nos três data centers da região primária protegendo de interrupções regionais e é replicado para outro data center de outro região usando LRS, que no caso é o par da região principal. Caso toda a região primária venha a sofrer algum dano climático ou catastrófico, os dados permanecem acessíveis.

## Serviços de armazenamento do Azure

Inclui os seguintes serviços:

Blobs do Azure
É uma forma de armazenar os objetos na nuvem do Azure. Ele armazena qualquer tipo de arquivos e não trabalha de forma estruturada. Pode armazenar grandes quantidade de arquivos e não são limitados a tamanho de arquivos comuns. Os desenvolvedores não precisam se preocupar com o discos e nem com o gerenciamento deles, os blobs do azure fazer todo o gerenciamento.
Existem arquivos que depois de irem para a nuvem da Azure não são acessados frequentemente, ou seja, são acessados raramente diferente de outros que com mais frequência, interferindo nos custos. Diante disso, existem as camadas de acesso disponíveis:
Camada de acesso quente - dados de são acessados com mais frequência
Camada de acesso esporádico - dados acessados com menos frequência e armazenados por pelo menos 30 dias
Camada de acesso frio - dados acessados com pouca frequência e armazenados por pelo menos 90 dias
Camada de acesso aos arquivos - dados acessados raramente e armazenados por pelo menos 180 dias
Todos os dados de armazenamento do blob podem ser acessados de qualquer lugar do mundo através de HTTP ou HTTPS.

Arquivos do Azure
São fornecidos na nuvem de forma gerenciada através dos protocolos SMB e NFS. De forma geral, é o famoso acesso \\ que é utilizado em muitas redes. Ele esta disponível para ser acessado através do Windows, Linux e MacOS.

Filas do Azure
Disponível para armazenar grandes quantidades de mensagens sendo acessadas de qualquer lugar do mundo através de chamadas autenticadas usando HTTP ou HTTPS. A quantidade de mensagem da fila é determinada pela conta de armazenamento do usuário. Cada mensagem individual pode ter até 64KB de tamanho.

Discos do Azure
São discos virtualizados utilizados como VMs do Azure, onde é possível somente provisionar o disco e deixar que o Azure faça o resto.

Tabelas do Azure
Armazena grandes quantidades de dados estruturados e não relacionais, sendo repositórios de dados NoSQL que aceita chamados de dentro e fora da nuvem do Azure.

## Migração de dados do Azure

Fornece a migração dos dados do data center interno da empresa para a nuvem do Azure através de opções como o AzCopy e o Azure Data Box.

AzCopy - é um utilitário de linha de comando que auxilia a cópia de arquivos pequenos ou individuais para uma conta de armazenamento da nuvem Azure. É possível copiar, baixar arquivos e também sincronizar dados blobs.

Azure Data Box - É literalmente um caixa física onde é possível armazenar até 80 terabytes de dados. Ela serve para transferir grandes quantidade de dados e é disponibilizada pela Microsoft para ela seja transportada até o local do cliente e depois da cópia concluída retorne para que seja feita a cópia dos dados para a nuvem da Azure. Toda essa transferência de dados é realizada de forma criptografada.  

## Identidade, acesso e segurança

Microsoft Entra ID
É o novo nome para o Microsoft Active Directory. Com ele é possível fazer o gerenciamento das contas de identidade na nuvem, ou seja, acesso aos aplicativos de nuvem da Microsoft e os aplicativos desenvolvidos pela empresa.




