[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-05/aulas/1-Certifica%C3%A7%C3%A3o%20de%20CI.md)

Discutimos até aqui os processos da integração contínua: repositórios, servidor de integração, relatórios, notificações, artefato de build e assim por diante. Contudo, será que só essas práticas são o suficiente no desenvolvimento de softwares?

Observemos o famoso manifesto ágil:

``` "Working software over comprehensive documentation" ```

Um softawere funcional é mais importante do que uma documentação enorme. Mas o que significa um software funcional?

Novamente observaremos outra citação do manifesto ágil: 

``` "Our highest priority is to satisfy the customer through early and continuous delivery of valuable software." ```

A prioridade mais alta é deixar o cliente satisfeito, e isso é feito por meio de entrega contínua. Isto é, um software funcional é aquele usado pelo cliente com suas novas features de maneira confiável. A integração contínua é uma parte fundamental para se chegar à entrega contínua.

Ao revisitarmos a metáfora do botão de integração em que tudo é simples e automatizado, devemos ter um outro botão de "release", isto é, de deploy.

Qual alteração que chega em nosso trunk principal e pode entrar em produção? Obviamente existem decisões de negócio sobre lançar novas features, como esperar datas comerciais importantes. Mas na visão técnica, devemos saber quais são as modificações aplicáveis.

A entrega contínua é um assunto para um próximo curso, mas sobrevoaremos alguns conceitos e suas principais características.

Dentro da arquitetura da aplicação, é anexado um novo requisito funcional: "deployability". Esta característica deveria ser pensada desde o início, pois devemos entregar com frequência o software funcional.

Um deployment pipeline é um fluxo em que o artefato passa e cada etapa incrementa e agrega mais segurança ao se aproximar do ambiente de produção.

Deploys de baixo risco são aqueles experimentais, contínuos, atualizações pontuais acompanhadas. Devemos separar a ideia de "deploy" e "publicação".Otimizar para resiliência é prevenir erros. No contexto de integração e entrega contínua temos o deploy contínuo.

As equipes de desenvolvimento normalmente possuem divisões, como as pessoas do QA,deploy e operações. As tarefas são delegadas para os subgrupos durante o projeto. Equipes separadas que mal se comunicam dificultam o andamento do trabalho, aumentam a possibilidade de problemas e atrasam os deploys.

A entrega contínua também exige uma mudança no comportamento e na cultura da empresa: as pessoas precisam trabalhar integradas.

[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-05/aulas/4-Sobre%20DevOps.md)
