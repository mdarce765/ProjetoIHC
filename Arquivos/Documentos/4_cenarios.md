# Cenário de Análise/Problema

<!-- -> **_NOTE:_**: A equipe deve pensar em cenários existentes na atualidade (que causam problemas para os usuários) e que a interface prevista ajudará a resolver o problema. Cenário de Análise/Problema é uma história triste. Não descreve a solução. Descreve somente o problema.
-->
## Qualidade de uso
- Usabilidade:
  - Sua importância é muito necessária, o intuito do projeto é o de facilitar o desenvolvimento de arenas relacionadas a arena da sala k4-04, para isso foi pensado um sistema de botões que representam as posições em que os obstáculos possam ser posicionados na arena real, pois é visado a fidelidade da arena e suas possíveis formações.
- Experiência de usuário:
  - É esperado que o usuário se sinta satisfeito ao utilizar o produto, por conta de ter um processo facilitado, quando comparado com ter que modificar manualmente a arena. 
- Acessibilidade:
  - O programa possuirá uma maneira para aplicar zoom nas imagens e aumentar o texto, para auxiliar pessoas com deficiências visuais. 
- Comunicabilidade:
  - A interface principal possui uma imagem da arena presente na K4-04 com a vista de cima, facilitando o entendimento e interpretação do oque está fazendo.

## Cenário de Análise/Problema
  * **Persona: Robervaldo Arantes.**  
    * Robervaldo Arantes é um estudante que recém ingressou no curso de engenharia de robôs, na instituição da FEI, o mesmo ficou sabendo sobre uma arena onde testes com robôs podem ser realizados na sala K4-04, para utilizar a sala, é necessária uma autorização da instituição ou do professor que estiver utilizando a sala no momento as quais limitam muito o acesso de Robervaldo. Para tentar contornar isso, Robervaldo conseguiu um modelo da Arena da sala para utilizar em algum simulador, mas o mesmo não sabe sobre os obstáculos que podem ser implementados, tornando o uso da mesma, confuso e complicado.

  * **Persona: Edson Adalberto.**
    * O professor Edson Adalberto é um professor que trabalha muito com robôs, o professor estava pensando em um plano de aulas com exemplos mais práticos, para isso o mesmo decidiu utilizar a sala da K4-04 onde existe uma arena que o mesmo pode utilizar, esta arena possui uma base pronta, mas pode ser alterada pelo usuário com a adição de placas que funcionariam como paredes para dificultar a locomoção de um robô, mas o mesmo encontrou um problema que seria relacionado ao desenvolvimento da arena, para desenvolver labirintos para serem utilizados na aula, o mesmo precisa estar no campus e montar e desmontar a arena diversas vezes até encontrar uma arena que cumpra os requisitos que o mesmo deseja.

* **Persona: Kelly do Nascimento.**
    * Kelly do Nascimento começou a desenvolver uma iniciação cientifica com o título de "Aprimoramento de robô funcional da instituição." que possui o objetivo de melhorar um robô desenvolvido por outro aluno da instituição. Kelly conseguiu acesso ao robô real, seu modelo simulado e ao modelo simulado da arena os quais ela planeja usar para testes, logo o seu orientador concedeu acesso à sala K4-04 para a Kelly conseguir a usar fora dos horários de aula. Infelizmente devido a seu trabalho e a suas aulas, Kelly não tem tempo o suficiente para planejar, montar e testar uma arena presencialmente, então pensou em utilizar a arena simulada para ajudar no planejamento do presencial, mas sem as marcações de aonde as paredes podem estar o desenvolvimento se dificultou, forçando Kelly a gastar bastante tempo implementando na arena presencial.
 
# Questões de Refinamento
* **Persona: Robervaldo Arantes.**
  * Por quê?  
     1 - Por que usar a arena?  
     2 - Por que não consegue utilizar a arena?  
  * Como?  
     3 - Como pode se utilizar o modelo da arena?  
     4 - Como pode contornar a falta de autorização?  
  * O que é?  
     5 - O que é a arena da K4-04?  
     6 - O que são os testes realizados?  
  * Pode ser feito da maneira?  
     7 - Como podem ser feitos os testes?  
     8 - Como pode ser utilizada a sala e a arena?  
  * Faz parte de?  
     9 - A quem a arena pertence?  
     10 - Qual o grande foco de alunos que fazem parte do grupo que pode utilizar a sala?  
  * Objetivo?  
     11 - Qual o objetivo do interesse?  
     12 - Qual o objetivo de testar os robôs?  
  * Ambiente?  
     13 - Onde está localizada a arena?  
     14 - Quais alterações podem ser feitas?  
  * Ator(es)?  
     15 - Quem pode permitir o acesso à arena?  
     16 - Quem possui o modelo da arena?  
  * Planejamento?  
     17 - Por que deseja acessar a arena?  
     18 - Como deseja utilizar a arena?  
  * Ação?  
     19 - O que é realizado na arena?  
     20 - O que o usuário pode realizar com a simulação?  
  * Evento?  
     21 - Quando se pode utilizar a sala?  
     22 - Quando os alunos podem utilizar a sala sem uma autorização da instituição?  
  * Avaliação?  
     23 - Como os testes são avaliados?  
     24 - Como é avaliado quem pode utilizar a sala?  

