# Cenário de Análise/Problema

<!-->> **_NOTE:_**: A equipe deve pensar em cenários existentes na atualidade (que causam problemas para os usuários) e que a interface prevista ajudará a resolver o problema. Cenário de Análise/Problema é uma história triste. Não descreve a solução. Descreve somente o problema.
-->

<!--
* Porque os atores querem ou precisam alcançar esse objetivo?
  * R: Para obter uma arena com mais facilidade.
* De que informações ou conhecimentos os atores precisam para realizar esse objetivo?
  * R: Entendimento sobre a arena da K404 e como a mesma funciona.
* Em que situações o cenário ocorre (quase, onde e pq)?
  * R: Quando disponível na Sala k404 da FEI por conta de aula ou testes.
* Quais são as tecnologias utilizadas no ambiente de trabalho? Como os usuários as utilizam?
  * R: Robôs, simuladores e ROS
* Quais características dos atores lhes auxiliam ou atrapalham em alcançar o objetivo?
  * R: Entendimento lógico, entendimento sobre a arena da K404, falta de autorização.
* Quem precisa ser notificado da conclusão (bem/mal sucedida) do objetivo?
  * R: O usuário
* Como os atores alcançam o objetivo atualmente?
  * R: Precisam montar arenas fisicamente e testar manualmente se a mesma lhes agrada.
* De que maneira o ambiente e o sistema auxiliam ou impedem que os atores tomem decisões adequadas?
  * R: Por ser um simulador, a interface auxilia no desenvolvimento da arena, tornando o processo manual para virtual.
* Que recursos estão disponíveis para realizá-la?
  * R: Simuladores e o computador.
* Quais problemas ou dificuldades podem surgir ao realizá-la?
  * R: Um processo a mais para fazer, mas facilitando outro futuro.
* Quais eventos disparam a necessidade de alcançar o objetivo?
  * R: A necessidade de montar arenas manualmente.
* Quais eventos são (deveriam ser) disparados pela conclusão desse objetivo?
  * R: facilitar o desenvolvimento de arenas simuladas baseadas na arena da k404
* Como os atores conseguem saber se uma ação foi concluída e realizada com sucesso?
  * R: O programa gera arquivos de mapa e .sdf para o usuário utilizar.
* Qual é o resultado do alcance do objetivo?
  * R: O usuário consegue desenvolver arenas de maneira mais simples, podendo desenvolver de maneira mais rápida.
  -->


<!--
## Ambiente e contexto

* Porque os atores querem ou precisam alcançar esse objetivo?
  * R: Para obter uma arena com mais facilidade.
* De que informações ou conhecimentos os atores precisam para realizar esse objetivo?
  * R: Entendimento sobre a arena da K404 e como a mesma funciona.
* Em que situações o cenário ocorre (quase, onde e pq)?
  * R: Quando disponível na Sala k404 da FEI por conta de aula ou testes.
* Quais são as tecnologias utilizadas no ambiente de trabalho? Como os usuários as utilizam?
  * R: Robôs, simuladores e ROS
* Quais características dos atores lhes auxiliam ou atrapalham em alcançar o objetivo?
  * R: Entendimento lógico, entendimento sobre a arena da K404, falta de autorização.
* Quem precisa ser notificado da conclusão (bem/mal sucedida) do objetivo?
  * R: O usuário
* Como os atores alcançam o objetivo atualmente?
  * R: Precisam montar arenas fisicamente e testar manualmente se a mesma lhes agrada.
* De que maneira o ambiente e o sistema auxiliam ou impedem que os atores tomem decisões adequadas?
  * R: Por ser um simulador, a interface auxilia no desenvolvimento da arena, tornando o processo manual para virtual.
* Que recursos estão disponíveis para realizá-la?
  * R: Simuladores e o computador.
* Quais problemas ou dificuldades podem surgir ao realizá-la?
  * R: Um processo a mais para fazer, mas facilitando outro futuro.
* Quais eventos disparam a necessidade de alcançar o objetivo?
  * R: A necessidade de montar arenas manualmente.
* Quais eventos são (deveriam ser) disparados pela conclusão desse objetivo?
  * R: facilitar o desenvolvimento de arenas simuladas baseadas na arena da k404
* Como os atores conseguem saber se uma ação foi concluída e realizada com sucesso?
  * R: O programa gera arquivos de mapa e .sdf para o usuário utilizar.
* Qual é o resultado do alcance do objetivo?
  * R: O usuário consegue desenvolver arenas de maneira mais simples, podendo desenvolver de maneira mais rápida.
  -->
  * **Persona: Robervaldo Arantes.**  
    * Robervaldo Arantes é um estudante que recém ingressou no curso de engenharia de robôs, na instituição da FEI, o mesmo ficou sabendo sobre uma arena onde testes com robôs podem ser realizados na sala K4-04, para utilizar a sala, é necessária uma autorização da instituição ou do professor que estiver utilizando a sala no momento as quais limitam muito o acesso de Robervaldo. Para tentar contornar isso, Robervaldo conseguiu um modelo da Arena da sala para utilizar em algum simulador, mas o mesmo não sabe sobre os obstáculos que podem ser implementados, tornando o uso da mesma, confuso e complicado.

  * **Persona: Edson Adalberto.**
    * O professor Edson Adalberto é um professor que trabalha muito com robôs, o professor estava pensando em um plano de aulas com exemplos mais práticos, para isso o mesmo decidiu utilizar a sala da K4-04 onde existe uma arena que o mesmo pode utilizar, esta arena possui uma base pronta, mas pode ser alterada pelo usuário com a adição de placas que funcionariam como paredes para dificultar a locomoção de um robô, mas o mesmo encontrou um problema que seria relacionado ao desenvolvimento da arena, para desenvolver labirintos para serem utilizados na aula, o mesmo precisa estar no campus e montar e desmontar a arena diversas vezes até encontrar uma arena que cumpra os requisitos que o mesmo deseja.

