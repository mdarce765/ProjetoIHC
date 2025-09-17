# Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

## Funcionalidades
1. Botões para inserir paredes  
2. Criação do mapa com as paredes selecionadas  
3. --Acessibilidade--
4. --?--

## HTA
### 1 - Botões para inserir paredes
A parte visual terá botões, igual às possíveis paredes na arena, junto de uma imagem em overlay, para deixar mais fácil a visualização de como a arena final seria.  
```mermaid
graph TD;

    id1[0- Salvar botões selecionados <br>1+2]
    id2[1.1- Overlay da imagem do mapa]
    id3[1.2- Posicionar botões]
    
    id1-->id2;
    id1-->id3;
```
### 2 - Criação do mapa com as paredes selecionadas
Levando em conta os botões selecionados na parte visual, será criada paredes nas posições correspondentes na arena.  
```mermaid
graph TD;
    
    id1[0- Salvar modelo com as paredes nas posições dos botões <br>1+2+3]
    id2[1.1- Inserir paredes em posições específicas na arena]
    id3[1.2- Relacionar botões com posições na arena]
    id4[1.3- Adquirir modelo da arena base]
    
    id1-->id2;
    id1-->id3;
    id1-->id4;
```
### 3 -
### 4 -

## GOMS (Fazer KLM?)
### 1 - Botões para inserir paredes
Se pode criar uma arena customizada utilizando cliques, selecionando as paredes que serão colocadas, facilitando a criação e também uma "pré-visualização" da nova arena.  
- GOAL 0: Criar uma arena customizada, baseada em uma arena base.     
    - GOAL 1: Adicionar/Remover ou editar paredes extras.    
        - METHOD 2.A: Clicar nos botões onde se deseja adicionar/remover paredes.  
          (SELECTION RULE: Caso a parede esteja longe/preferência)  
        - METHOD 2.B: Selecionar as paredes utilizando setas e Enter  
          (SELECTION RULE: Caso a parede estja perto/preferência)  
          - METHOD 2.B.1: Movimentar entre as paredes usando as setas do teclado  
          - METHOD 2.B.2: Adicionar/Remover parede selecionada utilizando a tecla Enter  
    - GOAL 3: Salvar arena customizada.  
        - METHOD 3.A: Clicar no botão de salvar.  
          (SELECTION RULE: Preferência)    
        - METHOD 3.B: Usar atalho Control+S.  
          (SELECTION RULE: Comando rápido)  
      

        
### 2 - Criação do mapa com as paredes selecionadas  
Obter o arquivo do mapa customizado, utilizando a interface de seleção de paredes.  
- GOAL 0: Obter o mapa gerado, baseado nos botões pressionados e da arena base.  
  - METHOD 0.A: Criar um mapa baseado nas paredes salvas.  
    (SELECTION RULE: Preferência)   
      - METHOD 0.A.1: Abrir a interface de seleção de paredes.  
      - METHOD 0.A.2: Selecionar paredes até estar satisfeito.  
      - METHOD 0.A.3: Salvar as paredes selecionadas.  
      - METHOD 0.A.4: Clicar em Criar Mapa.  
    
### 3 -
### 4 -

## CTT
### 1 - Botões para inserir paredes
Para Criar uma arena customizada, o usuário precisa primeiro decidir as paredes que devem ser inseridas, selecioná-las e depois clicar em salvar.  
ABS - Criar arena customizada -> (USR - Decidir que paredes devem ser inseridas >> USR-SYS - Clicar nos botões aonde deseja que as paredes estejam >> USR-SYS - Clicar em salvar []>> SYS - Salvar os botões selecionados)      
<img width="1048" height="304" alt="Screenshot 2025-09-17 at 09 16 56" src="https://github.com/user-attachments/assets/4dddae4a-1cc7-4f73-b359-0456aa961b88" />  



### 2 - Criação do mapa com as paredes selecionadas
Para utilizar uma arena customizada, o usuário precisa criar a arena, e depois a carregar    
ABS - Utilizar arena customizada -> (ABS - Criar arena customizada []>> USR-SYS - Pressionar o botão de Criar Mapa []>> SYS - Criar mapa baseado nas paredes selecionadas []>> USR-SYS - Carregar mapa em um simulador) 
### 3 -
### 4 -
