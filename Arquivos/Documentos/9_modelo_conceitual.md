
# **Cenários de Interação**

## Edson Adalberto
- O professor Edson Adalberto é um professor de engenharia de robôs [9], o professor estava pensando em um plano de aulas para a matéria de "Introdução a robótica móvel" [10] com exemplos mais práticos [1], onde poderia atrair mais a atenção de seus alunos e permitir que os mesmos tenham uma base mais forte relacionada a prática da robótica quanto antes [21] para isso o mesmo decidiu utilizar a sala da K4-04 [7] onde existe uma arena que o mesmo pode utilizar [3] para ministrar as aulas e também para que seus alunos possam realizar suas tarefas [17], que consistem em verificar o quão rápido um robô sai do ponto de partida e chega ao outro lado da arena [24], esta arena possui uma base pronta, mas pode ser alterada pelo usuário com a adição de placas [14] que funcionariam como paredes para dificultar a locomoção de um robô [4], mas o mesmo encontrou um problema que seria relacionado ao desenvolvimento da arena, para desenvolver labirintos para serem utilizados na aula, o mesmo precisa estar no campus montar e desmontar manualmente [8] [19] a arena diversas vezes até encontrar uma arena que cumpra os requisitos que o mesmo deseja [5] que são os de serem labirintos que possuam ao menos três caminhos fechados e no máximo um atalho [23] **e como solução utilizaria a interface, onde o mesmo consegue criar as arenas baseadas na da sala de aula e mostrar para os seus alunos**.

## Robervaldo Arantes
- Robervaldo Arantes é um estudante que recém ingressou no curso de engenharia de robôs, na instituição da FEI [9], o mesmo ficou sabendo sobre uma arena onde testes com robôs podem ser realizados [7] na sala K4-04 [13], a mesma é uma arena que possui diversos pontos onde paredes podem ser posicionadas [14] para formarem diferentes labirintos [5], para assim entender cada vez mais sobre como utilizá-los e estudá-los [12] e com esses labirintos, testes de locomoção, desempenho, etc. podem ser realizados [6], o mesmo possui um interesse [17] em adiantar o entendimento sobre matérias e conteúdos futuros que envolvam testes realizados com robôs [1] [11] para utilizar a sala, é necessária uma autorização da instituição ou do professor que estiver utilizando a sala [15], geralmente que são aulas de engenharia [10], no momento [8] as quais limitam muito o acesso de Robervaldo [2]. Para tentar contornar isso, Robervaldo conseguiu com um veterano que utiliza a sala [16] um modelo simulado da Arena [4] que o mesmo recebeu de seu professor [16] para utilizar em algum simulador [3] e realizar os seus próprios testes [20], **utilizando a interface o mesmo pode pegar alguns modelos feitos por outros alunos e professores e assim realizar alguns testes e entender as regras da arena**.

## Kelly do Nascimento
- Kelly do Nascimento, aluna no 6⁠º Semestre do curso de engenharia de robôs [9], já está na metade (6 meses) da sua IC [22] "Aprimoramento de algoritmo de rotas", que é sobre a melhoria do algoritmo de rotas [5] sendo atualmente utilizado no robô de Luciano, aluno no 8⁠º Semestre do curso de engenharia de robôs [10] [15], o qual possui sua própria IC "Otimização de visão computacional utilizando IAs generativas", os dois se conhecem e decidiram fazer ICs que se complementam [2]. A IC da Kelly tem como meta aprimorar o algoritmo atual de rotas em 10%, ou analisar partes do algoritmo que podem ser otimizados/refatorados para ter melhoria [6].

  Kelly tem acesso ao robô e à sala K4-04 nas segundas e terças durante os horários onde a sala não tem aula [13]. A sala dispõe de uma arena que ela utiliza para os seus testes, ela também conseguiu o modelo do mapa da arena para possivelmente fazer testes simulados [7] para complementar os 3 dias que ela não possui acesso ao robô ou à sala [14]. Mas Kelly está preocupada: Ela conseguiu um estágio recentemente, a fazendo ter pouco tempo para dedicar à IC, e está com medo de não conseguir terminar a tempo!

  Kelly discutiu com seu Orientador, Pedro [16] [20] [21], sobre o que ela conseguiria fazer sobre isso. Ela estava um pouco adiantada quanto ao cronograma [23] [24], mas o ritmo dela havia caído dramaticamente desde o começo de seu estágio. O orientador mencionou que na IC estavam descritas as melhores formas de fazer testes simulados utilizando Gazebo Classic [3] para adiantar o máximo possível em casa, via testes simulados, ao invés de testes na sala K4-04 em caso da sala ficar indisponível por bastante tempo [17] [19]. Ela usa nosso projeto, __clicando__ nas paredes que deseja adicionar ao mapa, sabendo que elas estão indo para os lugares devidos na arena real, __usa a rodinha do mouse para dar zoom__, a auxiliando a ver as modificações/estado atual do mapa. Quando satisfeita, ela __clica__ em salvar, e logo após __clica__ em exportar, criando o mapa com as paredes selecionadas.

