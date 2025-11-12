# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel).

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **Identificação de diferenças de desempenho entre sistemas robóticos simulados com e sem software conteinerizado, utilizando Simulador Gazebo, ROS 2 e Docker** sob orientação do Professor **Leonardo Anjoletto Ferreira** e desenvolvido pelos seguintes alunos:

- Murilo Darce Borges Silva
- Rodrigo Simões Ruy

## Resumo
Containerização é uma ferramenta muito útil quando se lida com projetos que precisam de diferentes dependências ou programas que podem ter conflitos entre si, que precisam de uma grande quantidade de configuração inicial, ou que precisam de portabilidade. Este projeto visa identificar e mostrar a diferença de desempenho entre robôs, que utilizam o Robot Operating System 2 (ROS 2),  simulados com e sem conteinerização. Para verificar esta diferença, os testes serão realizados no ambiente simulado do software Gazebo Classic. Os resultados mostram que o desempenho da simulação não é impactado pelo uso do Docker, que ocorre um pequeno aumento do uso de memória, porém sem variações significativas no uso do processador, indicando que a simulação usando containers é viável durante o processo de desenvolvimento.

## Introdução
<!--Introdução: falta funcionalidades, tecnologias, contexto de uso-->
A conteinerização é uma ferramenta poderosa no campo de desenvolvimento e implementação, disponibilizando certa camada de isolamento entre componentes de um projeto, assegurando que estes não irão conflitar, seja por funções internas ou dependências de versões diferentes sendo utilizadas. No campo da robótica, conteinerização é vista como uma técnica para facilitar o desenvolvimento, portabilidade e consistência em projetos de robótica, mas não foram feitas pesquisas detalhando sobre a integração destes projetos com Docker e quais efeitos o desempenho de um robô pode acabar sofrendo.

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
- [Prototipação em Papel](Arquivos/Documentos/6_prototipacao.md)
- [Coleta de Dados](Arquivos/Documentos/7_coleta_dados.md)
- [Ciclo de vida da engenharia de usabilidade](Arquivos/Documentos/8_ciclo_vida.md)
- [Modelo Conceitual](Arquivos/Documentos/9_modelo_conceitual.md) 
- [MOLIC](Arquivos/Documentos/10_molic.md)
- [FIGMA](Arquivos/Documentos/11_figma.md)
- [Planejamento da Avaliação](Arquivos/Documentos/12_planejamento_avaliacao.md)
- [Avaliação de IHC através de Inspeção Heurística](Arquivos/Documentos/13_heuristica.md)
- [Avaliação de Usabilidade baseado em Observação do Usuário](Arquivos/Documentos/14_observacao_usuario.md)



      

<!--
## Análise de concorrência

- Pesquise serviços ou podutos existentes atualmente que possam realizar o objetivo deste projeto.
- Selecione pelo menos 3 serviços ou podutos diferentes.
- Em relação aos concorrentes, respondam as seguintes perguntas?
  - Existe plataforma similar que atende o mesmo mercado e funcionalidades? Se sim: Quais os pontos positivos? Quais os pontos negativos?
  - Existe plataforma diferente quanto ao serviço, mas que atenda esse mercado? Se sim: Quais os pontos positivos? Quais os pontos negativos?
 -->

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
