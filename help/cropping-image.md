---
title: Recortar uma imagem
description: Saiba como recortar uma imagem no Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Recortar uma imagem{#cropping-an-image}

Você pode recortar imagens no Adobe Dynamic Media Classic. O sistema retém informações sobre imagens que foram cortadas para que você possa restaurá-las ao estado original. Também é possível recortar uma imagem e salvar a versão cortada com um novo nome.

Você pode recortar uma imagem para remover o espaço em branco ao seu redor ou recortar uma área da imagem.

>[!NOTE]
>
>Após cortar, você pode selecionar **[!UICONTROL Save As]** e salvar uma versão cortada da imagem com um nome diferente. Na janela Salvar como, selecione **[!UICONTROL Save As New Master]** para salvar uma segunda cópia da imagem. Selecione **[!UICONTROL Save As Addition View Of Master]** para que possa salvar o original e sua versão cortada com um nome diferente. Selecione **[!UICONTROL Replace Original]** para excluir o arquivo original do qual você cortou a imagem. Em seguida, insira um nome para a imagem e selecione **[!UICONTROL Submit]**.

## Recortar para remover o espaço em branco ao redor de uma imagem {#crop-to-remove-white-space-around-an-image}

Você pode cortar os pixels transparentes ou de cor sólida da borda de uma imagem.

1. Para recortar uma imagem, selecione seu botão **[!UICONTROL Edit]** sobreposto e selecione **[!UICONTROL Crop]**, ou exiba-o no Painel de navegação na Exibição de detalhes e selecione o botão **[!UICONTROL Crop]**.
1. Na página Editor de corte, siga um destes procedimentos:

   * Para aparar pixels de cor, vá para **[!UICONTROL Trim]** > **[!UICONTROL Color]**. Na caixa de diálogo **[!UICONTROL Auto Crop By Color]**, selecione o menu **[!UICONTROL Corner]** e escolha um canto com a cor de plano de fundo que deseja recortar. Em seguida, insira uma configuração **[!UICONTROL Tolerance]** de 0 a 1. A configuração 0 corta pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Os números mais próximos de 1 permitem mais diferenças de cor. Selecione **[!UICONTROL Crop]**.
   * Para aparar pixels transparentes, vá para **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. Na caixa de diálogo **[!UICONTROL Auto Crop By Transparency]**, insira uma configuração de tolerância de 0 a 1. A configuração 0 recorta pixels somente se forem transparentes. Os números mais próximos de 1 permitem mais transparência. Selecione **[!UICONTROL Crop]**.

1. Selecione **[!UICONTROL Save]**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de corte e selecione **[!UICONTROL Reset]**.

## Selecionar uma área para cortar {#select-an-area-to-crop}

1. Para recortar uma imagem, selecione seu botão **[!UICONTROL Edit]** sobreposto e escolha **[!UICONTROL Crop]**, ou exiba-o no Painel de navegação na Exibição de detalhes e selecione **[!UICONTROL Crop]**.

1. Na janela Editor de corte, coloque a parte da imagem que não deseja cortar na caixa de corte. O que aparece dentro da caixa é o que permanecerá depois que você selecionar **[!UICONTROL Save]** e cortar a imagem.
1. Para ajustar a área de corte, siga um destes procedimentos:

   * Arraste um lado ou canto da caixa. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma) da caixa de corte.
   * Insira medições de pixel nas caixas Tamanho.
   * Arraste para mover a caixa de corte. Mova o ponteiro para dentro do limite da caixa. Ao ver a seta de quatro pontas, arraste a caixa até um novo local na imagem.

1. Selecione **[!UICONTROL Save]**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de corte e selecione **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recortar espaço em branco de um arquivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recortar nas laterais das páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

