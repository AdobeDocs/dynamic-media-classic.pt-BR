---
title: Configuração das predefinições do visualizador de zoom
description: Saiba como configurar as Predefinições do visualizador de zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Visualizadores,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Configuração das predefinições do visualizador de zoom{#setting-up-zoom-viewer-presets}

As Predefinições do visualizador de zoom determinam o estilo, o comportamento e a aparência dos visualizadores de zoom. O Dynamic Media Classic oferece muitas opções para personalizar e aprimorar visualizadores. O Dynamic Media Classic vem com predefinições básicas (rápidas), de fly-out e de visualizador de zoom personalizado. Se você for um administrador, poderá criar Predefinições de visualizador de zoom da empresa ou editar uma predefinição padrão e salvá-la com um novo nome.

Todos os Visualizadores de zoom têm botões para aumentar, diminuir o zoom, diminuir o panorama e redefinir a imagem para o estado original após o zoom. A aparência desses botões e a forma como a janela em si será exibida dependem da escolha de Predefinições de visualizador de zoom. É possível configurar uma Predefinição do Visualizador de Zoom com cores, bordas, fontes e configurações de imagem diferentes. Ao configurar um Visualizador de zoom guiado, você também pode escolher onde colocar os destinos de zoom. Os direcionamentos de zoom são as miniaturas que os usuários clicam para aumentar o zoom para as áreas especificadas.

## Sobre predefinições do visualizador de zoom {#about-zoom-viewer-presets}

O Dynamic Media Classic oferece estas predefinições do visualizador de zoom:

* **Visualizador de zoom: Básico**  - Fornece um zoom básico na imagem original.

* **Visualizador de zoom: Fly-out**  - Exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção para a área que desejam visualizar.

Ao determinar o uso total da largura de banda para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem do flyout é determinado pelo tamanho da imagem principal (Largura e Altura do Palco) e pelo Fator de Zoom. Para impedir que o tamanho do arquivo flyout se torne muito grande, equilibre esses dois valores: se você tiver um tamanho de imagem principal grande, abaixe o valor de Fator de Zoom. (A Largura do Flyout e a Altura do Flyout determinam o tamanho da janela do flyout, mas não o tamanho da imagem do flyout que é servida no visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com um Fator de Zoom de 3, a imagem de flyout resultante será de 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de Zoom de 4, a imagem de flyout será de 1200 por 1200 pixels. Dependendo da configuração de qualidade JPEG (as configurações recomendadas estão entre 80 e 90), você pode diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

O Dynamic Media Classic recomenda os seguintes parâmetros para predefinições do visualizador de zoom de fly-out:

* **Tamanho da imagem ampliado**  - Aproximadamente 1500 por 1500 pixels, não deve exceder 2000 por 2000 pixels.

* **Tamanho da imagem**  - 100 KB ou menos, não deve exceder 150 KB (compacte o arquivo para mantê-lo abaixo de 150 KB).

* **Visualizador de zoom: Personalizado**  - Fornece zoom guiado ou não guiado com imagens, Conjuntos de imagens com várias exibições ou Conjuntos de amostras de cores.

## Criação e edição de predefinições do visualizador de zoom {#creating-and-editing-zoom-viewer-presets}

1. Na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Siga um destes procedimentos:

   * **Criação de uma predefinição**  - Clique em  **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha um visualizador de zoom e clique em **[!UICONTROL Add]**. Insira um nome para a predefinição na caixa Nome da predefinição .

   * **Editar uma predefinição**  - Selecione uma predefinição de visualizador de zoom e clique em  **[!UICONTROL Edit]**.

1. Especifique as configurações conforme desejado.

   Para ver uma descrição de uma opção, clique no ícone **[!UICONTROL Info Tip]** ao lado da opção .

   A página Visualização exibe o visualizador conforme você atualiza e altera as configurações.

1. Clique em **[!UICONTROL Save]** ou **[!UICONTROL Save As]**.
1. Na página Predefinições do visualizador , examine a Predefinição do visualizador de zoom ou a Predefinição do visualizador de zoom guiado que você criou. Se precisar de ajuste, clique em **[!UICONTROL Edit]**, altere as configurações na página Configurar Visualizador e clique em ****[!UICONTROL Save]****.

Para obter informações sobre o gerenciamento de Predefinições do visualizador na tela Predefinições do visualizador, consulte [Predefinições do visualizador](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Criação e edição de predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets)

