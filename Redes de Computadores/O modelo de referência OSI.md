
Segundo _Tanenbaum (1997)_, o desejo da **ISO** era desenvolver um modelo para interconexão de sistemas abertos. Para isso, foi desenhado um modelo em sete camadas  que deveriam atender os seguintes requisitos:
- A função das camadas deve ser escolhida em razão dos protocolos que foram padronizados
- Cada camada deve executar a função a qual foi destinada
- Os limites entre as camadas devem ser escolhidos de forma que minimize os esforços ao fluxo das mensagens pelas interfaces
- O número de camadas deve ser do tamanho suficiente para alocar todas as funcionalidades possíveis nas redes

Segundo _Tanenbaum (1997)_, o modelo de referência **OSI** (_Open Systems Interconnection_ – _Sistemas Abertos de Conexão_), efetua todos os processos necessários para que ocorra a transmissão de dados, fazendo com que as camadas (ou layers) nele existentes efetuem a divisão dos processos lógicos.

Dessa forma, a **ISO** desenvolveu o modelo de referência **OSI**, que foi um marco para o desenvolvimento dos protocolos de comunicação que são utilizados nos serviços consumidos diariamente pela internet. A arquitetura do modelo é a seguinte:

![](modelo_de_referencia_OSI.png)

A partir de 1984, os fabricantes de hardwares e desenvolvedores de softwares entenderam que o modelo proposto em camadas tinha como intuito permitir a interoperabilidade entre equipamentos de diferentes origens, o que poderia dar uma vantagem competitiva no mercado, abrindo espaço para parcerias e novos desenvolvimentos.

## Hierarquia e interfaces dos protocolos nos serviços de redes

Segundo _Tanenbaum (1997)_, assim como determina o modelo de referência **OSI**, os protocolos são organizados em pilhas ou camadas. Porém, em todas as redes, a função primordial é fornecer serviços às camadas superiores.

A função primordial dos protocolos é fornecer serviços às camadas superiores.

Para isso, o mecanismo utilizado faz com que a camada “n” de um dispositivo se comunique com a camada “n” de outro dispositivo. Basicamente, o protocolo efetua a “negociação” entre as partes para que seja provida a comunicação, conforme pode ser observado na figura a seguir:

![](camadas_e_interfaces.png)

Quando os dados são transferidos, cada camada processa o seu serviço respectivo. Para que isso ocorra, a cada par de camadas existe uma interface responsável por definir as operações e os serviços que a camada inferior tem que encaminhar à layer superior.
