# Requisitos: Chuva de Bugs

## Introdução
Chuva de Bugs é um jogo de navegador para quem quer testar reflexos em uma partida rápida. O jogador controla um dev, coleta cafés para pontuar e desvia de bugs que caem do céu.

## Glossário
- **Dev**: personagem controlado pelo jogador.
- **Item**: café ou bug que cai na área do jogo.
- **Recorde**: maior pontuação alcançada pelo jogador neste navegador.

## Requisitos

### Requisito 1: Telas do jogo
**História de usuário:** Como jogador, quero ver as telas de início, partida e fim de jogo, para saber quando começar, acompanhar a partida e jogar novamente.

**Critérios de aceitação**
- **1.1** O SISTEMA DEVE exibir na tela inicial o nome do jogo e a instrução para começar com Espaço.
- **1.2** QUANDO o jogador pressionar Espaço na tela inicial, O SISTEMA DEVE iniciar a partida.
- **1.3** ENQUANTO a partida estiver em andamento, O SISTEMA DEVE exibir a pontuação e as vidas restantes.
- **1.4** QUANDO a partida terminar, O SISTEMA DEVE exibir a pontuação da partida, o recorde e a instrução para jogar novamente com Espaço.

### Requisito 2: Movimento do dev
**História de usuário:** Como jogador, quero mover o dev para os lados, para alcançar cafés e evitar bugs.

**Critérios de aceitação**
- **2.1** QUANDO o jogador pressionar a seta para a esquerda ou a tecla A durante a partida, O SISTEMA DEVE mover o dev para a esquerda.
- **2.2** QUANDO o jogador pressionar a seta para a direita ou a tecla D durante a partida, O SISTEMA DEVE mover o dev para a direita.
- **2.3** O SISTEMA DEVE manter o dev dentro dos limites da área do jogo.

### Requisito 3: Itens que caem
**História de usuário:** Como jogador, quero que cafés e bugs caiam em posições variadas, para ter de reagir durante a partida.

**Critérios de aceitação**
- **3.1** ENQUANTO a partida estiver em andamento, O SISTEMA DEVE fazer cafés e bugs caírem do topo da área do jogo em posições variadas.
- **3.2** QUANDO um item chegar ao chão sem tocar o dev, O SISTEMA DEVE removê-lo sem alterar a pontuação ou as vidas.

### Requisito 4: Pontuação e vidas
**História de usuário:** Como jogador, quero ganhar pontos ao coletar cafés e perder vidas ao tocar bugs, para acompanhar meu desempenho e o risco da partida.

**Critérios de aceitação**
- **4.1** QUANDO o dev tocar um café, O SISTEMA DEVE acrescentar 1 ponto à pontuação da partida.
- **4.2** QUANDO o dev tocar um bug, O SISTEMA DEVE retirar 1 vida.
- **4.3** O SISTEMA DEVE iniciar cada partida com 3 vidas.

### Requisito 5: Dificuldade progressiva
**História de usuário:** Como jogador, quero que a partida fique mais desafiadora com o tempo, para testar meus reflexos.

**Critérios de aceitação**
- **5.1** ENQUANTO a partida estiver em andamento, O SISTEMA DEVE aumentar gradualmente a velocidade de queda dos itens.
- **5.2** ENQUANTO a partida estiver em andamento, O SISTEMA DEVE aumentar gradualmente a frequência de surgimento dos itens.

### Requisito 6: Fim e reinício da partida
**História de usuário:** Como jogador, quero que a partida termine quando minhas vidas acabarem e possa começar outra, para continuar jogando.

**Critérios de aceitação**
- **6.1** QUANDO o jogador perder a última vida, O SISTEMA DEVE encerrar a partida e exibir a tela de fim de jogo.
- **6.2** QUANDO o jogador pressionar Espaço na tela de fim de jogo, O SISTEMA DEVE iniciar uma nova partida com a pontuação zerada e 3 vidas.
- **6.3** QUANDO a pontuação da partida superar o recorde, O SISTEMA DEVE atualizar o recorde e mantê-lo salvo mesmo após o jogador fechar a página.

### Requisito 7: Apresentação visual
**História de usuário:** Como jogador, quero reconhecer o dev e os itens em uma área de jogo organizada, para acompanhar a ação com clareza.

**Critérios de aceitação**
- **7.1** O SISTEMA DEVE apresentar o dev, os cafés e os bugs com os emojis 🧑‍💻, ☕ e 🐛, respectivamente.
- **7.2** O SISTEMA DEVE exibir a área do jogo em tamanho fixo e centralizada na página, sobre um fundo escuro com aparência de editor de código.

## Fora do escopo
- Som e música.
- Multiplayer.
- Login.
- Ranking online.
- Níveis ou fases.

## Suposições
- "Posições aleatórias" significa que os itens podem surgir em diferentes posições horizontais dentro da área do jogo.
- O recorde é individual para o navegador em uso e persiste após fechar a página.