---
title: Criação de metas de zoom para zoom guiado
description: Saiba como criar metas de zoom para o Zoom guiado.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# Criação de destinos de zoom para zoom guiado{#creating-zoom-targets-for-guided-zoom}

Os direcionamentos de zoom orientam seus visualizadores a determinadas partes de uma imagem. Além do zoom de forma livre, os visualizadores podem clicar em uma miniatura de destino de zoom e aplicar zoom na parte da imagem em que deseja que se concentrem. Os direcionamentos de zoom são uma oportunidade para que você destaque as partes atraentes ou interessantes de uma imagem.

![Criação de metas de zoom para zoom guiado](/help/assets/zo_guided_zoom.png)

## Sobre direcionamentos de zoom {#about-zoom-targets}

A porcentagem máxima de zoom dos destinos de zoom é de 100%. A porcentagem mínima de zoom varia com base em uma combinação do tamanho do visualizador e do tamanho da imagem, conforme mostrado nesta tabela:

| Tamanho da imagem | Tamanho do visualizador | Porcentagem de zoom |
|--- |--- |--- |
| Grande | Menor | Menor mínimo |
| Pequeno | Maior | Maior mínimo |

Você pode alterar o tamanho do Visualizador de Zoom para corresponder ao tamanho usado em sua página da Web. Para alterar essa configuração permanentemente, você pode alterar o tamanho do visualizador na tela Configuração (se você for um administrador). Consulte [Configuração das predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Criar e editar destinos de zoom {#creating-and-editing-zoom-targets}

Crie e edite metas de zoom na tela Editor de direcionamento de zoom . Para abrir esta tela, selecione uma imagem e siga um destes procedimentos:

* Clique no botão **[!UICONTROL Edit]** de sobreposição e escolha Metas de zoom.
* No Painel Procurar, exiba a imagem em **[!UICONTROL Detail View]** e clique em **[!UICONTROL Zoom Targets]**.

Na tela Editor de direcionamento de zoom, clique no botão **[!UICONTROL Select Target]** (seta) para selecionar um destino antes de alterar seu tamanho ou posição. Clique em **[!UICONTROL Add Targets]** (retângulo) para criar um direcionamento de zoom na imagem. A tela Editor de direcionamento de zoom também oferece ferramentas para excluir, copiar e nomear direcionamentos de zoom.

### Criação de um direcionamento de zoom {#creating-a-zoom-target}

Abra a tela Editor de direcionamento de zoom e siga estas etapas para criar um direcionamento de zoom:

1. Clique em **[!UICONTROL Add Targets]** (retângulo), mova o ponteiro sobre a imagem e clique no local em que deseja direcionar o zoom.

   Uma imagem em miniatura do destino de zoom aparece no painel no lado direito da tela.

1. Clique em **[!UICONTROL Select Target]** (seta), clique para selecionar o direcionamento de zoom que você criou e ajuste o tamanho e a posição do destino.

   * ****
RedimensionamentoMova o ponteiro sobre um canto do destino de zoom e arraste para aumentar ou diminuir o destino.

   * ****
PosicionamentoMova o ponteiro sobre o destino de zoom e arraste-o para um local diferente.

1. Digite um nome para o direcionamento de zoom na caixa Nome.

   >[!NOTE]
   >
   >O que você insere na caixa Nome é mais do que um nome. Quando os usuários movem o ponteiro sobre o destino de zoom, eles veem o que você insere na caixa Nome. Insira uma breve descrição do direcionamento de zoom na caixa Nome para que os usuários saibam o que podem ampliar.

1. Opcionalmente, informe os dados do usuário no campo Dados do Usuário. Este campo é para designers de sites da Web adicionarem informações ao direcionamento de zoom.
1. Clique em **[!UICONTROL Save]**.

   As coordenadas e o nível de zoom do destino de zoom são salvos. Uma miniatura do destino de zoom com o nome digitado é exibida no lado direito da tela.

>[!NOTE]
>
>Para ver a aparência dos destinos de zoom em um Visualizador de zoom, clique no botão Visualizar na tela Editor de direcionamento de zoom e escolha um Visualizador de zoom na tela Visualização. Para obter informações sobre essa tela, consulte [Visualização de imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar destinos de zoom {#editing-zoom-targets}

Use essas técnicas na tela Editor de direcionamento de zoom para editar metas de zoom:

* ****
Reposicionamento Com o botão Selecionar meta (a seta), clique no target para selecioná-lo. Em seguida, arraste o target para um local diferente.

* ****
Redimensionamento Com o botão Selecionar destino (a seta), clique no destino para selecioná-lo. Em seguida, mova o ponteiro sobre um canto do destino de zoom e arraste para aumentar ou diminuir o destino.

* ****
ExclusãoClique na imagem em miniatura do público-alvo no lado direito da tela. Em seguida, clique em **[!UICONTROL Delete Target]**.

* ****
RenomeaçãoClique na imagem em miniatura do público-alvo no lado direito da tela. Em seguida, insira um nome no campo de texto **[!UICONTROL Name]** e clique em **[!UICONTROL Save]**.

### Copiando destinos de zoom {#copying-zoom-targets}

Você pode copiar destinos de zoom de uma imagem para outra. Copie os destinos quando duas imagens apresentarem conteúdo semelhante e seus destinos de zoom pertencerem aos mesmos locais. Siga estas etapas para copiar os destinos de zoom para outra imagem:

1. Abra a imagem com direcionamentos de zoom que deseja copiar na tela Editor de direcionamento de zoom.
1. Clique em **[!UICONTROL Copy Targets To]**.
1. Na caixa de diálogo Selecionar imagens , selecione uma imagem e clique em **[!UICONTROL Select]**.

