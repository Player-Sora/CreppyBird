# CreepyBird - Halloween Edition 🪦

## Visão geral

<b>CreepyBird</b> é uma recriação do clássico Flappy Bird, mas com um toque assustador! Em vez de guiar um pássaro alegre através de canos, você controla um corvo sombrio voando através de um cemitério cheio de lápides e árvores mortas. O desafio permanece o mesmo: sobreviver o máximo possível sem colidir com os obstáculos. No entanto, agora o ambiente está repleto de sombras, sons arrepiantes e uma atmosfera sombria que vai te deixar no clima de Halloween!

Prepare-se para uma experiência divertida e aterrorizante, com gráficos inspirados no mundo do terror e sons que farão sua espinha gelar. Você consegue guiar o corvo até o amanhecer?

<hr></hr>

<br></br>
## 🎮 Funcionalidades

<ul>
    <li><b>Personagem Principal</b>: Um corvo sombrio, com asas batendo em um cenário assustador.</li>
    <li><b>Obstáculos de Halloween</b>: Passe por lápides aterrorizantes.</li>
    <li><b>Cenário Sinistro</b>: Um cemitério envolto em névoa, com um fundo escuro e lua cheia.</li>
    <li><b>Efeitos Sonoros de Terror</b>: Sons sinistros e risadas macabras para aumentar a imersão.</li>
    <li><b>Música Temática</b>: Uma trilha sonora sombria para complementar a atmosfera de Halloween.</li>
    <li><b>Sistema de Pontuação</b>: A cada obstáculo superado, sua pontuação aumenta.</li>
    <li><b>Dificuldades</b>: Quanto mior os pontos, mais veloz fica o desafio.</li>
</ul>

<hr></hr>

<br></br>
## 🧛‍♂️ Requisitos

<ul>
    <li><b>Python:</b> 3.7 ou superior</li>
    <li><b>Sistema Operacional:</b> Windows 7 ou maior (64 bit)</li>
    <li><b>Processador:</b> 1.7+ GHz ou melhor</li>
    <li><b>Memória:</b> 2 GB de RAM</li>
    <li><b>Armazenamento:</b> 50,0 MB de espaço disponível</li>
    <li><b>Placa de som:</b> DirectX Compatible Sound Card</li>
    <li><b>Bibliotecas:</b></li>
    <ul>
        <li><a href="https://www.pygame.org/wiki/GettingStarted"><code>pygame (biblioteca principal, utilizada para desenvolver o jogo)</code> </a></li>
        <li><a href="https://pillow.readthedocs.io/en/latest/installation/basic-installation.html"><code>PIL (do pacote Pillow)</code> </a></li>
    </ul>
    <font size="4"><b>Instalações</b></font>
    <br></br>
    <pre><code>python --version</code></pre>
    <pre><code>pip install pygame</code></pre>
    <pre><code>pip install pillow</code></pre>
    <br>
    <font size="4"><b>Ou</b></font>
    <br></br>
    <pre><code>pip install -r requirements.txt</code></pre>
</ul>

<hr></hr>

<br></br>

## 🎃 Como Jogar


<ol>
    <li>Pressione a tecla Espaço para fazer o corvo bater asas e voar.</li>
    <li>Evite colidir com os obstáculos assustadores no caminho.</li>
    <li>Quanto mais você voar, mais alta será sua pontuação.</li>
    <li>Cada vez que você bater em um obstáculo perderá um coração</li>
    <li>Tente superar seu recorde anterior e desafie seus amigos a fazerem o mesmo!</li>
    <br>
    <font size="4"><b>Controles</b></font>
    <br></br>
    <ul>
        <li><b>Espaço</b>: Faz o corvo bater as asas.</li>
    </ul>
</ol>

<hr></hr>

<br></br>


## 🕆 Fluxo do jogo


