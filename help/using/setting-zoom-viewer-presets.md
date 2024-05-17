---
title: Configurar predefinições do visualizador de zoom
description: Saiba como configurar as Predefinições do visualizador de zoom no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Configurar predefinições do visualizador de zoom{#setting-up-zoom-viewer-presets}

As predefinições do visualizador de zoom determinam o estilo, o comportamento e a aparência dos visualizadores de zoom. O Adobe Dynamic Media Classic oferece muitas opções para personalizar e atribuir capa aos visualizadores. O Adobe Dynamic Media Classic vem com predefinições básicas (rápidas), de saída e personalizadas do visualizador de zoom. Se você for um administrador, poderá criar Predefinições do visualizador de zoom de empresa ou editar uma predefinição padrão e salvá-la com um novo nome.

Todos os Visualizadores de zoom têm botões para ampliar, reduzir, deslocar e redefinir a imagem para seu estado original após o zoom. A aparência desses botões e a forma como a janela é exibida dependem da escolha de Predefinições do visualizador de zoom. É possível configurar uma Predefinição do visualizador de zoom com diferentes cores, bordas, fontes e configurações de imagem. Ao configurar um Visualizador de zoom guiado, você também pode escolher onde colocar os Destinos de zoom. Os destinos de zoom são as miniaturas em que os usuários clicam para aplicar zoom nas áreas especificadas.

## Sobre as predefinições do visualizador de zoom {#about-zoom-viewer-presets}

O Adobe Dynamic Media Classic oferece estas Predefinições do visualizador de zoom:

* **Zoom Viewer: Basic**: fornece um zoom básico na imagem original.

* **Zoom Viewer: Fly-out**: exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção sobre a área que desejam visualizar.

Ao determinar o uso completo da largura de banda para esse visualizador, considere que tanto a imagem principal quanto a imagem suspensa são fornecidas no visualizador. O tamanho da imagem suspensa é determinado usando o tamanho da imagem principal (Largura e Altura do Palco) e o Fator de Zoom. Para evitar que o tamanho do arquivo de imagem suspensa fique muito grande, equilibre esses dois valores: se você tiver um tamanho grande de imagem principal, diminua o valor do Fator de zoom. (A Largura da imagem suspensa e a Altura da imagem suspensa determinam o tamanho da janela da imagem suspensa, mas não o tamanho da imagem suspensa que é exibida no visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com um Fator de Zoom de 3, a imagem suspensa resultante será 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de Zoom de 4, a imagem suspensa será de 1200 por 1200 pixels. Dependendo da configuração de qualidade do JPEG (as configurações recomendadas estão entre 80 e 90), é possível diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

O Adobe Dynamic Media Classic recomenda os seguintes parâmetros para as Predefinições do visualizador de zoom de saída:

* **Tamanho da imagem ampliado**: Aproximadamente 1500 por 1500 pixels, não devendo exceder 2000 por 2000 pixels.

* **Tamanho da imagem**: 100 KB ou menos, para não exceder 150 KB (compacte o arquivo para mantê-lo abaixo de 150 KB).

* **Visualizador de zoom: personalizado**: oferece zoom guiado ou não guiado com imagens, Conjuntos de imagens com várias exibições ou Conjuntos de amostras de cores.

## Criar e editar as predefinições do visualizador de zoom {#creating-and-editing-zoom-viewer-presets}

1. Na barra de Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Siga um destes procedimentos:

   * **Criar uma predefinição**: Selecionar **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha um visualizador de zoom e selecione **[!UICONTROL Add]**. Digite um nome para a predefinição na caixa Nome da predefinição.

   * **Editar uma predefinição**: selecione uma Predefinição do visualizador de zoom e, em seguida, selecione **[!UICONTROL Edit]**.

1. Especifique as configurações conforme desejado.

   Para ver uma descrição de uma opção, selecione a opção **[!UICONTROL Info Tip]** ícone ao lado da opção.

   A página Visualizar exibe o visualizador à medida que você atualiza e altera as configurações.

1. Selecionar **[!UICONTROL Save]** ou **[!UICONTROL Save As]**.
1. Na página Predefinições do visualizador, examine a Predefinição do visualizador de zoom ou a Predefinição do visualizador de zoom guiado que você criou. Se precisar de ajuste, selecione **[!UICONTROL Edit]**, alterar configurações no `Configure Viewer` e selecione **[!UICONTROL Save]**.

Para obter informações sobre o gerenciamento de Predefinições do visualizador na tela Predefinições do visualizador, consulte [Predefinições do visualizador](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Criar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets)
