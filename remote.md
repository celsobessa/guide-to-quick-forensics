# Verificação remota de dispositivos

Nesta época de confinamento quase mundial, estamos adicionando aqui algumas etapas que podem ajudar a verificar remotamente os dispositivos potencialmente comprometidos. Por enquanto, elas incluem apenas soluções para computadores Windows e Mac OS usando [Teamviewer](https://www.teamviewer.com/en/) e [Chrome Remote Desktop](https://remotedesktop.google.com/), pois ainda não temos nenhuma solução satisfatória para smartphones (qualquer sugestão [é bem-vinda](https://github.com/securitywithoutborders/guide-to-quick-forensics/issues)).

## Limitações da perícia remota

### O problema da confiança

Com qualquer solução de área de trabalho remota que dependa de uma plataforma de terceiros, há uma questão importante de confiança. Quando você instala um software de área de trabalho remota desse tipo, precisa saber que a empresa que desenvolve a solução pode usar o software para acessar o seu computador, mas também pode gravar qualquer interação que você tenha por meio da solução. Portanto, é muito importante usar uma solução em que você confie com base em seu modelo de ameaças.

Neste guia, usamos dois softwares:

* O [Teamviewer] (https://www.teamviewer.com/en/) foi desenvolvido pela TeamViewer AG, uma empresa alemã com sede em Göppingen.
* O [Chrome Remote Desktop] (https://remotedesktop.google.com/) foi desenvolvido pelo Google e está integrado ao ecossistema do Google (o que exige o uso de contas do Google).

O Teamviewer teve vários problemas de segurança no passado, a empresa FireEye alegou que foi violado por um [grupo patrocinado pelo Estado chinês em outubro de 2019] (https://www.securitynewspaper.com/2019/10/14/fireeye-confirms-that-apt14-group-hacked-teamviewer-attackers-would-have-accessed-billions-of-devices/). Tendemos a confiar mais no Google por sua segurança, mas, dependendo do seu modelo de ameaças, o Teamviewer pode ser uma opção melhor. Estamos usando o Teamviewer para Windows aqui porque a Área de Trabalho Remota do Chrome ainda não é compatível com o Mac OS (sem compartilhamento de arquivos).

### O problema de precisar de acesso on-line

Outro problema com a verificação de dispositivos remotamente é que você precisa que o dispositivo tenha acesso à Internet. Como [explicado anteriormente] (safety.md), isso pode levar a alguns riscos para o usuário. Se o dispositivo for realmente comprometido e monitorado remotamente, os operadores poderão identificar que o usuário está recebendo suporte técnico e isso poderá causar retaliação contra a pessoa que você está tentando apoiar.

Você deve certificar-se de abordar esse risco antes de prestar qualquer suporte remoto.

## Algumas informações sobre o processo

Para agendar a verificação de um dispositivo remotamente, você precisa conversar previamente com a pessoa para informá-la de que:

* Ela terá de instalar um software de área de trabalho remota antes
* Terá de ficar na frente do computador durante a verificação para inserir a senha de administrador (uma verificação geralmente dura entre 30 minutos e uma hora)
* Terão de remover o software de área de trabalho remota depois


Lembre-se de que [trust](trust.md) é uma parte fundamental de qualquer suporte de segurança, portanto, certifique-se de que o processo esteja claro para a pessoa que você está apoiando e que ela consinta com isso.


