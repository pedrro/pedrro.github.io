---
title:  "Testes de Performance"
description: Uma breve introdução sobre Testes de Performance e como ele é útil para o nosso sistema.
## date: add a date when publishing
---

Essa semana aprendi um pouco sobre testes de performance, que até então, eu não sabia NA-DA. Nesse post, irei falar sobre o que é o teste de performance, tipos e ferramentas, beleza?

## Testes de performance, o que é?

Testes de performance, tem como objetivo, avaliar como o seu sistema se comporta em diversas situações, por exemplo:
>Em uma situação de stress, o seu sistema irá ser avaliado durante algum tempo com uma alta carga de request que seu sistema não está acostumado a receber. 

Isso é muito legal, porque me faz pensar, quantas vezes estamos realmente pensando na performance do sistema durante o seu desenvolvimento? Quase nunca, mas, todos devemos ter esse pensamento, pois a performance do seu sistema vai impactar para o usuário final, que vai impactar para a avaliação do seu sistema e vai impactar em como as pessoas olham para o seu trabalho e quando você se der conta, que o cuidado com a performance do sistema não foi levado em consideração, já vai ser tarde demais e acabará se tornando um snowball sem fim, OMG!

Mas não se assuste, o teste de performance abrange vários conceitos que podem ser aplicados para diversas situações.

## Tipos de testes de performance

Então, para começo de conversa, sei de 3 tipos principais de testes, que são:

###Teste de carga
Teste de carga serve para verificar quanto tempo um request demora a carregar no servidor com uma certa quantidade de usuário, digamos que tem 1000 usuários realizando login ao mesmo tempo, ai com esse tipo de teste, voce consegue verificar como a sua aplicação se comporta. Ele também pode ser aplicado aumentando gradativamente o número de requests que a aplicação vai receber, com isso você consegue observar como o sistema vai reagindo até atingir um ponto em que ele se torna instável e depois você diminui os requests também gradativamente para até chegar um ponto que ele ficará estável novamente.

![Teste de Carga](/assets/images/posts/teste_de_performance/Teste_de_Carga.png)

###Teste de stress
Testes de stress, é realizado para saber como o seu sistema vai reagir em uma situação aonde seu sistema não está acostumado a lidar, um exemplo seria um pico de usuários durante algumas horas no seu site, digamos que seja black friday, como sabemos, muitas vezes começam a meia noite de sexta-feira e quando as promoções são liberadas a essa hora o número de usuários que normalmente acessam um site cresce muitas vezes mais, então o teste de stress vai avaliar como seu servidor vai aguentar e como ele se comporta durante esse tempo de estresse. E esse teste não vem a ser executado só com foco em performance, mas, também focado na segurança do sistema, pois, um sistema que está sobre estresse, em uma situação como essa, pode vir a mostrar suas vulnerábilidades e estar mais aberto a sofrer ataques.

![Teste de Carga](/assets/images/posts/teste_de_performance/Teste_de_Stress.png)

###Teste de capacidade
Teste de capacidade são responsáveis por medir até aonde o seu sistema é capaz de atuar sem problemas com determinada carga até que o tempo de resposta seja inaceitável(certa vez eu li, que um sistema web não deve ultrapassar mais de 10 segundos de carregamento de uma página e esse tempo de resposta é mais baixo para dispositivos móveis). Geralmente são realizados com uma carga normal, pois acima disso ele já se torna um teste de stress.

![Teste de Carga](/assets/images/posts/teste_de_performance/Teste_de_Capacidade.png)

E aí, explicado o que são cada um desses testes, o que você achou? Na minha opinião eles são muito parecidos, são apenas pequenos detalhes e modos que são executados que realmente diferem um teste do outro. Por exemplo, a diferença entre o teste de stress e o de capacidade é a diferença de requests que você vai realizar no teste e com esses requests que os testes se diferenciam.

##Ferramentas de teste de performance

Beleza, agora que já falei o que é o teste de performance e quais são os tipos de performance você deve estar se preocupando, aonde eu escrevo os testes para isso? Então amigo, vou mostrar algumas ferramentas agora, as mais famosas pelo menos.

###JMeter
[JMeter](http://jmeter.apache.org/) eu acho que é a mais famosa ferramenta open-source para testes de performance, ela oferece uma UI(um pouco bagunçada na minha opinião) para você realizar seus testes, também existe a possibilidade de adicionar alguns plugins que irão facilitar a sua vida e criar os seus testes para JUnit, também conta com muito material pela internet para estudo.

###LoadRunner
[LoadRunner](http://www8.hp.com/us/en/software-solutions/loadrunner-load-testing/), sinceramente eu não conheço muito sobre essa ferramenta, o pouco que sei é que ela foi criada pela HP e é uma ferramenta paga, que é bastante usada em empresas grandes que ainda utilizam formas tradicionais de desenvolvimento(Waterfall).

###Gatling
[Gatling](http://gatling.io/#/) é uma ferramenta de testes de performance que vem crescendo e se tornando conhecida, nela você usa a linguagem Scala para fazer seus testes de performance. Pelo pouco que vi da ferramenta, ela gera gráficos e relatórios mais visuais que o JMeter e não tem uma UI tão bagunçada.

#### Links de referência

Para pegar como base para fazer esse artigo, utilizei esses artigos:
<ul>
 <li>[Client-Side performance testing tutorial](https://www.thoughtworks.com/insights/blog/client-side-performance-testing-tutorial)</li>
 <li>[Bug Bang - Destilando Jmeter](http://www.bugbang.com.br/destilando-jmeter-i-introducao-e-conceitos/)	</li>
</ul>

Então, esse é o final desse post, espero que você tenha aprendido pelo menos o básico sobre testes de performance, assim como eu aprendi. Para o futuro planejo criar um post para explicar como implementar alguns cenários de testes no JMeter, abraços!