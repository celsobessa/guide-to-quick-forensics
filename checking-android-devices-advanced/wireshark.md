# Wireshark

## Pré-requisito

Configure o monitoramento de tráfego de rede de acordo com [network.md](../smartphones/network.md "mention").

## Uso

O Wireshark é uma ferramenta para capturar o tráfego de rede fluindo por uma interface de rede.

Durante a primeira inicialização, é preciso selecionar a interface de rede que você deseja monitorar. Esta deve ser a interface de rede atuando como o Ponto de Acesso (AP) para o telefone. Observação: quando não tiver certeza sobre qual, desconecte o adaptador Wi-Fi, conecte-o novamente e verifique `sudo dmesg` para o nome da interface detectada.

Assim que o tráfego for mostrado fluindo, podemos começar a procurar por atividades suspeitas.

![Um exemplo de captura do Wireshark quando um aplicativo é iniciado no telefone.](<../.gitbook/assets/wireshark Screenshot\_20220718\_161819.png>)

## Indicadores (O que procurar?)

### Geral

* Domínios suspeitos, por exemplo, `goog1e.com`
* Conexão direta a um IP sem consulta DNS.
* Conexão periódica, por exemplo, a cada hora, sempre que o dispositivo inicializa
* Conexão persistente
* Portas TCP e UDP incomuns
* Conexão não correlacionada com a atividade do usuário, como quando a tela do dispositivo está desligada, mas vendo muito tráfego de rede.

### Ameaças direcionadas

Malware altamente furtivo, tende a ocultar seu tráfego com outros aplicativos benignos.

### Trojans de acesso remoto (RATs)

Os RATs geralmente precisam se comunicar com servidores de comando e controle (servidores C2 ou servidores C\&C) operados pelo invasor. O invasor pode emitir comandos para controlar remotamente o dispositivo infectado. Isso deve envolver muito tráfego bidirecional.

### Spyware / stalkerware

Esses malwares geralmente não têm servidores C2, mas apenas coletam e carregam continuamente informações do usuário (como atividade do usuário no sistema, localização) para servidores de coleta.

### Adware / mineradores de criptomoedas

Esta categoria de software é a menos intrusiva. O adware geralmente se conecta a muitos sites diferentes para produzir cliques em anúncios. Os mineradores usam o poder de processamento do dispositivo para minerar criptomoedas e geralmente teriam que se conectar a pools de mineração para dar resultados.

## Referências

* Mais informações sobre análise de tráfego de rede: [https://www.rapid7.com/fundamentals/network-traffic-analysis/](https://www.rapid7.com/fundamentals/network-traffic-analysis/)
