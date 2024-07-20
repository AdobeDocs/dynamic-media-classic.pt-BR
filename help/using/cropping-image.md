---
title: Cortar uma imagem
description: Saiba como cortar uma imagem no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Cortar uma imagem{#cropping-an-image}

Você pode recortar imagens na Adobe Dynamic Media Classic. O sistema retém informações sobre imagens que foram cortadas para que você possa restaurá-las ao seu estado original. Também é possível cortar uma imagem e salvar a versão cortada com um novo nome.

Você pode cortar uma imagem para remover um espaço em branco ao redor dela ou cortar uma área da imagem.

>[!NOTE]
>
>Após o recorte, você pode selecionar **[!UICONTROL Save As]** e salvar uma versão cortada da imagem com um nome diferente. Na janela Salvar como, selecione **[!UICONTROL Save As New Primary]** para salvar uma segunda cópia da imagem. Selecione **[!UICONTROL Save As Addition View Of Primary]** para poder salvar o original e sua versão cortada com um nome diferente. Selecione **[!UICONTROL Replace Original]** para excluir o arquivo original do qual cortou a imagem. Em seguida, digite um nome para a imagem e selecione **[!UICONTROL Submit]**.

## Recortar para remover o espaço em branco ao redor da imagem {#crop-to-remove-white-space-around-an-image}

Você pode cortar os pixels transparentes ou de cores sólidas da borda de uma imagem.

1. Para recortar uma imagem, selecione o botão de sobreposição **[!UICONTROL Edit]** e selecione **[!UICONTROL Crop]** ou exiba-a no painel Procurar do Modo de Exibição de Detalhes e selecione o botão **[!UICONTROL Crop]**.
1. Na página do Editor de corte, siga um destes procedimentos:

   * Para cortar pixels de cor, vá para **[!UICONTROL Trim]** > **[!UICONTROL Color]**. Na caixa de diálogo **[!UICONTROL Auto Crop By Color]**, selecione o menu **[!UICONTROL Corner]** e escolha um canto com a cor do plano de fundo que você deseja cortar. Em seguida, insira uma configuração de **[!UICONTROL Tolerance]** de 0 a 1. A configuração 0 recorta os pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Números próximos a 1 permitem mais diferença de cor. Selecione **[!UICONTROL Crop]**.
   * Para cortar pixels transparentes, vá para **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. Na caixa de diálogo **[!UICONTROL Auto Crop By Transparency]**, insira uma configuração de tolerância de 0 a 1. A configuração 0 corta os pixels somente se eles forem transparentes. Números mais próximos de 1 permitem mais transparência. Selecione **[!UICONTROL Crop]**.

1. Selecione **[!UICONTROL Save]**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de Recorte e selecione **[!UICONTROL Reset]**.

## Selecione uma área para cortar {#select-an-area-to-crop}

1. Para recortar uma imagem, selecione o botão de sobreposição **[!UICONTROL Edit]** e escolha **[!UICONTROL Crop]** ou exiba-a no painel Procurar do Modo de Exibição de Detalhes e selecione **[!UICONTROL Crop]**.

1. Na janela Editor de corte, coloque a parte da imagem que você não deseja cortar na caixa de corte. O que aparecer dentro da caixa é o que permanecerá após você selecionar **[!UICONTROL Save]** e recortar a imagem.
1. Para ajustar a área de corte, siga um destes procedimentos:

   * Arraste um lado ou canto da caixa. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantenha a proporção (a forma) da caixa de corte.
   * Insira medidas de pixel nas caixas Tamanho.
   * Arraste para mover a caixa de corte. Mova o ponteiro para dentro do limite da caixa. Ao visualizar a seta de quatro pontas, arraste a caixa para um novo local na imagem.

1. Selecione **[!UICONTROL Save]**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de Recorte e selecione **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Opções para edição de imagens no carregamento](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Cortar espaço em branco de um arquivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Cortar dos lados das páginas de PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)
