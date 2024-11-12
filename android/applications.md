 Revisão dos aplicativos instalados

## ID do aplicativo

Alguns aplicativos mal-intencionados são apresentados como aplicativos legítimos, muitas vezes sendo uma cópia de um aplicativo legítimo com código mal-intencionado adicionado a eles. Vá para **Configurações > Aplicativos** e clique em cada aplicativo para verificar a respectiva ID na parte inferior da página.



![](../.gitbook/assets/Screenshot\_20220506-170511\_Settings.png)

O ID do aplicativo deve refletir o nome exibido do aplicativo, por exemplo, o ID do aplicativo autêntico da “Play Store” é `com.android.vending`; no entanto, também existem [malwares] (https://www.tomsguide.com/news/octo-android-malware-can-take-over-your-phone-how-to-protect-yourself) que fingem ser a Play Store com o ID `com.restthe71`.



### Versão do aplicativo

Na mesma página App Info, a versão do aplicativo também é exibida. É possível pesquisar a versão do aplicativo no Google para determinar se a versão realmente existe.Se houver muitos resultados de pesquisa retornados para a string de versão, então a versão provavelmente existe.Por exemplo, a captura de tela acima mostra que o aplicativo com.twitter.android versão 9.36.0-release.0 está instalado, e a pesquisa por “twitter 9.36.0” retorna muitos resultados de pesquisa, o que indica que essa versão provavelmente é legítima.No entanto, se você vir algo como “versão 100”, então o aplicativo provavelmente é falso.



## Permissões

Após concluir a verificação, desinstale os aplicativos do scanner para evitar a coleta de dados adicionais.

## Extraia pacotes de aplicativos (APKs)

Algumas ferramentas exigem que você extraia os arquivos APK manualmente e os carregue.



Abaixo estão algumas ferramentas que podem extrair APKs. * [Apk Extractor](https://play.google.com/store/apps/details?id=com.ext.ui\&hl=zh\_TW)



* [Apk Extractor (código aberto, última atualização em 2018)](https://f-droid.org/packages/axp.tool.apkextractor/)



* [Kanade](https://github.com/alexrintt/kanade) (código aberto, última atualização em 2022)

Depois que um APK é extraído, também é possível calcular o hash do arquivo (MD5 ou SHA) e pesquisar o hash usando sites como o VirusTotal.com .

## Ferramentas on-line

### [Exodus Privacy] (https://reports.exodus-privacy.eu.org/en/)

O Exodus Privacy é uma ferramenta para privacidade.

Ela pode analisar aplicativos e listar rastreadores contidos em um aplicativo.

### [Hybrid-analysis.com](https://www.hybrid-analysis.com/)

O Hybrid-analysis permite que você carregue um arquivo APK para análise.



Ele verifica o APK usando vários softwares antivírus e o VirusTotal.

### [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF)

O MobSF descompila o aplicativo e analisa seu conteúdo, listando itens como URLs, arquivos estáticos e atividades.Esses itens podem ser usados para motivar análises adicionais.

* Verifique se o aplicativo tem permissão para instalar outros aplicativos: consulte **Instalar aplicativos desconhecidos**

## Aplicativos em execução



Para inspecionar os aplicativos em execução, siga [este guia] (https://web.archive.org/web/20220509061723/https://www.techrepublic.com/article/how-to-view-all-running-services-on-android-11/).

Verifique os aplicativos desconhecidos em execução pesquisando seus nomes no Google.

Desative as Opções do desenvolvedor após inspecionar os aplicativos em execução para evitar o vazamento de informações.
