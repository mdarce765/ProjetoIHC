# Avaliação de IHC através de inspeção HEURÍSTICA
## Dez Heurísticas de Nielsen

**Descrição da avaliação**

Avaliação heurística, definida por Nielsen e Molich (1994), é um método de avaliação de usabilidade onde um avaliador procura problemas de usabilidade numa interface com o usuário através da análise e interpretação de um conjunto de princípios ou heurísticas. Este método de avaliação é baseado no julgamento do avaliador.

## **Tabela 1 \- Conjunto de heurísticas de Nielsen (1994)**

| 1\. | Visibilidade do status do sistema: |
| :---- | :---- |
| O sistema deve sempre manter os usuários informados sobre o que está acontecendo através de feedback apropriado, em um tempo razoável. | 3 - O sistema retorna quando o usuário aciona uma placa (alterando a cor/opacidade da placa selecionada); a contagem de placas é alterada a cada placa posicionada ou removida; retorna as janelas do sistema operacional quando salva, carrega ou exporta a arena. Caso não seja atualizada em algum desses pontos, o sistema está com algum problema.<img width="1161" height="736" alt="image" src="https://github.com/user-attachments/assets/8d7efd89-8b12-41d8-b0fe-e7027046b6be" /> |
| **2\.** | **Compatibilidade entre sistema e mundo real:** |
| O sistema deve utilizar a linguagem do usuário, com palavras, frases e conceitos familiares para ele, ao invés de termos específicos de sistemas. Seguir convenções do mundo real, fazendo com que a informação apareça em uma ordem lógica e natural.| 0 - O sistema possui linguagem de fácil entendimento para o usuário, mesmo sendo relacionado à sala K4-04 e voltado para o desenvolvimento de arenas para a mesma, então o público-alvo conseguirá entender normalmente o que é dito, mas mesmo assim possui linguagem de fácil entendimento.<img width="1161" height="736" alt="image" src="https://github.com/user-attachments/assets/7d2352f3-a0cc-4b95-941e-60cc49914d1a" /> |
| **3\.** | **Controle e liberdade para o usuário:** |
| Estão relacionados à situação em que os usuários frequentemente escolhem as funções do sistema por engano e então necessitam de "uma saída de emergência” claramente definida para sair do estado não desejado sem ter que percorrer um longo diálogo, ou seja, é necessário suporte a *undo* e *redo*. | 1 - O sistema possui poucas telas, e as que possui, todas são fáceis de sair ou retornar para a tela anterior. |
| **4\.** | **Consistência e padrões:** |
| Referem-se ao fato de que os usuários não deveriam ter acesso a diferentes situações, palavras ou ações representando a mesma coisa. o sistema deve ter convenções não-ambíguas. | 1 - O sistema não possui convenções ambíguas, seu foco são interações simples e não muito complexas, caso haja, será de fácil correção. |
| **5\.** | **Prevenção de erros:** |
| Os erros são as principais fontes de frustração, ineficiência e ineficácia durante a utilização do sistema. | 3 - O sistema não possui interações muito complexas, e caso haja erros, ou serão com o posicionamento de placas, que caso o mesmo selecione uma parede errada, precisa apenas selecionar novamente para remover, ou com o sistema onde o sistema está sendo executado com relação à parte de importação e exportação de mapas. |
| **6\.** |  **Reconhecimento em lugar de lembrança:** |
| Tornar objetos, ações, opções visíveis e coerentes. O usuário não deve ter que lembrar informações de uma parte do diálogo para outra. Instruções para o uso do sistema devem estar visíveis ou facilmente acessíveis. | 1 - O sistema possui um botão com um texto informativo sobre como utilizar o sistema.<img width="1161" height="736" alt="image" src="https://github.com/user-attachments/assets/ccc495f4-ca19-4413-9170-eec860e0ac05" /> |
| **7\.** | **Flexibilidade e eficiência de uso:** |
| A ineficiência nas tarefas pode reduzir a eficácia do usuário e causar-lhes frustração. O sistema deve ser adequado tanto para usuários inexperientes quanto para usuários experientes. | 2 - O sistema não possui 'truques' para tornar a interação mais eficiente, não criando distinção entre um usuário inexperiente e experiente<br>Exemplo: Permitir que o usuário possa segurar o clique do mouse para selecionar várias paredes, diminuindo a quantidade de cliques e tornando a interação mais suave. |
| **8\.** | **Projeto minimalista e estético:** |
| Os diálogos não devem conter informações irrelevantes ou raramente necessárias. Cada unidade extra de informação em um diálogo compete com unidades relevantes e diminui sua visibilidade relativa. | 1 - O sistema possui o botão de tutorial que possui todas as informações sobre o sistema, para o usuário poder tirar suas dúvidas a qualquer momento. |
| **9\.** | **Auxiliar os usuários a reconhecer, diagnosticar e recuperar erros:** |
| Mensagens de erro devem ser expressas em linguagem natural (sem códigos), indicando precisamente o erro e sugerindo uma solução. | 1 - O sistema possui um contador sobre o uso das placas. Quando o usuário usar mais placas do que tem, um pop-up aparecerá avisando, com linguagem simples e de fácil entendimento para todos.<br> |
| **10\.** | **Ajuda e documentação:** |
| Mesmo que seja melhor que o sistema possa ser usado sem documentação, pode ser necessário fornecer ajuda e documentação. Tais informações devem ser fáceis de encontrar, ser centradas na tarefa do usuário, listar passos concretos a serem seguidos e não ser muito grandes. A ajuda deve estar facilmente acessível e on-line. | 0 - A ajuda se encontra no sistema, tendo um curto manual de todas as funcionalidades; não está disponível de forma separada online.<br> |

## **Tabela 2 \- Grau de severidade dos problemas de usabilidade**

| Grau de severidade | Tipo | Descrição |
| ----- | :---- | :---- |
| 0 | Sem importância | Não afeta a operação da interface |
| 1 | Cosmético | Não há necessidade imediata de solução |
| 2 | Simples | Problema de baixa prioridade (pode ser reparado) |
| 3 | Grave | Problema de alta prioridade (deve ser reparado) |
| 4 | Catastrófico | Muito grave, deve ser reparado de qualquer forma. |

## **INDICAÇÃO DE BOAS PRÁTICAS DE HEURÍSTICA \- HEURÍSTICAS NÃO VIOLADAS**
O usuário é capaz de sair do programa a qualquer momento, sendo que o botão de fechar a página está sempre disponível
