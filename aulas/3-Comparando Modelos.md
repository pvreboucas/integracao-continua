[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/1-O%20que%20s%C3%A3o%20branching%20models.md)

Discutimos o que são as ramificações, e é chegado o momento de comparar os modelos populares que existem e elencar suas vantagens e desvantagens.

Alguns branching models famosos são:

* Temporários (branches locais) São branches localizados apenas na máquina local e deverão se extiguir, são utilizados para organizar fluxos de trabalho e depois realizar o commit.

* Feature Branches São utilizados para implementar funcionalidades ou orientar tarefas.

* Historical Branches (master e develop) As alterações ficam organizadas em commits baseados na cronologia no caso de um projeto de software.

* Environment Branches (Staging e Production)] Existem branches que são baseados no ambiente, isto é, em que espaço é realizado o deploy.

* Maintenance Branches (Release e Hotfix) Temos, ainda, os branches de manutenção do sistema.

Estudaremos cada um deles com mais detalhes. O primeiro modelo é o mais simples, menos sofisticado de todas as ramificações, mas reduz a distância de um branch para o master até o mínimo possível. [Nesta página](https://trunkbaseddevelopment.com/) encontramos algumas referências de como utilizar essta metologia.

O modelo future branch workflow, já mencionado no curso, faz parte da realidade de mais desenvolvedores. A ideia é simples: precisamos implementar uma nova funcionalidade e então criamos uma ramificação para este fim. 

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/3-1-feeeature.png)

Uma vez implementado, ele será comitado ao master e então teremos duas fontes de rebase, e que ainda deverão ser discutidas.

Algo comum - inclusive utilizado aqui na Alura - é combinar o future branch work flow com o pull request. 

![02](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/3-2-pul%2Brequest.png)

A partir de um recurso do Git, fazemos a implementação, mas não podemos - ou não queremos - fazer o merge diretamente no master. Neste caso, utilizamos o pull request. Uma fez que a feature estiver finalizada, o pull request notifica todos os envolvidos da equipe, e então será avaliado o merge com o master.

Contudo, lembramos que a ideia da integração contínua são commits diários no repositório principal, e o pull request não deixa de ser uma barreira.

Esse processo é muito comum em projetos open source, em que outras pessoas podem clonar o código e enviar pull requests, e neste caso é um processo que faz sentido. Contudo, em um ambiente de equipe temos uma barreira.

O pull request dialoga com a prática de code review, em que os desenvolvedores conversam e discutem sobre a estrutura do código e fazem tomadas de decisão. Mas o code review independe do pull request. Esse fluxo de trabalho é chamado de Github Flow.

Outro modelo de ramificações é o Gitlab Flow, que apresenta as mesmas características principais do Github Flow, contudo possui mais ramificações, chamados environment branches. 

![03](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/3-3-ramificacoes.png)

Eventualmente, não podemos realizar o deploy integral de tudo que está no master de uma vez. Precisaremos fazer um deploy planejado antes de inserir a aplicação em produção.

Novamente, esse processo gera mais complexidades e mais dificuldades, mas em alguns casos esse processo é necessário.

O mais popular - e mais complexo - modelo de trabalho é o Git Flow. Obviamente, apesar da popularidade do modelo, os problemas de gerar muitos intermédios são os mesmos. 

![04](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/imagens/3-4-git.png)

O branch que representa o histórico de trabalho é o "develop", e os features são integrados e ao final ocorre o commit. Se em algum momento desejamos criar uma nova versão, criaremos um novo branch a partir de um commit.

Uma vez que a nova versão foi liberada e revisada, se libera uma comitação no master, que represesenta os releases em produção.

Se surge algum problema em tempo de produção, é criado uma nova ramificação e implementar o Hotfix e então lançar uma nova versão no master.

Portanto existem vários caminhos que o código percorre. Não sabemos dizer qual é o trunk mais atualizado: master, release ou develop, afinal possuem uma autonomia que pode gerar confusão em algum momento, além de criar uma maior complexidade no sistema de automação.

Essa não é uma prática da integração contínua, como é declarado em vários artigos sobre o assunto.

Esses são os modelos mais comuns de work flow no mercado. A complexidade amplia gradativamente como foi apresentado na aula.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/5-Branch%20by%20abstraction.md)
