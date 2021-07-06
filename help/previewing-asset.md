---
title: Visualização de um ativo
description: Saiba como visualizar um ativo.
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Gerenciamento de ativos,Visualizadores
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Visualização de um ativo{#previewing-an-asset}

Você pode usar a Visualização para ver como um ativo digital aparece quando visualizado por um cliente. A Visualização usa o visualizador padrão atribuído ao ativo. Os visualizadores padrão são configurados na Configuração do aplicativo.

Consulte [Configuração de visualizadores padrão](application-setup.md#configuring_default_viewers).

Se você estiver visualizando um ativo de modelo com camadas de parâmetro, é possível alterar parâmetros ou alterar a predefinição de imagem. Como as alterações são feitas em linha, é possível exibir os resultados imediatamente na mesma janela de Visualização.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**Para visualizar um ativo:**

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo que você deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Grid View]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL List View]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Detail View]**.

1. Dependendo da exibição usada, siga um destes procedimentos:

   * Na janela Ativo da Exibição de Grade ou Exibição de Lista, selecione um único ativo e clique em **[!UICONTROL Preview]** próximo à imagem em miniatura.
   * Na barra de ferramentas acima da janela Ativos da Exibição de Grade, Exibição de Lista ou Exibição de Detalhes, clique em **[!UICONTROL Preview]**.

## Visualização de um ativo com base no tipo de plataforma do visualizador {#previewing-an-asset-based-on-viewer-platform-type}

Você pode usar a Lista de visualizadores para visualizar como um ativo aparece em um tipo específico de plataforma de visualizador, como o HTML5. Dependendo do tipo de ativo e do visualizador associado selecionado para visualização, nem todas as plataformas estarão disponíveis na Lista de visualizadores.

Você também pode usar a Lista de visualizadores para copiar o URL de um visualizador ou exibir e copiar o código do visualizador para incorporação em suas páginas da Web.

Para uma determinada plataforma de visualizador, a janela Lista de visualizadores permite que você veja visualmente quais dispositivos, como tablets e Smartphones, um visualizador está disponível para uso.

**Para visualizar um ativo com base no tipo de plataforma do visualizador:**

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo que você deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo e, em seguida, abaixo da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo e, à direita da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, clique em **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

1. (Opcional) Na janela Lista de visualizadores, clique no cabeçalho da coluna **[!UICONTROL Name]** ou **[!UICONTROL Platform type]** para classificar a coluna em ordem crescente ou decrescente.
1. Na janela Lista de visualizadores, na coluna Ações da tabela, clique em **[!UICONTROL Preview]** para ver como o ativo aparece para um visualizador e tipo de plataforma selecionados.

   Feche a visualização exibida.

1. (Opcional) Na janela Lista do visualizador, na lista suspensa Codificação de URL para Geração de URL de cópia na parte inferior, selecione a codificação de URL que deseja aplicar ao URL do ativo quando ele for copiado.
1. (Opcional) Siga um destes procedimentos:

   * Na janela Lista de visualizadores, na coluna Ações da tabela, clique em **[!UICONTROL Copy URL]** para um visualizador e tipo de plataforma selecionados.

      Ao clicar em **[!UICONTROL Copy URL]**, o URL associado é copiado automaticamente para a área de transferência.

   * Na janela Lista de visualizadores, na coluna Ações da tabela, clique em **[!UICONTROL Embed Code]**.

      Quando você clica em **[!UICONTROL Embed Code]**, a janela Código incorporado é aberta, onde você pode revisar o código do visualizador. A edição do código não é permitida na janela . Você também pode copiar o código para a área de transferência, para colá-lo em suas páginas da Web.

      Feche a visualização exibida.

1. No canto inferior direito da janela Lista de visualizadores, clique em **[!UICONTROL Close]** para retornar à tela Ativos.

## Visualização de um ativo de imagem com base em sua Predefinição de imagem {#previewing-an-image-asset-based-on-its-image-preset}

Você pode visualizar um ativo de imagem com base em sua predefinição de imagem para descobrir como é a imagem quando ela é entregue dinamicamente ao seu site ou aplicativo em diferentes tamanhos.

Uma predefinição de imagem é uma coleção de configurações predefinidas que alteram o tamanho, a qualidade da imagem, o formato, a resolução e outros aspectos da aparência de uma imagem quando ela é exportada.

Consulte [Configuração de predefinições de imagem](setting-image-presets.md#setting_up_image_presets).

Consulte [Criação e ativação de predefinições de imagem](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**Para visualizar um ativo de imagem com base em sua Predefinição de imagem:**

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem e, em seguida, abaixo da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, clique em **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, clique em **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. Na janela Lista de predefinições de imagens, na tabela, selecione o nome de um tipo predefinido cujo ativo de imagem você deseja visualizar em linha no painel direito.
1. (Opcional) Na janela Lista de predefinições de imagem, na lista suspensa **[!UICONTROL URL Encoding for Copy URL Generation]** na parte inferior, selecione a codificação de URL a ser aplicada ao URL do ativo de imagem quando ele for copiado.
1. (Opcional) Na janela Lista de predefinições de imagem, na área superior direita do painel de visualização, clique em **[!UICONTROL Copy URL]** para o tipo de predefinição selecionado.

   Ao clicar em **[!UICONTROL Copy URL]**, o URL associado é copiado automaticamente para a área de transferência.

1. No canto inferior direito da janela Lista de predefinições de imagens, clique em **[!UICONTROL Close]** para retornar à tela Ativos.
