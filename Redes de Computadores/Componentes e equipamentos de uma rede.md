
Para estruturar as redes, existem alguns componentes de hardware que são básicos, porém essenciais para prover a comunicação entre os dispositivos. Entre eles podemos citar:

### Placas de rede
O controlador de interface da rede (**NIC** – Network Interface Controller) pode estar ou não integrado à placa-mãe. A arquitetura de seu barramento pode ser na forma **PCI**, **PCI Express**, **ISA** e **USB**, ou seja, o formato de encaixe na placa-mãe. A sua função lógica é efetuar o tratamento de endereçamentos no envio e recebimento das mensagens.

![](placa_de_rede.png)

### Modem 
O modem tem a função de fazer a modulação e demodulação das mensagens, e também é conhecido como transceptor. Em sua forma analógica, os dados são transmitidos pelo canal de voz; já na sua forma digital, é feita a codificação da banda base. Esse equipamento está entre os mais populares dos hardwares encontrados nas redes.

![](modem.png)


### Hub
O hub pode conter várias linhas de entrada que são responsáveis por distribuir conexão. Esse equipamento assume o papel de um repetidor, pois a mensagem ao chegar é replicada para todas as portas. Por ter o comportamento de repetidor dentro de uma rede e pelo motivo de replicar uma mensagem para todos os dispositivos conectados a ele, deve-se evitar o cascateamento.

![](hub.png)

> _Cascateamento:_ é a interligação através de uma porta de um equipamento a outra porta de outro equipamento, com a largura de banda limitada à velocidade da porta (10/100/100 **Mbts**). Assume endereços **IP** distintos. Aceita interligar equipamentos distintos e de marcas distintas.

### Roteador
Contêm microprocessadores responsáveis pelo gerenciamento dos tráfego dos pacotes de dados. Tem a capacidade de analisar o endereçamento lógico (**TCP/IP**). 

Ele forma uma _tabela lógica dos equipamentos disponíveis nas redes:_ roteadores, switches, computadores, dispositivos móveis, impressoras e câmeras etc.  Para fazer esse processo é utilizado um mecanismos de descoberta de equipamentos vizinhos, através de protocolos de comunicação:
- **ICMP** - faz o diagnóstico da rede e relata os erros de recebimento de pacotes e informa características da rede
- **ARP** - efetua mapeamento dos endereços físicos (**MAC**) por meio do endereço lógico
- **RARP** - associa um endereço lógico ao físico (contrário do **ARP**)

Assim um roteador envia periodicamente um protocolo de atualização de vizinhança aos roteadores conhecidos, e um vai enviando a atualização aos outros sucessivamente, fazendo com que a tabela lógica de endereçamento dos equipamentos continue sempre atualizada.

![](roteador.jpg)

### SWITCH
É usado em redes que necessitam maior número de dispositivos.
Quando a mensagem chega a uma das interfaces de rede, o sistema do equipamento lê o endereço destino do cabeçalho e envia para a interface apropriada.
Domínio de colisão: impede que haja colisão de mensagens enviadas e recebidas

![](switch.png)


### BRIDGES
Enquanto o **switch** é utilizado para conectar dispositivos da rede, a **bridge** é utilizada para interligar duas redes (**LAN**). Mas nada impede que o administrador utilize o **switch** para interligar duas redes, desde que devidamente configurado e planejado.

![](bridge.png)

A vantagem em se utilizar as **bridges** é que a sua configuração é mais simples, necessitando apenas apontar o endereço das interfaces dos equipamentos das redes que estão sendo conectadas. Já ao se utilizar o **switch**, o ganho no processamento das informações pode proporcionar um ganho de desempenho na comunicação entre os dispositivos de redes distintas.

![](bridge_ponte.png)


Em uma rede privada, os recursos e sistemas compartilhados ficam restritos à organização e podem estar estruturados de duas formas:
- INTRANET: rede privada que utiliza em sua estrutura física e lógica o modelo de internet. No entanto, os serviços de rede, como servidores de arquivos e impressão, servidor web e as aplicações são de uso interno.
![](modelo_intranet.png)

- EXTRANET: a popular internet. Os recursos só podem ser acessados com autorização da rede de uma companhia.!
![](modelo_internet.png)