* **Persona: Edson Adalberto.**
  * Por quê?  
     1 - Por que utilizar a sala?  
     2 - Por que utilizar a arena da K4-04?  
  * Como?  
     3 - Como Edson planeja melhorar suas aulas?  
     4 - Como a arena pode ser editada?  
  * O que é?  
     5 - Qual a dificuldade em montar as arenas?  
     6 - ?  
  * Pode ser feito da maneira?  
     7 - Como Edson planeja tornar as aulas mais dinâmicas?  
     8 - Como as arenas são montadas atualmente?  
  * Faz parte de?  
     9 - Por que Edson pode utilizar a sala K4-04 livremente?  
     10 - Qual aula é ministrada por Edson?  
  * Objetivo?  
     11 - Qual o objetivo de Edson em utilizar a sala?  
     12 - ?  
  * Ambiente?  
     13 - Onde os testes serão realizados?  
     14 - Quais obstaculos podem ser utilizados na arena?  
  * Ator(es)?  
     15 - Quais alunos poderão testar os robôs?  
     16 - ?  
  * Planejamento?  
     17 - De que maneira é planejado que os alunos utilizem as arenas?  
     18 - Como Edson planeja montar as arenas?  
  * Ação?  
     19 - De que maneira as arenas podem ser alteradas?  
     20 - a?  
  * Evento?  
     21 - Por que Edson planeja realizar aulas mais dinâmicas?  
     22 - a?  
  * Avaliação?  
     23 - Como Edson pode saber que uma arena está bem feita?  
     24 - Como é definido que um robô concluiu uma arena?  
    
* **Persona: Kelly do Nascimento.**
  * Por quê?  
     1 - Por que ela prefere fazer o simulado?  
     2 - Por que a IC dela é melhorar o robô desenvolvido por outro aluno?  
  * Como?  
     3 - Que ferramentas ela está utilizando?  
     4 - Como ela está desenvolvendo atualmente?  
  * O que é?  
     5 - O que exatamente é essa IC?  
     6 - Que melhoria é procurada neste robô?  
  * Pode ser feito da maneira?  
     7 - Quais as opções que ela possui para teste?  
     8 - Os métodos utilizados são os melhores disponíveis?  
  * Faz parte de?  
     9 - Ela faz parte do curso de robótica?  
     10 - O aluno mencionado é do curso de robótica?  
  * Objetivo?  
     11 - Qual a métrica de sucesso na melhoria?  
     12 - Qual o objetivo por trás de utilizar as arenas?  
  * Ambiente?  
     13 - O  acesso na K4-04 é a qualquer hora?  
     14 - Ela possui equipamento para desenvolver o projeto em casa?  
  * Ator(es)?  
     15 - Quem é o outro aluno?  
     16 - Quem é o professor?  
  * Planejamento?  
     17 - A proposta da IC não considerava como seriam feitos os testes?  
     18 - O outro aluno (desenvolvedor do robô) não está envolvido no planejamento?  
  * Ação?  
     19 - Como ela está lidando com essa pressão?  
     20 - Ela já pediu por ajuda?  
  * Evento?  
     21 - Esses problemas já foram discutidos no encontro com o orientador?  
     22 - Quando será a entrega da IC dela?  
  * Avaliação?  
     23 - Ela sabe avaliar o progresso atual da IC?  
     24 - Como está o progresso atual dela?  

# Refinamento do Cenário Análise/Problema
<!--
* **Persona: Robervaldo Arantes.**
  * Por quê?  
     1 - Por que usar a arena?  
     2 - Por que não consegue utilizar a arena?  
  * Como?  
     3 - Como pode se utilizar o modelo da arena?  
     4 - Como pode contornar a falta de autorização?  
  * O que é?  
     5 - O que é a arena da K4-04?  
     6 - O que são os testes realizados?  
  * Pode ser feito da maneira?  
     7 - Como podem ser feitos os testes?  
     8 - Como pode ser utilizada a sala e a arena?  
  * Faz parte de?  
     9 - A quem a arena pertence?  
     10 - Qual o grande foco de alunos que fazem parte do grupo que pode utilizar a sala?  
  * Objetivo?  
     11 - Qual o objetivo do interesse?  
     12 - Qual o objetivo de testar os robôs?  
  * Ambiente?  
     13 - Onde está localizada a arena?  
     14 - Quais alterações podem ser feitas?  
  * Ator(es)?  
     15 - Quem pode permitir o acesso à arena?  
     16 - Quem possui o modelo da arena?  
  * Planejamento?  
     17 - Por que deseja acessar a arena?  
     18 - Como deseja utilizar a arena?  
  * Ação?  
     19 - O que é realizado na arena?  *
     20 - O que o usuário pode realizar com a simulação?  
  * Evento?  
     21 - Quando se pode utilizar a sala?  *
     22 - Quando os alunos podem utilizar a sala sem uma autorização da instituição?  *
  * Avaliação?  
     23 - Como os testes são avaliados?  *
     24 - Como é avaliado quem pode utilizar a sala?  *
     -->
