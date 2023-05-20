---
title: Exportar ativos do Adobe Dynamic Media Classic
description: Saiba como exportar ativos do Adobe Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Exportar ativos do Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Você pode salvar ativos editados no Adobe Dynamic Media Classic em uma unidade de rede local. Os ativos exportados são incluídos em um arquivo ZIP para download ou envio por email.

O arquivo Zip compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação. Além disso, você tem permissão de um máximo de 500 ativos totais por trabalho de exportação.

O Adobe Dynamic Media Classic mantém um registro dos trabalhos de exportação na tela Trabalhos.

**Para exportar ativos do Adobe Dynamic Media Classic:**

1. Selecione os ativos que deseja exportar e vá para **[!UICONTROL File]** > **[!UICONTROL Export]**.
1. Na janela Exportar ativos selecionados, clique em **[!UICONTROL Image Options]** e, em seguida, especifique qualquer uma das seguintes opções (os administradores determinam quais opções estão disponíveis para os usuários):

   * **[!UICONTROL Presets]** - Opcionalmente, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma Predefinição de imagem, as outras opções de formatação não estarão disponíveis, pois o ativo adota os formatos definidos pela Predefinição de imagem.

   * **[!UICONTROL Conversion]** - Converta o arquivo de ativo ou a imagem original.

   * **[!UICONTROL Size]** - É possível selecionar um tamanho padrão. Ou você pode selecionar **[!UICONTROL Other]** do **[!UICONTROL Size]** escolha a unidade de medida desejada e especifique a largura e a altura.

      Consulte também [Especifique as opções de exportação disponíveis para os usuários do Portal de mídia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]** - Escolher um formato de imagem.

   * **[!UICONTROL Color]** - Escolha RGB, CMYK ou Cinza.

   * **[!UICONTROL Resolution]** - Escolha 72 ppi, 150 ppi ou 300 ppi.

   * **[!UICONTROL Job Name]** - Você pode atribuir um nome de trabalho à exportação.

   * **[!UICONTROL Send Email To]** - Opcionalmente, informe um endereço de e-mail se pretender enviar os ativos por e-mail. A mensagem de email lista o URL no qual o destinatário pode ir para baixar os ativos.

1. Selecionar **[!UICONTROL Export]**.

São apoiadas três ações básicas de exportação:

* Arquivo original (exporte o arquivo original do ativo)
* Converter usando predefinição (use uma predefinição de imagem para formatar o ativo)
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
