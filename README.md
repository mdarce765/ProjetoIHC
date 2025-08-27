# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Identificação de diferenças de desempenho entre sistemas robóticos reais, simulados e com software conteinerizado, utilizando Simulador Gazebo, ROS 2 e Docker** sob orientação do Professor **Leonardo Anjoletto Ferreira** e desenvolvido pelos seguintes alunos:

- Murilo Darce Borges Silva
- Rodrigo Simões Ruy

## Resumo
Conteinerização é uma ferramenta muito útil quando se lida com projetos que precisam de diferentes dependências ou programas que podem ter conflitos entre sí, que precisam de uma grande quantidade de configuração inicial, ou que precisam de portabilidade. Isso a torna perfeita para projetos de robótica, mas os impactos do seu uso e suas peculiaridades em situações reais ainda não estão documentadas, o que é justamente oque este projeto propõe fazer. Haverão 2 partes para este projeto, a primeira parte será uma avaliação do desempenho em uma simulação utilizando Gazebo, e a segunda parte será a avaliação do desempenho de um turtlebot real.  

## Introdução
<!--Introdução: falta funcionalidades, tecnologias, contexto de uso-->
A conteinerização é uma ferramenta poderosa no campo de desenvolvimento e implementação, disponibilizando certa camada de isolamento entre componentes de um projeto, assegurando que estes não irão conflitar, seja por funções internas ou dependências de versões diferentes sendo utilizadas. No campo da robótica, conteinerização é vista como uma técnica para facilitar o desenvolvimento, portabilidade e consistência em projetos de robótica, mas não foram feitas pesquisas detalhando a integração destes projetos com Docker e seus efeitos no desempenho de um robô físico. A proposta do projeto é justamente esta: integrar ROS 2 e Docker, explicando os passos utilizados e comparando o desempenho com e sem conteinerização, sendo dividido em 2 partes: em um simulador Gazebo, e em um robô Turtlebot real. Será desenvolvida também uma interface gráfica interativa, utilizando a biblioteca pygames do python, que permite ao usuário posicionar obstáculos em uma arena simulada baseada na arena da k4-04 que está presente no campus da FEI. 

### Tecnologias
- Simulador Gazebo Classic: Software de simulação de físicas. Será utilizado para realizar os testes com o robô simulado.  
- ROS2 Humble: Software e plataforma para desenvolver aplicações para robôs. Será utilizado no turtlebot3 burger para realizar os testes.  
- Docker: Ferramenta utilizada para conteinerizar aplicações, as isolando de possíveis intereferências de outras aplicações. Será utilizada nos testes para o robô real/simulado com docker.  
- Pygames: Biblioteca em python para desenvolvimento de jogos. Será utilizada para desenvolver a interface gráfica interativa para o usuário.  

## Publico Alvo
<!--Publico-alvo: falta suas caracteristicas-->
Pessoas que trabalham com robôs e pessoas que desejam desenvolver arenas simuladas/reais de uma maneira mais rápida e simples.   
Este público alvo deseja realizar testes de maneira rápida e fácil, quanto menos configurações ou instalações manuais forem necessárias, o melhor. Facilitar o processo de desenvolver os mapas, mais rápido os mesmos poderão testar os robôs. Este público deseja velocidade, simplicidade, bom desempenho, possibilidades de serem criativos e etc.

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