* **Persona: Robervaldo Arantes.**
  * Robervaldo Arantes é um estudante que recém ingressou no curso de engenharia de robôs, na instituição da FEI **[9]**, o mesmo ficou sabendo sobre uma arena onde testes com robôs podem ser realizados **[7]** na sala K4-04 **[13]**, a mesma é uma arena que possui diversos pontos onde paredes podem ser posicionadas **[14]** para formarem diferentes labirintos **[5]**, para assim entender cada vez mais sobre como utilizá-los e estudá-los **[12]** e com esses labirintos, testes de locomoção, desempenho, etc. podem ser realizados **[6]**, o mesmo possui um interesse **[17]** em adiantar o entendimento sobre matérias e conteúdos futuros que envolvam testes realizados com robôs **[1] [11]** para utilizar a sala, é necessária uma autorização da instituição ou do professor que estiver utilizando a sala **[15]**, geralmente que são aulas de engenharia **[10]**, no momento **[8]** as quais limitam muito o acesso de Robervaldo **[2]**. Para tentar contornar isso, Robervaldo conseguiu com um veterano que utiliza a sala **[16]** um modelo simulado da Arena **[4]** que o mesmo recebeu de seu professor **[16]** para utilizar em algum simulador **[3]** e realizar os seus próprios testes **[20]**, mas o mesmo não sabe sobre os obstáculos que podem ser implementados, tornando o uso da mesma, confuso e complicado.
    
<!--
* **Persona: Edson Adalberto.**
  * Por quê?  
     1 - Por que utilizar a sala?  
     2 - Por que utilizar a arena da K4-04?  
  * Como?  
     3 - Como Edson planeja melhorar suas aulas?  
     4 - Como a arena pode ser editada?  
  * O que é?  
     5 - Qual a dificuldade em montar as arenas?  
     6 - ?  
  * Pode ser feito da maneira?  
     7 - Como Edson planeja tornar as aulas mais dinâmicas?  
     8 - Como as arenas são montadas atualmente?  
  * Faz parte de?  
     9 - Por que Edson pode utilizar a sala K4-04 livremente?  
     10 - Qual aula é ministrada por Edson?  
  * Objetivo?  
     11 - Qual o objetivo de Edson em utilizar a sala?  
     12 - ?  
  * Ambiente?  
     13 - Onde os testes serão realizados?  
     14 - Quais obstaculos podem ser utilizados na arena?  
  * Ator(es)?  
     15 - Quais alunos poderão testar os robôs?  
     16 - ?  
  * Planejamento?  
     17 - De que maneira é planejado que os alunos utilizem as arenas?  
     18 - Como Edson planeja montar as arenas?  
  * Ação?  
     19 - De que maneira as arenas podem ser alteradas?  
     20 - a?  
  * Evento?  
     21 - Por que Edson planeja realizar aulas mais dinâmicas?  
     22 - a?  
  * Avaliação?  
     23 - Como Edson pode saber que uma arena está bem feita?  
     24 - Como é definido que um robô concluiu uma arena?  
     -->
* **Persona: Edson Adalberto.**
   * O professor Edson Adalberto é um professor de engenharia de robôs **[9]**, o professor estava pensando em um plano de aulas para a matéria de "Introdução a robótica móvel" **[10]** com exemplos mais práticos **[1]**, onde poderia atrair mais a atenção de seus alunos e permitir que os mesmos tenham uma base mais forte relacionada a prática da robótica quanto antes **[21]** para isso o mesmo decidiu utilizar a sala da K4-04 **[7]** onde existe uma arena que o mesmo pode utilizar **[3]** para ministrar as aulas e também para que seus alunos possam realizar suas tarefas **[17]**, que consistem em verificar o quão rápido um robô sai do ponto de partida e chega ao outro lado da arena **[24]**, esta arena possui uma base pronta, mas pode ser alterada pelo usuário com a adição de placas **[14]** que funcionariam como paredes para dificultar a locomoção de um robô **[4]**, mas o mesmo encontrou um problema que seria relacionado ao desenvolvimento da arena, para desenvolver labirintos para serem utilizados na aula, o mesmo precisa estar no campus montar e desmontar manualmente **[8]** **[19]** a arena diversas vezes até encontrar uma arena que cumpra os requisitos que o mesmo deseja **[5]** que são os de serem labirintos que possuam ao menos três caminhos fechados e no máximo um atalho **[23]**.

