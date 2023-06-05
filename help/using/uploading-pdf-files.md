---
title: Fazer upload dos arquivos PDF
description: Saiba como fazer upload dos arquivos PDF associados a um eCatalog no Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Fazer upload dos arquivos PDF{#uploading-the-pdf-files}

Normalmente, os arquivos do Adobe PDF são a origem de um eCatalog. Esses arquivos contêm todas as informações de imagem, fontes e gráficos vetoriais. Também é possível criar um eCatalog com imagens. Depois de preparar os arquivos PDF para upload, na barra Navegação global, selecione **[!UICONTROL Upload]** para começar a carregar os PDF.

Ao fazer upload de um PDF para extração de página, o Adobe impõe o seguinte limite:

| tipo de limite de PDF | Limite imposto | Alteração para limitar em 31 de dezembro de 2022 |
| --- | --- | --- |
| Número máximo de páginas para um PDF a ser considerado para extração | 5000 (para novos uploads) | 100 (para todos os PDF) |

Consulte também [Limitações do Dynamic Media](/help/using/limitations.md).

## Preparar seus arquivos PDF {#preparing-your-pdf-files}

Prepare seus arquivos PDF antes de carregá-los no Adobe Dynamic Media Classic:

* Para facilitar o upload dos arquivos, coloque todos os arquivos na mesma pasta no computador ou na rede.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará a colocação das páginas na ordem adequada depois que os arquivos forem carregados.
* Para ver se as páginas de PDF contêm marcas de corte, destinos de registro ou barras de cores, examine as páginas. Essas marcas determinam onde cortar o papel quando os documentos forem impressos; elas devem ser removidas antes que seu eCatalog seja colocado na Web. O Adobe Dynamic Media Classic fornece opções de marcas de corte ao carregar arquivos PDF.
* Se você quiser que os visualizadores pesquisem seu eCatalog por palavra-chave, descubra se seus arquivos de PDF estão &quot;nivelados&quot;. Não é possível extrair palavras de pesquisa de arquivos de PDF nivelados. Para saber se um PDF está nivelado, tente selecionar o texto dentro dele. Se não for possível selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave no eCatalog.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o Adobe Dynamic Media Classic pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. No entanto, se você quiser usar um perfil de cores personalizado para converter imagens CMYK, faça isso.

   Consulte [Perfis ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Prática recomendada para opções de upload de PDF {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de upload, consulte [Carregamento de arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que deseja fazer upload e selecione-os *prática recomendada* Opções de PDF:

* **Opções de corte** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Crop Options]**. Se as páginas de PDF contiverem marcas de corte, marcas de registro ou outras marcas, no **[!UICONTROL Crop]** selecione **[!UICONTROL Manual]**. Insira o número de pixels para cortar nos lados superior, direito, inferior e esquerdo das páginas. As marcas de corte geralmente são definidas como uma margem de meia polegada. Suponha que você escolha **[!UICONTROL 150]** (recomendado) como a resolução de pixel por polegada e digite 75, 75, 75, 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo. Nesse caso, ele corta meia polegada das margens (a 150 ppi, metade de 1 é igual a 75 pixels).

* **Processando** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL PDF Options]**. No **[!UICONTROL Processing]** selecione **[!UICONTROL Rasterize]**. O arquivo PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no eCatalog.

* **Extrair palavras de pesquisa (opcional)** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL PDF Options]**. Na lista suspensa Extrair, escolha **[!UICONTROL Search words]** se quiser que os visualizadores possam pesquisar por palavra-chave no eCatalog.

* **Gerar eCatalog automaticamente a partir de PDF de várias páginas (opcional)** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL PDF Options]**. Selecionar **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** para criar automaticamente um eCatalog ao fazer upload. Você pode ir diretamente para a tela eCatalog e começar a trabalhar em seu eCatalog sem ter que primeiro selecionar arquivos PDF e selecionar o comando Build. O eCatalog é nomeado de acordo com seu arquivo PDF.

* **Resolução** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL PDF Options]**. No **[!UICONTROL Resolution]** campo de texto, insira um valor. A Adobe Dynamic Media Classic recomenda 150 pixels por polegada.

* **Espaço de cor** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL PDF Options]**. Na lista suspensa Espaço de cores, escolha **[!UICONTROL Detect automatically]**. Normalmente, os PDF criados para saída de impressão estão em CMYK; os PDF para visualização on-line são RGB. Se um PDF usar ambos os espaços de cores, você poderá selecionar um espaço de cores específico escolhendo Forçar como RGB ou Forçar como CMYK. Os PDF usam ambos os espaços de cores, por exemplo, quando os gráficos de página usam um espaço de cores CMYK, mas as imagens usam RGB. Se você carregou um perfil ICC, seu nome aparece no menu Espaço de cores e você pode escolhê-lo lá.

   Consulte [Perfis ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opções de perfil de cores** - Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Color Profile Options]** e escolha uma opção de Perfil de cor:

   * **Manter espaço de cor original** - Mantém o espaço de cores original.

   * **Personalizar De > Para** - Abre submenus para que você possa escolher um **[!UICONTROL Convert From]** e **[!UICONTROL Convert To]** espaço de cores. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Consulte [Perfis ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para obter detalhes sobre todas as opções de PDF, consulte [opções de upload de PDF](pdfs.md#pdf_upload_options).
