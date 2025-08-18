# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Identificação de diferenças de desempenho entre robôs reais, conteinerizados e simulados, utilizando simulador Gazebo, ROS 2 e Docker** sob orientação do Professor **Leonardo Anjoletto Ferreira** e desenvolvido pelos seguintes alunos:

- Murilo Darce Borges Silva
- Rodrigo Simões Ruy

## Resumo
Conteinerização é uma ferramenta muito útil quando se lida com projetos que precisam de diferentes dependências ou programas que podem ter conflitos entre si, que precisam de uma grande quantidade de configuração inicial, ou que precisam de portabilidade. Isso a torna perfeita para projetos de robótica, mas os impactos do seu uso e suas peculiaridades em situações reais ainda não estão documentadas, o que é justamente oque este projeto propõe fazer. Haverão 2 partes para este projeto, a primeira parte será uma avaliação do desempenho em uma simulação utilizando Gazebo, e a segunda parte será a avaliação do desempenho de um turtlebot real.  

## Introdução
<!--Introdução: falta funcionalidades, tecnologias, contexto de uso-->
A conteinerização é uma ferramenta poderosa no campo de desenvolvimento e implementação, disponibilizando certa camada de isolamento entre componentes de um projeto, assegurando que estes não irão conflitar, seja por funções internas ou dependências de versões diferentes sendo utilizadas. No campo da robótica, conteinerização é vista como uma técnica para facilitar o desenvolvimento, portabilidade e consistência em projetos de robótica, mas não foram feitas pesquisas detalhando a integração destes projetos com Docker e seus efeitos no desempenho de um robô físico. A proposta do projeto é justamente esta: integrar ROS 2 e Docker, explicando os passos utilizados e comparando o desempenho com e sem conteinerização, sendo dividido em 2 partes: em um simulador Gazebo, e em um robô Turtlebot real. Será desenvolvida também uma interface, utilizando a biblioteca pygames do python, que permite ao usuário posicionar obstáculos em uma arena baseada na arena da k404 que está presente no campus da FEI. 

## Publico Alvo
<!--Publico-alvo: falta suas caracteristicas-->
Pessoas que trabalham com robôs e pessoas que desejam desenvolver arenas simuladas/reais de uma maneira mais rápida e simples. Este público alvo deseja realizar testes de maneira rápida e quanto mais rápido, mais eles aproveitam. Facilitar o processo de desenvolver os mapas, mais rápido os mesmos poderão testar os robôs.

## Análise de concorrência

<!-- 1. Identifique os principais concorrentes ou softwares mais utilizados pelo seu público-alvo. X
2. Colete informações sobre os concorrentes selecionados. X
3. Analise as características e funcionalidades dos concorrentes. X
4. Avalie a experiência do usuário (UX). REVISAR
5. Examine os preços e modelos de negócio. FALTA O DO GAZEBO
6. Pesquisa de satisfação do cliente e opiniões. X
7. Identifique padrões e tendências no mercado. X
8. Elabore relatórios e sumarize os resultados. X
9. Extraia pontos positivos e faça recomendações. X 

Analise de concorrência: falta experiencia de utilização da ferramenta ou serviço, preços, feedbacks dos usuários, tendencias do mercado, pontos positivos e negativos
-->

Alguns concorrentes que encontramos foram o Gazebo Simulator e o Blender, ambos são utilizados para se desenvolver mapas/Arenas para robôs. O Simulador Gazebo, que também utilizaremos, pode ser usado para se desenvolver arenas, mas como não é o foco do software o desenvolvimento, o mesmo é muito limitado em diversos aspectos da criação, então é mais utilizado para simular algo já criado. O Blender é um software voltado para a criação de modelos 3d, às vezes utilizado para a criação de arenas mais complexas, mas o mesmo é voltado para a criação e não simulação, então os usuários exportam os modelos para utilizar em um simulador. Ambos os softwares possuem apreciação pelo público-alvo, mas por serem dois softwares separados acaba ocorrendo o problema da exportação de arquivos e conversão para utilizar no outro software. Ambos os softwares são gratuitos, com amplas comunidades e diversas versões que podem ser utilizadas pelos usuários. O modelo de negócio do Blender ocorre a partir de anúncios, merchandise, eventos, inscrições e doações, enquanto o do Simulador Gazebo ... . Observando estas duas concorrências, podemos observar que são bastante apreciadas por serem gratuitas, possuírem comunidades ativas, suporte para mais de uma plataforma e entre outros. Ambos os softwares são bons para o que cumprem, mas o gazebo poderia ter alguma forma de desenvolvimento que pudesse ser mais sofisticada para o desenvolvimento de arenas mais complexas com mais facilidade.
      
