

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
	- domínio de colisão: impede que haja colisão de mensagens enviadas e recebidas
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

