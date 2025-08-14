---
title: Fazer upload dos arquivos do PDF
description: Saiba como fazer upload dos arquivos PDF associados a um eCatalog no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Fazer upload dos arquivos do PDF{#uploading-the-pdf-files}

Normalmente, os arquivos do Adobe PDF são a origem de um eCatalog. Esses arquivos contêm todas as informações de imagem, fontes e gráficos vetoriais. Também é possível criar um eCatalog com imagens. Após preparar os arquivos PDF para carregamento, na barra Navegação global, selecione **[!UICONTROL Upload]** para começar a carregar os PDFs.

Ao fazer upload de uma PDF para extração de página, o Adobe impõe o seguinte limite:

| Tipo de limite do PDF | Limite imposto | Alteração para limitar em 31 de dezembro de 2022 |
| --- | --- | --- |
| Número máximo de páginas para que uma PDF seja considerada para extração | 5000 (para novos uploads) | 100 (para todos os PDFs) |

Consulte também [limitações do Dynamic Media](/help/using/limitations.md).

## Preparar seus arquivos do PDF

Prepare seus arquivos do PDF antes de carregá-los no Adobe Dynamic Media Classic:

* Para facilitar o upload dos arquivos, coloque todos os arquivos na mesma pasta no computador ou na rede.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará a colocação das páginas na ordem adequada depois que os arquivos forem carregados.
* Para ver se as páginas do PDF contêm marcas de corte, destinos de registro ou barras de cores, examine as páginas. Essas marcas determinam onde cortar o papel quando os documentos forem impressos; elas devem ser removidas antes que seu eCatalog seja colocado na Web. O Adobe Dynamic Media Classic fornece opções de marcas de corte ao fazer upload de arquivos PDF.
* Se você quiser que os visualizadores pesquisem seu eCatalog por palavra-chave, descubra se seus arquivos do PDF estão &quot;nivelados&quot;. Não é possível extrair palavras de pesquisa de arquivos PDF nivelados. Para saber se um PDF está nivelado, tente selecionar o texto dentro dele. Se não for possível selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave no seu eCatalog.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o Adobe Dynamic Media Classic pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. No entanto, se você quiser usar um perfil de cores personalizado para converter imagens CMYK, faça isso.

  Consulte [perfis do ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Prática recomendada para as opções de upload do PDF {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de carregamento, consulte [Carregando seus arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que você deseja carregar e selecione estas *práticas recomendadas* Opções do PDF:

* **Opções de Corte**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL Crop Options]**. Se as páginas do PDF contiverem marcas de corte, marcas de registro ou outras marcas, na lista suspensa **[!UICONTROL Crop]**, escolha **[!UICONTROL Manual]**. Insira o número de pixels a serem cortados da parte superior, direita, inferior e esquerda das páginas. As marcas de corte geralmente são definidas como uma margem de meia polegada. Suponha que você escolha **[!UICONTROL 150]** (recomendado) como a resolução pixel por polegada. Em seguida, digite 75, 75, 75, 75 nas caixas de texto Superior, Direito, Inferior e Esquerdo. Nesse caso, ele corta meia polegada das margens (a 150 ppi, metade de 1 é igual a 75 pixels).

* **Processando**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL PDF Options]**. Na lista suspensa **[!UICONTROL Processing]**, escolha **[!UICONTROL Rasterize]**. O arquivo do PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no eCatalog.

* **Extrair Palavras de Pesquisa (opcional)**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL PDF Options]**. Na lista suspensa Extrair, escolha **[!UICONTROL Search words]** se quiser que seus visualizadores possam pesquisar por palavra-chave em seu eCatalog.

* **Gerar automaticamente o eCatalog a partir do PDF de várias páginas (opcional)**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL PDF Options]**. Clique em **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** para criar automaticamente um eCatalog ao carregar. Você pode ir diretamente para a tela do eCatalog e começar a trabalhar no eCatalog sem ter que primeiro selecionar os arquivos do PDF e selecionar o comando Criar. O eCatalog é nomeado de acordo com seu arquivo PDF.

* **Solução**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL PDF Options]**. No campo de texto **[!UICONTROL Resolution]**, insira um valor. A Adobe Dynamic Media Classic recomenda 150 pixels por polegada.

* **Colorspace**: Na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL PDF Options]**. Na lista suspensa Espaço de cor, escolha **[!UICONTROL Detect automatically]**. Normalmente, os PDFs criados para saída de impressão estão em CMYK; os PDFs para visualização on-line estão em RGB. Se um PDF usar ambos os espaços de cores, você poderá selecionar um espaço de cores específico escolhendo Forçar como RGB ou Forçar como CMYK. Os PDFs usam ambos os espaços de cores, por exemplo, quando os gráficos de página usam um espaço de cores CMYK, mas as imagens usam RGB. Se você carregou um perfil ICC, seu nome aparece no menu Espaço de cores e você pode escolhê-lo lá.

  Consulte [perfis do ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opções de Perfil de Cores**: na caixa de diálogo Carregar Opções de Trabalho, selecione **[!UICONTROL Color Profile Options]** e escolha uma opção de Perfil de Cores:

   * **Manter Espaço de Cor Original**: retém o espaço de cor original.

   * **Personalizar de > Para**: abre submenus para que você possa escolher um espaço de cores **[!UICONTROL Convert From]** e **[!UICONTROL Convert To]**. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Consulte [perfis do ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para obter detalhes sobre todas as opções do PDF, consulte [opções de carregamento do PDF](pdfs.md#pdf_upload_options).
