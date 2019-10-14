---
title: Criação de metas de zoom para o zoom guiado
seo-title: Criação de metas de zoom para o zoom guiado
description: nulo
seo-description: Saiba como criar metas de zoom para o Zoom guiado.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6ff0141d1e8e96278b95f61c00602780984aaf67

---


# Criação de metas de zoom para o zoom guiado{#creating-zoom-targets-for-guided-zoom}

Os direcionamentos de zoom orientam seus visualizadores para determinadas partes de uma imagem. Além do zoom de forma livre, os visualizadores podem clicar em uma miniatura de destino de zoom e aplicar zoom na parte da imagem que deseja que eles se concentrem. Os direcionamentos de zoom são uma oportunidade para você destacar as partes atraentes ou interessantes de uma imagem.

![Criação de metas de zoom para o zoom guiado](/help/assets/zo_guided_zoom.png)

## Sobre direcionamentos de zoom {#about-zoom-targets}

A porcentagem máxima de zoom dos alvos é de 100%. A porcentagem mínima de zoom varia com base em uma combinação entre o tamanho do visualizador e o tamanho da imagem, conforme mostrado nesta tabela:

| Tamanho da imagem | Tamanho do visualizador | Porcentagem de zoom |
|--- |--- |--- |
| Grande | Menor | Menor mínimo |
| Pequeno | Maior | Mínimo maior |

Você pode alterar o tamanho do Visualizador de zoom para corresponder ao tamanho que está sendo usado em sua página da Web. Para alterar essa configuração permanentemente, você pode alterar o tamanho do visualizador na tela Configuração (se for um administrador). Consulte [Configuração das predefinições](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)do visualizador de zoom.

## Criação e edição de direcionamentos de zoom {#creating-and-editing-zoom-targets}

Crie e edite os direcionamentos de zoom na tela Editor de direcionamento de zoom. Para abrir essa tela, selecione uma imagem e execute um dos procedimentos a seguir:

* Clique no **[!UICONTROL Edit]** botão de sobreposição e escolha Zoom em Metas.
* No painel Procurar, exiba a imagem em **[!UICONTROL Detail View]** e clique em **[!UICONTROL Zoom Targets]**.

Na tela Editor de metas de zoom, clique no **[!UICONTROL Select Target]** botão (seta) para selecionar uma meta antes de alterar seu tamanho ou posição. Clique **[!UICONTROL Add Targets]** (retângulo) para criar um destino de zoom na imagem. A tela Editor de direcionamento de zoom também oferece ferramentas para excluir, copiar e nomear direcionamentos de zoom.

### Criação de uma meta de zoom {#creating-a-zoom-target}

Abra a tela Editor de direcionamento de zoom e siga estas etapas para criar um direcionamento de zoom:

1. Clique **[!UICONTROL Add Targets]** (retângulo), mova o ponteiro sobre a imagem e clique no local desejado para o destino de zoom.

   Uma imagem em miniatura do destino de zoom aparece no painel no lado direito da tela.

1. Clique **[!UICONTROL Select Target]** (seta), clique para selecionar a meta de zoom criada e ajuste o tamanho e a posição da meta.

   * **Redimensionamento** Mova o ponteiro sobre um canto do destino de zoom e arraste para ampliar ou diminuir o destino.

   * **Posicionamento** Mova o ponteiro sobre o destino de zoom e arraste-o para um local diferente.

1. Digite um nome para o alvo de zoom na caixa Nome.

   >[!NOTE]
   >
   >O que você digita na caixa Nome é mais do que um nome. Quando os usuários movem o ponteiro sobre a meta de zoom, eles veem o que você insere na caixa Nome. Digite uma breve descrição do alvo de zoom na caixa Nome para que os usuários saibam o que podem ampliar.

1. Opcionalmente, insira os dados do usuário no campo Dados do usuário. Este campo destina-se a designers de sites da Web que adicionem informações à meta de zoom.
1. Click **[!UICONTROL Save]**.

   As coordenadas e o nível de zoom do destino de zoom são salvos. Uma miniatura do destino de zoom com o nome digitado é exibida no lado direito da tela.

>[!NOTE]
>
>Para ver a aparência dos seus direcionamentos de zoom em um Visualizador de zoom, clique no botão Visualizar na tela Editor de direcionamento de zoom e escolha um Visualizador de zoom na tela Visualizar. Para obter informações sobre essa tela, consulte [Visualizar imagens com visualizadores](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)de zoom diferentes.

### Editar metas de zoom {#editing-zoom-targets}

Use essas técnicas na tela Editor de direcionamento de zoom para editar direcionamentos de zoom:

* **Reposicionamento** Com o botão Selecionar destino (a seta), clique no destino para selecioná-lo. Em seguida, arraste o destino para um local diferente.

* **Redimensionamento** Com o botão Selecionar destino (a seta), clique no destino para selecioná-lo. Em seguida, mova o ponteiro sobre um canto do destino de zoom e arraste para ampliar ou diminuir o destino.

* **Excluindo** Clique na imagem em miniatura do destino no lado direito da tela. Em seguida, clique em **[!UICONTROL Delete Target]**.

* **Renomeação** Clique na imagem em miniatura do destino, no lado direito da tela. Em seguida, insira um nome no campo de **[!UICONTROL Name]** texto e clique em **[!UICONTROL Save]**.

### Copiando direcionamentos de zoom {#copying-zoom-targets}

É possível copiar destinos de zoom de uma imagem para outra. Copie destinos quando duas imagens apresentam conteúdo semelhante e seus destinos de zoom pertencem aos mesmos locais. Siga estas etapas para copiar destinos de zoom para outra imagem:

1. Abra a imagem com direcionamentos de zoom que deseja copiar na tela Editor de direcionamento de zoom.
1. Click **[!UICONTROL Copy Targets To]**.
1. Na caixa de diálogo Selecionar imagens, selecione uma imagem e clique em **[!UICONTROL Select]**.

