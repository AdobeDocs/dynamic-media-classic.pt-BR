---
title: Configuração das predefinições do Visualizador de zoom
seo-title: Configuração das predefinições do Visualizador de zoom
description: nulo
seo-description: Saiba como configurar as Predefinições do visualizador de zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Configuração das predefinições do Visualizador de zoom{#setting-up-zoom-viewer-presets}

As predefinições do visualizador de zoom determinam o estilo, o comportamento e a aparência dos visualizadores de zoom. O Dynamic Media Classic oferece várias opções para personalizar e aprimorar visualizadores. O Dynamic Media Classic é fornecido com predefinições básicas (rápidas), fly-out e personalizadas do Visualizador de zoom. Se você for um administrador, poderá criar novas predefinições do visualizador de zoom da empresa ou editar uma predefinição padrão e salvá-la com um novo nome.

Todos os Visualizadores de zoom têm botões para aumentar o zoom, diminuir o zoom, diminuir o deslocamento e redefinir a imagem para seu estado original após o zoom. A aparência desses botões e a aparência da janela depende da escolha das Predefinições do visualizador de zoom. Você pode configurar uma Predefinição do visualizador de zoom com cores, bordas, fontes e configurações de imagem diferentes. Ao configurar um Visualizador de zoom guiado, você também pode escolher onde colocar os direcionamentos de zoom. Os direcionamentos de zoom são as miniaturas que os usuários clicam para aplicar zoom nas áreas especificadas.

## Sobre as predefinições do visualizador de zoom {#about-zoom-viewer-presets}

O Dynamic Media Classic oferece as seguintes predefinições do visualizador de zoom:

* **Visualizador de zoom: Básico** Fornece um zoom básico na imagem original.

* **Visualizador de zoom: Reverter** Exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção para a área que desejam visualizar.

Ao determinar o uso total da largura de banda para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem do flyout é determinado pelo tamanho da imagem principal (Largura e Altura do Palco) e pelo Fator de Zoom. Para impedir que o tamanho do arquivo de menu suspenso se torne muito grande, equilibre estes dois valores: se você tiver um tamanho de imagem principal grande, abaixe o valor do Fator de zoom. (A Largura do Flyout e a Altura do Flyout determinam o tamanho da janela do flyout, mas não o tamanho da imagem do flyout fornecida para o visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com o Fator de zoom de 3, a imagem de flyout resultante será de 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de zoom de 4, a imagem de flyout será de 1200 por 1200 pixels. Dependendo da configuração de qualidade JPEG (as configurações recomendadas estão entre 80 e 90), é possível diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

O Dynamic Media Classic recomenda estes parâmetros para predefinições de zoom do visualizador de fly-out:

* **Tamanho** de imagem ampliado Aproximadamente 1500 por 1500 pixels, não excedendo 2000 por 2000 pixels.

* **Tamanho** de imagem igual ou inferior a100KB, não deve exceder 150KB (compacte o arquivo para mantê-lo abaixo de 150KB).

* **Visualizador de zoom: Personalizado** Fornece zoom guiado ou não guiado com imagens, Conjuntos de imagens com várias exibições ou Conjuntos de amostras de cores.

## Criação e edição de predefinições do Visualizador de zoom {#creating-and-editing-zoom-viewer-presets}

Siga estas etapas para criar ou editar uma predefinição do visualizador de zoom:

1. Clique em **Configuração** &gt; Predefinições **do visualizador**.
1. Execute um dos procedimentos a seguir:

   * **Criação de uma predefinição** Clique em Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha um Visualizador de zoom e clique em Adicionar. Digite um nome para a predefinição na caixa Nome da predefinição.

   * **Editando uma predefinição** Selecione uma predefinição de visualizador de zoom e clique em **Editar**.

1. Especifique as configurações conforme desejado.

   Para ver uma descrição de uma opção, clique no ícone Dica de informações adjacente à opção.

   A tela de visualização exibe o visualizador à medida que você atualiza e altera as configurações.

1. Clique em **Salvar** ou **Salvar como**.
1. Na tela Predefinições do visualizador, examine a predefinição do visualizador de zoom ou a predefinição do visualizador de zoom guiado que você criou. Se precisar de ajuste, clique em **Editar**, altere as configurações na tela Configurar visualizador e clique em **Salvar**.

Para obter informações sobre como gerenciar predefinições do visualizador na tela Predefinições do visualizador, consulte Predefinições [do visualizador](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Criação e edição de predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets)

