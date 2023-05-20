---
title: Trabalhar com PDF
description: Saiba como trabalhar com PDF no Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Trabalhar com PDF{#working-with-pdfs}

Os arquivos PDF (Portable Document Format) são usados com mais frequência no Adobe Dynamic Media Classic para criar eCatalogs. Ao carregar um arquivo PDF, o Adobe Dynamic Media Classic rasteriza ou ripa as páginas por padrão, para que elas possam ser usadas para criar mídia avançada.

Ao fazer upload de um PDF para extração de página, o Adobe impõe o seguinte limite:

| Tipo de limite | Limite imposto | Alteração para limitar em 31 de dezembro de 2022 |
| --- | --- | --- |
| Número máximo de páginas para um PDF a ser considerado para extração | 5000 (para novos uploads) | 100 (para todos os PDF) |

Consulte também [Limitações do Dynamic Media](/help/limitations.md).

## opções de upload de PDF {#pdf-upload-options}

Ao fazer upload de um arquivo PDF, você pode formatá-lo de várias maneiras. Corta as páginas, extrai palavras de pesquisa, insere uma resolução de pixels por polegada e escolhe um espaço de cor. Os arquivos PDF geralmente contêm uma margem de apara, marcas de corte, marcas de registro e outras marcas de impressora. Você pode cortar essas marcas nas laterais das páginas ao fazer upload de um arquivo PDF.

As opções para fazer upload de arquivos PDF estão na página Upload em Opções de PDF.

### Opções de processamento

**[!UICONTROL Rasterize]** - (Padrão) Extrai as páginas no arquivo PDF e converte gráficos de vetor em imagens de bitmap. Para criar um eCatalog, escolha essa opção.

**[!UICONTROL Extract Search Words]** - Extrai palavras do arquivo PDF para que o arquivo possa ser pesquisado por palavra-chave em um eCatalog Viewer.

**[!UICONTROL Extract Links]** - Extrai links dos arquivos PDF e os converte em Mapas de imagem que são usados em um eCatalog Viewer.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]** - Cria automaticamente um eCatalog a partir do arquivo PDF. O eCatalog é nomeado com base no arquivo PDF que você carregou. (Essa opção só estará disponível se você rasterizar o arquivo de PDF à medida que fizer upload dele.)

### Resolução

Determina a configuração de resolução. Essa configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

### Opções de espaço de cor

Selecione o menu Espaço de cor e escolha um espaço de cor para o arquivo PDF. A maioria dos arquivos PDF tem imagens coloridas RGB e CMYK. O espaço de cores do RGB é preferível para visualização on-line.

* **[!UICONTROL Detect Automatically]** - Mantém o espaço de cores do arquivo PDF.

* **[!UICONTROL Force As RGB]** - Converte para o espaço de cores do RGB.

* **[!UICONTROL Force As CMYK]** - Converte para o espaço de cores CMYK.

* **[!UICONTROL Force As Grayscale]** - Converte para o espaço de cores Tons de cinza.

### Opções de perfil de cores

* **[!UICONTROL Convert To sRGB]** - Converte para sRGB (azul vermelho verde padrão). sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

* **[!UICONTROL Keep Original Color Space]** - Mantém o espaço de cores original.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic.

Consulte também [Perfis ICC](/help/icc-profiles.md#icc_profiles).

## Cortar espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para cortar automaticamente os pixels de espaço em branco de um arquivo PDF ao carregá-lo, selecione o menu Cortar e escolha Cortar.
1. Especifique as seguintes opções:

   * **[!UICONTROL Trim Away Based On]** - Escolha se deseja cortar com base na cor ou na transparência:

      * **[!UICONTROL Color]** - Escolha a opção Cor. Em seguida, selecione o **[!UICONTROL Corner]** e escolha o canto do PDF com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

      * **[!UICONTROL Transparency]** - Escolha a opção Transparência.
   * **[!UICONTROL Tolerance]** - Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

   * **[!UICONTROL Trimming based on color]** - Especifique 0 para cortar os pixels somente se eles corresponderem exatamente à cor selecionada no canto do PDF. Números próximos a 1 permitem mais diferença de cor.

   * **[!UICONTROL Trimming based on transparency]** - Especifique 0 para cortar os pixels somente se eles forem transparentes; números mais próximos a 1 permitem mais transparência.


## Cortar nas laterais das páginas de PDF {#cropping-from-the-sides-of-pdf-pages}

Você pode remover manualmente as marcas da impressora das laterais das páginas em um arquivo PDF ao carregá-lo.

1. No menu Cortar, selecione **[!UICONTROL Manual]**.
1. Insira as configurações de pixel nas caixas de texto Superior, Direito, Inferior e Esquerdo para cortar da parte superior, inferior e laterais das páginas.

O quanto da página é cortada depende da configuração Resolução PX/Inch inserida para o arquivo PDF. Por exemplo, suponha que você insira 150 (o padrão) como a configuração Resolução PX/Polegada. Em seguida, você corta 75 pixels das laterais das páginas. Nesse caso, 0,5 pol é cortado. A 150 pixels por polegada, 75 pixels equivale a meia polegada.
