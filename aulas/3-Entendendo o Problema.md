[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/1-Introdu%C3%A7%C3%A3o.md)

Nesta aula falaremos de práticas concretas relacionadas à integração contínua e quais são os problemas que ela busca resolver.

O software na atualidade não é criado a partir de um único desenvolvedor, as equipes são multifuncionais que alterarão a mesma base de código.

Cada desenvolvedor terá o seu código local em sua máquina, embora haja um repositório compartilhado. Muitas vezes o desenvolvedor deverá fazer alterações solicitadas pelo cliente, corrigir bugs e assim por diante.

As alterações, inicialmente, são feitas no código local de cada desenvolvedor e só então deverão ser aplicadas no repositório compartilhado. Neste momento é que temos o ponto crítico.

É comum que a sincronização da cópia local com o repositório demore, e então esta etapa é feita normalmente ao fim do processo de desenvolvimento.

No momento em que os desenvolvedores começam a sincronizar os códigos, aparecem os problemas. Trata-se de um evento especial, tanto que em alguns casos existe um desenvolvedor sênior que irá monitorar esse processo.

Como se trata de um processo demorado, outros ambientes ficam desatualizados, como o de teste. Muitas vezes testamos casos que não são mais reais dentro do projeto, por isso devemos conseguir acelerar esse processo.

Integração contínua, em outras palavras, nada mais é que integrar as atualizações frequentemente na base diária.

Temos o tempo, um sprint, em que existem várias interações. No fim desse sprint acontecem as integrações e isso aumenta o risco de problemas, exatamente pela sincronização se dar ao final do ciclo de software.

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/imagens/3-1-grafico.png)

O código que planejamos localmente e funcionava, pode sofrer incompatibilidade com as alterações de outros desenvolvedores, além de problemas de versões e bugs. Tudo isso irá atrasar o projeto.

O ideal é tenhamos uma integração contínua, pequenas alterações todo o tempo, e assim garantir que o software funcione de maneira adequada. Dessa maneira teremos sempre um feedback rápido.

![02](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/imagens/3-2-continuidade.png)

Segundo a Thought Works, integração contínua é: 

``` "Continouous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day." ```

Existem várias técnicas e ferramentas que podem ajudar a aplicarmos a CI. Ao longo do curso aprenderemos alguns recursos para de fato utilizar essa metodologia no dia a dia de desenvolvimento.


[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-01/aulas/5-Sistema%20de%20Controle%20de%20Vers%C3%A3o.md)