Alguns concorrentes que encontramos foram o Autodestk Fusion, Blender e o Gazebo Simulator. Estes softwares podem ser utilizados para se desenvolver mapas/Arenas para robôs.  
Autodesk Fusion é um software com grande foco na área de simulação de tensões de materiais e modelagem 3D, CAD, CAM, CAE e PCB, sendo utilizado em testes de novos materiais para hardware com simulações mecânicas e de movimento.  
Blender é um software completamente voltado para a criação de modelos 3d, sendo utilizado para a criação de arenas mais complexas com maior facilidade que outras ferramentas.  
O Simulador Gazebo, que será utilizado no projeto, pode ser usado para se desenvolver arenas, mas seu uso principal é para a simulação de sensores e algoritmos em um ambiente físico completamente simulado.
Estes softwares possuem apreciação pelo público-alvo, mas por serem softwares separados acaba ocorrendo o problema da exportação de arquivos e conversão para utilizar em outro software (Autodesk Fusion/Blender → Gazebo), já que alguns formatos de arquivos (como sdf) podem ter problemas ao serem convertidos para versões anteriores.  
Os softwares são gratuitos, com exceção do Autodesk Fusion que possui uma versão gratuita e versões pagas, com amplas comunidades e diversas versões que podem ser utilizadas pelos usuários. 
O modelo de negócio do Autodesk Fusion é baseado nos diversos tipos de softwares distribuídos pela Autodesk. Mesmo possuindo avaliações gratuitas e até versões gratuitas para uso pessoal, as outras versões dos softwares são pagas por meio de assinaturas mensais ou anuais.    
O modelo de negócio do Blender ocorre a partir de anúncios, merchandise, eventos, inscrições e doações, amplamente adotado pela comunidade de modeladores e até animadores 3D.  
O Gazebo Simulator é um software gratuito e de código aberto, amplamente adotado pela comunidade de robótica.    
Observando estas concorrências, podemos observar que são bastante apreciadas por possuírem comunidades ativas, suporte para mais de uma plataforma, liberdade criativa para desenvolvimento, entre outros.  
Estes softwares são ótimos para o que são utilizados, mas a modelagem no Gazebo é algo que continua difícil. Se o Gazebo tivesse alguma forma de modelar que pudesse ser mais fácil de utilizar, teríamos o melhor dos dois mundos: Um ótimo simulador de sensores e algoritmos de robôs, e uma ótima ferramenta para modelagem de mapas para utilizar dentro do simulador. Já que o Blender não é um simulador e o autodesk fusion é melhor para importação de CADs prontos e simulação de materiais.   

      
### Personas
<!--
- Descreva as personas que irão interagir com a aplicação ou produto. Deixe claro suas principais caracteristicas e contextos sociais, econômicos e culturais.
- Quais informações sobre o usuário o serviço ou poduto deve guardar?
-->
  #### Personas primárias
  * Edson Adalberto, 35 anos, professor de "Introdução à robótica móvel" - "Quanto mais prático, melhor"
    * Edson Adalberto é um dos professores de "Introdução à robótica móvel" há 5 anos. Edson realiza testes com robôs para entender mais sobre a disciplina que aplica e os limites dos robôs e, para isso, o mesmo utiliza ferramentas como Simulador Gazebo, pois assim ele consegue aulas mais dinâmicas para os seus alunos.
  * Robervaldo Arantes, 18 anos, aluno de "Engenharia de robôs" - "A robótica é o futuro da humanidade"
    * Robervaldo Arantes é um calouro na instituição da FEI, após observar a grade curricular, o mesmo ouviu de outro aluno que o mesmo já poderia utilizar um simulador gratuito para testar os robôs da maneira que desejasse, podendo assim se aprofundar no curso e se preparar para aulas futuras.
  * Kelly do Nascimento, 25 anos, aluna realizando uma Iniciação Científica sobre simulações - "Uma simulação torna um resultado mais próximo da realidade"
    * Kelly do Nascimento é uma aluna de engenharia mecânica, mas acabou por se interessar pelas simulações. Por conta disso, a mesma decidiu realizar uma Iniciação Científica com esta temática, a mesma está estudando diversos simuladores para poder avançar com o seu projeto.
  
  #### Persona secundária
  * Ayrton Fernandes, 22 anos, aluno desenvolvendo seu Trabalho de Conclusão de Curso.  
    * Ayrton Fernandes, é um aluno que está no último semestre e está desenvolvendo o seu TCC, o seu TCC consiste em desenvolver um robô funcional que consegue subir e descer escadas sem arriscar cair, para testar este feito, o mesmo resolveu testar o robô com simuladores para poder ver se o que ele desenvolveu esta no caminho certo.

### Mapa de empatia

![Mapa de empatia](empatia.png)

