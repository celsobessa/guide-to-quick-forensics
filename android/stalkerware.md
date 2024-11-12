# Opcional: Verifique se há indicadores de instalação de stalkerware

Stalkerwares são aplicativos maliciosos usados ​​no contexto de violência de parceiros íntimos. Uma das diferenças com o malware Android clássico é que eles são instalados por meio de um acesso físico ao smartphone. Por isso, a instalação requer algumas alterações no sistema Android que geralmente podem ser identificadas posteriormente.

## Verifique se a instalação de fontes desconhecidas está autorizada

Os aplicativos stalkerware são instalados diretamente do arquivo do aplicativo (APK), que é proibido por padrão pelo Android. Para instalar o aplicativo, a pessoa precisa permitir a instalação de fontes desconhecidas.

Antes do Android 8 "Oreo", esse recurso era habilitado para todo o telefone. Se você tem um telefone anterior ao Android 8, vá para **Configurações > Segurança** e verifique se **Fontes desconhecidas** está habilitado.

![](../.gitbook/assets/unknown\_sources.png)

Após o Android 8, esse recurso é habilitado por aplicativo. Vá para **Configurações > Segurança > Instalar aplicativos desconhecidos** para ver a lista de aplicativos com permissão para instalar aplicativos não confiáveis.

![](../.gitbook/assets/unknown\_sources2.png)

Qualquer aplicativo nesta lista é suspeito, especialmente navegadores e gerenciadores de arquivos.

## Verifique se o Google Play Protect está desabilitado

O Google Play Protect é uma detecção automatizada de aplicativos maliciosos desenvolvida e mantida pelo Google como parte do Google Play Services. Esse recurso geralmente precisa ser desabilitado durante a instalação de um aplicativo stalkerware porque ele pode detectar o aplicativo malicioso.

Para verificar essa configuração, você deve ir para **Configurações > Segurança > Verificar dispositivos em busca de ameaças à segurança** ou **Configurações > Segurança > Google Play Protect** dependendo da sua versão do Android.

![](../.gitbook/assets/androidscan.png)

## Verifique se o telefone está rooteado

Um aplicativo stalkerware geralmente requer um telefone rooteado para ter acesso a mais dados. Siga as recomendações [desta outra parte deste guia](root.md) para verificar se o telefone está com root.
