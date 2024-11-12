# Arquitetura do sistema do smartphone


Os smartphones são basicamente pequenos computadores de mão, e as principais diferenças arquitetônicas em relação aos computadores são:


* Os sistemas são mais bloqueados:
  * Carregadores de inicialização não personalizáveis
* Adição de coprocessadores para fins especiais
  * Enclave seguro
  * Banda base
  * Processamento de imagens
  * Aceleração de IA


### Co-processadores


Os coprocessadores são processadores usados somente para uma finalidade específica que não seja o sistema. Os coprocessadores ajudam o processador de aplicativos principal a lidar com determinadas tarefas e, portanto, precisam se comunicar com ele. Os coprocessadores geralmente executam seu próprio sistema operacional e aplicativo incorporados e não podem ser controlados diretamente pelo usuário. Os coprocessadores geralmente têm acesso privilegiado aos recursos do sistema e aos dados do usuário, portanto, às vezes, são alvos de explorações mais sofisticadas. Devido à natureza bloqueada, é difícil auditar ou obter dados forenses dos coprocessadores. Para os fins deste guia, você só precisará saber que:


* Os coprocessadores podem ser explorados
* As explorações de coprocessadores são sofisticadas e incomuns


O restante deste guia se concentrará, portanto, nos softwares executados no processador do aplicativo.


### Sistema operacional


Os sistemas operacionais dos smartphones diferem dos sistemas operacionais dos computadores, pois implementam mais controles e isolamento entre os diferentes componentes e aplicativos do sistema, de modo que um componente comprometido não pode afetar facilmente todo o sistema.


![](https://developer.android.com/guide/platform/images/android-stack\_2x.png)


É possível que os invasores explorem as vulnerabilidades do kernel, mas essas vulnerabilidades são bastante raras e geralmente exigem técnicas sofisticadas para serem exploradas.


### Aplicativos do sistema


Os aplicativos do sistema podem conter vulnerabilidades. Uma vez explorados, eles podem causar mais danos do que a exploração de aplicativos de usuário, pois geralmente têm mais privilégios para alterar o sistema subjacente. Um exemplo comum é o navegador incorporado, que é explorado com frequência.


### Aplicativos de usuário


Os aplicativos de usuário são menos privilegiados. No entanto, se as permissões forem concedidas, eles podem acessar informações confidenciais do usuário, portanto, ainda podem causar grandes danos. Às vezes, eles também podem enganar ou explorar o sistema subjacente para obter mais controle.
