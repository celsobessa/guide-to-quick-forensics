# Aplicativos de análise
## Aplicativos de verificação e antivírus
Alguns aplicativos verificam automaticamente os aplicativos instalados no sistema (para ver se eles são conhecidos como mal-intencionados).


* Koodous Antivirus](https://play.google.com/store/apps/details?id=com.koodous.android)
* [Lookout](https://play.google.com/store/apps/details?id=com.lookout)


Esses aplicativos de verificação funcionam extraindo e carregando os APKs instalados no sistema para sua própria plataforma e comparando os APKs com malwares conhecidos. Algumas informações do dispositivo e, possivelmente, outras informações pessoais também podem ser carregadas. É preciso verificar a política de privacidade das plataformas antes de instalar e fazer a varredura com esses aplicativos.


Como alternativa, há um aplicativo antivírus de código aberto [Hypatia](https://github.com/Divested-Mobile/Hypatia), que utiliza bancos de dados de assinaturas do ClamAV, ESET e da [lista de ameaças direcionadas feita pelo brotherder](https://github.com/botherder/targetedthreats).&#x20;


Esses aplicativos de scanner e antivírus só podem ver quais outros aplicativos estão instalados e não podem inspecionar profundamente o sistema operacional, pois eles próprios estão em sandbox. No entanto, malwares de média a alta sofisticação se incorporam ao sistema sem serem exibidos como um aplicativo. O conhecimento desses aplicativos de scanner e antivírus sobre malwares também depende de seus bancos de dados, cujas fontes geralmente vêm de seus clientes corporativos.Os coprocessadores ajudam o processador de aplicativos principal a lidar com determinadas tarefas e, portanto, precisam se comunicar com ele.Os coprocessadores geralmente executam seu próprio sistema operacional e aplicativo incorporados e não podem ser controlados diretamente pelo usuário.


Os coprocessadores geralmente têm acesso privilegiado aos recursos do sistema e aos dados do usuário, portanto, às vezes, são alvos de explorações mais sofisticadas.


Devido à natureza bloqueada, é difícil auditar ou obter dados forenses dos coprocessadores.


Para os fins deste guia, você só precisará saber que: * Os coprocessadores podem ser explorados


* As explorações de coprocessadores são sofisticadas e incomuns
O restante deste guia se concentrará, portanto, nos softwares executados no processador do aplicativo.
### Sistema operacional
Os sistemas operacionais dos smartphones diferem dos sistemas operacionais dos computadores, pois implementam mais controles e isolamento entre os diferentes componentes e aplicativos do sistema, de modo que um componente comprometido não pode afetar facilmente todo o sistema.
![](https://developer.android.com/guide/platform/images/android-stack\_2x.png)
É possível que os invasores explorem as vulnerabilidades do kernel, mas essas vulnerabilidades são bastante raras e geralmente exigem técnicas sofisticadas para serem exploradas.
### Aplicativos do sistema Os aplicativos do sistema podem conter vulnerabilidades.


Uma vez explorados, eles podem causar mais danos do que a exploração de aplicativos de usuário, pois geralmente têm mais privilégios para alterar o sistema subjacente.


Um exemplo comum é o navegador incorporado, que é explorado com frequência. ### Aplicativos de usuário
Os aplicativos de usuário são menos privilegiados.


No entanto, se as permissões forem concedidas, eles podem acessar informações confidenciais do usuário, portanto, ainda podem causar grandes danos.Às vezes, eles também podem enganar ou explorar o sistema subjacente para obter mais controle.


Há uma versão on-line do MobSF disponível em [https://mobsf.live](https://mobsf.live).


Você também pode [hospedar](https://mobsf.github.io/docs/#/installation) o MobSF por conta própria ou usar serviços de hospedagem gratuitos como o [Play with Docker](https://labs.play-with-docker.com/) para hospedar uma instância privada do MobSF. O Play with Docker fornece 4 horas de tempo de sessão.


## Outras ferramentas


Há também outras ferramentas de análise on-line. As listadas abaixo não são especializadas em APK.


* [https://cuckoo.cert.ee/] (https://cuckoo.cert.ee/)
* [https://app.any.run/](https://app.any.run/)
* [https://www.virustotal.com/](https://www.virustotal.com/)


## Interpretação dos resultados da análise


As ferramentas produzirão muitas informações técnicas sobre o aplicativo, e interpretá-las exigiria um conhecimento técnico de como os aplicativos móveis funcionam (por exemplo: o que são _provedores de conteúdo, serviços, atividade_). No entanto, uma análise parcial pode ser obtida simplesmente verificando se os arquivos, URLs e endereços IP contidos no aplicativo já são conhecidos como mal-intencionados.
