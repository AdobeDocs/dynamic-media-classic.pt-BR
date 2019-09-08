---
title: Fontes
seo-title: Fontes
description: 'null'
seo-description: Saiba como usar fontes no Dynamic Media Classic.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/support_ files
discoiquuid: 97 casu 6 a -30 aa -44 fe-a 611-fd 71 b 02 fd 5 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Fontes{#fonts}

Em alguns casos, o Sistema de publicação Scene 7 exige que você carregue um arquivo de fonte para inserir ou renderizar o texto em uma fonte específica. Por exemplo, para usar uma fonte específica para texto em uma camada de modelo, carregue o arquivo de fonte. Para exibir números de página do Visualizador do ecatalog em uma fonte específica, carregue o arquivo de fonte.

O Dynamic Media Classic oferece suporte a esses tipos de fontes:

* Todas as fontes truetype
* Fontes postscript®
* Fontes opentype/truetype
* Fontes opentype/postscript
* Photofonts

Depois que um arquivo de fonte é carregado, você pode alterar sua ID do SPS, nome da fonte e informações de tipo na tela Editar informações.

>[!NOTE]
>
>O Dynamic Media Classic recomenda carregar todos os estilos de fonte (negrito, itálico, negrito/itálico e regular) se você planeja usar fontes em camadas de modelo. O Dynamic Media Classic precisa desses estilos de fonte para processar solicitações. O upload de todos os arquivos postscript/Adobe Type 1 associados a uma fonte também é recomendado, pois algumas dessas fontes contêm informações detalhadas sobre kerning.

## Fazer upload de arquivos de fontes {#uploading-font-files}

Carregue arquivos de fontes com as mesmas técnicas usadas para fazer upload de outros arquivos. É possível armazenar arquivos de fonte em qualquer pasta SPS. Consulte [Carregar seus arquivos](uploading-files.md#uploading_your_files).

## Edição de informações de arquivo de fontes {#editing-font-file-information}

Você pode alterar o nome da ID de uma fonte, bem como suas informações de tipo. Editar um arquivo de fonte pode ser útil em pesquisas e facilitar a identificação das fontes.

No Painel Procurar, selecione o arquivo de fonte que deseja editar na exibição Detalhe e escolha Arquivo &gt; Editar informações. A tela Editar informações é aberta. Escolha as opções a seguir e selecione o botão Enviar.

**Nome da fonte** Esse nome identifica a fonte quando ela é publicada.

**Nome postscript** Nome é o nome postscript completo da fonte. Geralmente indica a espessura ou estilo.

**Nome RTF** Esse nome aparece em um menu pop-up no editor RTF, onde as camadas de texto de modelo são criadas.

**Nome da família de fontes** Esse nome lista o nome da fonte sem o indicador, peso ou indicador de tipo de fonte.

**Estilo de Fonte** As opções são Simples, Negrito, Itálico e Negrito-Itálico.

**Tipo de fonte** As opções são truetype e Adobe Type 1. Se você chamar essas fontes por outro nome, poderá inseri-las.

**Abreviação do tipo de fonte** As opções são as seguintes:

**Arquivos de fonte** Truetype TTF usados para renderização de PDF/postscript e serviço de imagem.

**Arquivos de fonte AFM** Adobe postscript que contêm informações de Métricas do Adobe Font e são usadas para o fornecimento de imagens.

**Arquivos de fonte PFM** Adobe postscript que contêm informações de métricas binárias.

**Arquivos de fonte PFB** Adobe postscript que contêm informações de contorno binário de fonte e são usadas para renderização de PDF/postscript e veiculação de imagens.
