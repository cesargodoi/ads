
prof. Gilberto Fernandes Jr.

PRINCIPIOS BÁSICOS DA COMUNICAÇÃO EM REDE

Rede de computadores:
- conjunto de computadores autônomos interconectados por uma única tecnologia
- dois computadores estão interconectados quando podem trocar informações
- a conexão pode ser feita por fios de cobre, fibras ópticas, micro-ondas, infravermelho e satélites
- existem redes de muitos tamanhos, modelos e formas
- ex.: internet

Redes(dispositivos autônomos conectas entre si)  !== sistemas distribuídos (configurados como se fossem um só)

[Cronologia das Redes de Computador](Cronologia%20das%20Redes%20de%20Computador.md)

## Princípios de Comunicação de dados

[Tipos de sinais](Tipos%20de%20sinais.md)
[Meios de Transmissão](Meios%20de%20Transmissão.md)



#### Modos de Operação

[RESUMO DO VIDEO CW1](RESUMO%20DO%20VIDEO%20CW1.md)

- simplex
- half-duplex
- full-duplex

Segundo Forouzan (2006) o conjunto dos vários dispositivos e links que possibilitam conectar redes geograficamente distribuídas, ou mesmo as redes locais, deve atender os seguintes critérios:
- _desempenho:_ métricas
- _confiabilidade:_ Qualidade do serviço QoS
- _segurança:_ políticas de acesso


## Importância e aplicações de redes de computadores

#### Aplicações comerciais
Compartilhamento de recursos e informações:
- tornar todos os programas, equipamentos e dados ao alcance de todas as pessoas na rede
- empresas possuem dependências vital de informações computadorizadas
- permitir acesso a informações e documentos relevantes de forma instantânea
Meio de comunicação
- email, VoIP, video chamada
Compartilhamento de desktop
- trabalho remoto
- reuniões com quadro e documentos compartilhados
Comércio eletrônico
- clientes: conveniência de compra em casa
- fabricantes: emitir pedidos eletronicamente, conforme necessário, reduz a necessidade de grandes estoques e aumenta a eficiência.
#### Aplicações domésticas
Conectividade
- conexão com o exterior
- internet, conversação, compra, noticias, bibliotecas online, etc
Comunicação entre pessoas
- email, mensagens instantâneas, video chamadas
- melhorar a comunicação entre seres humanos
- redes sociais
Comercio eletrônico
- catálogos online, suporte técnico online, instituições financeiras
Entretenimento
- distribuição de música, rádio, televisão, filmes, jogos
Computação ubíqua
- computação está embutida no dia a dia
- utilização de sensores
- RFID (Radio Frequency IDentification)

## Criando uma infraestrutura de rede

### Descrição da situação problema

- uma nova filial de uma empresa de desenvolvimento de jogos de Campinas
- os desenvolvedores só podem dar inicio a suas atividades, quando o novo endereço possuir uma infraestrutura de rede mínima.
- os equipamentos devem ser instalados da seguinte forma:
	- recepção: 1pc
	- sala do gerente de projetos: 
		- 1pc 
		- 1impressora
	- sala de desenvolvimento: 
		- 4pcs 
		- 1impressora 
		- 1 rub
	- sala de reunião: 
		- 1roteador 
		- 1hub
- Com base na infraestrutura mencionada, _você deverá efetuar as configurações e o desenvolvimento da infraestrutura da rede_, no software de simulação de redes **Cisco Packet Tracer**
	- se inscrever no curso do packet tracer e criar conta grátis: https://www.netacad.com/courses/packet-tracer/introduction-packet-tracer
	- Download (após login na conta):
		- https://www.netcad.com/portal/resources/packet-tracer
![](configuracao_rede.jpg)


## Gargalos em redes de computadores

- acessos simultâneos no mesmo ponto da rede

## Hardwares de rede

[Componentes e equipamentos de uma rede](Componentes%20e%20equipamentos%20de%20uma%20rede.md)

[Topologia de redes](Topologia%20de%20redes.md)


## Classificação de redes por escala e estrutura

### Por escala

#### Lan (Local Area Network - rede local):
- rede privada que opera dentro e próximo de um único prédio/residência/escritório/fábrica
- velocidade de 100Mbit/s a 10 Gigabits/s
![](LAN.jpg)

#### Man (Metropolitan Area Network - rede metropolitana):
- restrita a área de uma cidade/distrito
- ex.: TV a cabo, WiMax
![](MAN.jpg)

#### Wan (World Area Network - rede mundial):
- permite a transmissão de qualquer tipo de dados a longa distância, podendo ser entre cidades, estados, países e continentes
- computadores são ligados a sub-redes que transportam as mensagens. Essas sub-redes são mantidas por companhias telefônicas e outros provedores
- podem ser com ou sem fio (internet)

### Por estrutura

#### Redes distribuidas
- podem abranger uma área geográfica dentro de uma organização, cidade, país ou continente
- Objetivo: interligar um conjunto de dispositivos a fim de que algumas aplicações sejam executadas aos usuários
- Podem ser definidas como geograficamente distribuídas (wan), em que diversas LANs estão interligadas.

#### Redes sem fio
- LAN sem fio - IEEE 802.11 (wireless/wifi)
	- modem de rádio e uma antena para transmissão dos dados
	- abrangência restrita a um prédio, campus ou escritório
- WAN sem fio - IEEE 802.16 (WiMax)
	- antenas de transmissão potentes o suficiente para cobrir uma rede geograficamente distribuída (cidade)
	- velocidades podem variar conforme as características técnicas de transmissão e recepção do sinal.


## Classificação de redes por tecnologia e topologias de rede

### Por tecnologia

#### Redes de Broadcast - redes de difusão
- existe apenas um canal de comunicação em que todas as máquinas compartilham esse meio
- mensagens são enviadas e são recebidas por todos os nós da rede
- Exemplos: redes locais e rádio FM
![](broadcast.jpg)

#### Redes ponto a ponto
- os pacotes percorrem por diversos dispositivos intermediários até atingir o destino correto
- comunicação é feita entre transmissor e emissor
- Exemplos: WANs, ligações dedicadas
![](rede-ponto-a-ponto.jpg)

[Topologia de redes](Topologia%20de%20redes.md)
## Resolução da situação problema

### Otimizando a infraestrutura de uma rede de computadores

- Uma empresa de desenvolvimento de jogos se instalou em SP, e já possui uma infraestrutura de rede básica operando
- Porém relatou-se pelos desenvolvedores e demais colaboradores lentidão no compartilhamento dos arquivos e na impressão
- Esses problemas ocorreram graças ao cascateamento efetuado com os hubs
- Para solucionar o problema e garantir a qualidade do serviço os seguintes equipamentos foram adquiridos:
	- sala de gerente de projetos:
		- 1 servidor (modelo generic)
		- 1 notebook
	- sala de desenvolvimento
		- 1 switch (modelo generic)
		- 3 notebooks
	- Notebooks conectados no wi-fi do roteador da sala de reuniões
- Reestruturar a rede com estes equipamentos:
- ![](otimizando_infraestrutura_rede.jpg)


## Como verificar o IP em um computador?
## Como identificar a rota de uma mensagem?

#### Linux:
Para descobrir o ip da sua máquina e outras informações da rede: 
- ip -c -br a 
- ip addr (versão direta e sem cor)
- ifconfig
Para descobrir a rota até um endereço: traceroute (tem que instalar)
#### Windows
Para descobrir o ip da sua máquina e outras informações da rede: ipconfig
Para descobrir a rota até um endereço: tracert www.google.com