# 🐍 Snake — Jogo da Cobrinha

Um jogo clássico de arcade desenvolvido com **HTML5, CSS3 e JavaScript puro (Vanilla JavaScript)**. O projeto funciona diretamente no navegador, sem necessidade de instalar programas adicionais, utilizar frameworks ou depender de bibliotecas externas.

O objetivo é controlar a cobrinha, coletar alimentos, aumentar a pontuação e alcançar o maior recorde possível sem colidir com as paredes ou com o próprio corpo.

## 🎮 Demonstração do projeto

- **Nome:** Snake — Jogo da Cobrinha
- **Categoria:** Jogo de arcade
- **Plataforma:** Navegadores web modernos
- **Tecnologias:** HTML5, CSS3 e JavaScript
- **Formato:** Arquivo HTML único
- **Dependências externas:** Nenhuma

## ✨ Funcionalidades

- 🐍 **Movimentação da cobrinha:** controle por teclado ou botões direcionais.
- 🍎 **Coleta de alimentos:** cada alimento consumido aumenta a pontuação em 10 pontos.
- 📈 **Aumento de velocidade:** a cobrinha fica progressivamente mais rápida conforme a pontuação aumenta.
- 🏆 **Sistema de recordes:** armazena a melhor pontuação no navegador usando `localStorage`.
- ⏸️ **Pausar e continuar:** permite interromper e retomar uma partida.
- 🔄 **Reiniciar partida:** possibilita começar uma nova rodada.
- 💀 **Detecção de colisões:** encerra o jogo quando a cobrinha bate em uma parede ou em seu próprio corpo.
- 🏁 **Condição de vitória:** permite vencer ao ocupar todas as células disponíveis do tabuleiro.
- 📱 **Controles para dispositivos móveis:** botões direcionais para telas sensíveis ao toque.
- 🎨 **Interface moderna:** tema escuro, detalhes em verde, alimentos destacados em vermelho e efeitos visuais.
- ♿ **Acessibilidade básica:** inclui rótulos para elementos do jogo e destaque visual para o foco do teclado.
- 🖥️ **Layout responsivo:** adapta a interface a diferentes tamanhos de tela.

## 🛠️ Tecnologias aplicadas

### 🧱 HTML5 — Estrutura da aplicação

O HTML5 define a estrutura e os elementos da interface do jogo.

Principais recursos utilizados:

- `header`: apresenta o título e a descrição do jogo.
- `main`: organiza o conteúdo principal da aplicação.
- `section`: agrupa a área do jogo e os indicadores de pontuação.
- `button`: cria os controles de início, pausa, reinício e movimentação.
- `canvas`: fornece a área gráfica onde a cobrinha, o alimento e a grade são desenhados.
- Atributos de acessibilidade, como `aria-label`, que ajudam a descrever os elementos da interface.

### 🎨 CSS3 — Estilização e experiência visual

O CSS3 é responsável pela aparência, pelo posicionamento dos elementos e pela adaptação da interface a diferentes dispositivos.

Principais recursos utilizados:

- **Variáveis CSS:** centralizam cores e facilitam a manutenção do tema visual.
- **Flexbox e CSS Grid:** organizam os elementos e os controles direcionais.
- **Media queries:** adaptam a interface para dispositivos móveis e diferentes larguras de tela.
- **Gradientes:** criam profundidade no fundo da aplicação.
- **Bordas arredondadas e sombras:** aprimoram a apresentação dos painéis e botões.
- **Transições:** adicionam efeitos visuais aos botões.
- **Estados de foco e interação:** melhoram a navegação por teclado.
- **`prefers-reduced-motion`:** respeita a preferência do usuário por animações reduzidas.

### ⚙️ JavaScript — Lógica e funcionamento do jogo

O JavaScript implementa as regras, o controle da partida, a pontuação e a interação com o jogador.

Principais recursos utilizados:

- **Variáveis e constantes:** armazenam o estado da partida, a posição da cobrinha, o alimento e a pontuação.
- **Arrays e objetos:** representam os segmentos da cobrinha e as direções de movimento.
- **Funções:** organizam operações como iniciar, pausar, reiniciar, desenhar e atualizar o jogo.
- **Condicionais:** verificam colisões, mudanças de direção e condições de vitória.
- **Laços de repetição:** percorrem o tabuleiro para localizar posições livres e desenhar a grade.
- **Eventos do teclado:** permitem controlar a cobrinha com as setas ou com as teclas WASD.
- **Eventos de ponteiro e clique:** habilitam os controles direcionais para dispositivos móveis.
- **Canvas API:** desenha os elementos gráficos do jogo.
- **`requestAnimationFrame()`:** organiza o ciclo de atualização e renderização.
- **`localStorage`:** persiste o recorde entre partidas e visitas ao jogo, quando o armazenamento está disponível.
- **`try...catch`:** protege a leitura e a gravação do recorde contra falhas de armazenamento.

### 🧩 Canvas API — Renderização gráfica

O elemento `canvas` é utilizado para desenhar os componentes do jogo dinamicamente por meio de JavaScript.

O tabuleiro possui **24 × 24 células**, totalizando 576 posições possíveis.

A renderização inclui:

- Grade de referência do tabuleiro.
- Cabeça e corpo da cobrinha.
- Olhos orientados conforme a direção do movimento.
- Alimento com destaque visual e efeito de brilho.
- Atualização gráfica a cada movimento.

### 💾 LocalStorage — Persistência de dados

A API `localStorage` armazena a melhor pontuação utilizando a chave `snakeBest`.

