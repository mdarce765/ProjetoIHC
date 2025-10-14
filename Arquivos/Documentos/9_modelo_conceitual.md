
1) **Cenários de Interação (Fazer para os 3?)**
> **_NOTE:_**: destacar em negrito o texto alterado entre Cenário Problema e Cenário de Interação
É para então falar como eles lidariam caso tivesse NOSSO projeto? (com detalhes de interação, claro)
- Kelly Do Nascimento, aluna no 6⁠º Semestre do curso de engenharia de robôs [9], já está na metade (6 meses) da sua IC [22] "Aprimoramento de algoritmo de rotas", que é sobre a melhoria do algoritmo de rotas [5] sendo atualmente utilizado no robô de Luciano, aluno no 8⁠º Semestre do curso de engenharia de robôs [10] [15], o qual possui sua própria IC "Otimização de visão computacional utilizando IAs generativas", os dois se conhecem e decidiram fazer ICs que se complementam [2]. A IC da Kelly tem como meta aprimorar o algoritmo atual de rotas em 10%, ou analisar partes do algoritmo que podem ser otimizados/refatorados para ter melhoria [6].

  Kelly tem acesso ao robô e à sala K4-04 nas segundas e terças durante os horários onde a sala não tem aula [13]. A sala dispõe de uma arena que ela utiliza para os seus testes, ela também conseguiu o modelo do mapa da arena para possivelmente fazer testes simulados [7] para complementar os 3 dias que ela não possui acesso ao robô ou à sala [14]. Mas Kelly está preocupada: Ela conseguiu um estágio recentemente, a fazendo ter pouco tempo para dedicar à IC, e está com medo de não conseguir terminar a tempo!

  Kelly discutiu com seu Orientador, Pedro [16] [20] [21], sobre o que ela conseguiria fazer sobre isso. Ela estava um pouco adiantada quanto ao cronograma [23] [24], mas o ritmo dela havia caído dramaticamente desde o começo de seu estágio. O orientador mencionou que na IC estavam descritas as melhores formas de fazer testes simulados utilizando Gazebo Classic [3] para adiantar o máximo possível em casa, via testes simulados, ao invés de testes na sala K4-04 em caso da sala ficar indisponível por bastante tempo [17] [19]. Ela usa nosso projeto, __clicando__ nas paredes que deseja adicionar ao mapa, sabendo que elas estão indo para os lugares devidos na arena real, __usa a rodinha do mouse para dar zoom__, a auxiliando a ver as modificações/estado atual do mapa. Quando satisfeita, ela __clica__ em salvar, e logo após __clica__ em exportar, criando o mapa com as paredes selecionadas.

2) **Design Centrado na Comunicação**

**Nome do Cenário: Criar mapa**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Selecionar paredes | U: Preciso selecionar as paredes que eu preciso na arena<br>D: Quais? |
| > remover parede | U:Errei! Não quero aquela parede não!<br>D: Certo, qual parede quer remover? |
|  Salvar arena | U: Acho que esta bom agora |
| Criar mapa | U: Consegue montar uma arena com essas paredes selecionadas?<br>D:Claro, aqui está |

3) **Mapa de Objetivos**
> **_NOTE:_**: cada um coloca seu mapa de objetivos e deverá ter um diagrama de consolidação

| tipo de objetivo | você |
|---|---|
| final| quer criar um mapa de forma fácil e rápida|
| instrumental | quer utilizar uma ferramenta leve para criar um mapa de forma fácil e rápida |
| instrumental direto | quer utilizar uma ferramenta leve, capaz de facilmente iterar modificações em mapas, para ter seu desenvolvimento mais fácil e rápido |
| instrumental indireto | quer utilizar uma ferramenta leve, capaz de utilizar outros mapas já modificados disponibilizados por outros usuários, para ter seu desenvolvimento mais fácil e rápido |

| tipo de objetivo | você quer criar um mapa de forma rápida e fácil |
|---|---|
| final| |
| instrumental | |
| instrumental direto | |
| instrumental indireto | |



4) **Esquema Conceitual de Signos**

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
| Paredes | PA: só se pode colocar paredes aonde se foi demarcado | - |










