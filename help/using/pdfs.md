---
title: Trabalhar com PDF
description: Saiba como trabalhar com PDF no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Trabalhar com PDF{#working-with-pdfs}

Os arquivos PDF (Portable Document Format) são usados com mais frequência no Adobe Dynamic Media Classic para criar eCatalogs. Ao carregar um arquivo PDF, o Adobe Dynamic Media Classic rasteriza ou ripa as páginas por padrão, para que elas possam ser usadas para criar mídia avançada.

Ao fazer upload de um PDF para extração de página, o Adobe impõe o seguinte limite:

| Tipo de limite | Limite imposto | Alteração para limitar em 31 de dezembro de 2022 |
| --- | --- | --- |
| Número máximo de páginas para um PDF a ser considerado para extração | 5000 (para novos uploads) | 100 (para todos os PDF) |

Consulte também [limitações do Dynamic Media](/help/using/limitations.md).

## opções de upload de PDF {#pdf-upload-options}

Ao fazer upload de um arquivo PDF, você pode formatá-lo de várias maneiras. Corta as páginas, extrai palavras de pesquisa, insere uma resolução de pixels por polegada e escolhe um espaço de cor. Os arquivos PDF geralmente contêm uma margem de apara, marcas de corte, marcas de registro e outras marcas de impressora. Você pode cortar essas marcas nas laterais das páginas ao fazer upload de um arquivo PDF.

As opções para fazer upload de arquivos PDF estão na página Upload em Opções de PDF.

### Opções de processamento

**[!UICONTROL Rasterize]**: (Padrão) Extrai as páginas no arquivo PDF e converte gráficos de vetor em imagens de bitmap. Para criar um eCatalog, escolha essa opção.

**[!UICONTROL Extract Search Words]**: Extrai palavras do arquivo PDF para que as palavras-chave do arquivo possam ser pesquisadas em um Visualizador de eCatalog.

**[!UICONTROL Extract Links]**: Extrai links dos arquivos PDF e os converte em Mapas de Imagens que são usados em um Visualizador de eCatalog.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]**: cria automaticamente um eCatalog a partir do arquivo PDF. O eCatalog é nomeado com base no arquivo PDF que você carregou. (Essa opção só estará disponível se você rasterizar o arquivo de PDF à medida que fizer upload dele.)

### Resolução

Determina a configuração de resolução. Essa configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

### Opções de espaço de cor

Selecione o menu Espaço de cor e escolha um espaço de cor para o arquivo PDF. A maioria dos arquivos PDF tem imagens coloridas RGB e CMYK. O espaço de cores do RGB é preferível para visualização on-line.

* **[!UICONTROL Detect Automatically]**: retém o espaço de cores do arquivo PDF.

* **[!UICONTROL Force As RGB]**: Converte para o espaço de cores do RGB.

* **[!UICONTROL Force As CMYK]**: Converte para o espaço de cores CMYK.

* **[!UICONTROL Force As Grayscale]**: converte para o espaço de cores Tons de Cinza.

### Opções de perfil de cores

* **[!UICONTROL Convert To sRGB]**: Converte para sRGB (Vermelho Verde Azul Padrão). O sRGB é o espaço de cores recomendado para a exibição de imagens em uma página da Web.

* **[!UICONTROL Keep Original Color Space]**: retém o espaço de cores original.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]**: abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic.

Consulte também [perfis ICC](/help/using/icc-profiles.md#icc_profiles).

## Cortar espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

Você pode cortar automaticamente pixels de espaço em branco de um arquivo PDF ao carregá-lo.

1. Selecione o menu Cortar e escolha Cortar.
1. Especifique as seguintes opções:

   * **[!UICONTROL Trim Away Based On]**: Escolha se deseja cortar com base na cor ou na transparência:

      * **[!UICONTROL Color]**: Escolha a opção Cor. Em seguida, selecione o menu **[!UICONTROL Corner]** e escolha o canto do PDF com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

      * **[!UICONTROL Transparency]**: Escolha a opção Transparência.

   * **[!UICONTROL Tolerance]**: arraste o controle deslizante para especificar uma tolerância de 0 a 1.

   * **[!UICONTROL Trimming based on color]**: especifique 0 para cortar os pixels apenas se eles corresponderem exatamente à cor selecionada no canto do PDF. Números próximos a 1 permitem mais diferença de cor.

   * **[!UICONTROL Trimming based on transparency]**: especifique 0 para cortar pixels apenas se eles forem transparentes; números mais próximos a 1 permitem mais transparência.

## Cortar nas laterais das páginas de PDF {#cropping-from-the-sides-of-pdf-pages}

Você pode remover manualmente as marcas da impressora das laterais das páginas em um arquivo PDF ao carregá-lo.

1. No menu Cortar, selecione **[!UICONTROL Manual]**.
1. Insira as configurações de pixel nas caixas de texto Superior, Direito, Inferior e Esquerdo para cortar da parte superior, inferior e laterais das páginas.

O quanto da página é cortada depende da configuração Resolução PX/Inch inserida para o arquivo PDF. Por exemplo, suponha que você insira 150 (o padrão) como a configuração Resolução PX/Polegada. Em seguida, você corta 75 pixels das laterais das páginas. Nesse caso, 0,5 pol é cortado. A 150 pixels por polegada, 75 pixels equivale a meia polegada.
