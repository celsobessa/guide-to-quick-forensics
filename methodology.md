# Metodologia

A metodologia para realizar análises forenses rápidas pode ser bastante ad-hoc e, com o tempo, você desenvolverá a sua própria metodologia. Este guia deve ajudar nesse processo. Em geral, ao tentar fazer a triagem de uma possível infecção, você procurará qualquer anomalia que possa identificar no dispositivo. Essas anomalias, por exemplo, podem ser:

1. Aplicativos e processos em execução no dispositivo que você e o proprietário do dispositivo não reconhecem. Aplicativos e processos que apresentam algumas características incomuns, como nomes e locais de arquivos suspeitos ou tentativas de ocultação.
2. Como o spyware normalmente deseja sobreviver a um desligamento do dispositivo, você procurará aplicativos que mantenham a persistência no dispositivo e, portanto, estejam registrados para execução automática na inicialização.
3. Conexões de rede suspeitas com infraestrutura e serviços que você e o proprietário do dispositivo não reconhecem.
4. Contas, perfis ou configurações que não pertencem ao proprietário do dispositivo.

Embora não seja possível compilar uma lista de verificação exaustiva de anomalias precisas a serem observadas, o processo de desenvolvimento de uma metodologia forense rápida e robusta exigirá _treinaro seu olho_, inspecionando o maior número de dispositivos possível. Eventualmente, você começará a reconhecer padrões em vários sistemas operacionais e se tornará mais rápido e eficiente para descartar aplicativos legítimos e identificar aqueles que se destacam. Isso requer prática.


**Aviso**: a metodologia que descrevemos neste guia depende muito do uso de ferramentas que estão disponíveis publicamente e são altamente populares. Por esse motivo, malwares mais sofisticados podem ser capazes de contornar ou evadir essas ferramentas e fazer com que você acredite que está vendo um sistema limpo. Portanto, **essametodologia precisa ser considerada um esforço máximo** Você deve levar em conta a possibilidade de falsos negativos e ajustar sua avaliação de acordo (especialmente em relação à [segurança] do proprietário do dispositivo (preparations/safety.md)).

## Considerações sobre litígios legais

Em algumas circunstâncias, é possível que o proprietário do dispositivo tenha interesse em entrar com alguma ação legal contra os autores do ataque que você está documentando ou, talvez, contra os produtores da tecnologia usada para conduzi-lo. Esse pode ser o caso, por exemplo, de vítimas de violência doméstica ou talvez de ativistas que buscam provar a vigilância ilegal de suas comunicações.


Se você acredita que a pessoa que você está ajudando pode estar interessada em qualquer forma de litígio legal, especialmente com base no seu trabalho, talvez seja necessário adaptar sua metodologia. De país para país, de jurisdição para jurisdição, as regras e as práticas recomendadas para a coleta de evidências digitais admissíveis no tribunal podem variar. Geralmente, por causa da [cadeia de custódia] (https://en.wikipedia.org/wiki/Chain\_of\_custody) e para proteger a integridade do dispositivo, a aquisição de dados (especialmente de telefones) pode ser muito restrita.

Você deve se informar sobre as leis e as práticas padrão da jurisdição em que normalmente opera. Idealmente, você deve buscar orientação de especialistas forenses locais e talvez até mesmo buscar a assistência de uma empresa forense credenciada.
