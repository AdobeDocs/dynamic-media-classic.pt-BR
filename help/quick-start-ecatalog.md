---
title: '" Início rápido: Ecatalogs "'
seo-title: '" Início rápido: Ecatalogs "'
description: 'null'
seo-description: Uma introdução e um Início rápido aos ecatalogs para ajudá-lo a começar a usar rapidamente as técnicas ecatalog.
uuid: 1 ec 41927-3 df 6-4845-8 d 9 d-bb 92 cf 6 dca 08
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/ecatalogs
discoiquuid: 781 dacd 0-ef 0 c -42 b 7-92 e 0-12791994874 d
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Início rápido: Ecatalogs{#quick-start-ecatalogs}

Um ecatalog é uma versão digital da Web de material impresso— um catálogo, um folheto, um flyer, um manual de produtos ou circular, por exemplo. Um ecatalog é exibido em um visualizador do ecatalog em um site. Esse visualizador simula a experiência de ler material impresso. Dependendo das configurações escolhidas para o catálogo eletrônico, o visualizador pode permitir que você faça o seguinte:

* Pesquise o catálogo de palavras-chave ou palavras-chave. Os resultados da pesquisa são exibidos como uma lista de miniaturas em um painel de pesquisa no lado esquerdo do catálogo. Cada miniatura clicável representa um catálogo espalha onde o termo de pesquisa destacado foi encontrado.

* Compartilhe o catálogo por meio de mídia social; baixar o catálogo para exibir offline; habilite Favoritos para marcar os itens que deseja retornar rapidamente ou imprimir o catálogo.
* Navegue pelo catálogo usando o sumário ou a exibição de grade da página; página para frente ou para trás clicando na borda central de uma página.
* Aumente o zoom, reduza o zoom e o deslocamento para examinar os itens em uma página.
* Mova o ponteiro sobre uma região de página (chamada de Mapa de imagem) para ver uma janela pop-up com informações sobre um item.
* Clique em uma região da página para abrir uma nova página da Web com mais informações sobre um item.
* Escreva uma nota adesiva e anexe-à uma página do ecatalog.
* Toque em ícones do mapa de imagem para iniciar páginas da Web relacionadas ou painéis de informações em contexto.
* Use interações de gesto, incluindo pinçamento para aplicar zoom e deslizar para virar páginas.
* Pesquisar por palavra-chave para itens.

![O ecatalog quando ele procura os usuários. A) Página de abertura do ecatalog. B) O ecatalog foi movido para a página 2.](/help/assets/ec_cat_viewer_popup.png)

Para criar um ecatalog, normalmente você usa arquivos PDF de alta resolução criados no Adobe® Acrobat® ou em outro programa de impressão, mas também pode criar um ecatalog a partir de arquivos de imagem.

Como parte da criação do ecatalog, você pode organizar páginas ou páginas espelhadas de página na ordem escolhida. Você também pode declarar se deseja páginas únicas, páginas espelhadas duplas ou espelhamentos de várias páginas. É possível criar Mapas de imagem para regiões de página para que os visualizadores possam, por exemplo, clicar em uma área na página e abrir uma nova página em seu site. É possível gerenciar o texto de sobreposição que aparece usando as configurações do infopanel na tela do ecatalog. Você também pode configurar o ecatalog Viewer escolhendo entre mais de 100 opções de configuração diferentes. Você pode adaptar os recursos e a aparência do seu visualizador para seu público-alvo específico.

**Início rápido**

O Início rápido do ecatalog foi projetado para ajudá-lo a começar a usar rapidamente com o ecatalogs. Siga as etapas de 1 a 7. Depois de cada etapa é uma referência cruzada para um cabeçalho de tópico onde você pode encontrar mais informações.

**1. Fazer upload dos arquivos PDF**

Os arquivos Adobe PDF geralmente são a fonte de um ecatalog. Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. O Sistema de publicação Scene 7 detecta essas imagens e as converte usando um perfil de cores CMYK padrão. No entanto, talvez seja necessário fazer upload e usar um perfil de cores personalizado.

Clique em Carregar na barra de navegação global para começar a fazer upload de arquivos PDF ou imagens para o seu ecatalog. Você pode carregar arquivos de seu desktop ou via FTP; O FTP é recomendado se você estiver carregando muitos arquivos ou arquivos maiores que 100 MB.

Em Opções de PDF, a tela Carregar fornece opções para fazer upload de arquivos PDF com resolução correta e corrigir espaço de cores. Uma resolução de 150 pixels por polegada é recomendada. Você pode selecionar a opção Gerar automaticamente ecatalog para criar um ecatalog quando fizer upload de um arquivo PDF.