* **Persona: Kelly do Nascimento.**
    * Kelly do Nascimento começou a desenvolver uma iniciação cientifica com o título de "Aprimoramento de robô funcional da instituição." que possui o objetivo de melhorar um robô desenvolvido por outro aluno da instituição. Kelly conseguiu acesso ao robô real, seu modelo simulado e ao modelo simulado da arena os quais ela planeja usar para testes, logo o seu orientador concedeu acesso à sala K4-04 para a Kelly conseguir a usar fora dos horários de aula. Infelizmente devido a seu trabalho e a suas aulas, Kelly não tem tempo o suficiente para planejar, montar e testar uma arena presencialmente, então pensou em utilizar a arena simulada para ajudar no planejamento do presencial, mas sem as marcações de aonde as paredes podem estar o desenvolvimento se dificultou, forçando Kelly a gastar bastante tempo implementando na arena presencial.
 
# Questões de Refinamento
<!--
Robervaldo Arantes é um estudante que recém ingressou no curso de engenharia de robôs, na instituição da FEI, o mesmo ficou sabendo sobre uma arena onde testes com robôs podem ser realizados na sala K4-04, para utilizar a sala, é necessária uma autorização da instituição ou do professor que estiver utilizando a sala no momento as quais limitam muito o acesso de Robervaldo. Para tentar contornar isso, Robervaldo conseguiu um modelo da Arena da sala para utilizar em algum simulador, mas o mesmo não sabe sobre os obstáculos que podem ser implementados, tornando o uso da mesma, confuso e complicado.
-->
* **Persona: Robervaldo Arantes.**
  * Por quê?
    1. Por que usar a arena?
    2.  Por que não consegue utilizar a arena?
  * Como?
    1. Como pode se utilizar o modelo da arena?
    2.  Como pode contornar a falta de autorização?
  * O que é?
    1. O que é a arena da K4-04?
    2.  O que são os testes realizados?
  * Pode ser feito da maneira?
    1. Como podem ser feitos os testes?
    2.  Como pode ser utilizada a sala e a arena?
  * Faz parte de?
    1. A quem a arena pertence?
    2.  Qual o grande foco de alunos que fazem parte do grupo que pode utilizar a sala?
  * Objetivo?
    1. Qual o objetivo do interesse?
    2.  Qual o objetivo de testar os robôs?
  * Ambiente?
    1. Onde está localizada a arena?
    2.  Quais alterações podem ser feitas?
  * Ator(es)?
    1. Quem pode permitir o acesso à arena?
    2.  Quem possui o modelo da arena?
  * Planejamento?
    1. Por que deseja acessar a arena?
    2.  Como deseja utilizar a arena?
  * Ação?
    1. O que é realizado na arena?
    2.  O que o usuário pode realizar com a simulação?
  * Evento?
    1. Quando se pode utilizar a sala?
    2.  Quando os alunos podem utilizar a sala sem uma autorização da instituição?
  * Avaliação?
    1. Como os testes são avaliados?
    2.  Como é avaliado quem pode utilizar a sala?  
* **Persona: Edson Adalberto.**
  * Por que?
    1. Quem pode realizar os testes?
    2.  a?
  * Como?
    1. Quem pode realizar os testes?
    2.  a?
  * O que é?
    1. Quem pode realizar os testes?
    2.  a?
  * Pode ser feito da maneira?
    1. Quem pode realizar os testes?
    2.  a?
  * Faz parte de?
    1. Quem pode realizar os testes?
    2.  a?
  * Objetivo?
    1. Quem pode realizar os testes?
    2.  a?
  * Ambiente?
    1. Quem pode realizar os testes?
    2.  a?
  * Ator(es)?
    1. Quem pode realizar os testes?
    2.  a?
  * Planejamento?
    1. Quem pode realizar os testes?
    2.  a?
  * Ação?
    1. Quem pode realizar os testes?
    2.  a?
  * Evento?
    1. Quem pode realizar os testes?
    2.  a?
  * Avaliação?
    1. Quem pode realizar os testes?
    2.  a?  
* **Persona: Kelly do Nascimento.**
  * Por que?
    1. Quem pode realizar os testes?
    2.  a?
  * Como?
    1. Quem pode realizar os testes?
    2.  a?
  * O que é?
    1. Quem pode realizar os testes?
    2.  a?
  * Pode ser feito da maneira?
    1. Quem pode realizar os testes?
    2.  a?
  * Faz parte de?
    1. Quem pode realizar os testes?
    2.  a?
  * Objetivo?
    1. Quem pode realizar os testes?
    2.  a?
  * Ambiente?
    1. Quem pode realizar os testes?
    2.  a?
  * Ator(es)?
    1. Quem pode realizar os testes?
    2.  a?
  * Planejamento?
    1. Quem pode realizar os testes?
    2.  a?
  * Ação?
    1. Quem pode realizar os testes?
    2.  a?
  * Evento?
    1. Quem pode realizar os testes?
    2.  a?
  * Avaliação?
    1. Quem pode realizar os testes?
    2.  a?  
# Refinamento do Cenário Análise/Problema
* **Persona: Robervaldo Arantes.**
* **Persona: Edson Adalberto.**
* **Persona: Kelly do Nascimento.**