Isso permite que o recorde continue disponível após reiniciar a partida ou recarregar a página no mesmo navegador e origem, desde que o armazenamento esteja habilitado e os dados não sejam apagados.

## 🕹️ Como jogar

### 1. Iniciar a partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Clique no botão **Começar jogo**.
3. Prepare-se para controlar a cobrinha e coletar os alimentos.

Também é possível iniciar a movimentação usando uma tecla direcional.

### 2. Controles do jogo

| Ação | Tecla ou controle |
|---|---|
| ⬆️ Mover para cima | Seta para cima ou `W` |
| ⬅️ Mover para a esquerda | Seta para a esquerda ou `A` |
| ⬇️ Mover para baixo | Seta para baixo ou `S` |
| ➡️ Mover para a direita | Seta para a direita ou `D` |
| ⏸️ Pausar ou continuar | Barra de espaço |
| ▶️ Iniciar ou reiniciar após o fim | `Enter` ou botão correspondente |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |
| 📱 Controlar no celular | Botões direcionais na tela |

**Atenção:** a cobrinha não pode inverter diretamente o sentido do movimento. Por exemplo, se estiver indo para a direita, não poderá virar imediatamente para a esquerda.

### 3. Objetivo e pontuação

- 🍎 Conduza a cobrinha até o alimento.
- ➕ Ganhe **10 pontos** a cada alimento consumido.
- 🐍 Observe o crescimento da cobrinha conforme ela coleta alimentos.
- ⚡ Prepare-se para movimentos mais rápidos à medida que a pontuação aumenta.
- 🏆 Tente superar seu recorde pessoal.

### 4. Como perder ou vencer

**Fim de jogo:** a partida termina quando a cabeça da cobrinha colide com uma parede ou com o próprio corpo.

**Vitória:** o jogador vence se conseguir ocupar todas as células do tabuleiro, deixando nenhuma posição disponível para um novo alimento.

### 5. Como pausar e retomar

Utilize a barra de espaço ou o botão **Pausar** para interromper a partida. Para continuar, utilize novamente a barra de espaço ou clique em **Retomar**.

O jogo também pausa automaticamente quando a aba do navegador perde a visibilidade durante uma partida ativa.

## 🧠 Conceitos de programação aplicados

O projeto permite estudar conceitos importantes do desenvolvimento web e da lógica de jogos.

| Conceito | Aplicação no projeto |
|---|---|
| 🧮 Lógica de programação | Implementação das regras e condições do jogo. |
| 📦 Variáveis e constantes | Armazenamento das informações da partida. |
| 🗂️ Arrays e objetos | Representação da cobrinha, das posições e das direções. |
| 🔁 Laços de repetição | Percurso das células do tabuleiro. |
| 🔀 Estruturas condicionais | Verificação de colisões, pontuação e vitória. |
| 🧩 Funções | Organização e reutilização da lógica. |
| 🎯 Eventos | Captura de comandos do teclado e de interações com botões. |
| 🎨 Renderização gráfica | Desenho dos elementos usando Canvas API. |
| ⏱️ Animação | Atualização periódica do estado do jogo. |
| 💾 Persistência de dados | Salvamento do recorde com `localStorage`. |
| 📱 Design responsivo | Adaptação da interface para diferentes dispositivos. |
| ♿ Acessibilidade | Uso de rótulos e recursos de navegação por teclado. |

## 📂 Estrutura do projeto

O projeto foi desenvolvido em um único arquivo, sem a necessidade de separar HTML, CSS e JavaScript.

```text
snake-game/
└── index.html    # Estrutura, estilos e lógica do jogo
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos visuais e regras responsivas, dentro da tag `<style>`.
- **JavaScript:** lógica do jogo, dentro da tag `<script>`.

Essa organização facilita a distribuição, a execução e o estudo do código por iniciantes.

## 🚀 Como executar o projeto

Não é necessário instalar dependências, configurar servidores ou compilar o código.

1. 📥 Baixe ou copie o arquivo `index.html`.
2. 📁 Salve o arquivo em uma pasta de sua preferência.
3. 🌐 Abra o arquivo com um navegador moderno, como Google Chrome, Microsoft Edge ou Mozilla Firefox.
4. 🎮 Clique em **Começar jogo** e divirta-se!

O jogo foi desenvolvido para funcionar localmente no navegador, sem conexão com a internet para carregar bibliotecas externas.

## 📌 Considerações técnicas

- O jogo utiliza JavaScript puro, sem frameworks ou bibliotecas de terceiros.
- O tabuleiro possui dimensões lógicas de 24 por 24 células.
- A velocidade é ajustada conforme a pontuação, com um intervalo mínimo de atualização de 70 milissegundos.
- O recorde é salvo localmente e não é compartilhado entre dispositivos ou navegadores.
- A interface inclui controles para teclado e dispositivos com interação por ponteiro.
- O comportamento pode variar em navegadores muito antigos, especialmente em relação aos recursos gráficos mais recentes do Canvas API.

## 🎯 Objetivo educacional

Este projeto demonstra como construir um jogo interativo utilizando apenas tecnologias nativas da web. É uma oportunidade para praticar HTML, CSS e JavaScript, compreender o ciclo de atualização de um jogo e explorar conceitos como colisões, eventos, renderização gráfica, controle de estado e persistência de dados.

## 👨‍💻 Conclusão

O **Snake — Jogo da Cobrinha** combina uma mecânica clássica com uma interface moderna e responsiva. A utilização de HTML5, CSS3 e JavaScript puro demonstra que é possível desenvolver uma aplicação interativa e funcional sem depender de ferramentas externas.

🐍 **Coma, cresça e bata seu recorde!**
