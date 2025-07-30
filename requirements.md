## Documento de Requisitos
### Introdução
Este documento define os requisitos funcionais e não funcionais para o desenvolvimento do jogo de realidade aumentada. O objetivo é guiar o jogador em uma narrativa imersiva para resgatar Will Byers, utilizando tecnologias web e AR.

### Requisitos Funcionais
- Tela Inicial e Carregamento : Exibir logo, barra de progresso e botão de início após carregamento de assets para suporte offline.
- Narração e Áudios : Iniciar com ligação de Dustin, reproduzir áudios específicos em cada missão.
- Navegação : Usar GPS para seta e bússola, com vibração ao chegar em locais (tolerâncias de 10-20m).
- Elementos AR : Rastreamento de marcadores (ex: Hiro) para exibir GIFs, modelos 3D (GLB) e itens coletáveis.
- Missões Sequenciais : 6 missões com interações como clicar em objetos AR, derrotar inimigos e aplicar filtros visuais no "Mundo Invertido".
- Finalização : Concluir ao resgatar Will, com possível tela de vitória.
### Requisitos Não Funcionais
- Desempenho : Otimizado para mobile Android, com carregamento rápido e suporte offline.
- Compatibilidade : Funcionar em navegadores com WebXR, testado em PC e celular.
- Segurança : Permissões limitadas a câmera, GPS e vibração.
- Usabilidade : Interface intuitiva, com feedbacks auditivos e vibratórios.
- Tecnologias : AR.js, A-Frame, Three.js, MindAR.js, Model Viewer.
### Assets Necessários
- Imagens, áudios, GIFs e modelos 3D listados na pasta assets/ .