<ol>
    <li><b>Tela Inicial:</b> O usuário pode optar por jogar ou sair. A música de fundo é tocada e o volume pode ser ajustado.</li>
    <li><b>Contagem Regressiva:</b> Antes do início do jogo, uma contagem de 3 segundos é exibida.</li>
    <li><b>Loop Principal:</b> O jogador deve controlar o corvo para evitar os caixões. A pontuação aumenta a cada cano ultrapassado.</li>
    <li><b>Colisões:</b> Se o corvo colide, ele perde uma vida e entra em modo de invencibilidade temporária.</li>
    <li><b>Game Over:</b> Quando todas as vidas são perdidas, a tela de Game Over é exibida, e o jogador pode reiniciar o jogo.</li>
    
</ol>

<hr></hr>

<br></br>
## 👻 Estrutura do Projeto


<pre><code>CreppyBird/
│
├── imgs/                           # Imagens do jogo
│   ├── background_cemiterio.png    # Imagem de fundo (Background) do Jogo.
│   ├── background_inicial.png      # Tela inicial que aparece no menu do jogo.
│   ├── caixao.png                  # Caixão (Obstáculo)
│   └── crow.gif                    # Corvo (Personagem)
│
├── sons/                           # Sons do jogo
│   ├── mixkit-evil.wav             # Risadas macabras
│   ├── StockTune-Creepy.mp3        # Som da tela inicial
│   ├── this-is-halloween.mp3       # Trilha sonora principal do jogo
│   └── mixkit-arcade-fast.wav      # Som da colisão
│
├── FlappyBird.py                   # Código do jogo e configurações
├── README.md                       # Documentação
└── requirements.txt                # Bibliotecas utilizadas no projeto
</code></pre>

<hr></hr>

<br></br>

## 🔥 Alterações por grupo

<br>
<ol>
    <li><b>Grupo 1: Tela Inicial</b></li>
    <ul>
        <li>Implementaram a tela inicial do jogo com opções de "Play" e "Quit", além dos botões para aumentar e diminuir o volume da música de fundo.</li>
    </ul>
    <br>
    <li><b>Grupo 2: Animação e Personagem</b></li>
    <ul>
        <li>Adicionaram uma animação GIF para o corvo utilizando a biblioteca Pillow e gerenciaram a lógica de invencibilidade.</li>
    </ul>
    <br>
    <li><b>Grupo 3: Sons e Efeitos</b></li>
    <ul>
        <li>Implementaram os efeitos sonoros, incluindo música de fundo e sons para eventos específicos como pulo e colisão.</li>
    </ul>
    <br>
    <li><b>Grupo 4: Vidas e Pontuação</b></li>
    <ul>
        <li>Implementaram o sistema de pontuação e vidas, com a lógica para exibir diferentes ícones de vida e uma tela de Game Over.</li>
    </ul>
    <br>
    <li><b>Grupo 5: Incremento de Dificuldade</b></li>
    <ul>
        <li>Adicionaram um aumento progressivo na velocidade dos canos conforme a pontuação aumenta, para dificultar o jogo.</li>
    </ul>
    
</ol>

<hr></hr>

<br></br>
## 🕸️ Componentes do Jogo


<ul>
    <font size="4"><b>Corvo</b></font>
    <br></br>
    <ul>
        <li>O personagem principal é um corvo sombrio que precisa voar por entre obstáculos místicos de Halloween.</li>
        <li>Ele é controlado pelo jogador e se move para frente automaticamente, com a gravidade puxando-o para baixo. Cada vez que o jogador pressiona a tecla Espaço, o corvo bate asas e sobe.</li>
    </ul>
    <br></br>
    <font size="4"><b>Obstáculos de Halloween</b></font>
    <br></br>
    <ul>
        <li><b>Caixões:</b> Aparecem de forma similar aos canos do Flappy Bird, como obstáculos verticais que devem ser evitados.</li>
        <li><b>Aranhas:</b> Surgem caindo do céu, evite-as para não perder seus corações de vida.</li>
    </ul>
    <br></br>
    <font size="4"><b>Cenário Sinistro</b></font>
    <br></br>
    <ul>
        <li>O fundo do jogo é composto por um céu escuro e lua cheia.</li>
    </ul>
    <br></br>
    <font size="4"><b>Efeitos Sonoros</b></font>
    <br></br>
    <ul>
        <li>Sons arrepiantes, como risadas macabras criam uma experiência imersiva.</li>
        <li>Efeitos sonoros para colisão e pontos também estão incluídos.</li>
    </ul>
    <br></br>
    <font size="4"><b>Pontuação</b></font>
    <br></br>
    <ul>
        <li>A cada conjunto de obstáculos superado, a pontuação aumenta em 5 pontos.</li>
        <li>A pontuação é exibida na parte superior da tela.</li>
        <li>Cada vez que o jogador acumula 50 pontos, a velocidade do desafio aumenta.</li>
    </ul>
