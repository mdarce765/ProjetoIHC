# Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

## Funcionalidades
1. Botões para inserir paredes  
2. Criação do mapa com as paredes selecionadas  
3. Importar arena
4. Aplicar zoom

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

### 3 - Importar arena
```mermaid
graph TD;
    id0[0 - Importar arena para a interface<br>1+2+3]

    id1[1 - Utilizar o botão 'Arquivo' da interface<br>1>2/3]
    id1.1[1.1 - Selecionar a opção de abrir arquivo<br>________________________]
    id1.2[1.2 - Digitar o nome do arquivo<br>________________________]
    id1.3[1.3 - Selecionar o arquivo<br>________________________]

    id2[2 - Utilizar atalho do teclado<br>1/2]
    id2.1[2.1 - Digitar o nome do arquivo<br>________________________]
    id2.2[2.2 - Selecionar o arquivo<br>________________________]

    id3[3 - Inicializar a arena pelo terminal<br>________________________]

    id0-->id1
    id0-->id2
    id0-->id3

    id1-->id1.1
    id1-->id1.2
    id1-->id1.3

    id2-->id2.1
    id2-->id2.2
```

### 4 - Aplicar zoom
```mermaid
graph TD;
    id0[0 - Aplicar zoom em uma área<br>1+2]

    id1[1 - Utilizar a roda do mouse<br>1/2]
    id1.1[1.1 - Rolar a roda do mouse para cima para aplicar zoom-in<br>________________________]
    id1.2[1.2 - Rolar a roda do mouse para baixo para aplicar zoom-out<br>________________________]

    id2[2 - Utilizar botão pop-up da interface<br>1/2]
    id2.1[2.1 - Utilizar o botão '+' para aplicar zoom in<br>________________________]
    id2.2[2.2 - Utilizar o botão '-' para aplicar zoom out<br>________________________]

    id0-->id1
    id0-->id2

    id1-->id1.1
    id1-->id1.2

    id2-->id2.1
    id2-->id2.2
```

## GOMS
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
    
### 3 - Importar arena
  - **GOAL 0**: Importar arena para a interface.
    - **METHOD 0.A:** Utilizar o botão 'Arquivo' da interface  
    **(SEL. RULE:** Falta de costume/conhecimento. **)**
      - **OP 0.A.1:** Selecionar a opção de "Abrir Arquivo"
        - **METHOD 0.A.1.A:** Selecionar arquivo  
        **(SEL. RULE:** Preferencia. **)**
          - **OP 0.A.1.A.1:** Digitar o nome do arquivo
          - **OP 0.A.1.A.2:** Selecionar o arquivo
        

    - **METHOD 0.B:** Utilizar comando do teclado  
    **(SEL. RULE:** Praticidade. **)**
      - **OP 0.B.1:** Digitar o nome do arquivo
      - **OP 0.B.2** Selecionar o arquivo

    - **METHOD 0.C:** Inicializar pelo terminal  
    **(SEL. RULE:** Praticidade. **)**

### 4 - Aplicar zoom
- **GOAL 0**: Aplicar Zoom na interface.
  - **METHOD 0.A:** Utilizar a roda do mouse.  
  **(SEL. RULE:** Praticidade. **)**
  - **METHOD 0.B:** Utilizar o ícone presente na interface.  
  **(SEL. RULE:** Falta de costume/entendimento. **)**

## CTT
### 1 - Botões para inserir paredes
Para Criar uma arena customizada, o usuário precisa primeiro decidir as paredes que devem ser inseridas, selecioná-las e depois clicar em salvar.  
ABS - Criar arena customizada -> (USR - Decidir que paredes devem ser inseridas >> ABS - Clicar nos botões aonde deseja que as paredes estejam ->(USR-SYS - Clicar em um botão []>> SYS - Mudar a opacidade do botão selecionado) >> USR-SYS - Clicar em salvar []>> SYS - Salvar os botões selecionados)      
<img width="905" height="362" alt="Screenshot 2025-09-17 at 15 05 44" src="https://github.com/user-attachments/assets/c68dba2a-466f-4553-b9bf-84fdba08e80b" />



### 2 - Criação do mapa com as paredes selecionadas
Para utilizar uma arena customizada, o usuário precisa criar a arena, e depois a carregar    
ABS - Utilizar arena customizada -> (ABS - Criar arena customizada []>> USR-SYS - Pressionar o botão de Criar Mapa []>> SYS - Criar mapa baseado nas paredes selecionadas []>> USR-SYS - Carregar mapa em um simulador) 
<img width="1068" height="333" alt="Screenshot 2025-09-17 at 15 14 18" src="https://github.com/user-attachments/assets/11477bee-a640-40cb-b023-02f7213691cd" />

### 3 - Importar arena
### 4 - Aplicar zoom
