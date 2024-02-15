
_Filippetti (2008)_ afirma que o padrão **TCP/IP** foi desenvolvido pelo **DOD** (Departamento de Defesa dos EUA) para garantir a integridade das mensagens enviadas em caso de guerra. Isso é compreensível, pois, em razão do envolvimento em diversos conflitos ao longo dos tempos, o exército necessitou de técnicas relacionadas à comunicação.

A arquitetura do protocolo **TCP/IP** foi desenvolvida em quatro camadas, e um conjunto de processos (ou aplicações) e utilizado para prover diversos serviços. Para compreender suas camadas, observe a imagem abaixo, que compare o modelo de referência **OSI** e o protocolo **TCP/IP**:

![](OSI_TCPIP.png)

Podemos definir a função de cada uma das camadas do protocolo **TCP/IP** como:

| Camada | Descrição |
| ---- | ---- |
| **Aplicação** | **Application Layer**<br>Nesta camada define-se como os programas vão se comunicar com as diversas aplicações disponíveis nas redes. Ainda é de responsabilidade desta camada efetuar o gerenciamento da interface pela qual o usuário vai interagir com a aplicação. |
| **Transporte** | **Host-to-host Layer**<br>É idêntica à camada de transporte do modelo de referência **OSI**, ou seja, responsável por prover, gerenciar e encerrar uma conexão _ponto-a-ponto_. Ao efetuar o gerenciamento da conexão, visa-se garantir a integridade dos dados pelo sequenciamento dos pacotes segmentados para efetuar o envio/recebimento das mensagens. |
| **Internet** | **Internet Layer**<br>Tem o mesmo objetivo da camada de rede do modelo de referência **OSI**, sendo responsável por definir o endereçamento dos dispositivos por meio do **IP** e garantir o roteamento dos pacotes nas redes. |
| **Acesso à Rede** | **Network Access Layer**<br>Desempenha a mesma função das camadas de enlace e física do modelo de referência **OSI**. Efetua o monitoramento do tráfego e analisa o endereçamento de hardware antes da transmissão pelo meio físico. |

Podemos destacar algumas semelhanças entre o modelo **OSI** e o protocolo **TCP/IP**

- Divisão em camadas
- As camadas de transporte e rede são equivalentes
- A comutação de pacotes é definida no modelo e efetuada no protocolo
- Os profissionais de redes necessitam conhecer ambos

