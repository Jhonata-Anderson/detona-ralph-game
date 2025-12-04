# 🎮 Detona Ralph (Whac-A-Mole Clone)

Um jogo simples no estilo **Acerte o Ralph**, baseado no personagem **Detona Ralph**, desenvolvido usando HTML, CSS e JavaScript puro.

## ✨ Visão Geral

O objetivo do jogo é **acertar o personagem Ralph** o maior número de vezes possível dentro do tempo limite. O Ralph aparecerá aleatoriamente em uma das nove casas do painel.

O jogo apresenta:
* Um painel de **pontuação** e **tempo restantes**.
* Movimentação aleatória do "Ralph" (inimigo).
* Contagem de pontuação ao acertar o inimigo.
* Feedback sonoro.
* Encerramento do jogo e exibição do resultado ao final do tempo.



---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura básica da página.
* **CSS3:** Estilização e layout, incluindo a utilização de `flexbox` para o menu e imagens de fundo para o cenário (`wall.png`) e o inimigo (`ralph.png`).
* **JavaScript (ES6+):** Lógica principal do jogo, gerenciamento de estado (`state` object), controle de *timers* (`setInterval`), geração de posições aleatórias e escuta de eventos (`mousedown`).

---

## ⚙️ Configuração do Jogo (JavaScript)

Você pode facilmente ajustar a dificuldade do jogo modificando as propriedades no objeto `state.values` dentro do arquivo `src/scripts/engine.js`:

| Variável | Descrição | Valor Padrão |
| :--- | :--- | :--- |
| `gameVelocity` | Define a velocidade de reaparecimento do inimigo (em **milissegundos**). | `1000` (1 segundo) |
| `curretTime` | Define o tempo inicial total do jogo (em **segundos**). | `60` (60 segundos) |

**Exemplo:** Para deixar o jogo mais desafiador, aumentando a velocidade e diminuindo o tempo:

```javascript
// src/scripts/engine.js

const state = {
    // ...
    values: {
        gameVelocity: 600, // Ralph aparece a cada 0.6 segundo
        hitPosition: 0,
        result: 0,
        curretTime: 30, // Jogo dura apenas 30 segundos
    },
    // ...
}
```

## 👨‍💻 Expert

<p>
    <img 
      align=left 
      margin=10 
      width=80 
      src="https://avatars.githubusercontent.com/u/168501597?v=4"
    />
    <p>&nbsp&nbsp&nbspJhonata Anderson<br>
    &nbsp&nbsp&nbsp
    <a href="https://github.com/Jhonata-Anderson">
    GitHub</a>&nbsp;|&nbsp;
    <a href="https://www.linkedin.com/in/jhonata-anderson/">LinkedIn</a>
&nbsp;|&nbsp;
</p>
<br/><br/>
<p>
Feito com 💙 como parte da Trilha de CSS da Digital Innovation One (DIO).