### Personas

- Descreva as personas que irão interagir com a aplicação ou produto. Deixe claro suas principais caracteristicas e contextos sociais, econômicos e culturais.
- Quais informações sobre o usuário o serviço ou poduto deve guardar?

  - Persona primaira ...
  - Persona secundária ...
  - Outras personas ...

### Mapa de empatia

![Mapa de empatia](empatia.png)

- Determine o mapa de empatia[^1] de pelo menos uma persona primária e uma sercundária.
  - O que o usuário vê: aqui estamos falando do ambiente visual em que o usuário se encontra. Ou seja, o que ele efetivamente enxerga, as pessoas e objetos que estão ao seu redor. Isso ajuda a entender o contexto em que o usuário está inserido e as influências visuais que está recebendo.
  - O que o usuário ouve: neste quadrante, buscamos entender o que o usuário está ouvindo, os sons que o cercam e como eles influenciam suas ações.
  - O que o usuário diz e faz: aqui consideramos ações e comportamentos que o usuário apresenta durante sua interação com serviço ou poduto.
  - O que o usuário pensa e sente: neste quadrante, buscamos entender os pensamentos, sentimentos, emoções e percepções que o usuário tem em relação ao serviço ou poduto. Quais expectativas o usuário cria sobre o serviço ou poduto?
  Que tipo de serviço ou poduto mais agrada essa persona?
  - Dores: quando falamos sobre dores do usuário, estamos fazendo referência a quaisquer obstáculos, necessidades ou frustrações que o usuário possa experimentar ao tentar realizar uma tarefa ou alcançar um objetivo. Isso inclui, por exemplo, problemas de usabilidade, dificuldades de acesso ou outros desafios que podem afetar a experiência do usuário.
  - Ganhos: nesse caso estamos falando de quaisquer benefícios ou recompensas que o usuário possa experimentar ao utilizar o serviço ou poduto. Isso pode incluir economia de tempo ou facilidade de uso, por exemplo. Que desejos do usuário o serviço ou poduto satisfaz?

## Contexto de uso

- Descreva o ambiente em que o serviço ou poduto deve ser utilizado.
- Qual/quais o(s) contexto(s) sociais, econômicos e culturais existentes neste ambiente?
- Quais informações sobre o ambiente, o serviço ou poduto deve guardar antes de iniciar a interação?
- O que normalmente deve estar acontecendo com o ambiente quando o usuário interagir com o serviço ou poduto?

## Jornada do usuário

- Criar uma narrativa para o o seu serviço ou poduto com o usuário.
- Determine o que o usuário realiza desde a primeira até o última interação com o serviço ou poduto.
  - Descreva o que acontece ou pode acontecer passo a passo
  - Como a tarefa começa? Como a tarefa se desenvolve? Como a tarefa termina?


<!--
## Análise de concorrência

- Pesquise serviços ou podutos existentes atualmente que possam realizar o objetivo deste projeto.
- Selecione pelo menos 3 serviços ou podutos diferentes.
- Em relação aos concorrentes, respondam as seguintes perguntas?
  - Existe plataforma similar que atende o mesmo mercado e funcionalidades? Se sim: Quais os pontos positivos? Quais os pontos negativos?
  - Existe plataforma diferente quanto ao serviço, mas que atenda esse mercado? Se sim: Quais os pontos positivos? Quais os pontos negativos?
 -->
 
## Coleta de dados

## Modelo de tarefas

## Design

- Pense nas características de Affordances do seu serviço ou poduto. 
    - Que tipo de acessibilidades devem ser consideradas dentro do seu projeto?
- Discuta o papel das expectativas do usuário no projeto deste serviço ou poduto. Qual a importância e pontos a serem considerados se você quiser vender esse serviço ou poduto?

### Prototipação em baixo nível (papel)
#### Avaliação heurística

### Prtotipação em médio nível (Figma)
#### Avaliação heurística

### Prtotipação em alto nível (React)
#### Avaliação heurística

[^1]: Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>

<!-- TODOs:
- Add exemplos
 -->