<!-- - Determine o mapa de empatia[^1] de pelo menos uma persona primária e uma sercundária.
  - O que o usuário vê: aqui estamos falando do ambiente visual em que o usuário se encontra. Ou seja, o que ele efetivamente enxerga, as pessoas e objetos que estão ao seu redor. Isso ajuda a entender o contexto em que o usuário está inserido e as influências visuais que está recebendo.
  - O que o usuário ouve: neste quadrante, buscamos entender o que o usuário está ouvindo, os sons que o cercam e como eles influenciam suas ações.
  - O que o usuário diz e faz: aqui consideramos ações e comportamentos que o usuário apresenta durante sua interação com serviço ou poduto.
  - O que o usuário pensa e sente: neste quadrante, buscamos entender os pensamentos, sentimentos, emoções e percepções que o usuário tem em relação ao serviço ou poduto. Quais expectativas o usuário cria sobre o serviço ou poduto?
  Que tipo de serviço ou poduto mais agrada essa persona?
  - Dores: quando falamos sobre dores do usuário, estamos fazendo referência a quaisquer obstáculos, necessidades ou frustrações que o usuário possa experimentar ao tentar realizar uma tarefa ou alcançar um objetivo. Isso inclui, por exemplo, problemas de usabilidade, dificuldades de acesso ou outros desafios que podem afetar a experiência do usuário.
  - Ganhos: nesse caso estamos falando de quaisquer benefícios ou recompensas que o usuário possa experimentar ao utilizar o serviço ou poduto. Isso pode incluir economia de tempo ou facilidade de uso, por exemplo. Que desejos do usuário o serviço ou poduto satisfaz?
-->
### Persona primária
<!-- * Kelly do Nascimento, 25 anos, aluna realizando uma Iniciação Científica sobre simulações - "Uma simulação torna um resultado mais próximo da realidade"
    * Kelly do Nascimento é uma aluna de engenharia mecânica, mas acabou por se interessar pelas simulações. Por conta disso, a mesma decidiu realizar uma Iniciação Científica com esta temática, a mesma está estudando diversos simuladores para poder avançar com o seu projeto. -->
* Kelly do Nascimento, 25 anos.
  - O que o usuário vê: Alunos. Partes Mecânicas. Softwares de simulações.  
  - O que o usuário ouve: Assiste a vídeos relacionados a análise de carros. Muito interessada em acompanhar a equipe Baja FEI no Instagram. Precisa se esforçar para entregar os laboratórios.  
  - O que o usuário diz e faz: Utiliza roupas relacionadas ao curso de mecânica. Gosta de mexer na parte física das máquinas. 
  - O que o usuário pensa e sente: Quanto mais se analisa um assunto, mais fácil de se trabalhar no mesmo. A mecânica é uma área tão abrangente que pode se espalhar para outras áreas.
  - Dores: Trabalhar e estudar é cansativo e exaustivo. É cansativo analisar tantos assuntos para se acompanhar a própria área.
  - Ganhos: Acompanhar tantos assuntos é cansativo, mas recompensador pelo entendimento. Criar um carro 100% nacional é um de seus maiores objetivos. MUDAR(Relacionar com o projeto)
    
### Persona Secundária
<!-- 
  * Ayrton Fernandes, 22 anos, Aluno desenvolvendo seu Trabalho de conclusão de curso  
    * Ayrton Fernandes, é um aluno que está no ultimo semestre e está desenvolvendo o seu TCC, o seu TCC consiste de desenvolver um robô funcional que consegue subir e descer escadas sem correr o risco de cair, para testar este feito, o mesmo resolveu testar o robô com simuladores para poder ver se o que ele desenvolveu esta no caminho certo. 
    -->
* Ayrton Fernandes, 22 anos.
  - O que o usuário vê: Artigos científicos. Orientador. Testes de software.
  - O que o usuário ouve: Assiste vídeos sobre testes em robôs. Palestras sobre avanços tecnológicos.
  - O que o usuário diz e faz: Entende e busca melhorar cada vez mais o projeto. Atualiza seu robô com base na anatomia humana.
  - O que o usuário pensa e sente: Um robô que consegue subir e descer escadas sem cair será um avanço tecnológico. O avanço tecnológico pode tanto auxiliar quanto prejudicar.
  - Dores: Este projeto é muito exigente e conciliar com seus outros projetos é extramente difícil.
  - Ganhos: Este projeto será inovador e de suma importância, podendo ajudar a muitos.MUDAR(relacionar com o projeto)
    
