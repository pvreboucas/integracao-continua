[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/5-Branch%20by%20abstraction.md)

Conversamos sobre branches, work flows e como evitar ramificações de vida longa. Nesta aula, atacaremos um novo problema em que deveremos optar por merge ou rebase.

Mas quais são as diferenças entre merge e rebase? Temos um master e um feature branch, baseado no primeiro commit do master e as duas ramificações evoluiram ao mesmo tempo. Em algum momento, o desenvolvedor decide enviar as atualizações para o master, isto é, realizar a sincronização.

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/6-1-sincro.png)

O comando clássico para essa situação é o merge, e então ocorre o chamado "merge commit", cria-se um novo commit que representa esse momento de sincronização.

![02](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/6-2-merge%2Bcommit.png)

Há desenvolvedores que não gostam desse processo, afinal trata-se de um commit que simplesmente representa um evento e que seu estado é baseado nas alterações realizadas na feature branch e na commit do master. Dessa maneira já não temos uma linha histórica muito interessante no desenvolvimento do projeto, o que pode gerar confusões.

Outra maneira de sincronizar o branch é pelo uso do rebase. Neste caso, a ideia é que se mude a base do commit, e então as modificações são aplicadas nessa nova base.

Dessa maneira, temos um histórico diferente de trabalho, e é por isso que o rebase deve ser aplicado apenas em máquina local.

![03](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/6-3-rebase.png)

A mudança então pode ser enviada de fato ao master e novamente temos um histórico linear. 

![04](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/6-4-linear.png)

Quando este processo estiver concluído, podemos inclusive excluir a feature branch.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/1-Self%20Testing.md)
