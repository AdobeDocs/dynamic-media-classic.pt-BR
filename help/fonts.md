---
title: Fontes
description: Saiba como usar fontes no Adobe Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Fontes{#fonts}

Às vezes, o Adobe Dynamic Media Classic exige que você faça o upload de um arquivo de fonte para inserir ou renderizar o texto em uma fonte específica. Por exemplo, para usar uma fonte específica para o texto em uma camada de modelo, faça upload do arquivo de fonte. Para exibir os números de página do Visualizador de catálogo eletrônico em uma fonte específica, faça upload do arquivo de fonte.

O Adobe Dynamic Media Classic é compatível com esses tipos de fonte:

* Todas as fontes TrueType
* Fontes PostScript®
* Fontes OpenType/TrueType
* Fontes OpenType/PostScript
* PhotoFonts

Depois que um arquivo de fonte for carregado, é possível alterar o Adobe Dynamic Media Classic ID, o nome da fonte e digitar as informações na tela Editar informações.

>[!NOTE]
>
>O Adobe Dynamic Media Classic recomenda o upload de todos os estilos de fonte (negrito, itálico, negrito/itálico e regular) se você planeja usar fontes em camadas de modelo. O Adobe Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. O upload de todos os arquivos PostScript/Adobe Type1 associados a uma fonte também é recomendado, pois algumas dessas fontes contêm informações detalhadas de ajuste do espaço.

## Upload de arquivos de fonte {#uploading-font-files}

Faça upload de arquivos de fonte com as mesmas técnicas usadas para fazer upload de outros arquivos. Você pode armazenar arquivos de fontes em qualquer pasta do Adobe Dynamic Media Classic. Consulte [Fazer upload de seus arquivos](uploading-files.md#uploading_your_files).

## Editar informações do arquivo de fonte {#editing-font-file-information}

É possível alterar o nome da ID de uma fonte e suas informações de tipo. Editar um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação de fontes.

No Painel Procurar, selecione o arquivo de fonte que deseja editar na Exibição de detalhes e escolha Arquivo > Editar informações. A tela Editar informações é aberta. Escolha as opções a seguir e selecione **[!UICONTROL Submit]**.

* **[!UICONTROL Font Name]** - Esse nome identifica a fonte quando é publicada.

* **[!UICONTROL PostScript Name]** - Esse nome é o nome completo do PostScript para a fonte. Normalmente, indica o peso ou o estilo.

* **[!UICONTROL RTF Name]** - Esse nome aparece em um menu pop-up no editor RTF, onde as camadas de texto do modelo são criadas.

* **[!UICONTROL Font Family Name]** - Esse nome lista o nome da fonte sem o indicador de estilo, peso ou tipo de fonte.

* **[!UICONTROL Font Style]** - As opções são Simples, Negrito, Itálico e Negrito-Itálico.

* **[!UICONTROL Font Type]** - As opções são TrueType e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

* **[!UICONTROL Font Type Abbreviation]** - As opções são as seguintes:

   * **[!UICONTROL TTF]** - Arquivos de fonte TrueType usados para renderização de PDF/PostScript e exibição de imagens.

   * **[!UICONTROL AFM]** - Arquivos de fonte Adobe PostScript que contêm informações de Métricas de fonte do Adobe e são usados para exibição de imagens.

   * **[!UICONTROL PFM]** - Arquivos de fonte Adobe PostScript que contêm informações de métrica de fonte binária.

   * **[!UICONTROL PFB]** - Arquivos de fonte Adobe PostScript que contêm informações binárias sobre contorno de fonte e são usados para renderização de PDF/PostScript e veiculação de imagens.
