---
title: Como fazer upload dos arquivos PDF
seo-title: Como fazer upload dos arquivos PDF
description: nulo
seo-description: Saiba como fazer upload dos arquivos PDF associados a um eCatalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---


# Como fazer upload dos arquivos PDF{#uploading-the-pdf-files}

Geralmente, os arquivos Adobe PDF são a fonte de um eCatalog; esses arquivos contêm todas as informações de imagem, além de fontes e gráficos vetoriais. Você também pode criar um eCatalog com imagens. Depois de preparar seus arquivos PDF para upload, selecione o botão Carregar na barra de navegação global para começar a carregar os PDFs.

## Preparação de arquivos PDF {#preparing-your-pdf-files}

Prepare seus arquivos PDF antes de carregá-los no Dynamic Media Classic:

* Coloque todos os arquivos na mesma pasta do computador ou da rede para facilitar o upload dos arquivos.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará o posicionamento das páginas na ordem correta após o upload dos arquivos.
* Examine as páginas do PDF para ver se contêm marcas de corte, públicos alvos de registro ou barras coloridas. Estas marcas determinam onde cortar o papel quando os documentos são impressos; eles devem ser removidos antes que seu eCatalog seja colocado na Web. O Dynamic Media Classic fornece opções para marcas de corte ao carregar arquivos PDF.
* Se você quiser que os visualizadores pesquisem seu eCatalog por palavra-chave, descubra se seus arquivos PDF estão &quot;nivelados&quot;. Não é possível extrair palavras de pesquisa de arquivos PDF nivelados. Para descobrir se um PDF está nivelado, tente selecionar o texto dentro dele. Se não for possível selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave no seu eCatalog.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o Dynamic Media Classic pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. Entretanto, se você quiser usar um perfil de cores personalizado para converter imagens CMYK, poderá fazê-lo.

   Consulte perfis [](icc-profiles.md#icc_profiles)ICC.

## Opções de upload de PDF com práticas recomendadas {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de upload, consulte [Fazer upload dos arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que deseja carregar e, em seguida, selecione as *melhores práticas* Opções de PDF:

* **Recortar** Selecione o menu Recortar e escolha Manual se as páginas contiverem marcas de recorte, marcas de registro ou outras marcas. Insira o número de pixels a serem cortados nos lados superior, direito, inferior e esquerdo das páginas. As marcas de corte geralmente são definidas em uma margem de meia polegada. Supondo que você escolha 150 como a resolução pixel por polegada (a configuração recomendada), inserir 75, 75, 75, 75, 75 nas caixas de texto Superior, Direita, Inferior e Esquerda corta meia polegada das margens (a 150 ppi, metade de uma polegada equivale a 75 pixels).

* **Processamento** Selecione o menu Processamento e escolha Rasterizar. O arquivo PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no eCatalog.

* **Extrair palavras de pesquisa (opcional)** Selecione essa opção se desejar que os visualizadores possam pesquisar por palavra-chave no seu eCatalog.

* **Gerar automaticamente o eCatalog de várias páginas PDF (opcional)** Selecione esta opção para criar automaticamente um eCatalog ao fazer upload. Você pode ir diretamente para a tela eCatalog e começar a trabalhar no eCatalog sem precisar selecionar primeiro arquivos PDF e selecionar o comando Build. O eCatalog recebe o nome do arquivo PDF.

* **Resolução** O Dynamic Media Classic recomenda 150 pixels por polegada.

* **O Colorspace** Dynamic Media Classic recomenda escolher Detectar automaticamente. Normalmente, os PDFs criados para saída de impressão estão em CMYK; Os PDFs para visualização online são RGB. Se um PDF usar ambos os espaços de cor, você pode selecionar um espaço de cor específico escolhendo Forçar como RGB ou Forçar como CMYK. Os PDFs usam ambos os espaços de cor, por exemplo, quando os gráficos de página usam um espaço de cor CMYK, mas as imagens usam RGB. Se você tiver carregado um perfil ICC, seu nome será exibido no menu Espaço de cores e você poderá escolhê-lo lá.

   Consulte perfis [](icc-profiles.md#icc_profiles)ICC.

* **Perfil de cores** Escolha uma opção Perfil de cores:

* **ConvertTo SRGB** Converte em SRGB (Padrão Vermelho Verde Azul). SRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

* **Manter espaço** de cor original Retém o espaço de cor original.

* **Menus Personalizado de > Para** abrir para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Dynamic Media Classic.

Consulte perfis [](icc-profiles.md#icc_profiles)ICC.

>[!NOTE]
>
>Para obter detalhes sobre todas as opções de PDF, consulte Opções [de upload de](pdfs.md#pdf_upload_options)PDF.