<!--
* **Persona: Kelly do Nascimento.**
* Por quê?  
   1 - Por que ela prefere fazer o simulado?  *
   2 - Por que a IC dela é melhorar o robô desenvolvido por outro aluno?  
* Como?  
   3 - Que ferramentas ela está utilizando?  
   4 - Como ela está desenvolvendo atualmente?  
* O que é?  
   5 - O que exatamente é essa IC?  
   6 - Que melhoria é procurada neste robô?  
* Pode ser feito da maneira?  
   7 - Quais as opções que ela possui para teste?  
   8 - Os métodos utilizados são os melhores disponíveis?  *
* Faz parte de?  
   9 - Ela faz parte do curso de robótica?  
   10 - O aluno mencionado é do curso de robótica?  
* Objetivo?  
   11 - Qual a métrica de sucesso na melhoria?  *
   12 - Qual o objetivo por trás de utilizar as arenas?  *
* Ambiente?  
   13 - O  acesso na K4-04 é a qualquer hora?  
   14 - Ela possui equipamento para desenvolver o projeto em casa?  
* Ator(es)?  
   15 - Quem é o outro aluno?  
   16 - Quem é o professor?  
* Planejamento?  
   17 - A proposta da IC não considerava como seriam feitos os testes?  
   18 - O outro aluno (desenvolvedor do robô) não está envolvido no planejamento?  *
* Ação?  
   19 - Como ela está lidando com essa pressão?  
   20 - Ela já pediu por ajuda?  
* Evento?  
   21 - Esses problemas já foram discutidos no encontro com o orientador?  
   22 - Quando será a entrega da IC dela?  
* Avaliação?  
   23 - Ela sabe avaliar o progresso atual da IC?  
   24 - Como está o progresso atual dela? 
  -->  
* **Persona: Kelly do Nascimento.**
   * Kelly do nascimento, aluna no 6⁠º Semestre do curso de engenharia de robôs **[9]**, já está na metade (6 meses) da sua IC **[22]** "Aprimoramento de algoritmo de rotas", que é sobre a melhoria do algoritmo de rotas **[5]** sendo atualmente utilizado no robô de Luciano, aluno no 8⁠º Semestre do curso de engenharia de robôs **[10]** **[15]**, o qual possui sua própria IC "Otimização de visão computacional utilizando IAs generativas", os dois se conhecem e decidiram fazer ICs que se complementam **[2]**. A IC da Kelly tem como meta aprimorar o algoritmo atual de rotas em 10%, ou analisar partes do algoritmo que podem ser otimizados/refatorados para ter melhoria **[6]**. Kelly tem acesso ao robô e à sala K4-04 nas segundas e terças durante os horários onde a sala não tem aula **[13]**. A sala dispõe de uma arena que ela utiliza para os seus testes, ela também conseguiu o modelo do mapa da arena para possivelmente fazer testes simulados **[7]** para complementar os 3 dias que ela não possui acesso ao robô ou à sala **[14]**. Mas Kelly está preocupada: Ela conseguiu um estágio recentemente, a fazendo ter pouco tempo para dedicar à IC, e está com medo de não conseguir terminar a tempo! Kelly discutiu com seu Orientador, Pedro **[16]** **[20]** **[21]**, sobre o que ela conseguiria fazer sobre isso. Ela estava um pouco adiantada quanto ao cronograma  **[23]** **[24]**, mas o ritmo dela havia caído dramaticamente desde o começo de seu estágio. O orientador mencionou que na IC estavam descritas as melhores formas de fazer testes simulados utilizando Gazebo Classic **[3]** para adiantar o máximo possível em casa, via testes simulados, ao invés de testes na sala K4-04 em caso da sala ficar indisponível por bastante tempo  **[17]** **[19]**. Ela conseguiu instalar as ferramentas e rodar o mapa simulado na sua máquina em casa **[4]**, e conseguiu ir adiantando sua IC de forma simulada, acumulando arenas e hipóteses para confirmar no físico de uma vez, ajudando-a a usar seu tempo de forma efetiva. Mas quando foi para testar as suas arenas simuladas no físico, ela percebeu que as arenas que ela criou no simulado eram impossíveis de replicar fielmente no real! As posições das paredes na arena real são padronizadas, algo que ela não levou em conta quando montou suas arenas simuladas, então agora irá ter que refazer não só as arenas, mas também os testes.     
