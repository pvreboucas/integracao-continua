[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-02/aulas/6-Merge%20e%20Rebase.md)

Estudamos os branchs, os work flows e concluímos que dentro da prática da integração contínua, devemos nos afastar o mínimo possível do nosso trunk master principal.

Com as alterações que realizamos o tempo todo em nosso software, como podemos garantir a qualidade do código? Testes. No caso da integração contínua, precisaremos utilizar testes automatizados. O ideal é que a cada alteração, seja realizado um novo teste automatizado, para termos certeza de nenhum problema será gerado.

* Testes fazem parte da construção do software
* Devem ser realizados antes do commit
* TDD pode ajudar neste processo
* Desempenho bom em testes 

Os testes demorados podem ser uma barreira para a integração contínua, por isso precisamos ficar atentos.

Abordaremos o TDD (Test Drive Development). Os testes em integração contínua são sobre feedback do software, como a maioria dos métodos ágeis.

![01](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/imagens/1-1-design.png)

Existem diversas categorias e níveis de testes automatizados, aqui descaremos três: unit tests, integration tests e functional tests.

Os unit tests verificam unidades, como métodos e funções dentro do software. São os testes mais rápidos, baratos de escrever e sua manutenção é simples.

Os testes de integração são de um nível mais alto, e testam a relação de elementos, como por exemplo um banco de dados e o software. A realização destes testes é mais lenta, afinal possuem um outro grau de complexidade.

Testes de um nível ainda maior, são os functional tests, que testam o sistema completo e garante a correção de funcionalidades no ponto de vista do cliente.

O que é importante pensarmos é no tempo de execução de testes que teremos. Os testes de unidade existem desde o início do projeto, qualquer commit deveria ser acompanhado por um teste.

É comum que o desenvolvedor que queria concluir um projeto rapidamente deixe de fazer testes para otimizar o tempo. Como resolver esse impasse? Antes do commit, devemos executar todos os testes, embora saibamos que isso é em um plano ideal, e muitas vezes desnecessário dependendo da modificação que foi realizada. Até mesmo executar todos os testes unitários pode ser complicado.

Uma técnica comum é executar o que chamamos de smoke tests. Na prática, trata-se de uma seleção de testes que garantem que as funcionalidades mais importantes do sistema estejam operando corretamente. Esses testes avaliam um conjunto menor de elementos, por isso são mais rápidos, e dessa maneira teremos a garantia de que o software está operante em sua estrutura básica. Depois disso, podemos aplicar todos os testes e garantir uma varredura maior de erros.

Em resumo, devemos observar a categoria de cada teste; em ambientes diferentes fazer escolhas de desempenho e que melhor atendam nossa demanda; aplicar boas práticas de testes ( testes isolados, legíveis, expressivos); realizar testes na parte de build e adquirir feedbacks o mais rápido o possível.

[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-03/aulas/3-Build%20Automatizado.md)
