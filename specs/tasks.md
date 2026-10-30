# Plano de implementação: Chuva de Bugs

> Como usar: rode `/4-implementar N` para cada tarefa, teste no navegador e faça um commit local ao concluir cada tarefa. Nunca faça push.

- [ ] 1. Monte o esqueleto visível do jogo
  - Crie a página, o canvas centralizado, a configuração inicial e o loop com `requestAnimationFrame` e delta time.
  - Desenhe no canvas o título e a instrução para começar, mesmo antes de implementar a partida.
  - **Arquivos:** `index.html`, `style.css`, `src/config.js`, `src/main.js`, `src/renderer.js`
  - **Como verificar:** abra a página pelo servidor do projeto → a área fica centralizada sobre o fundo escuro e mostra o título e a instrução de início.
  - _Requisitos: 1.1, 7.2_

- [ ] 2. Implemente a partida básica
  - Crie o estado da partida e faça Espaço iniciar o jogo; mova o dev com as setas ou A/D, mantendo-o dentro da área.
  - Faça cafés e bugs caírem em posições horizontais variadas; remova os itens que chegam ao chão sem colisão.
  - Resolva colisões, pontuação e vidas; desenhe o dev, os itens e o HUD durante a partida.
  - **Arquivos:** `src/config.js`, `src/main.js`, `src/game.js`, `src/renderer.js`
  - **Como verificar:** inicie com Espaço, mova o dev para os dois lados, colete um café e toque um bug → posição, pontuação e vidas respondem; itens que passam sem colisão somem sem alterar os valores.
  - _Requisitos: 1.2, 1.3, 2.1, 2.2, 2.3, 3.1, 3.2, 4.1, 4.2, 4.3, 7.1_

- [ ] 3. Complete dificuldade, fim e recorde
  - Aumente gradualmente a velocidade dos itens e a frequência de surgimento, respeitando os limites definidos em `CONFIG`.
  - Encerre a partida ao perder a última vida e desenhe pontuação final, recorde e instrução de reinício.
  - Permita reiniciar com Espaço e salve no armazenamento local qualquer novo recorde.
  - **Arquivos:** `src/config.js`, `src/main.js`, `src/game.js`, `src/renderer.js`
  - **Como verificar:** em uma sessão nova, jogue até perder as vidas e confira a tela final; bata o recorde, atualize a página e confirme que ele continua salvo; pressione Espaço para iniciar outra partida com pontuação zerada e 3 vidas.
  - _Requisitos: 1.3, 1.4, 5.1, 5.2, 6.1, 6.2, 6.3_

- [ ] 4. Refine e confira todos os critérios
  - Ajuste o desenho, o posicionamento dos textos e a apresentação responsiva sem alterar a resolução lógica do canvas.
  - Corrija problemas encontrados na conferência dos limites, colisões, telas, controles, progressão, recorde e caminhos relativos.
  - **Arquivos:** `index.html`, `style.css`, `src/config.js`, `src/main.js`, `src/game.js`, `src/renderer.js`
  - **Como verificar:** jogue uma partida completa no navegador e confira cada critério de 1.1 a 7.2, incluindo os limites da área, o reinício e o recorde após recarregar a página.
  - _Requisitos: 1.1, 1.2, 1.3, 1.4, 2.1, 2.2, 2.3, 3.1, 3.2, 4.1, 4.2, 4.3, 5.1, 5.2, 6.1, 6.2, 6.3, 7.1, 7.2_

## Correções
Vazio por enquanto; o comando `/corrigir-bug` escreve aqui.

