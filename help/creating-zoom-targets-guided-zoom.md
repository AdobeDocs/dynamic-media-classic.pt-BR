---
title: Criação de públicos alvos de zoom para o zoom guiado
description: Saiba como criar públicos alvos de zoom para o Zoom guiado.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---


# Criação de públicos alvos de zoom para zoom guiado{#creating-zoom-targets-for-guided-zoom}

Públicos alvos de zoom guiam seus visualizadores para certas partes de uma imagem. Além do zoom de forma livre, os visualizadores podem clicar em uma miniatura do público alvo de zoom e aplicar zoom na parte da imagem que deseja que eles se concentrem. Públicos alvos de zoom são uma oportunidade para você destacar as partes interessantes ou atraentes de uma imagem.

![Criação de públicos alvos de zoom para o zoom guiado](/help/assets/zo_guided_zoom.png)

## Sobre públicos alvos de zoom {#about-zoom-targets}

A porcentagem máxima de zoom de públicos alvos de zoom é de 100%. A porcentagem mínima de zoom varia com base em uma combinação entre o tamanho do visualizador e o tamanho da imagem, conforme mostrado nesta tabela:

| Tamanho da imagem | Tamanho do visualizador | Porcentagem de zoom |
|--- |--- |--- |
| Grande | Menor | Menor mínimo |
| Pequeno | Maior | Mínimo maior |

Você pode alterar o tamanho do Visualizador de zoom para corresponder ao tamanho que está sendo usado em sua página da Web. Para alterar essa configuração permanentemente, você pode alterar o tamanho do visualizador na tela Configuração (se for um administrador). Consulte [Configuração das predefinições do visualizador de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Criação e edição de públicos alvos de zoom {#creating-and-editing-zoom-targets}

Crie e edite públicos alvos de zoom na tela Editor de Públicos alvos de zoom. Para abrir essa tela, selecione uma imagem e execute um dos procedimentos a seguir:

* Clique no botão de sobreposição **[!UICONTROL Edit]** e escolha Públicos alvos de zoom.
* No painel Procurar, exiba a imagem em **[!UICONTROL Detail View]** e clique em **[!UICONTROL Zoom Targets]**.

Na tela Editor de Públicos alvos de zoom, clique no botão **[!UICONTROL Select Target]** (seta) para selecionar um público alvo antes de alterar seu tamanho ou posição. Clique em **[!UICONTROL Add Targets]** (retângulo) para criar um público alvo de zoom na imagem. A tela Editor de zoom de Públicos alvos também oferta ferramentas para excluir, copiar e nomear públicos alvos de zoom.

### Criação de um público alvo de zoom {#creating-a-zoom-target}

Abra a tela Editor de zoom de Público alvo e siga estas etapas para criar um público alvo de zoom:

1. Clique em **[!UICONTROL Add Targets]** (retângulo), mova o ponteiro sobre a imagem e clique no local desejado para o público alvo de zoom.

   Uma imagem em miniatura do público alvo de zoom é exibida no painel do lado direito da tela.

1. Clique em **[!UICONTROL Select Target]** (seta), clique para selecionar o público alvo de zoom criado e ajuste o tamanho e a posição do público alvo.

   * ****
RedimensionamentoMova o ponteiro sobre um canto do público alvo de zoom e arraste para ampliar ou diminuir o público alvo.

   * ****
PosicionamentoMova o ponteiro sobre o público alvo de zoom e arraste-o para um local diferente.

1. Digite um nome para o público alvo de zoom na caixa Nome.

   >[!NOTE]
   >
   >O que você digita na caixa Nome é mais do que um nome. Quando os usuários movem o ponteiro sobre o público alvo de zoom, eles veem o que você digita na caixa Nome. Digite uma breve descrição do público alvo de zoom na caixa Nome para que os usuários saibam o que podem ampliar.

1. Opcionalmente, insira os dados do usuário no campo Dados do usuário. Este campo destina-se aos designers de sites da Web para adicionar informações ao público alvo de zoom.
1. Clique em **[!UICONTROL Save]**.

   As coordenadas e o nível de zoom do público alvo de zoom são salvos. Uma miniatura do público alvo de zoom com o nome digitado é exibida no lado direito da tela.

>[!NOTE]
>
>Para ver a aparência dos públicos alvos de zoom em um Visualizador de zoom, clique no botão Pré-visualização na tela Editor de Públicos alvos de zoom e escolha um Visualizador de zoom na tela de Pré-visualização. Para obter informações sobre essa tela, consulte [Visualizar imagens com visualizadores de zoom diferentes](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Edição de públicos alvos de zoom {#editing-zoom-targets}

Use essas técnicas na tela Editor de Públicos alvos de zoom para editar públicos alvos de zoom:

* ****
ReposicionamentoCom o botão Selecionar Público alvo (a seta), clique no público alvo para selecioná-lo. Em seguida, arraste o público alvo para um local diferente.

* ****
RedimensionamentoCom o botão Selecionar Público alvo (a seta), clique no público alvo para selecioná-lo. Em seguida, mova o ponteiro sobre um canto do público alvo de zoom e arraste para ampliar ou diminuir o público alvo.

* ****
ExclusãoClique na imagem em miniatura do público alvo no lado direito da tela. Em seguida, clique em **[!UICONTROL Delete Target]**.

* ****
RenomeaçãoClique na imagem em miniatura do público alvo no lado direito da tela. Em seguida, insira um nome no campo de texto **[!UICONTROL Name]** e clique em **[!UICONTROL Save]**.

### Copiando públicos alvos de zoom {#copying-zoom-targets}

É possível copiar públicos alvos de zoom de uma imagem para outra. Copie públicos alvos quando duas imagens apresentarem conteúdo semelhante e seus públicos alvos de zoom pertencerem aos mesmos locais. Siga estas etapas para copiar públicos alvos de zoom para outra imagem:

1. Abra a imagem com públicos alvos de zoom que deseja copiar na tela Editor de Públicos alvos de zoom.
1. Clique em **[!UICONTROL Copy Targets To]**.
1. Na caixa de diálogo Selecionar imagens, selecione uma imagem e clique em **[!UICONTROL Select]**.

