[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/3-Build%20Automatizado.md)


Discutimos sobre testes automatizados e builds automatizados. Idealmente, cada desenvolvedor deverá realizar os testes adequados para garantir que não haja quebras e então passar as informações para o repositório central. Mas quem pode garantir que o desenvolvedor de fato cumprirá esse processo?

Existem casos por questão de tempo em que não podemos realizar todos os testes necessários ou o projeto é tão complexo que não pode ser testado integralmente em uma máquina local.

Em algum momento precisamos encontrar um local que realmente será capaz de testar todo o projeto, e este é o CI Daemon ou server de integração. Esse servidor irá garantir que a cada modificação seja realizado um novo teste, então o repositório é sempre checado e builds contínuos são uma realidade.

A prática de integração contínua não especifica que o CI Daemon é necessário, mas hoje em dia podemos considerar como uma obrigação nos projetos. Contudo, só porque utilizamos um server desas natureza estamos praticando integração contínua, uma ação é realizada por pessoas.

O CI Daemon realiza builds contínuos e notifica os desenvolvedores se alguma alteração se deu corretamente ou não. Normalmente esses softwares já possui um test board que oferecem os dados do build, então as informações e relatórios são de fácil acesso.

Existem alguns serviços no mercado que podem ser instalados localmente, o Jenkins é um exemplo. Existem também serviços na nuvem já associados. É importante que apenas que o servidor realize buidls a cada commit e notifique os desenvolvedores de maneira clara e funcional.

Alguns servidores oferecem o private build, que possibilita o desenvolvedor a fazer uma observação do repositório e testa-lo antes da produção, com um build mais completo.

Mas e se ocorre a notificação de um erro? Como devemos proceder?


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-04/aulas/4-Build%20Quebrado.md)
