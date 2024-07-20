---
title: Fontes
description: Saiba como usar fontes no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Fontes{#fonts}

Às vezes, o Adobe Dynamic Media Classic exige que você carregue um arquivo de fonte para inserir ou renderizar texto em uma fonte específica. Por exemplo, para usar uma fonte específica para texto em uma camada de modelo, faça upload do arquivo de fonte. Para exibir os números de página do Visualizador de eCatalog em uma fonte específica, faça upload do arquivo de fonte.

O Adobe Dynamic Media Classic é compatível com estes tipos de fonte:

* Todas as fontes TrueType
* PostScript® fonts
* fontes OpenType/TrueType
* Fontes do OpenType/PostScript
* PhotoFonts

Depois que um arquivo de fonte for carregado, você poderá alterar sua Adobe Dynamic Media Classic ID, o nome da fonte e digitar as informações na tela Editar informações.

>[!NOTE]
>
>O Adobe Dynamic Media Classic recomenda fazer upload de todos os estilos de fonte (negrito, itálico, negrito/itálico e regular) se você planeja usar fontes nas camadas de modelo. O Adobe Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. Também é recomendável carregar todos os `PostScript/Adobe Type1` arquivos associados a uma fonte, pois algumas dessas fontes contêm informações detalhadas de kerning.

## Fazer upload de arquivos de fonte {#uploading-font-files}

Fazer upload de arquivos de fonte com as mesmas técnicas usadas para fazer upload de outros arquivos. Você pode armazenar arquivos de fontes em qualquer pasta da Adobe Dynamic Media Classic. Consulte [Carregando seus arquivos](uploading-files.md#uploading_your_files).

## Editar informações do arquivo de fontes {#editing-font-file-information}

Você pode alterar o nome da ID de uma fonte e suas informações de tipo. A edição de um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação das fontes.

No painel Procurar, selecione o arquivo de fonte que deseja editar na Exibição de detalhes e escolha Arquivo > Editar informações. A tela Editar informações é aberta. Escolha as opções a seguir e selecione **[!UICONTROL Submit]**.

* **[!UICONTROL Font Name]**: Este nome identifica a fonte quando ela é publicada.

* **[!UICONTROL PostScript Name]**: este é o nome completo do PostScript para a fonte. Normalmente, indica o peso ou estilo.

* **[!UICONTROL RTF Name]**: esse nome aparece em um menu pop-up no editor RTF onde as camadas de texto do modelo são criadas.

* **[!UICONTROL Font Family Name]**: este nome lista o nome da fonte sem o indicador style, weight ou font-type.

* **[!UICONTROL Font Style]**: As opções são Simples, Negrito, Itálico e Negrito-Itálico.

* **[!UICONTROL Font Type]**: As opções são TrueType e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

* **[!UICONTROL Font Type Abbreviation]**: As opções são as seguintes:

   * **[!UICONTROL TTF]**: arquivos de fonte TrueType usados para renderização de PDF/PostScript e fornecimento de imagens.

   * **[!UICONTROL AFM]**: arquivos de fontes do Adobe PostScript que contêm informações de Métricas de Fontes do Adobe e são usados para veiculação de imagens.

   * **[!UICONTROL PFM]**: arquivos de fontes do Adobe PostScript que contêm informações de métricas de fontes binárias.

   * **[!UICONTROL PFB]**: arquivos de fontes Adobe PostScript que contêm informações binárias de contorno de fontes e são usados para renderização de PDF/PostScript e veiculação de imagens.
