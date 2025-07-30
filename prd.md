Jogo de realidade aumentada com temática da série stranger things
Quero criar um jogo de realidade aumentada usando meu navegador do android do meu celular samsung s20fe com Snapdragon.
O jogo será hospedado no github pages.
quero usar tecnologias:

Rastreamento de Imagem (NFT - Natural Feature Tracking)
AR.js
A-Frame
WebXR
ORB-SLAM 3
MindAR.js
Markerless
Three.js

Model Viewer para os glb animados

Quero que o desenvolvimento do projeto seja feito em etapas, e quero poder testar primeiro no meu pc e depois no celular antes de avançar para a próxima etapa

O jogo deve iniciar com uma página onde aparece o logo da série “assets/img/stranger-things-logo.png”, abaixo um texto escrito carregando e abaixo uma barra de carregamento que irá indicar quando todos os elementos do jogo foram carregados para que o jogo possa funcionar offline, já que em alguns lugares do bairro pode não ter sinal de internet.
Após carregar todos os elementos, o texto e a barra de carregamento desaparecem e no lugar aparece um botão escrito “Iniciar o Jogo”.
O jogo inicia com uma ligação do personagem DUSTIN.
No navegador deve aparecer uma imagem “assets/img/dustin-call.png” simulando uma ligação com o rosto de Dustin. Ao clicar na imagem o jogador recebe uma mensagem de áudio “assets/audio/dustin-intro.mp3” de Dustin dizendo:
“Ei aqui é o Dustin, consegue me ouvir? Will desapareceu após uma partida de Dungeons & Dragons. Você, como membro do grupo, deve ir até a Floresta das Trevas para encontrar pistas sobre seu paradeiro”.
Ao final da mensagem, a câmera do celular é ativada e uma seta, se possível feita svg ou outro elemento, indica a direção da Floresta da Trevas, com uma bússola. O sistema deve usar a posição atual do jogador e calcular a direção para onde ele deve ir até chegar na Floresta das Trevas.

Essa é a localização da Floresta das Trevas: -27.63985135643477, -48.66777779450669
Ao chegar a 10 metros dessa localização, a seta deve desaparecer e o celular deve vibrar duas vezes indicando que está próximo do local da primeira missão. Caso o jogador se afaste 10 metros da localização da missão e ainda não tenha concluído a missão, a seta deve voltar a aparecer para orientar o jogador para voltar a localização para terminar a missão.
Neste local, o jogador deve utilizar a câmera do celular e procurar um elemento AR que deve ser um modelo 3d da bicicleta do Will. O arquivo está disponível na pasta “assets/models/bicicleta-will.glb”.
Ao localizar a bicicleta o jogador deve clicar no elemento AR da bicicleta e irá coletar essa pista, concluindo a primeira missão.

Ao final dessa etapa os arquivos do jogo devem ser enviados ao repositório do github para que sejam testados pelo meu celular no github pages.

Após concluir a missão o jogador recebe outra mensagem de audio “assets/audio/dustin-missao-1-completa.mp3” de Dustin dizendo:

“Ei, ótimo trabalho! Você encontrou a bicicleta do Will. Isso indica que alguma coisa ruim aconteceu. Vá até a casa do Will e procure mais pistas.
Ao finalizar a mensagem de voz a imagem de Dustin desaparece e aparece a seta indicando o local da próxima missão.
Essa é a localização da casa do Will:-27.64018223044791, -48.66796420763507

Ao final dessa etapa os arquivos do jogo devem ser enviados ao repositório do github para que sejam testados pelo meu celular no github pages.

Ao chegar a 20 metros dessa localização, a seta deve desaparecer e o celular deve vibrar duas vezes indicando que está próximo do local da segunda missão.
Neste local, o jogador deve utilizar a câmera do celular e apontar para o marcador hiro na parede e então irá exibir o gif animado “assets/img/luzes-piscando.gif” deve aparecer na parede onde está a imagem de rastreamento. Uma nova mensagem de audio “assets/audio/dustin-missao-2-completa.mp3” de Dustin aparece dizendo:

Cuidado Camille! O Demogorgon está nesta casa. Fuja agora!
A seta indica a direção que o jogador deve ir para fugir do Demogorgon.

Localização do local onde o jogador deve ir para fugir do Demogorgon: -27.63939989306851, -48.66739759100892


Depois que o jogador chegou no local indicado ele recebe outra mensagem de áudio “assets/audio/dustin-missao-3-completa.mp3” do Dustin dizendo:

“Ufa essa foi por pouco. Agora você precisa ir Loja Melvald's General Store, para pegar suprimentos para lutar contra o Demogorgon.
A seta novamente aparece e indica a direção da Loja.
A localização da Loja Melvald's General Store é: -27.64018876475326, -48.667940067755126

Ao chegar no local, o jogador deve apontar a câmera em volta e encontrar elemento AR para coletar. Os elementos serão um taco de basebol “assets/img/taco.png” e um galão de gasolina “assets/img/gasolina.png”. O jogador deve apontar a câmera para o objeto e clicar nele para coletar.
Após coletar os objetos, uma nova mensagem de audio “assets/audio/dustin-missao-4-completa.mp3” do Dustin aparece dizendo:

“Ei Camille, ótimo trabalho! Agora você deve ir até o Laboratório Nacional de Hawkins e descobrir uma entrada para o mundo invertido e encontrar o Will.
A seta aparece e indica a direção da próxima missão que será no Laboratório Nacional de Hawkins.
Essa é a localização do Laboratório Nacional de Hawkins: -27.63948543364662, -48.66733120633911

Chegando no local, o jogador deve utilizar a câmera e apontar para o marcador hiro.
Ao apontar a câmera para o marcador hiro, um gif animado irá aparecer “assets/gif/portal.gif”.
O jogador deve clicar no gif animado e será como se tivesse entrado no mundo invertido. Agora quando o jogador olha pela câmera do celular a imagem tem um filtro esverdeado e partículas aparecem pairando no ar.
Novamente aparece uma mensagem de audio “assets/audio/dustin-missao-4-completa.mp3” do Dustin, dizendo:

Camille! Agora que você está dentro do mundo invertido, vá até a casa do Will para resgata-lo. Mas tome cuidado, você pode encontrar o Demogorgon no caminho.
A seta aparece e indica a direção da próxima missão que será encontro com o demogorgon.

Essa é a localização do encontro com o demogorgon: -27.63980145794119, -48.667683246669554
Quando o jogador chegar neste local o celular deve vibrar duas vezes e um elemento 3d “assets/models/demogorgon_animated.glb” deve aparecer.
O jogador deve apontar a câmera para o objeto 3D e clicar nele 3 vezes para fazer ele desaparecer, derrotando assim o demogorgon.
A seta aparece e indica a direção da próxima missão que será encontrar Will.

Essa é a localização para encontrar Will: -27.639195545822158, -48.66734595890275

Chegando na localização que está Will, o jogador deve utilizar a câmera para encontrar o elemento “assets/models/will_byers.glb” e clicar nele para finalizar a última missão.





