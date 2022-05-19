[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/3-Comparando%20Modelos.md)

Discutimos bastante o que são branches e quais estratégias de workflow se baseiam essa lógica. Em alguns momentos, foi mencionado que idealmente devemos utilizar menos ramificações quanto for possível, pois cada novo afastamento do trunk principal aumenta fatores de risco.

Uma nova funcionalidade pode demorar para ser implementada, então muitas vezes faz sentido termos um feature branch para desenvolver até a nova versão estar estável. Contudo, até nestes casos existem metodologias que evitam a criação de branches de vida longa. O nome dessas metodologias são Feature Flags e Branch by Abstraction*.

O que é o Feature Flag? Suponhamos uma nova funcionalidade em nosso projeto que terá um tempo longo de implementação. Contudo, não queremos criar uma nova ramificação para esse processo, queremos trabalhar diretamente com o master ainda que o código não esteja completo.

Anteriormente, comentamos que cada commit deve ser releasable, isto é, pode ser publicado. Existe uma maneira de trabalhar sem branches: a feature flag.

O código é inserido no master, mas ele não é visível para a equipe. O Feature flag server também para testar funcionalidades, por exemplo.

Branch by Abstraction, apesar do nome, não envolve a criação de uma nova ramificação. Temos um módulo ligado, uma parte da aplicação utiliza uma biblioteca antiga e precisa ser substituída. Esse é um processo lento, e muitos elementos precisam ser alterados.

O primeiro passo é introduzir uma abstração no código principal, isto é, uma camada intermediária para isolar o código que utiliza o módulo, portanto todas as chamadas deverão passar pela camada de abstração. Essa camada pode ser uma interface, várias ou mesmo uma classe que realiza delegações.

Uma vez que é aplicada essa técnica de desacoplamento, podemos gradativamente fazer a re-implementação. Podemos utilizar um módulo legado para o que é de fato utilizava o módulo antigo. 

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/5-2-modulo.png)

Com o tempo, o módulo antigo fica em desuso e pode ser suprimido completamente.

No mundo ideal, todas as features tem uma granulidade suficiente para não precisar necessitar de um branch de vida longa, mas como nem sempre o ideal é possível, foram criadas essas técnicas.

[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/6-Merge%20e%20Rebase.md)
