---
title: Visualizar um ativo
description: Saiba como visualizar um ativo no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 0%

---

# Visualizar um ativo{#previewing-an-asset}

Você pode usar a Visualização para ver como um ativo digital aparece quando visualizado por um cliente. A Visualização usa o visualizador padrão atribuído ao ativo. Os visualizadores padrão são configurados em Configuração do aplicativo.

Consulte [Configurar visualizadores padrão](application-setup.md#configuring_default_viewers).

Se você estiver visualizando um ativo de modelo com camadas de parâmetros, poderá alterar os parâmetros ou alterar a predefinição da imagem. Como as alterações são feitas em linha, é possível visualizar os resultados imediatamente na mesma janela de Pré-visualização.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**Para visualizar um ativo:**

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta Ativo que contém o ativo que deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL List View]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**.

1. Dependendo da exibição usada, execute um dos procedimentos a seguir:

   * Na janela Ativo da Exibição em Grade ou em Lista, selecione um único ativo e selecione **[!UICONTROL Preview]** próximo à imagem em miniatura.
   * Na barra de ferramentas acima da janela Ativos da Exibição em Grade, Exibição em Lista ou Exibição Detalhada, selecione **[!UICONTROL Preview]**.

## Visualizar um ativo com base no tipo de plataforma do visualizador {#previewing-an-asset-based-on-viewer-platform-type}

Você pode usar a Lista de visualizadores para visualizar como um ativo aparece em um tipo específico de plataforma do visualizador, como HTML5. Dependendo do tipo de ativo e do visualizador associado que você selecionou para visualização, nem todas as plataformas estão disponíveis na Lista do visualizador.

Você também pode usar a Lista de visualizadores para copiar o URL de um visualizador ou visualizá-lo e copiar o código do visualizador para incorporação nas páginas da Web.

Para determinada plataforma de visualização, a janela Lista de visualizadores permite ver visualmente quais dispositivos, como tablets e smartphones, um visualizador está disponível para uso.

**Para visualizar um ativo com base no tipo de plataforma do visualizador:**

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta Ativo que contém o ativo que deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo e, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

1. (Opcional) Na janela Lista de visualizadores, selecione o cabeçalho da coluna **[!UICONTROL Name]** ou **[!UICONTROL Platform type]** para classificar a coluna em ordem crescente ou decrescente.
1. Na janela Lista de visualizadores, na coluna Ações da tabela, selecione **[!UICONTROL Preview]** para ver como o ativo aparece para um visualizador e tipo de plataforma selecionados.

   Fechar a visualização exibida.

1. (Opcional) Na janela Lista de visualizadores, na lista suspensa Codificação de URL para geração de URL de cópia na parte inferior, selecione a codificação de URL a ser aplicada ao URL do ativo quando ele for copiado.
1. (Opcional) Siga qualquer um destes procedimentos:

   * Na janela Lista de visualizadores, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]** para um visualizador e tipo de plataforma selecionados.

     Ao selecionar **[!UICONTROL Copy URL]**, seu URL associado é copiado automaticamente para a área de transferência.

   * Na janela Lista de visualizadores, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

     Ao selecionar **[!UICONTROL Embed Code]**, a janela Código de inserção é aberta, onde você pode revisar o código do visualizador. A edição do código não é permitida na janela. Você também pode copiar o código para a área de transferência para poder colá-lo em suas páginas da Web.

     Fechar a visualização exibida.

1. No canto inferior direito da janela Lista de visualizadores, selecione **[!UICONTROL Close]** para retornar à tela Ativos.

## Visualizar um ativo de imagem com base em sua Predefinição de imagem {#previewing-an-image-asset-based-on-its-image-preset}

Você pode visualizar um ativo de imagem com base em sua Predefinição de imagem para descobrir como sua imagem será exibida quando for entregue dinamicamente ao seu site ou aplicativo em tamanhos diferentes.

Uma predefinição de imagem é uma coleção de configurações predefinidas que alteram o tamanho, a qualidade da imagem, o formato, a resolução e outros aspectos da aparência de uma imagem quando ela é exportada.

Consulte [Configurar predefinições da imagem](setting-image-presets.md#setting_up_image_presets).

Consulte [Criar e ativar predefinições de imagem](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**Para visualizar um ativo de imagem com base em sua Predefinição de imagem:**

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta Ativo que contém o ativo de imagem que deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem e, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. Na janela Lista de predefinições de imagem, na tabela, selecione o nome de um tipo de predefinição cujo ativo de imagem você deseja visualizar em linha no painel direito.
1. (Opcional) Na janela Lista de predefinições de imagens, no **[!UICONTROL URL Encoding for Copy URL Generation]** na parte inferior, selecione a codificação de URL a ser aplicada ao URL do ativo de imagem quando ele for copiado.
1. (Opcional) Na janela Lista de predefinições de imagens, na área superior direita do painel de visualização, selecione **[!UICONTROL Copy URL]** para o tipo de predefinição selecionado.

   Ao selecionar **[!UICONTROL Copy URL]**, seu URL associado é copiado automaticamente para a área de transferência.

1. No canto inferior direito da janela Lista de predefinições de imagens, selecione **[!UICONTROL Close]** para retornar à tela Ativos.