</ul>

<hr></hr>

<br></br>
## 👽 Funções e Módulos
<br></br>

<code>Classe Passaro</code>
<ul>
    <li>Funções para desenhar e controlar o comportamento do Corvo, como:</li>
    <ul>
        <li>Movimentação</li>
        <li>Pulo e gravidade</li>
    </ul>
</ul>
<hr></hr>


<code>Classe Cano</code>
<ul>
    <li>Funções para desenhar e controlar os obstáculos do jogo, como:</li>
    <ul>
        <li>Movimentação e altura dos caixões e aranhas</li>
        <li>Colisões com o corvo</li>
    </ul>
</ul>
<hr></hr>


<code>Classe Chao</code>
<ul>
    <li>Funções para desenhar o chão do jogo e gerar impressão de movimento.</li>
</ul>
<hr></hr>


<code>Função load_gif()</code>
<ul>
    <li>Carrega uma animação GIF para o corvo.</li>
</ul>
<hr></hr>


<code>Função tela_inicial()</code>
<ul>
    <li>Exibe a tela inicial do jogo.</li>
    <li>Adiciona botão de play e quit para o jogo.</li>
    <li>Mixer com uma barra para controlar o volume do jogo.</li>
</ul>
<hr></hr>


<code>Função contagem()</code>
<ul>
    <li>Função para exibir uma contagem regressiva antes do jogo começar.</li>
</ul>
<hr></hr>


<code>Função desenhar_tela()</code>
<ul>
    <li>Pede como parametro as instancias das classes principais para desenhar os elementos na tela, como:</li>
    <ul>
        <li>O corvo.</li>
        <li>Corações de vida.</li>
        <li>Chão do jogo.</li>
        <li>Pontos obtidos pelo jogador.</li>
    </ul>
</ul>
<hr></hr>


<code>Função exibir_game_over()</code>
<ul>
    <li>Mostra a tela de Game Over com os pontos obtidos pelo jogador ao decorrer da partida.</li>
</ul>
<hr></hr>


<code>Função main()</code>
<ul>
    <li>Contém o loop principal do jogo e é responsável por:</li>
    <ul>
        <li>Instanciar os objetos do game.</li>
        <li>Iniciar o jogo.</li>
        <li>Controlar a lógica de aparições e velocidade dos obstáculos.</li>
        <li>Controlar a lógica de movimento.</li>
        <li>Detectar colisões.</li>
        <li>Gerenciar a pontuação.</li>
        <li>Reeniciar o jogo após o fim.</li>
    </ul>
</ul>


<hr></hr>

<br></br>

## 👿 Possíveis melhorias


<ol>
    <li><b>Salvar Pontuação Máxima:</b> Implementar um sistema para salvar a pontuação mais alta do jogador.</li>
    <li><b>Mais Obstáculos e Desafios:</b> Adicionar outros tipos de obstáculos e níveis de dificuldade.</li>
    <li><b>Variedade de Personagens:</b> Incluir diferentes personagens para o jogador escolher.</li>
    <li><b>Suporte a Multijogador:</b> Implementar um modo multiplayer, onde dois jogadores competem simultaneamente.</li>
    
</ol>

<hr></hr>

<br></br>



## 🔮 Adicionais
<br></br>

<font size="3"><b>Projeto desenvolvido pelo Professor Roberto de Pádua Carvalho Reis e aprimorado pela turma do 5º período de Engenharia de software 3. Curso de Sistemas de informações, turno matutino.</b></font>
