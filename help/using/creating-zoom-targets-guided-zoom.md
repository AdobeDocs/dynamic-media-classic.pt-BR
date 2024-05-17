---
title: Criar destinos de zoom para zoom guiado
description: Saiba como criar Destinos de zoom para zoom guiado no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Criar destinos de zoom para zoom guiado{#creating-zoom-targets-for-guided-zoom}

Os destinos de zoom orientam os visualizadores para determinadas partes de uma imagem. Além do zoom de forma livre, os visualizadores podem selecionar uma miniatura de destino de zoom e aplicar zoom à parte da imagem na qual você deseja que eles se concentrem. Os destinos de zoom são uma oportunidade para destacar as partes atraentes ou interessantes de uma imagem.

![Criar destinos de zoom para zoom guiado](/help/using/assets/zo_guided_zoom.png)

## Sobre as Metas de Zoom {#about-zoom-targets}

A porcentagem máxima de zoom dos Destinos de zoom é 100%. A porcentagem mínima de zoom varia com base em uma combinação do tamanho do visualizador e do tamanho da imagem, conforme mostrado nesta tabela:

| Tamanho da imagem | Tamanho do visualizador | Porcentagem de zoom |
| --- | --- | --- |
| Grande | Menor | Mínimo menor |
| Pequeno | Maior | Mínimo maior |

Você pode alterar o tamanho do Zoom Viewer para corresponder ao tamanho que está sendo usado em sua página da Web. Você pode alterar essa configuração permanentemente alterando o tamanho do visualizador na tela Configuração (se você for um administrador). Consulte [Configurar predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Criar e editar Destinos de Zoom {#creating-and-editing-zoom-targets}

Criar e editar Destinos de Zoom na tela Editor de Destino de Zoom. Para abrir essa tela, selecione uma imagem e siga um destes procedimentos:

* Selecione a sobreposição **[!UICONTROL Edit]** e escolha Destinos de zoom.
* No painel Procurar, exiba a imagem em **[!UICONTROL Detail View]** e selecione **[!UICONTROL Zoom Targets]**.

Na tela Editor de destino de zoom, selecione a **[!UICONTROL Select Target]** botão (seta) para selecionar um alvo antes de alterar seu tamanho ou posição. Para criar um destino de zoom na imagem, selecione **[!UICONTROL Add Targets]** (retângulo). A página Editor de destino de zoom também oferece ferramentas para excluir, copiar e nomear destinos de zoom.

### Criar um destino de zoom {#creating-a-zoom-target}

Para criar um destino de zoom, abra a página Editor do Destino de Zoom e faça o seguinte:

1. Selecionar **[!UICONTROL Add Targets]** (retângulo), mova o ponteiro sobre a imagem e selecione onde deseja que o destino de zoom esteja.

   Uma imagem em miniatura do destino de zoom é exibida no painel no lado direito da tela.

1. Escolher **[!UICONTROL Select Target]** (seta), selecione o destino de zoom criado e ajuste o tamanho e a posição do destino.

   * **Redimensionar**: mova o ponteiro sobre um canto do destino de zoom e arraste para aumentar ou reduzir o destino.

   * **Position**: Mova o ponteiro sobre o destino de zoom e arraste-o para um local diferente.

1. Digite um nome para o destino do zoom na caixa Nome.

   >[!NOTE]
   >
   >O que você digita na caixa Nome é mais do que um nome. Quando os usuários movem o ponteiro sobre o destino de zoom, eles veem o que você insere na caixa Nome. Insira uma breve descrição do destino do zoom na caixa Nome para que os usuários saibam o que podem ampliar.

1. Opcionalmente, informe os dados do usuário no campo Dados do Usuário. Este campo é para designers de sites adicionarem informações ao destino de zoom.
1. Selecionar **[!UICONTROL Save]**.

   As coordenadas e o nível de zoom do destino de zoom são salvos. Uma miniatura do destino de zoom com o nome inserido é exibida no lado direito da tela.

>[!NOTE]
>
>Para ver a aparência dos Destinos de zoom em um Visualizador de zoom, selecione a **[!UICONTROL Preview]** na tela Editor de destino de zoom. Em seguida, escolha um Visualizador de zoom na tela Visualizar. Para obter mais informações sobre essa tela, consulte [Visualizar imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar Destinos de Zoom {#editing-zoom-targets}

Para editar Destinos de Zoom, use as seguintes técnicas na página Editor de Destino de Zoom:

* **Reposicionar**: Com o botão Select Target (a seta), selecione o target. Em seguida, arraste o target para um local diferente.

* **Redimensionar**: Com o botão Select Target (a seta), selecione o target. Para ampliar ou reduzir o destino, mova o ponteiro sobre um canto do destino de zoom e arraste.

* **Excluir**: selecione a imagem da miniatura de destino no lado direito da tela. Em seguida, selecione **[!UICONTROL Delete Target]**.

* **Renomeando**: selecione a imagem da miniatura de destino no lado direito da tela. Em seguida, insira um nome no campo **[!UICONTROL Name]** e selecione **[!UICONTROL Save]**.

### Copiar Destinos de Zoom {#copying-zoom-targets}

É possível copiar Destinos de zoom de uma imagem para outra. Copiar destinos quando duas imagens apresentarem conteúdo semelhante e seus Destinos de zoom pertencerem aos mesmos locais. Para copiar Destinos de Zoom em outra imagem, faça o seguinte:

1. Abra a imagem com Destinos de Zoom que você deseja copiar na tela Editor de Destino de Zoom.
1. Selecionar **[!UICONTROL Copy Targets To]**.
1. Na caixa de diálogo Selecionar imagens, selecione uma imagem e escolha **[!UICONTROL Select]**.
