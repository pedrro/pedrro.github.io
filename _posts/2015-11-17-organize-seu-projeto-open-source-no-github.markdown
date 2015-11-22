---
title:  "Organize seu projeto open-source no Github"
description: Saiba como organizar seu projeto open-source no Github.
date: 2015-11-17
---


Sabemos que no Github existem milhões de projetos open-source, cada um com seu objetivo e sua necessidade, mas eu sinto uma imensa dificuldade em saber, como eu realmente posso contribuir nesse projeto? Pois muitas vezes essas necessidades não estão documentadas em lugar nenhum, deixando possíveis contribuintes a deriva.
Então, para você que tem um projetinho open-source no Github, aqui vai algumas dicas de como organizar o seu projeto e atrair mais contribuidores.

###README
README? SIM, README! Ter um readme organizado ajuda as pessoas a entender o objetivo do seu projeto, então vale a pena você ter um read me que seja grande mas que demonstre o que você quer com o seu projeto. Ok, beleza, mas o que eu devo ter no meu read me então?

Adicione no seu readme tudo que seja relevante para quem for ajudar não fique perdido, alguns bons tópicos a serem colocados são:

<ul>
 <li>intenção do projeto</li>
 <li>tech stack	</li>
 <li>rodar o projeto local</li>
 <li>como contribuir</li>
 <li>licença</li>
</ul>


Exemplos de bons readme para serem vistos:

* [Registro Livre](https://github.com/ThoughtWorksInc/registrolivre)
* [FreeCodeCamp](https://github.com/FreeCodeCamp/FreeCodeCamp)
* [Go](https://github.com/golang/go)


Um ponto que deve ser levado em consideração(pelo menos eu levo), se seu readme está grande demais, talvez seja melhor refatorar e criar uma wiki para seu projeto.

###Wiki
Sim, o Github fornece a possibilidade de criar wiki's para o seu projeto, aonde nessa wiki, é colocada informações relevantes sobre o projeto, por exemplo:

<ul>
 <li>como cada componente funciona</li>
 <li>como a arquitetura do projeto foi pensada</li>
 <li>qual o padrão de nomenclatura do projeto</li>
 <li>como resolver possíveis erros no projeto</li>
 <li>instalação</li>
 <li>contribuidores</li>
</ul>


Basicamente, tudo que não se encaixou no readme e é relevante para o projeto, vai para a wiki. Na wiki tópicos podem ser divididos por páginas o que torna as informações mais visiveis e organizadas, existe uma sessão no github aonde mostra uma lista com vários projeto que usam a wiki de formas bem legais, você pode encontrar [aqui](https://github.com/showcases/projects-with-great-wikis).

###Issues
 O GitHub também provê de uma sessão de cadastro de issues aonde podem ser adicionados labels customizados para defeitos, estórias, bug's e etc.. O uso do issues é muito importante para um colaborador, pois através dele, o colaborador consegue entender qual é a necessidade do projeto atual do projeto e como ele pode contribuir.

 Mas ainda assim, não basta cadastrar a issue, ela tem que ser descrita de forma que o colaborador entenda qual a intenção da issue. Outra forma de utilizar a sessão de issues, é transformar a lista em um board kanban através de ferramentas como o [Tablero](https://github.com/TWtablero/tablero) e o [Waffle](https://waffle.io/).

![Board Issues Pixelated](/assets/images/posts/organize_github/Issues_pixelated.png)

![Exemplo kanban online com tablero](/assets/images/posts/organize_github/pixelated_tablero.png)

 Um ponto legal é sinalizar suas issues com tag's customizadas, que podem informar se a issue é um bug, uma feature, se pode ser resolvidade por iniciantes ou não, essas coisas ajudam a entender sobre a issue que está sendo criada.



Bom pessoal, esse post fica por aqui, espero que com ele você consiga estruturar melhor o seu repositório no github. :)
