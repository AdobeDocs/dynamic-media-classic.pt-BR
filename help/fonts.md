---
title: Fontes
seo-title: Fontes
description: nulo
seo-description: Saiba como usar fontes no Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Fontes{#fonts}

Em alguns casos, o Dynamic Media Classic exige o upload de um arquivo de fonte para inserir ou renderizar o texto em uma fonte específica. Por exemplo, para usar uma fonte específica para o texto em uma camada de modelo, carregue o arquivo de fonte. Para exibir os números de página do Visualizador de eCatalog em uma fonte específica, faça upload do arquivo de fonte.

O Dynamic Media Classic é compatível com estes tipos de fonte:

* Todas as fontes TrueType
* Fontes PostScript®
* Fontes OpenType/TrueType
* Fontes OpenType/PostScript
* PhotoFonts

Após o upload de um arquivo de fonte, é possível alterar a ID do Dynamic Media Classic, o nome da fonte e digitar informações na tela Editar informações.

>[!NOTE]
>
>O Dynamic Media Classic recomenda fazer upload de todos os estilos de fonte (negrito, itálico, negrito/itálico e regular) se você planeja usar fontes em camadas de modelo. O Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. O upload de todos os arquivos PostScript/Adobe Tipo 1 associados a uma fonte também é recomendado, pois algumas dessas fontes contêm informações detalhadas de ajuste de espaço.

## Upload de arquivos de fonte {#uploading-font-files}

Carregue arquivos de fonte com as mesmas técnicas usadas para carregar outros arquivos. É possível armazenar arquivos de fonte em qualquer pasta do Dynamic Media Classic. Consulte [Fazer upload dos arquivos](uploading-files.md#uploading_your_files).

## Editar informações do arquivo de fonte {#editing-font-file-information}

É possível alterar o nome da ID de uma fonte, bem como suas informações de tipo. Editar um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação de fontes.

No painel Procurar, selecione o arquivo de fonte que deseja editar na visualização Detalhe e escolha Arquivo > Editar informações. A tela Editar informações é aberta. Escolha as seguintes opções e selecione o botão Enviar.

**Nome** da fonteEsse nome identifica a fonte quando é publicada.

**Nome** PostScript Esse nome é o nome PostScript completo para a fonte. Geralmente indica o peso ou estilo.

**Nome** RTF Esse nome aparece em um menu pop-up no editor RTF onde as camadas de texto do modelo são criadas.

**Nome** da família da fonte Esse nome lista o nome da fonte sem o indicador de estilo, peso ou tipo de fonte.

**Estilo** da fonte As opções são Simples, Negrito, Itálico e Negrito-Itálico.

**Tipo** de fonte As opções são TrueType e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

**Abreviação** do tipo de fonte As opções são as seguintes:

**Arquivos de fonte TTF** TrueType usados para renderização de PDF/PostScript e serviço de imagem.

**Arquivos de fonte AFM** do Adobe PostScript que contêm informações de Métricas de fonte da Adobe e são usados para o serviço de imagem.

**Arquivos de fonte PFM** Adobe PostScript que contêm informações de métricas de fonte binária.

**Arquivos de fonte PFB** do Adobe PostScript que contêm informações de contorno de fonte binária e são usados para renderização de PDF/PostScript e disponibilização de imagem.
