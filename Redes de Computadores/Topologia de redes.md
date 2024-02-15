### Topologia Malha
Cada um dos dispositivos da rede (nós) possui um link dedicado com os demais da rede
![](topologia_malha.jpg)

### Topologia em anel
Cada dispositivo possui uma conexão com seu "vizinho". O sinal, quando enviado, percorre o anel até que o destino seja encontrado

![](topologia_anel.jpg)

### Topologia estrela
Cada dispositivo possui um link ponto a ponto com um concentrador, podendo este ser um hub, roteador ou switch

![](topologia_estrela.jpg)

### Topologia de barramento
Esta topologia é considerada ponto a ponto, pois para fazer a conexão é necessário um **backbone** (tronco central) para interligar os dispositivos

![](topologia_barramento.jpg)





As redes utilizadas diariamente possuem em suas infraestruturas alguns equipamentos essenciais para prover a comunicação entre os dispositivos:

- GATEWAY
	- está relacionado ao conceito de "borda de rede"
		![](gateway.png)
	- pode ter funções específicas, dependendo do planejamento do administrador de redes:
		- _direcionamento:_  no qual todas as mensagens são enviadas para o nodo da rede, podendo ser roteadas ou switch.
		- _proxi:_ uma lista de sites cujo acesso é ou não permitido por meio dos dispositivos da rede interna.
		- _firewall:_ um dispositivo de segurança que verifica o conteúdo dos pacotes e efetua seu bloqueio, se necessário.

