[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/6-Organiza%C3%A7%C3%A3o%20dos%20Reposit%C3%B3rios.md)

Discutimos o que é a integração contínua, os problemas que ela busca resolver e suas vantagens enquanto prática de desenvolvimento. Além disso, apresentamos alguns modelos de repositório: Multi e Mono-repo.

Nesta aula estudaremos as ramificações ou branching models. De certa forma,o código deveria ter uma linha principal e todas as alterações realizadas devem refletir, por meio de commits, em seu master ou linha principal.

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/1-1-master.png)

No momento em que começamos a desenvolver uma nova funcionalidade, pode fazer sentido que se saia master para focar nessa nova característica. Esse processo é chamado de ramificação, o fluxo separado do código principal.

![02](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/1-2-ramificacao.png)

Não se trata de um processo novo, mas por que tocar neste tópico? O Git é a ferramenta mais popular no que envolve as práticas de integração contínua, e com ele a criação de ramos no código é menos custosa.

Criar os ramos com SVS, por exemplo, eram muito mais difíceis de realizar. Com o Git elas são mais leves, rápidas e fáceis de criar, o que reconduz estratégias de projeto.

Poderíamos pensar que existe uma ramificação para o desenvolvimento outra apenas para os releases como homologação.

![03](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/1-3-release.png)

Podemos ir muito além, existem modelos mais complexos: para cada feature existirá um ramo específico. 

![04](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/1-4-models.png)

Foram criadas por diferentes empresas e equipes semânticas específicas para o uso de modelos de ramificação. Um dos mais populares é o Git flow, mas teremos ainda o one flow, pull request flow, gitlab flow e assim por diante.

Devemos lembrar que o nosso master deve representar o core, o estado principal da aplicação. No momento em que criamos um branch, você se afasta do seu core. Muitas vezes isso é confortável para o desenvolvedor, porque ele atua em ambiente isolado e pode testar ações com mais autonomia.

Mas qual era a ideia de integração contínua? Alterar de maneira contínua o repositório principal. Martin Fowler declara: 

``` "Everyone commits To the Mainline every day." ```

A regra da integração continua é antecipar os problemas. A princípio, o branch pode ser um perigo, um ampliador de risco. Existem alguams regras que podemo minimizar esse risco:

* commits simples e releaseble, orientados à uma tarefa

* branches de vida curta, margens mais simples

* estratégia combinada pela equipe

Devemos lembrar que muitos branches geram mais burocracia, e apresentam suas desvantagens. Na próxima aula analisaremos algumas estratégias e modelos específicos.

[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/3-Comparando%20Modelos.md)
