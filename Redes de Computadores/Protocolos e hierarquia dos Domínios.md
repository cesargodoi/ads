Os protocolos definidos por _Tanenbaum_, são:

| Protocolo | Descrição |
| ---- | ---- |
| **HTTP** | **HyperText Transfer Protocol**<br>Trata-se de um protocolo utilizado para acessar conteúdo web na rede mundial de computadores. Permite que ocorra a transferência ponto a ponto entre clientes e servidores de serviços do tipo elástico e streaming multimídia. |
| **SMTP** | **Simple Mail Transfer Protocol** <br>Protocolo Simples de Transferência de E-mail. É o protocolo utilizado para efetuar o envio e recebimento de e-mail de um servidor a outro. |
| **SSH** | **Secure SHell**<br>Esse protocolo é utilizado para se efetuar acesso remoto em outro dispositivo, por meio de um terminal, assim como o _prompt_ de comando do DOS/UNIX. A grande diferença das outras técnicas (Telnet e RSH) de acesso remoto está na segurança. Ao fazer um acesso remoto em um dispositivo, a transmissão de dados recebe uma criptografia que pode variar conforme o algoritmo de encriptação das mensagens, garantindo assim a integridade do que é compartilhado. |
| **RTP** | **Real-Time Transfer Protocol**<br>É o protocolo de transporte utilizado na camada de aplicação para prover _streaming_ de áudio e vídeo. Ou seja: protocolo de transferência em tempo real. |
| **SIP** | **Session Initiation Protocol** <br>Apesar deste protocolo não pertencer à camada de aplicação e sim à de sessão, vale ressaltar seu grau de importância para os serviços multimídia. Este protocolo é responsável pela criação, modificação e finalização de sessões de transferência de arquivos de serviços multimídia. |
| **POP3** | **Post Office Protocol 3**<br>Essa expressão pode ser traduzida como protocolo de correio, já disponível em sua terceira versão. Ele permite que o usuário descarregue as mensagens que estejam localizadas em um servidor de e-mail em seu dispositivo. Essa ferramenta permite o recebimento das mensagens, mas não o envio. |
| **IMAP** | **Internet Messaging Access Protocol**<br>Este protocolo, assim como ocorre com o **POP3**, sincroniza as mensagens que estão alocadas em um servidor de e-mail. Entretanto, o **IMAP** se mantém conectado, a fim de sincronizar, em tempo real, as mensagens recebidas. |
| **NTP** | **Network Time Protocol**<br>(Protocolo de Tempo de Redes). Ele tem como função sincronizar os relógios dos servidores, roteadores e computadores das redes. |

## Hierarquia dos domínios

| **Domínio Genérico** | São definidos os registros conforme o segmento do site, podendo ser: _.com_, _.net_, _.org_, _.edu_, _.gov_, entre outros. |
| ---- | ---- |
| **Domínio de Países** | É utilizada a abreviatura com dois caracteres para identificar em qual país o domínio foi registrado, podendo ser: _.br_ (Brasil), _.us_ (Estados Unidos), _.ar_ (Argentina), entre outros. |
| **Domínio Reverso** | Faz o processo reverso a consulta ao servidor **DN**S. Quando um servidor recebe uma solicitação, é feita uma consulta em sua “tabela”, que por sua vez encaminha o pedido do cliente ao servidor relacionado à URL digitada pelo usuário, sendo utilizado o endereço **IP**. |
