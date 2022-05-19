[<< ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/tree/aula-02/aulas)

# Para saber mais: Algumas ferramentas



As ferramentas de automação e construção variam muito pois são especificas da linguagem e plataforma mas também variam na área de uso como desenvolvimento web, mobile ou data science. Além disso, existem ferramentas especificas para uma etapa de build como teste ou deploy. Enfim, a lista abaixo representa apenas alguns exemplos.

Ferramentas de automação e construção, separado por linguagem/plataforma:

* Java: Ant, Maven, Gradle
* Front-end: Gulp, Grunt, Webpack
* .NET: MSBuild
* Ruby: Rake
* Kotlin: Gradle
* Clojure: Leiningen
* C/C++: CMake/Make
* PHP: Composer

E alguns frameworks famosos da área de teste:

* Selenium (automação do navegador)
* Cucumber (testes de aceitação)
* Postman e SoapUI (testes de API)
* JMeter (stress tests)
* JUnit, xUnit, PHPUnit (automação de testes)
* entre muitos outros frameworks e bibliotecas

Para o configuration management e provisioning podemos mencionar:

* Ansible
* Puppet
* Chef
* Salt
* Terraform (cloud)

O configuration management / provisioning é sobre a instalação e manutenção da maquina.

Na Alura temos cursos específicos para a maioria das ferramentas.


# O que Aprendemos?



Nesta aula, aprendemos que:

* Para usar integração contínua com sucesso, é preciso ter testes automatizados
   * Esses testes devem verificar a maior parte do código
   * TDD é uma metodologia que pode ajudar na criação dos testes
   * Os testes representam feedback sobre a saúde/qualidade do seu projeto
* O desenvolvedor deve rodar os testes antes de enviar as alterações para o repositório
   * Se for impossível executar todos os testes (por causa da infraestrutura ou demora da execução), é possível executar apenas os testes de unidade ou uma suíte de testes mais importantes (smoke testes)
* O build do projeto deve ser simples e totalmente automatizado
   * É boa prática o uso de uma ferramenta especializada para o build do software
   * Tente usar um "single command build" para executar o build
* A execução dos testes e build não deve se tornar uma razão para atrasar o build, para evitar:
   * Otimize build
   * Tente respeitar o tempo de 10 minutos para o build (alguns falam de 5 minutos)
   * Se o build for falhar, a ideia é que ele falhe o mais rápido possível



[PRÓXIMO >>](https://github.com/pvreboucas/integracao-continua-ci/tree/aula-04/aulas)
