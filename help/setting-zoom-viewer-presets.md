---
title: Configuração de predefinições do visualizador de zoom
seo-title: Configuração de predefinições do visualizador de zoom
description: 'null'
seo-description: Saiba como configurar as Predefinições do visualizador de zoom.
uuid: 202 d 80 cb -8282-45 d 4-89 e 8-942 c 8677 aa 93
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/zoom
discoiquuid: 5023 a 933-e 229-4 d 3 c -8 e 91-3 ac 5 e 9 f 4970 b
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuração de predefinições do visualizador de zoom{#setting-up-zoom-viewer-presets}

As predefinições do visualizador de zoom determinam o estilo, o comportamento e a aparência dos seus visualizadores de zoom. O Dynamic Media Classic oferece várias opções para personalizar e destacar Visualizadores. O Dynamic Media Classic vem com Predefinições de zoom padrão (rápidas), fly-out e personalizadas do visualizador. Se for um administrador, você poderá criar novas predefinições do Visualizador de zoom ou editar uma predefinição padrão e salvá-la com um novo nome.

Todos os visualizadores de zoom têm botões para aumentar, diminuir o zoom, deslocar e redefinir a imagem para seu estado original após o zoom. A aparência desses botões depende de sua escolha de Predefinições do visualizador de zoom. É possível configurar uma Predefinição do visualizador de zoom com diferentes cores, bordas, fontes e configurações de imagem. Ao configurar um Visualizador de zoom orientado, você também pode escolher onde colocar os destinos de zoom. Os destinos de zoom são as miniaturas que os usuários clicam para aplicar zoom às áreas especificadas.

## Sobre as predefinições do visualizador de zoom {#about-zoom-viewer-presets}

O Dynamic Media Classic oferece essas Predefinições do visualizador de zoom:

**Visualizador de zoom: Básico** Fornece um zoom básico na imagem original.

**Visualizador de zoom: Fly-out** Exibe uma segunda imagem da área ampliada ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção sobre a área que desejam visualizar.

Ao determinar o uso de largura de banda completo para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem em flyout é determinado pelo tamanho da imagem principal (Largura e altura do palco) e pelo fator de zoom. Para impedir que o tamanho do arquivo flyout fique muito grande, equilibre estes dois valores: se você tiver um tamanho de imagem principal grande, reduza o valor do fator de zoom. (A Largura Flyout e a Altura do Flyout determinam o tamanho da janela flyout, mas não o tamanho da imagem flyout que é servida no visualizador.)

Por exemplo, se o tamanho da imagem principal for de 350 em 350 pixels, com um fator de zoom igual a 3, a imagem resultante será de 1050 em 1050 pixels. Se o tamanho da imagem principal for de 300 em 300 pixels, com um fator de zoom de 4, a imagem flyout será de 1200 em 1200 pixels. Dependendo da configuração de qualidade JPEG (configurações recomendadas estão entre 80-90), é possível diminuir significativamente o tamanho do arquivo. Os fatores de zoom recomendados são de 2.5 a 4, dependendo do tamanho da imagem principal.

O Dynamic Media Classic recomenda esses parâmetros para predefinições de zoom de zoom:

**Tamanho da imagem ampliado** Aproximadamente 1500 em 1500 pixels, e não excede 2000 por 2000 pixels.

**Tamanho da imagem** 100 KB ou abaixo, não exceder 150 KB (compactar o arquivo para mantê-lo menos de 150 KB).

**Visualizador de zoom: Personalizado** fornece zoom centralizado ou não orientado com imagens, Conjuntos de imagens com várias exibições ou Conjuntos de amostras de cores.

## Criação e edição de predefinições do visualizador de zoom {#creating-and-editing-zoom-viewer-presets}

Siga estas etapas para criar ou editar uma Predefinição do visualizador de zoom:

1. Clique **em Configuração** &gt; **Predefinições do visualizador**.
1. Execute um dos procedimentos a seguir:

   **Criando uma predefinição** Clique em Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha um visualizador de zoom e clique em Adicionar. Digite um nome para a predefinição na caixa Nome predefinido.

   **Editar uma predefinição** Selecione uma predefinição do visualizador de zoom e clique **em Editar**.

1. Especifique as configurações conforme desejado.

   Para ver uma descrição de uma opção, clique no ícone Dica de informações adjacente à opção.

   A tela de visualização exibe o visualizador à medida que você atualiza e altera as configurações.

1. Clique **em Salvar** ou **Salvar como**.
1. Na tela Predefinições do visualizador, examine a Predefinição do visualizador de zoom ou Predefinição do visualizador guiada que você criou. Se precisar de ajuste, clique **em Editar**, altere as configurações na tela Configurar visualizador e clique **em Salvar**.

Para obter informações sobre como gerenciar Predefinições do visualizador na tela Predefinições do visualizador, consulte [Predefinições do visualizador](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Criação e edição de predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets)

