[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/1-Self%20Testing.md)

Discutimos sobre testes automatizados e a importância dessa prática na lógica da integração contínua. Apenas executar testes durante a integração do commit não basta, precisamos também construir nosso software, que segue algumas etapas clássicas.

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/imagens/3-1-etapas.png)

Primeiro realizamos os smoke tests para garantir as funcionalidades essenciais estejam operantes. Então podemos incluir uma análise estática para garantir que o commit coninua baseado nos padrões estabelecidos, e então poderemos criar o primeiro artefato do build.

Para realizar essas etapas de maneira contínua, devemos automatizar o máximo possível esses processos. Existem ferramentas específicas para isso, no mundo Java existe o Gradle e Maven por exemplo.

Em resumo:

* Build a cada commit
* Automatização
* Build independente da IDE
* Todo conteúdo necessário armazenado no repositório

A metáfora do "integrate button" nós é útil agora. Devemos ter um comando simples para realizar builds rápidos. A depender do projeto, é possível que nem todas as fases sejam realizadas.

![02](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/imagens/3-2-book.png)

Quando falamos em um buil rápido, podemos utilizar as ideias de XP Programming, em que o build não deve durar mais de 10 minutos. Otimizar o build é importante, e nestes casos métricas ajudam, e elas podem ser adquiridas por meio das ferramentas de automação que comentamos anteriormente.

Em resumo:

* Verifique a fase de testes e analise o código
* Verifique a ordem dessas fases
* Verifique a infra do build system
* Use cache
* Use staged build/pipeline

Não devemos fazer builds periódicos, e eles devem ser independentes da IDE, todo conteúdo necessário para o desenvolvimento deve estar no repositório.

Precisamos, ainda, definir a organização dos artefatos que forem criados pela aplicação, em que locais serão armazenados os scripts e relatórios, por exemplo. Além disso, devemos usar um build machine, afinal pode ser que na máquina local não seja possível executar todas as etapas do build. Nos aprofundaremos mais no assunto na próxima aula.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-04/aulas/1-Servidor%20de%20Integra%C3%A7%C3%A3o%20Cont%C3%ADnua.md)
