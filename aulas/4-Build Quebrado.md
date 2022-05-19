[<< AULA ANTERIOR](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-04/aulas/1-Servidor%20de%20Integra%C3%A7%C3%A3o%20Cont%C3%ADnua.md)

No último vídeo falamos sobre servidores de integração, e paramos no ponto em que o um erro é notificado no build. É importante lembrar - e devemos pensar também no conceito de entrega contínua - que o software funcional é a principal métrica que devemos nos atentar.

É tarefa de toda uma equipe resolver um problema no build o mais rápido possível, afinal não poderá ser realizados novos commits até que o build esteja estável e confiável novamente. 

``` "Nobody has a higher priority task than fixing the build." -Kent Beeck ```

Caso o build não possa ser corrigido em um intervalo de tempo curto, o commit que gerou o problema deve ser desfeito para o que o projeto continue, e este é um ponto fundamental.

O que mais envolve a integração contínua? Conversaremos sobre o deploy nas próximas aulas.

[PRÓXIMA AULA >>](https://github.com/pvreboucas/integracao-continua-ci/blob/aula-05/aulas/1-Certifica%C3%A7%C3%A3o%20de%20CI.md)
