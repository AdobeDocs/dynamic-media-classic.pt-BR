---
title: Configuração das predefinições do visualizador de zoom
description: Saiba como configurar as Predefinições do visualizador de zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# Configuração das predefinições do visualizador de zoom{#setting-up-zoom-viewer-presets}

As Predefinições do visualizador de zoom determinam o estilo, o comportamento e a aparência dos visualizadores de zoom. O Dynamic Media Classic oferece muitas opções para personalizar e aprimorar visualizadores. O Dynamic Media Classic vem com predefinições básicas (rápidas), de fly-out e de visualizador de zoom personalizado. Se você for um administrador, poderá criar novas Predefinições de Visualizador de Zoom da empresa ou editar uma predefinição padrão e salvá-la com um novo nome.

Todos os Visualizadores de zoom têm botões para aumentar, diminuir o zoom, diminuir o panorama e redefinir a imagem para o estado original após o zoom. A aparência desses botões e a aparência da janela dependem da escolha entre Predefinições de visualizador de zoom. É possível configurar uma Predefinição do Visualizador de Zoom com cores, bordas, fontes e configurações de imagem diferentes. Ao configurar um Visualizador de zoom guiado, você também pode escolher onde colocar os destinos de zoom. Os direcionamentos de zoom são as miniaturas que os usuários clicam para aumentar o zoom para as áreas especificadas.

## Sobre predefinições do visualizador de zoom {#about-zoom-viewer-presets}

O Dynamic Media Classic oferece estas predefinições do visualizador de zoom:

* **Visualizador de zoom:**
BásicoFornece um zoom básico na imagem original.

* **Visualizador de zoom: Fly-**
outExibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção para a área que desejam visualizar.

Ao determinar o uso total da largura de banda para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem do flyout é determinado pelo tamanho da imagem principal (Largura e Altura do Palco) e pelo Fator de Zoom. Para impedir que o tamanho do arquivo flyout se torne muito grande, equilibre esses dois valores: se você tiver um tamanho de imagem principal grande, abaixe o valor de Fator de Zoom. (A Largura do Flyout e a Altura do Flyout determinam o tamanho da janela do flyout, mas não o tamanho da imagem do flyout que é servida no visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com um Fator de Zoom de 3, a imagem de flyout resultante será de 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de Zoom de 4, a imagem de flyout será de 1200 por 1200 pixels. Dependendo da configuração de qualidade JPEG (as configurações recomendadas estão entre 80 e 90), você pode diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

O Dynamic Media Classic recomenda esses parâmetros para as Predefinições de visualizador de zoom de fly-out:

* **Ampliação do**
tamanho da imagemAproximadamente 1500 por 1500 pixels, sem exceder 2000 por 2000 pixels.

* **Tamanho da imagem**
de 100 KB ou menos, não deve exceder 150 KB (compacte o arquivo para mantê-lo abaixo de 150 KB).

* **Visualizador de zoom:**
PersonalizadoFornece zoom guiado ou não guiado com imagens, Conjuntos de imagens com várias exibições ou Conjuntos de amostras de cores.

## Criação e edição de predefinições do visualizador de zoom {#creating-and-editing-zoom-viewer-presets}

Siga estas etapas para criar ou editar uma Predefinição do Visualizador de Zoom:

1. Clique em **Configurar** > **Predefinições do visualizador**.
1. Siga um destes procedimentos:

   * **Criação de uma**
predefiniçãoClique em Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha um visualizador de zoom e clique em Adicionar. Insira um nome para a predefinição na caixa Nome da predefinição .

   * **Editar uma**
predefiniçãoSelecione uma predefinição do visualizador de zoom e clique em 
**Editar**.

1. Especifique as configurações conforme desejado.

   Para ver uma descrição de uma opção, clique no ícone Dica de informações adjacente à opção.

   A tela de visualização exibe o visualizador conforme você atualiza e altera as configurações.

1. Clique em **Salvar** ou **Salvar como**.
1. Na tela Predefinições do visualizador, examine a Predefinição do visualizador de zoom ou a Predefinição do visualizador de zoom guiado que você criou. Se precisar de ajuste, clique em **Editar**, altere as configurações na tela Configurar Visualizador e clique em **Salvar**.

Para obter informações sobre o gerenciamento de Predefinições do visualizador na tela Predefinições do visualizador, consulte [Predefinições do visualizador](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Criação e edição de predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets)

