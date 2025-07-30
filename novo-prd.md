# Novo Documento de Requisitos do Produto (PRD) para o Jogo de Realidade Aumentada "Mundo Invertido"
## Introdução
Este PRD descreve os requisitos para o desenvolvimento de um jogo de realidade aumentada (AR) inspirado na série Stranger Things. O jogo será hospedado no GitHub Pages e otimizado para dispositivos Android, como o Samsung S20 FE com Snapdragon. O foco é em uma experiência imersiva, utilizando rastreamento de imagem e elementos AR para guiar o jogador através de missões no mundo real.

O desenvolvimento será realizado em etapas, com testes iniciais no PC e subsequentes no celular, garantindo compatibilidade e desempenho.

## Objetivos
- Criar uma narrativa envolvente baseada em Stranger Things, onde o jogador resgata Will Byers do Mundo Invertido.
- Utilizar tecnologias web para AR, permitindo jogabilidade offline após carregamento inicial.
- Integrar áudio, modelos 3D e elementos visuais para uma experiência imersiva.
- Garantir acessibilidade e usabilidade em dispositivos móveis.
## Tecnologias
- Rastreamento de Imagem : NFT (Natural Feature Tracking) com MindAR.js e Markerless.
- Frameworks AR : AR.js, A-Frame, WebXR.
- Outras Bibliotecas : ORB-SLAM 3 para rastreamento espacial, Three.js para renderização 3D, Model Viewer para modelos GLB animados.
- Hospedagem : GitHub Pages.
- Compatibilidade : Navegadores Android (testado em Samsung S20 FE).
## Requisitos Funcionais
### Tela de Carregamento
- Exibir logo da série ( assets/img/stranger-things-logo.png ).
- Texto "Carregando" com barra de progresso para indicar carregamento de assets.
- Após carregamento, exibir botão "Iniciar o Jogo".
- Garantir que todos os assets sejam baixados para jogabilidade offline.
### Início do Jogo
- Simular ligação de Dustin com imagem ( assets/img/dustin-call.png ).
- Ao clicar, reproduzir áudio ( assets/audio/dustin-intro.mp3 ).
- Ativar câmera e exibir seta/bússola indicando direção para a Floresta das Trevas (coordenadas: -27.63985135643477, -48.66777779450669).
### Missões
O jogo é composto por missões sequenciais, com navegação via GPS, vibração do dispositivo e interações AR.

1. Missão 1: Floresta das Trevas
   
   - Navegação até local (10m de tolerância).
   - Vibração ao chegar.
   - Procurar e clicar em modelo 3D da bicicleta de Will ( assets/models/bicicleta-will.glb ).
   - Áudio de conclusão ( assets/audio/dustin-missao-1-completa.mp3 ).
2. Missão 2: Casa do Will
   
   - Navegação até local (-27.64018223044791, -48.66796420763507, 20m de tolerância).
   - Rastrear marcador Hiro para exibir GIF ( assets/gif/luzes-piscando.gif ).
   - Áudio de alerta ( assets/audio/dustin-missao-2-completa.mp3 ).
   - Fugir para local seguro (-27.63939989306851, -48.66739759100892).
3. Missão 3: Loja Melvald's General Store
   
   - Navegação até local (-27.64018876475326, -48.667940067755126).
   - Coletar itens AR: taco de beisebol ( assets/img/taco.png ) e galão de gasolina ( assets/img/gasolina.png ).
   - Áudio de conclusão ( assets/audio/dustin-missao-4-completa.mp3 ).  // Nota: Áudio referenciado como missão 4 no original, mas ajustado para sequência.
4. Missão 4: Laboratório Nacional de Hawkins
   
   - Navegação até local (-27.63948543364662, -48.66733120633911).
   - Rastrear marcador Hiro para exibir GIF de portal ( assets/gif/portal.gif ).
   - Ao clicar, aplicar filtro esverdeado e partículas (entrada no Mundo Invertido).
   - Áudio de orientação ( assets/audio/dustin-missao-4-completa.mp3 ).
5. Missão 5: Encontro com Demogorgon
   
   - Navegação até local (-27.63980145794119, -48.667683246669554).
   - Vibração e exibição de modelo 3D animado ( assets/models/demogorgon_animated.glb ).
   - Derrotar clicando 3 vezes.
6. Missão 6: Resgate de Will
   
   - Navegação até local (-27.639195545822158, -48.66734595890275).
   - Encontrar e clicar em modelo 3D de Will ( assets/models/will_byers.glb ).
   - Finalizar jogo.
### Recursos Adicionais
- Navegação : Seta e bússola baseadas em GPS; reaparece se o jogador se afastar.
- Áudios : Reprodução automática após eventos.
- Vibração : Para alertas de proximidade.
- Filtros AR : Efeitos visuais no Mundo Invertido.
## Requisitos Não Funcionais
- Desempenho : Otimizado para mobile, com carregamento offline.
- Segurança : Permissões mínimas (câmera, GPS, vibração).
- Testes : Etapas incrementais com commits no GitHub para testes no PC e mobile.
- Acessibilidade : Suporte a áudio e vibração para orientação.
## Assets
- Imagens : stranger-things-logo.png, dustin-call.png, taco.png, gasolina.png.
- Áudios : dustin-intro.mp3, dustin-missao-[1-8]-completa.mp3, main-theme.mp3.
- GIFs : luzes-piscando.gif, portal.gif.
- Modelos 3D : bicicleta-will.glb, demogorgon_animated.glb, will_byers.glb.
- Fontes : stranger-things.ttf.
## Plano de Desenvolvimento
- Etapa 1 : Implementar tela de carregamento e início do jogo. Testar e commit.
- Etapa 2 : Adicionar Missão 1. Testar e commit.
- Etapa 3 : Adicionar Missão 2 e fuga. Testar e commit.
- Etapa 4 : Adicionar Missão 3 e coleta de itens. Testar e commit.
- Etapa 5 : Adicionar Missão 4 e entrada no Mundo Invertido. Testar e commit.
- Etapa 6 : Adicionar Missão 5 e batalha. Testar e commit.
- Etapa 7 : Adicionar Missão 6 e finalização. Testar e commit.
Este PRD serve como base para o desenvolvimento, podendo ser ajustado com base em feedbacks e testes.