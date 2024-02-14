### Tipos de sinais:
- Analógicos: segundo Tanenbaum(2003) os sinais analógicos são ondas eletromagnéticas que assumem infinitos valores ao longo do tempo. Esse sinal é representado por uma onda senoidal com as seguintes características:
	- _Amplitude:_ representa intensidade mais alta dos sinais eletricos (volts)
	- _Frequência:_ é medida em hertz, define a quantidade de ciclos em um intervalo de tempo
	- _Fase:_ define o formato da onda senoidal, pode ser medida em graus ou radianos.
	![](sinal_analogico.png)
	
- Digitais: é representado por 0s e 1s, ou seja, é um sinal binário. A representação dos seus valores é dada como discreta ao longo do tempo e amplitude. Então , é possível diminuir a taxa de oscilação, fenômeno este responsável pelo aumento da qualidade de serviço. Quando ocorre uma. transmissão de dados, ocorre um processo  de codificação (digitalização) desse sinal. Com isso, os sinais digitais:
	- Não sofrem degradação dos serviços por interferência ou ruídos
	- Pode ser transmitida maior quantidade de informações.
![](sinal_digital.png)

Em redes de computadores esses dois sinais também estão presentes nos tipos de transmissão e determinam a qualidade do serviço.
Esses sinais em uma transmissão feita por uma internet cabeada (oferecida pelas operadoras), em que se pretende acessar um site a partir de um dispositivo, ocorrem da seguinte forma:
- Os modems fornecidos pelas operadoras fazem a adequação do sinal digital com o meio disponibilizado pela operadora.
- O modem recebe os sinais emitidos pelo computador (entende-se notebook, tablet e smartphone) e os coloca no meio de transmissão fornecida pela operadora (processo conhecido como modulação)
- ao chegar ao destino, é efetuado o processo inverso.

Os modos de transmissão dos sinais nas redes de comunicação de dados podem variar conforme:
- o sentido em que ocorrem as trocas de mensagens, 
- o número de bits enviados simultaneamente e
- a sincronização entre computador e servidor

### Componentes de uma rede

Para estruturar as redes, existem alguns componentes de hardware que são básicos, porém essenciais para prover a comunicação entre os dispositivos. Entre eles podemos citar:
- Placas de rede: O controlador de interface da rede (NIC – Network Interface Controller) pode estar ou não integrado à placa-mãe. A arquitetura de seu barramento pode ser na forma PCI, PCI Express, ISA e USB, ou seja, o formato de encaixe na placa-mãe. A sua função lógica é efetuar o tratamento de endereçamentos no envio e recebimento das mensagens.
![](placa_de_rede.png)
- Modem: O modem tem a função de fazer a modulação e demodulação das mensagens, e também é conhecido como transceptor. Em sua forma analógica, os dados são transmitidos pelo canal de voz; já na sua forma digital, é feita a codificação da banda base. Esse equipamento está entre os mais populares dos hardwares encontrados nas redes.
![](modem.png)
- Hub: O hub pode conter várias linhas de entrada que são responsáveis por distribuir conexão. Esse equipamento assume o papel de um repetidor, pois a mensagem ao chegar é replicada para todas as portas. Por ter o comportamento de repetidor dentro de uma rede e pelo motivo de replicar uma mensagem para todos os dispositivos conectados a ele, deve-se evitar o cascateamento.
![](hub.png)
_Cascateamento:_ é a interligação através de uma porta de um equipamento a outra porta de outro equipamento, com a largura de banda limitada à velocidade da porta (10/100/100 Mbts). Assume endereços IP distintos. Aceita interligar equipamentos distintos e de marcas distintas.

Em uma rede privada, os recursos e sistemas compartilhados ficam restritos à organização e podem estar estruturados de duas formas:
- INTRANET: rede privada que utiliza em sua estrutura física e lógica o modelo de internet. No entanto, os serviços de rede, como servidores de arquivos e impressão, servidor web e as aplicações são de uso interno.
![](modelo_intranet.png)

- EXTRANET: a popular internet. Os recursos só podem ser acessados com autorização da rede de uma companhia.!
![](modelo_internet.png)


### Topologia de redes

As redes utilizadas diariamente possuem em suas infraestruturas alguns equipamentos essenciais para prover a comunicação entre os dispositivos:

