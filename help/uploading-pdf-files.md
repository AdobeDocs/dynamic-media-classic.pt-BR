---
title: Fazer upload dos arquivos do PDF
description: Saiba como fazer upload dos arquivos do PDF associados a um eCatalog no Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Fazer upload dos arquivos do PDF{#uploading-the-pdf-files}

Normalmente, os arquivos Adobe PDF são a fonte de um eCatalog. Esses arquivos contêm todas as informações de imagem, fontes e gráficos vetoriais. Você também pode criar um eCatalog com imagens. Depois de preparar os arquivos de PDF para upload, na barra Navegação global, selecione **[!UICONTROL Upload]** para começar a fazer upload do PDF.

>[!NOTE]
>
>Ao fazer upload de um PDF para extração de página, o Adobe impõe a diretriz de práticas recomendadas e o limite imposto a seguir.
>
>* Número máximo de páginas por PDF consideradas para extração
   >   * Prática recomendada: 100
   >   * Limite imposto: 1000 (para uploads de atualização)


## Prepare seus arquivos do PDF {#preparing-your-pdf-files}

Prepare seus arquivos do PDF antes de carregá-los no Adobe Dynamic Media Classic:

* Para facilitar o upload dos arquivos, coloque todos os arquivos na mesma pasta no computador ou na rede.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará colocar as páginas na ordem correta após os arquivos serem carregados.
* Para ver se as PDF pages contêm marcas de corte, destinos de registro ou barras de cores, examine as páginas. Estas marcas determinam onde cortar o papel quando os documentos são impressos; eles devem ser removidos antes que seu eCatalog seja colocado na Web. O Adobe Dynamic Media Classic fornece opções para marcas de corte ao carregar arquivos PDF.
* Se você deseja que os visualizadores pesquisem seu eCatalog por palavra-chave, descubra se os arquivos do PDF estão &quot;nivelados&quot;. Não é possível extrair palavras de pesquisa de arquivos PDF nivelados. Para descobrir se um PDF está nivelado, tente selecionar o texto dentro dele. Se você não conseguir selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave em seu eCatalog.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o Adobe Dynamic Media Classic pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. No entanto, se você quiser usar um perfil de cor personalizado para converter imagens CMYK, poderá fazer isso.

   Consulte [Perfis ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Opções de upload do PDF de práticas recomendadas {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de upload, consulte [Upload de arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que deseja fazer upload e selecione-os *prática recomendada* Opções de PDF:

* **Opções de corte** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL Crop Options]**. Se as PDF pages contiverem marcas de corte, marcas de registro ou outras marcas, na **[!UICONTROL Crop]** lista suspensa, escolha **[!UICONTROL Manual]**. Insira o número de pixels para cortar a partir dos lados superior, direito, inferior e esquerdo das páginas. As marcas de corte são frequentemente definidas a uma margem de meia polegada. Suponha que você escolha **[!UICONTROL 150]** (recomendado) como a resolução de pixel por polegada e insira 75, 75, 75, 75 nas caixas de texto Superior, Direita, Inferior e Esquerda. Nesse caso, ele recorta uma meia polegada das margens (em 150 ppi, metade de 1 é igual a 75 pixels).

* **Processamento** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL PDF Options]**. No **[!UICONTROL Processing]** lista suspensa, escolha **[!UICONTROL Rasterize]**. O arquivo PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no eCatalog.

* **Extrair palavras de pesquisa (opcional)** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL PDF Options]**. Na lista suspensa Extrair , escolha **[!UICONTROL Search words]** se você quiser que seus visualizadores possam pesquisar por palavra-chave em seu eCatalog.

* **Gerar o eCatalog automaticamente a partir de vários PDF de página (opcional)** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL PDF Options]**. Selecionar **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** para criar automaticamente um eCatalog ao fazer upload. Você pode ir direto para a tela eCatalog e começar a trabalhar em seu eCatalog sem precisar selecionar primeiro os arquivos do PDF e selecionar o comando Build. O eCatalog é nomeado após seu arquivo PDF.

* **Resolução** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL PDF Options]**. No **[!UICONTROL Resolution]** , insira um valor. A Adobe Dynamic Media Classic recomenda 150 pixels por polegada.

* **Colorspace** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL PDF Options]**. Na lista suspensa Espaço de cores, escolha **[!UICONTROL Detect automatically]**. Geralmente, os PDF criados para saída de impressão estão em CMYK; PDF para exibição online são RGB. Se um PDF usar ambos os espaços de cores, você pode selecionar um espaço de cores específico escolhendo Forçar como RGB ou Forçar como CMYK. O PDF usa ambos os espaços de cores, por exemplo, quando os gráficos de página usam um espaço de cores CMYK, mas as fotos usam o RGB. Se você tiver carregado um perfil ICC, seu nome aparecerá no menu Colorspace e você poderá escolhê-lo lá.

   Consulte [Perfis ICC (International Color Consortium)](/help/icc-profiles.md).

* **Opções de perfil de cores** - Na caixa de diálogo Upload Job Options , selecione **[!UICONTROL Color Profile Options]** e escolha uma opção de Perfil de cor:

   * **Manter espaço de cor original** - Mantém o espaço de cores original.

   * **Personalizado De > Para** - Abre submenus para que você possa escolher um **[!UICONTROL Convert From]** e **[!UICONTROL Convert To]** espaço de cores. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Consulte [Perfis ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para obter detalhes sobre todas as opções do PDF, consulte [Opções de upload do PDF](pdfs.md#pdf_upload_options).
