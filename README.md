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
Este público alvo deseja realizar testes de maneira rápida e fácil, quanto menos configurações ou instalações manuais forem necessárias, o melhor. Quanto mais facilitar o processo de desenvolver os mapas, mais rápido os mesmos poderão testar os robôs. Este público deseja velocidade, simplicidade, bom desempenho, possibilidades de serem criativos e etc.

## Desenvolvimento
- [Análise de Concorrência](Arquivos/Documentos/2_concorencia.md)
- [Personas](Arquivos/Documentos/3_personas.md)
- [Cenário de Análise/Problema](Arquivos/Documentos/4_cenarios.md)
- [Análide de Tarefas](Arquivos/Documentos/5_analise_tarefas.md)
- [Prototipação em Papel](Arquivos/Documentos)
- [Coleta de Dados](Arquivos/Documentos)
- [Ciclo de vida da engenharia de usabilidade](Arquivos/Documentos)
- [Modelo Conceitual](Arquivos/Documentos) 
- [MOLIC](Arquivos/Documentos)
- [FIGMA](Arquivos/Documentos)
- [Planejamento da Avaliação](Arquivos/Documentos)
- [Avaliação de IHC através de Inspeção Heurística](Arquivos/Documentos)
- [Avaliação de Usabilidade baseado em Observação do Usuário](Arquivos/Documentos)



      

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
  - É esperado que o usuário se sinta satisfeito ao utilizar o produto, por conta de ter um processo facilitado, quando comparado com ter que modificar manualmente a arena. 
- Acessibilidade:
  - O programa possuirá uma maneira para aplicar zoom nas imagens e aumentar o texto, para auxiliar pessoas com deficiências visuais. 
- Comunicabilidade:
  - A interface principal possui uma imagem da arena presente na K4-04 com a vista de cima, facilitando o entendimento e interpretação do oque está fazendo.

<!--## Coleta de dados

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
-->
<!-- TODOs:
- Add exemplos
 -->
