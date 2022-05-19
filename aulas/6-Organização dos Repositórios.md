[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/5-Sistema%20de%20Controle%20de%20Vers%C3%A3o.md)


Nesta aula veremos como organizar nossos repositórios. Em uma empresa encontramos mais de um projeto por vez, e é importante que saibamos como representar estes projetos dentro do repositório.

O que é mais natural é utilizar um repositório para cada projeto, de um tamanho razoável com escopo bem definido. Essa forma de organização é chamada Multi-repo.

No entanto, nos últimos anos, surgiu uma nova forma de organização dos nossos projetos dentro de repositórios. Empresas grandes de tecnologia como Google e Facebook não utilizam o esquema Multi-repo, porque são empresas que trabalham em inúmeros projetos de maneira concomitante. Empresas que atuam com outra dimensão de projetos utilizam o Mono-repo, ou seja, um único e gigantesco repositório que acumula todos os projetos.

A desvantagem do segundo modelo é o repositório precisará ser realmente grande, e o build pode ser lento, talvez nem o Git seja mais a ferramenta adequada para fazer o controle de versões para esta situação. Contudo, como temos apenas um grande repositório temos uma administração relativamente mais simples, então a verificação de padrões é facilitada. A refatorações são globais, afinal estão todos dentro da mesma base.

Nosso curso será voltado para o Multi-repo, afinal é o mais comum no dia a dia da maioria dos desenvolvedores.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/1-O%20que%20s%C3%A3o%20branching%20models.md)
