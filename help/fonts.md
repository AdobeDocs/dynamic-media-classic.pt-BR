---
title: Fontes
description: Saiba como usar fontes no Adobe Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Fontes{#fonts}

Às vezes, o Adobe Dynamic Media Classic exige que você carregue um arquivo de fonte para inserir ou renderizar texto em uma fonte específica. Por exemplo, para usar uma fonte específica para texto em uma camada de modelo, faça upload do arquivo de fonte. Para exibir os números de página do Visualizador de eCatalog em uma fonte específica, faça upload do arquivo de fonte.

O Adobe Dynamic Media Classic é compatível com estes tipos de fonte:

* Todas as fontes TrueType
* PostScript® fonts
* fontes OpenType/TrueType
* Fontes OpenType/PostScript
* PhotoFonts

Depois que um arquivo de fonte for carregado, você poderá alterar sua Adobe Dynamic Media Classic ID, o nome da fonte e digitar as informações na tela Editar informações.

>[!NOTE]
>
>O Adobe Dynamic Media Classic recomenda fazer upload de todos os estilos de fonte (negrito, itálico, negrito/itálico e regular) se você planeja usar fontes nas camadas de modelo. O Adobe Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. O upload de todos os arquivos PostScript/Adobe Type associados a uma fonte também é recomendado porque algumas dessas fontes contêm informações detalhadas de kerning.

## Fazer upload de arquivos de fonte {#uploading-font-files}

Fazer upload de arquivos de fonte com as mesmas técnicas usadas para fazer upload de outros arquivos. Você pode armazenar arquivos de fontes em qualquer pasta da Adobe Dynamic Media Classic. Consulte [Carregamento de arquivos](uploading-files.md#uploading_your_files).

## Editar informações do arquivo de fontes {#editing-font-file-information}

Você pode alterar o nome da ID de uma fonte e suas informações de tipo. A edição de um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação das fontes.

No Painel de navegação, selecione o arquivo de fonte que deseja editar na Exibição de detalhes e escolha Arquivo > Editar informações. A tela Editar informações é aberta. Escolha as seguintes opções e selecione **[!UICONTROL Submit]**.

* **[!UICONTROL Font Name]** - Esse nome identifica a fonte quando ela é publicada.

* **[!UICONTROL PostScript Name]** - Esse é o nome PostScript completo da fonte. Normalmente, indica o peso ou estilo.

* **[!UICONTROL RTF Name]** - Esse nome aparece em um menu pop-up no editor RTF, onde as camadas de texto do modelo são criadas.

* **[!UICONTROL Font Family Name]** - Esse nome lista o nome da fonte sem o estilo, peso ou indicador de tipo de fonte.

* **[!UICONTROL Font Style]** - As opções são Plain (Comum), Bold (Negrito), Italic (Itálico) e Bold-Italic (Negrito-Itálico).

* **[!UICONTROL Font Type]** - As opções são TrueType e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

* **[!UICONTROL Font Type Abbreviation]** - As opções são as seguintes:

   * **[!UICONTROL TTF]** - Arquivos de fontes TrueType usados para renderização de PDF/PostScript e fornecimento de imagens.

   * **[!UICONTROL AFM]** - Arquivos de fontes do Adobe PostScript que contêm informações de Métricas de fontes do Adobe e são usados para veiculação de imagens.

   * **[!UICONTROL PFM]** - Arquivos de fontes do Adobe PostScript que contêm informações de métricas de fontes binárias.

   * **[!UICONTROL PFB]** - Arquivos de fontes Adobe PostScript que contêm informações binárias de contorno de fontes e são usados para renderização de PDF/PostScript e fornecimento de imagens.