## Contexto de uso

<!-- - Descreva o ambiente em que o serviço ou poduto deve ser utilizado.
- Qual/quais o(s) contexto(s) sociais, econômicos e culturais existentes neste ambiente?
- Quais informações sobre o ambiente, o serviço ou poduto deve guardar antes de iniciar a interação?
- O que normalmente deve estar acontecendo com o ambiente quando o usuário interagir com o serviço ou poduto? -->

  O produto possui o foco de ser utilizado por pessoas envolvidas com a instituição FEI de São Bernardo do Campo, pois a arena em que o produto foi baseada é a da sala k4-04, qualquer interessado pode utilizar o produto, mas para acessar a arena da k4-04 é necessária uma permissão da instituição para utilizar a mesma.
  O produto deve guardar as informações relacionadas à arena e as alterações realizadas pelo usuário, como posições, ajustes, etc, para então o mesmo testar em um simulador próprio.
  O ambiente deve estar sempre pronto para alterações do usuário, tanto quanto criar, posicionar ou deletar as paredes que funcionarão como obstáculos na simulação.
  COMPLEMENTAR(falar sobre a sala k404, relacionar, falar como o usuário vai executar o projeto)

## Jornada do usuário
<!--
- Criar uma narrativa para o o seu serviço ou poduto com o usuário.
- Determine o que o usuário realiza desde a primeira até o última interação com o serviço ou poduto.
  - Descreva o que acontece ou pode acontecer passo a passo
  - Como a tarefa começa? Como a tarefa se desenvolve? Como a tarefa termina? -->

  1. Usuário acessa o executável da interface.
  2. Executável inicia a interface.
  3. Usuário seleciona a opção de adicionar obstáculos a uma arena vazia (Apenas o modelo da arena, sem nenhum obstáculo).
  4. Interface mostra um mapa com botões interativos. Estes botões interativos representam os "furos" em que podem se inserir os apoios dos obstáculos da arena física.
  5. Usuário seleciona um botão.
  6. Botão muda de cor.
  7. O usuário seleciona outro botão próximo ao botão selecionado.
  8. Interface conecta ambos os botões.
  9. Programa escreve no arquivo a posição em que uma parede será posicionada.
  10. Usuário seleciona finalizar.
  11. Interface gera um arquivo ".sdf" com o mapa finalizado e um mapa para ser utilizado pelo robô. (falar a extensão do arquivo do mapa)
  12. Usuário encerra a interface.
  13. Interface é finalizada.


<!--
## Análise de concorrência

- Pesquise serviços ou podutos existentes atualmente que possam realizar o objetivo deste projeto.
- Selecione pelo menos 3 serviços ou podutos diferentes.
- Em relação aos concorrentes, respondam as seguintes perguntas?
  - Existe plataforma similar que atende o mesmo mercado e funcionalidades? Se sim: Quais os pontos positivos? Quais os pontos negativos?
  - Existe plataforma diferente quanto ao serviço, mas que atenda esse mercado? Se sim: Quais os pontos positivos? Quais os pontos negativos?
 -->
## Qualidade de uso
- Usabilidade:
  - Sua importância é muito necessária, o intuito do projeto é o de facilitar o desenvolvimento de arenas relacionadas a arena da sala k4-04, para isso foi pensado um sistema de botões que representam as posições em que os obstáculos possam ser posicionados na arena real, pois é visado a fidelidade da arena e suas possíveis formações.
- Experiência de usuário:
  - É esperado que o usuário se sinta satisfeito ao utilizar o produto, por conta de ter um processo facilitado com relação ao desenvolvimento de arenas. 
- Acessibilidade: 
- Comunicabilidade:
  - A interface principal é um mapa similar à arena presente na K4-04 com a vista de cima. O usuário reconhecerá a arena caso já tenha visto a mesma.

## Ambiente e contexto

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
