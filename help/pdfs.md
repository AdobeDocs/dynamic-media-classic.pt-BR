---
title: Trabalhar com PDF
description: Saiba como trabalhar com o PDF no Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Trabalhar com PDF{#working-with-pdfs}

Os arquivos PDF (Portable Document Format) são usados com mais frequência no Adobe Dynamic Media Classic para criar catálogos eletrônicos. Quando você faz upload de um arquivo PDF, o Adobe Dynamic Media Classic rasteriza ou rasga as páginas por padrão, para que as páginas possam ser usadas para criar mídia avançada.

Ao fazer upload de um PDF para extração de página, o Adobe aplica o seguinte limite:

| Tipo de limite | Limite imposto | Alteração do limite em 31 de dezembro de 2022 |
| --- | --- | --- |
| Número máximo de páginas para um PDF a ser considerado para extração | 5000 (para novos uploads) | 100 (para todos os PDF) |

Consulte também [Limitações do Dynamic Media](/help/limitations.md).

## Opções de upload do PDF {#pdf-upload-options}

Ao fazer upload de um arquivo PDF, você pode formatá-lo de várias maneiras. Você recorta suas páginas, extrai palavras de pesquisa, digita uma resolução de pixels por polegada e escolhe um espaço de cores. Os arquivos PDF geralmente contêm uma margem de aparação, marcas de corte, marcas de registro e outras marcas de impressora. Você pode recortar essas marcas das laterais das páginas ao carregar um arquivo PDF.

As opções para carregar arquivos do PDF estão na página Upload em Opções de PDF.

### Opções de processamento

**[!UICONTROL Rasterize]** - (Padrão) Ripsa as páginas no arquivo PDF e converte gráficos vetoriais em imagens bitmap. Para criar um eCatalog, escolha essa opção.

**[!UICONTROL Extract Search Words]** - Extrai palavras do arquivo PDF para que o arquivo possa ser pesquisado por palavra-chave em um visualizador de eCatalog.

**[!UICONTROL Extract Links]** - Extrai links dos arquivos do PDF e os converte em mapas de imagem usados em um visualizador de eCatalog.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]** - Cria automaticamente um eCatalog a partir do arquivo do PDF. O eCatalog é nomeado após o arquivo PDF que você carregou. (Essa opção só estará disponível se você rasterizar o arquivo PDF à medida que fizer upload dele.)

### Resolução

Determina a configuração de resolução. Esta configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

### Opções de Espaço de cor

Selecione o menu Espaço de cores e escolha um espaço de cores para o arquivo PDF. A maioria dos arquivos PDF tem imagens de cores RGB e CMYK. O espaço de cores do RGB é preferível para visualização online.

* **[!UICONTROL Detect Automatically]** - Mantém o espaço de cores do arquivo PDF.

* **[!UICONTROL Force As RGB]** - Converte para o espaço de cores RGB.

* **[!UICONTROL Force As CMYK]** - Converte para o espaço de cores CMYK.

* **[!UICONTROL Force As Grayscale]** - Converte para o espaço de cor Escala de Cinza.

### Opções de perfil de cor

* **[!UICONTROL Convert To sRGB]** - Converte em sRGB (Azul Verde Vermelho Padrão). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

* **[!UICONTROL Keep Original Color Space]** - Mantém o espaço de cores original.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Adobe Dynamic Media Classic.

Consulte também [Perfis ICC](/help/icc-profiles.md#icc_profiles).

## Recortar espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para cortar automaticamente os pixels de espaço em branco de um arquivo de PDF à medida que você o carrega, selecione o menu Recortar e escolha Aparar.
1. Especifique as seguintes opções:

   * **[!UICONTROL Trim Away Based On]** - Escolha se deseja cortar com base na cor ou na transparência:

      * **[!UICONTROL Color]** - Escolha a opção Color . Em seguida, selecione o **[!UICONTROL Corner]** e escolha o canto da PDF com a cor que melhor representa a cor do espaço em branco que deseja recortar.

      * **[!UICONTROL Transparency]** - Escolha a opção Transparency .
   * **[!UICONTROL Tolerance]** - Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

   * **[!UICONTROL Trimming based on color]** - Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PDF. Os números mais próximos de 1 permitem mais diferenças de cor.

   * **[!UICONTROL Trimming based on transparency]** - Especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos de 1 permitem mais transparência.


## Recortar das laterais das PDF pages {#cropping-from-the-sides-of-pdf-pages}

Você pode remover manualmente as marcas da impressora das laterais das páginas em um arquivo PDF à medida que faz o upload.

1. No menu Cortar, selecione **[!UICONTROL Manual]**.
1. Insira as configurações de pixel nas caixas de texto Superior, Direita, Inferior e Esquerda para cortar da parte superior, inferior e lados das páginas.

A quantidade de páginas cortadas depende da configuração de Resolução PX/Inch inserida para o arquivo PDF. Por exemplo, se você digitar 150 (padrão) como a configuração Resolução PX/Polegada e cortar 75 pixels das laterais das páginas, meia polegada será cortada; a 150 pixels por polegada, 75 pixels é igual a meia polegada.
