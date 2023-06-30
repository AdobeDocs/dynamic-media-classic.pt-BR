---
title: Criar destinos de zoom para Zoom guiado
description: Saiba como criar destinos de zoom para Zoom guiado no Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Criar destinos de zoom para Zoom guiado{#creating-zoom-targets-for-guided-zoom}

Os destinos de zoom orientam os visualizadores para determinadas partes de uma imagem. Além do zoom de forma livre, os visualizadores podem selecionar uma miniatura de destino de zoom e aplicar zoom à parte da imagem na qual você deseja que eles se concentrem. Os destinos de zoom são uma oportunidade para destacar as partes atraentes ou interessantes de uma imagem.

![Criar destinos de zoom para Zoom guiado](/help/using/assets/zo_guided_zoom.png)

## Sobre destinos de zoom {#about-zoom-targets}

A porcentagem máxima de zoom dos destinos de zoom é de 100%. A porcentagem mínima de zoom varia com base em uma combinação do tamanho do visualizador e do tamanho da imagem, conforme mostrado nesta tabela:

| Tamanho da imagem | Tamanho do visualizador | Porcentagem de zoom |
| --- | --- | --- |
| Grande | Menor | Mínimo menor |
| Pequeno | Maior | Mínimo maior |

Você pode alterar o tamanho do Zoom Viewer para corresponder ao tamanho que está sendo usado em sua página da web. Para alterar essa configuração permanentemente, é possível alterar o tamanho do visualizador na tela Configuração (se você for um administrador). Consulte [Configurar predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Criar e editar destinos do zoom {#creating-and-editing-zoom-targets}

Criar e editar destinos de zoom na tela Editor de destino de zoom. Para abrir essa tela, selecione uma imagem e siga um destes procedimentos:

* Selecione a sobreposição **[!UICONTROL Edit]** e escolha Destinos de zoom.
* No painel Procurar, exiba a imagem em **[!UICONTROL Detail View]** e selecione **[!UICONTROL Zoom Targets]**.

Na tela Editor de destino de zoom, selecione **[!UICONTROL Select Target]** botão (seta) para selecionar um alvo antes de alterar seu tamanho ou posição. Para criar um destino de zoom na imagem, selecione **[!UICONTROL Add Targets]** (retângulo). A página Editor de destino de zoom também oferece ferramentas para excluir, copiar e nomear destinos de zoom.

### Criar um destino de zoom {#creating-a-zoom-target}

Para criar um destino de zoom, abra a página Editor do Destino de Zoom e faça o seguinte:

1. Selecionar **[!UICONTROL Add Targets]** (retângulo), mova o ponteiro sobre a imagem e selecione onde deseja que o destino de zoom esteja.

   Uma imagem em miniatura do destino de zoom é exibida no painel no lado direito da tela.

1. Escolher **[!UICONTROL Select Target]** (seta), selecione o destino de zoom criado e ajuste o tamanho e a posição do destino.

   * **Redimensionar** - Mova o ponteiro sobre um canto do destino de zoom e arraste para aumentar ou reduzir o destino.

   * **Position** - Mova o ponteiro sobre o destino de zoom e arraste-o para um local diferente.

1. Digite um nome para o destino do zoom na caixa Nome.

   >[!NOTE]
   >
   >O que você digita na caixa Nome é mais do que um nome. Quando os usuários movem o ponteiro sobre o destino de zoom, eles veem o que você insere na caixa Nome. Insira uma breve descrição do destino do zoom na caixa Nome para que os usuários saibam o que podem ampliar.

1. Opcionalmente, informe os dados do usuário no campo Dados do Usuário. Este campo é para designers de sites adicionarem informações ao destino de zoom.
1. Selecionar **[!UICONTROL Save]**.

   As coordenadas e o nível de zoom do destino de zoom são salvos. Uma miniatura do destino de zoom com o nome inserido é exibida no lado direito da tela.

>[!NOTE]
>
>Para ver a aparência dos seus destinos de zoom em um Visualizador de zoom, selecione a **[!UICONTROL Preview]** na tela Editor de destino de zoom e escolha um Visualizador de zoom na tela Visualizar. Para obter informações sobre essa tela, consulte [Visualizar imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar destinos de zoom {#editing-zoom-targets}

Para editar destinos de zoom, use as seguintes técnicas na página Editor de destino de zoom:

* **Reposicionar** - Com o botão Selecionar destino (a seta), selecione o destino. Em seguida, arraste o target para um local diferente.

* **Redimensionar** - Com o botão Selecionar destino (a seta), selecione o destino. Para ampliar ou reduzir o destino, mova o ponteiro sobre um canto do destino de zoom e arraste.

* **Excluir** - Selecione a imagem em miniatura do público alvo no lado direito da tela. Em seguida, selecione **[!UICONTROL Delete Target]**.

* **Renomeando** - Selecione a imagem em miniatura do público alvo no lado direito da tela. Em seguida, insira um nome no campo **[!UICONTROL Name]** e selecione **[!UICONTROL Save]**.

### Copiar destinos de zoom {#copying-zoom-targets}

É possível copiar destinos de zoom de uma imagem para outra. Copie destinos quando duas imagens apresentarem conteúdo semelhante e seus destinos de zoom pertencerem aos mesmos locais. Para copiar destinos de zoom para outra imagem, faça o seguinte:

1. Abra a imagem com os destinos de zoom que deseja copiar na tela Editor de destino de zoom.
1. Selecionar **[!UICONTROL Copy Targets To]**.
1. Na caixa de diálogo Selecionar imagens, selecione uma imagem e escolha **[!UICONTROL Select]**.
