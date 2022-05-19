[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/3-Entendendo%20o%20Problema.md)



Antes de passarmos para os modelos de integração, discutiremos brevemente sobre os VCS, Modelos de controle de versão.

Em uma equipe de desenvolvimento, precisaremos de uma ajuda para sincronizar e manter o histórico do código, de maneira concreta utilizamos ferramentas como Git e SVN.

A integração contínua não possui necessidade de muitas ferramentas, em tese, mas alguns auxílios que são padrão em práticas de desenvolvimento são requiridos.

O Git é o mais popular em integração hoje em dia, mas não precisamos utiliza-lo, basta que tenhamos algum modelo de controle de versão de nossa escolha.

A ferramenta em si não importa, mas o que devemos inserir em nosso sistema de controle? De maneira geral, deve conter tudo aquilo que é necessário para a construção do projeto.

* código
* scripts
* migrações, schemas
* IDE Configs

Devemos definir uma formatação de código para a equipe. Para começarmos um projeto é necessário fazer o clone - a cópia local - e o comando unificado.

Não significa que devemos comitar o artefato de construção, ou seja, no caso de um desenvolvedor Ruby ou Gem não deveria estar dentro do repositório, o mesmo ocorre no mundo Java. Resultados da construção do software não são comitados como como gem, jar, image e modules.

Sabemos o que comitar e o que não comitar, então seguiremos estudando os modelos de repositório que exitem no mercado.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/6-Organiza%C3%A7%C3%A3o%20dos%20Reposit%C3%B3rios.md)