# **Design Centrado na Comunicação**

**Nome do Cenário: Criar mapa**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Selecionar paredes | U: Preciso selecionar as paredes que eu preciso na arena<br>D: Quais? |
| > remover parede | U:Errei! Não quero aquela parede não!<br>D: Certo, qual parede quer remover? |
|  Salvar arena | U: Acho que esta bom agora |
| Criar mapa | U: Consegue montar uma arena com essas paredes selecionadas?<br>D:Claro, aqui está |

**Nome do Cenário: Importar mapa**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Importar a arena | U: Quero importar uma arena para a interface<br> D: Como você deseja importar a arena? Botão da aplicação, Comando de teclado ou pelo terminal?|
| Selecionar o arquivo | U: Quero escolher o arquivo para importar?<br> D: Como você quer procurar? Digitando o nome ou selecionando com o mouse? |

**Nome do Cenário: Aplicar zoom**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Escolher como aplicar | U: Eu não estou enxergando bem, eu quero aproximar mais a tela.<br> D: Como você quer aplicar o zoom? Pop-up da interface ou usando o mouse? |
| Aplicar com o pop-up | U: Eu quero usar o pop-up.<br> D: Certo, Aperte o botão "+" para ampliar e "-" para tirar o zoom. 
| Aplican com o mouse | U: Eu quero usar o mouse.<br> D: Certo, posicione o mouse onde deseja e use a roda do mouse para aplicar ou retirar. |

# **Mapa de Objetivos**
> **_NOTE:_**: cada um coloca seu mapa de objetivos e deverá ter um diagrama de consolidação

| tipo de objetivo | você |
|---|---|
| final| quer criar um mapa de forma fácil e rápida|
| instrumental | quer utilizar uma ferramenta leve para criar um mapa de forma fácil e rápida |
| instrumental direto | quer utilizar uma ferramenta leve, capaz de facilmente iterar modificações em mapas, para ter seu desenvolvimento mais fácil e rápido |
| instrumental indireto | quer utilizar uma ferramenta leve, que força o usuário a colocar as paredes nas posições corretas, para que outros consigam iterar em seus mapas de forma corrta |

| tipo de objetivo | você quer criar um mapa de forma rápida e fácil |
|---|---|
| final| |
| instrumental | |
| instrumental direto | |
| instrumental indireto | |

# **Esquema Conceitual de Signos**

> **_NOTE:_**: fazer a junção das 3 tabelas abaixo em uma única

| Mapa (M) \- Mapa a ser modificado |  |  |
| :---- | :---- | :---- |
| **signo** | **origem** | **observações** |
| Paredes | Domínio | Botões nos lugares onde podem ser colocadas paredes no mapa |
| Barra De Zoom | Aplicação | Barra que define/representa o valor de zoom |
| Salvar | Domínio | Botão que salva as paredes selecionadas até agora |
| Exportar | Domínio | Botão que transforma as paredes selecionadas em paredes no mapa simulado, as exportando para um arquivo de arena |

| Mapa (M) \- Mapa a ser modificado |  |  |  |
| :---- | :---- | :---- | :---- |
| **signo** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** |
| Paredes | Seleção Simples | Se pode apenas colocar paredes aonde se possui botões | Nenhuma selecionada |
| Barra de zoom | Barra selecionável(?) | 20%-200% Zoom | 100% Zoom |

| Mapa (M) \- Mapa a ser modificado |  |  |
| :---- | :---- | :---- |
| **signo** | **prevenção** | **recuperação** |
| Paredes | PP: só se pode colocar paredes aonde se foi demarcado | - |
| X | PA: Aparece um aviso caso não tenha salvo o arquivo antes de tentar fechar | RA: Pede confirmação se realmente não quer salvar as mudanças|
