---
title: Fontes
description: Saiba como usar fontes no Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Fontes{#fonts}

Às vezes, o Dynamic Media Classic exige que você carregue um arquivo de fonte para inserir ou renderizar o texto em uma fonte específica. Por exemplo, para usar uma fonte específica para o texto em uma camada de modelo, faça upload do arquivo de fonte. Para exibir os números de página do Visualizador de catálogo eletrônico em uma fonte específica, faça upload do arquivo de fonte.

O Dynamic Media Classic é compatível com esses tipos de fonte:

* Todas as fontes TrueType
* Fontes PostScript®
* Fontes OpenType/TrueType
* Fontes OpenType/PostScript
* PhotoFonts

Depois que um arquivo de fonte for carregado, é possível alterar a ID do Dynamic Media Classic, o nome da fonte e digitar as informações na tela Editar informações .

>[!NOTE]
>
>O Dynamic Media Classic recomenda fazer o upload de todos os estilos de fonte (negrito, itálico, negrito/itálico e normal) se você planeja usar fontes em camadas de modelo. O Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. O upload de todos os arquivos PostScript/Adobe Type 1 associados a uma fonte também é recomendado, pois algumas dessas fontes contêm informações detalhadas de ajuste do espaço.

## Upload de arquivos de fonte {#uploading-font-files}

Faça upload de arquivos de fonte com as mesmas técnicas usadas para fazer upload de outros arquivos. Você pode armazenar arquivos de fontes em qualquer pasta do Dynamic Media Classic. Consulte [Fazer upload de seus arquivos](uploading-files.md#uploading_your_files).

## Edição de informações do arquivo de fonte {#editing-font-file-information}

É possível alterar o nome da ID de uma fonte e suas informações de tipo. Editar um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação de fontes.

No painel Procurar, selecione o arquivo de fonte que deseja editar na exibição Detalhes e escolha Arquivo > Editar informações. A tela Editar informações é aberta. Escolha as opções a seguir e selecione o botão Submit .

* **Nome da fonte**  - esse nome identifica a fonte quando é publicada.

* **Nome PostScript**  - Esse nome é o nome PostScript completo para a fonte. Normalmente, indica o peso ou o estilo.

* **Nome RTF**  - Esse nome aparece em um menu pop-up no editor RTF, onde as camadas de texto do modelo são criadas.

* **Nome da família da fonte**  - Esse nome lista o nome da fonte sem o indicador de estilo, peso ou tipo de fonte.

* **Estilo da fonte**  - As opções são Simples, Negrito, Itálico e Negrito-Itálico.

* **Tipo de fonte**  - as opções são TrueType e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

* **Abreviação do tipo de fonte**  - As opções são as seguintes:

   * **** Arquivos de fonte TTFTrueType usados para renderização de PDF/PostScript e veiculação de imagens.

   * **** Arquivos de fonte AFMAdobe PostScript que contêm informações de Métricas de fonte Adobe e são usados para exibição de imagens.

   * **** Arquivos de fonte PFMAdobe PostScript que contêm informações de métricas de fonte binária.

   * **** Arquivos de fonte PFBAdobe PostScript que contêm informações binárias sobre contorno de fonte e são usados para renderização de PDF/PostScript e veiculação de imagens.