- ROTEADOR
	- ele forma _tabelas lógicas dos equipamentos disponíveis nas redes:_ roteadores, switches, computadores, dispositivos móveis, impressoras e câmeras etc. Para fazer esse processo é utilizado um mecanismos de descoberta de equipamentos vizinhos, através de protocolos de comunicação:
		- ICMP - faz o diagnóstico da rede e relata os erros de recebimento de pacotes e informa características da rede
		- ARP - efetua mapeamento dos endereços físicos (MAC) por meio do endereço lógico
		- RARP - associa um endereço lógico ao físico (contrário do ARP)
		
		Assim um roteador envia periodicamente um protocolo de atualização de vizinhança aos roteadores conhecidos, e um vai enviando a atualização aos outros sucessivamente, fazendo com que a tabela lógica de endereçamento dos equipamentos continue sempre atualizada.
- SWITCH
	- usado em redes que necessitam maior número de dispositivos.
	- quando a mensagem chega a uma das interfaces de rede, o sistema do equipamento lê o endereço destino do cabeçalho e envia para a interface apropriada.
	- ![](switch.png)
- BRIDGES (Pontes)
	- usada para conectar duas redes distintas
	- parecido com o switch, mas com aplicação diferente:
		![](bridge_ponte.png)
	- Enquanto o switch é utilizado para conectar dispositivos da rede, a Bridge é utilizada para interligar duas redes (LAN). Mas nada impede que o administrador utilize o switch para interligar duas redes, desde que devidamente configurado e planejado.

		A vantagem em se utilizar as bridges é que a sua configuração é mais simples, necessitando apenas apontar o endereço das interfaces dos equipamentos das redes que estão sendo conectadas. Já ao se utilizar o switch, o ganho no processamento das informações pode proporcionar um ganho de desempenho na comunicação entre os dispositivos de redes distintas.

- GATEWAY
	- está relacionado ao conceito de "borda de rede"
		![](gateway.png)
	- pode ter funções específicas, dependendo do planejamento do administrador de redes:
		- _direcionamento:_  no qual todas as mensagens são enviadas para o nodo da rede, podendo ser roteadas ou switch.
		- _proxi:_ uma lista de sites cujo acesso é ou não permitido por meio dos dispositivos da rede interna.
		- _firewall:_ um dispositivo de segurança que verifica o conteúdo dos pacotes e efetua seu bloqueio, se necessário.

#### RESUMO DO VIDEO:

_Formas que a rede pode ser organizada:_
	- SIMPLEX:  a comunicação ocorre em apenas um sentido. Ex: computador para impressora
	- HALF-DUPLEX: a comunicação ocorre nos dois sentidos, mas não simultaneamente. Ex: walktok
	- FULL-DUPLEX: os dados trafegam nos dois sentidos simultaneamente
![](intranet.png)
![](extranet_internet.png)

_Os dispositivos podem estar organizados em:
- REDE DE DIFUSÃO: um pc envia mensagem para outro, mas todos recebem e verificam se a mensagem é para ele ou não, aceitando ou recusando.
![](rede_de_difusao.png)
- REDE PONTO A PONTO: a mensagem é enviada apenas para o endereço de destino correto
![](esquema_p2p.png)

##### Como a mensagem sabe aonde deve chegar?

A mensagem é enviada, e o dispositivo responsável pela entrada e saída de dados é a _placa de rede._
Integrado à placa de rede está o _modem_ que é responsável por fazer a conversão digital-analógica da mensagem
Agora a mensagem segue para um _Hub, Switch ou Roteador_
- o Hub recebe a mensagem e passa para todos os dispositivos
- o Switch e roteador enviam apenas para o endereçamento lógico correto
- o Roteador ainda calcula a melhor rota para chegar ao destino

As redes podem ser estruturadas em diferentes _topologias:
- TOPOLOGIA EM MALHA: todos os equipamentos estão ligados entre si
- TOPOLOGIA DE ESTRELA: um equipamento central é responsável por conectar todos os dispositivos
- BARRAMENTO: um tronco, chamado de backbone, distribui a conexão aos equipamentos intermediários
- TOPOLOGIA DE ANEL: um equipamento faz conexão apenas com seu vizinho
- TOPOLOGIA HÍBRIDA: apresenta a característica de mais de uma topologia











