---
title: Exportar ativos do Adobe Dynamic Media Classic
description: Saiba como exportar ativos do Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:47:10.191Z'
TQID: 'https://experienceleague.adobe.com/wE2C1kA1I2fYIkXCqMvw-hPWIV5GMcj1Y0-dgkALyyc'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 425
ht-degree: 0%

---

# Exportar ativos do Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Você pode salvar ativos editados no Adobe Dynamic Media Classic em uma unidade de rede local. Os ativos exportados são incluídos em um arquivo ZIP para download ou envio por email.

O arquivo Zip compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação. Além disso, você tem permissão de um máximo de 500 ativos totais por trabalho de exportação.

O Adobe Dynamic Media Classic mantém um registro dos trabalhos de exportação na tela Trabalhos.

**Para exportar ativos do Adobe Dynamic Media Classic:**

1. Selecione os ativos que deseja exportar e vá para **[!UICONTROL File]** > **[!UICONTROL Export]**.
1. Na janela Exportar Assets Selecionado, clique em **[!UICONTROL Image Options]** e especifique qualquer uma das seguintes opções (os administradores determinam quais opções estão disponíveis para os usuários):

   * **[!UICONTROL Presets]**: como opção, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma Predefinição de imagem, as outras opções de formatação não estarão disponíveis, pois o ativo adota os formatos definidos pela Predefinição de imagem.

   * **[!UICONTROL Conversion]**: Converter o arquivo de ativo ou a imagem original.

   * **[!UICONTROL Size]**: Você pode selecionar um tamanho padrão. Ou você pode selecionar **[!UICONTROL Other]** na lista suspensa **[!UICONTROL Size]**, escolher a unidade de medida desejada e especificar a largura e a altura.

     Consulte também [Especificar opções de exportação disponíveis para usuários do Portal de Mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]**: Escolher um formato de imagem.

   * **[!UICONTROL Color]**: Escolha RGB, CMYK ou Cinza.

   * **[!UICONTROL Resolution]**: Escolha 72 ppi, 150 ppi ou 300 ppi.

   * **[!UICONTROL Job Name]**: você pode atribuir um nome de trabalho à exportação.

   * **[!UICONTROL Send Email To]**: Opcional. Insira um endereço de email se você pretende enviar os ativos por email. A mensagem de email lista o URL no qual o destinatário pode ir para baixar os ativos.

1. Selecione **[!UICONTROL Export]**.

São apoiadas três ações básicas de exportação:

* Arquivo original (exporte o arquivo original do ativo)
* Converter usando predefinição (use uma Predefinição de imagem para formatar o ativo)
* Converter sem predefinição (use a caixa de diálogo de exportação para especificar modificadores de imagem)

Os tipos de ativos a seguir não podem ser exportados. Todos os outros geram uma exportação.

* Conjuntos de imagem
* Conjuntos de renderização
* Conjuntos de rotação
* Conjuntos de mídia
* Conjuntos de taxa múltipla
* eCatalogs

Além disso, os modelos não podem ser exportados como um &quot;arquivo original&quot;.

Você pode usar a conversão para exportar os seguintes tipos de ativos:

* Imagens
* Modelos
* Imagens ajustadas
* PDF (gera páginas convertidas)
* PostScript®

O seguinte comportamento resulta da introdução no exportador de uma grande seleção de vários tipos de ativos:

* Todos os tipos de ativos que não podem ser exportados são removidos da lista antes do envio do trabalho
* Se uma conversão for solicitada, todos os tipos que podem ser convertidos serão, e todos os outros serão exportados como originais