Consulte [Upload dos arquivos PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Criação de um ecatalog**

Crie o ecatalog selecionando arquivos PDF ou de imagem no Painel Procurar e clicando no botão Build e selecionando ecatalogs. A tela do ecatalog é aberta.

Na guia Ordenar páginas, selecione um botão Layout— 1 para cima, 2 para cima ou Personalizado— para escolher se deseja usar as páginas espelhadas únicas, duplas ou personalizadas. É possível reorganizar páginas ou páginas espelhadas arrastando-as ou, em um grande catálogo, escolhendo um nome de página no menu Mover para.

Para adicionar páginas, selecione uma pasta na Biblioteca de ativos e arraste arquivos PDF ou de imagem até a tela de Páginas de pedido. Em vez de números de página padrão, você pode fornecer nomes de página personalizados ou importar um grande número de nomes de página.

Clique no botão Salvar, insira um nome para o catálogo eletrônico, escolha uma pasta SPS para armazenamento e selecione o botão Salvar. Sempre que você alterar a ordem de páginas ou editar o catálogo eletrônico, salve as alterações clicando no botão Salvar.

Consulte [Criar um ecatalog](creating-ecatalog.md).

**3. Criar mapas de imagem**

Os Mapas de imagem adicionam outra dimensão a páginas do ecatalog. Um Mapa de imagem é uma região em uma página que fornece mais informações sobre um item. Quando os visualizadores rolam o ponteiro sobre um Mapa de imagem, eles veem uma descrição do item. Clicar em um Mapa de imagem ativa uma referência externa que abre uma nova página da Web, onde você pode aprender mais sobre um item.

Para criar um Mapa de imagem, abra a tela do ecatalog. Em seguida, vá para a guia Mapear páginas da tela ecatalog e desenhe o mapa com a ferramenta Mapa de imagem retangular ou com o Mapa de imagem de polígono. É possível ajustar a posição e o tamanho dos Mapas de imagem arrastando bordas do mapa com a ferramenta Deslocamento.

Depois de desenhar o Mapa de imagem, insira o endereço de URL para o qual você deseja ir ao clicar no Mapa de imagens. Também é possível inserir o texto de sobreposição que aparece quando você move seu ponteiro sobre o Mapa de imagem.

Consulte [Criar mapas de imagem do ecatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Usar mapas de imagem para incorporar mídia avançada em um ecatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

É possível configurar e gerenciar o texto do mapa de imagem usando as configurações do Painel Informações na tela do ecatalog.

Consulte [Gerenciamento do conteúdo do painel Informações](info-panel-content.md#managing-info-panel-content).

**4. Configuração das predefinições do visualizador do ecatalog**

Os usuários finais veem o ecatalog no Visualizador do ecatalog. Se for um administrador, você poderá configurar o ecatalog Viewer. Você pode alterar sua cor de contorno e selecionar uma nova «capa» para marcar o ecatalog. O Dynamic Media Classic vem com várias predefinições de «prática recomendada» do ecatalog Viewer. Você pode escolher uma dessas predefinições para exibir seus ecatalogs. Você também pode criar uma Predefinição do ecatalog Viewer se for um administrador.

Para criar uma Predefinição do visualizador do ecatalog, clique no botão Configuração na barra Navegação global e escolha Predefinições do visualizador. Em seguida, clique em Adicionar, escolha uma plataforma e escolha ecatalog &gt; Visualizador.

Consulte [Configuração das predefinições](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)do visualizador do ecatalog.

**5. Visualização de ecatalogs no Visualizador do ecatalog**

Predefinições do Visualizador do ecatalog determinam o estilo e o comportamento dos visualizadores ecatalog.

Para descobrir como as Predefinições do Visualizador do ecatalog exibem seu ecatalog, selecione o ecatalog no Painel Procurar e clique em Visualizar. A tela Visualizar é aberta no visualizador padrão.

Observe a orientação, o esquema de cores, a aparência dos controles de alteração de páginas e a aparência das páginas quando elas são viradas.

Consulte [Visualizar ecatalogs no Visualizador do ecatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publicar o ecatalog e pdfs associados**

Publicar seu ecatalog e o PDF associado a coloca em servidores de imagem do Dynamic Media para que possa ser entregue ao seu site e aplicativo. Como parte do processo de publicação, o Sistema de publicação Scene 7 ativa a sequência de caracteres do URL para o seu catálogo. Use este URL para chamar o ecatalog de Servidores de imagem do Dynamic Media a seu site ou aplicativo.

Depois de marcar seu ecatalog e PDF para publicação no Painel Procurar, selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na tela Publicar, clique em Iniciar publicação.

Consulte [Publicação do ecatalogs e pdfs associados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Vincular um ecatalog a uma página da Web**

O Dynamic Media Classic ativa a sequência de caracteres de chamada de URL necessária para exibir o ecatalog quando você o publica em servidores de imagem do Dynamic Media. É possível copiar essa sequência de caracteres de URL na tela Visualizar e no Painel Procurar (na exibição Detalhe) selecionando urls no painel. Depois de copiar a sequência de URL, ela fica disponível para seus sites e aplicativos.

Entre em contato com a sua equipe de TI para colocar o link para o ecatalog no lugar apropriado em sua página da Web. Quando os usuários clicarem no link, o ecatalog Viewer será exibido e os usuários poderão navegar em seu ecatalog.

Consulte [Vincular um ecatalog a uma página da Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
