---
title: Upload de arquivos PDF
description: Saiba como fazer upload dos arquivos PDF associados a um eCatalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Visualizadores,Catálogo eletrônico
role: Business Practitioner
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---

# Upload dos arquivos PDF{#uploading-the-pdf-files}

Normalmente, os arquivos Adobe PDF são a fonte de um eCatalog. Esses arquivos contêm todas as informações de imagem, fontes e gráficos vetoriais. Você também pode criar um eCatalog com imagens. Depois de preparar os arquivos PDF para upload, selecione o botão Upload na barra de navegação global para começar a carregar os PDFs.

## Preparando seus arquivos PDF {#preparing-your-pdf-files}

Prepare seus arquivos PDF antes de carregá-los no Dynamic Media Classic:

* Para facilitar o upload dos arquivos, coloque todos os arquivos na mesma pasta no computador ou na rede.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará colocar as páginas na ordem correta após os arquivos serem carregados.
* Para ver se as páginas em PDF contêm marcas de corte, destinos de registro ou barras de cores, examine as páginas. Estas marcas determinam onde cortar o papel quando os documentos são impressos; eles devem ser removidos antes que seu eCatalog seja colocado na Web. O Dynamic Media Classic fornece opções para marcas de corte ao carregar arquivos PDF.
* Se você quiser que os visualizadores pesquisem seu eCatalog por palavra-chave, descubra se seus arquivos PDF estão &quot;nivelados&quot;. Não é possível extrair palavras de pesquisa de arquivos PDF nivelados. Para descobrir se um PDF está nivelado, tente selecionar texto dentro dele. Se você não conseguir selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave em seu eCatalog.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o Dynamic Media Classic pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. No entanto, se você quiser usar um perfil de cor personalizado para converter imagens CMYK, poderá fazer isso.

   Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

## Opções de upload de PDF de práticas recomendadas {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de upload, consulte [Fazer upload de seus arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que deseja fazer upload e, em seguida, selecione estas *Opções de PDF de Práticas Recomendadas*:

* ****
RecortarSelecione o menu Recortar e escolha Manual se as páginas contiverem marcas de recorte, marcas de registro ou outras marcas. Insira o número de pixels para cortar a partir dos lados superior, direito, inferior e esquerdo das páginas. As marcas de corte são frequentemente definidas a uma margem de meia polegada. Suponha que você escolha 150 (recomendado) como a resolução de pixel por polegada e digite 75, 75, 75, 75, 75 nas caixas de texto Superior, Direita, Inferior e Esquerda. Nesse caso, ele recorta uma meia polegada das margens (em 150 ppi, metade de 1 é igual a 75 pixels).

* ****
ProcessamentoSelecione o menu Processamento e escolha Rasterizar. O arquivo PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no eCatalog.

* **Extrair palavras de pesquisa (opcional)**
Selecione essa opção se desejar que seus visualizadores possam pesquisar por palavra-chave em seu eCatalog.

* **Gerar automaticamente o catálogo eletrônico a partir de várias páginas em PDF (opcional)**
Selecione esta opção para criar automaticamente um catálogo eletrônico quando fizer upload. Você pode ir direto para a tela eCatalog e começar a trabalhar em seu eCatalog sem precisar primeiro selecionar arquivos PDF e selecionar o comando Criar. O eCatalog é nomeado após seu arquivo PDF.

* ****
Solução O Dynamic Media Classic recomenda 150 pixels por polegada.

* ****
ColorspaceO Dynamic Media Classic recomenda escolher Detectar automaticamente. Geralmente, os PDFs criados para saída de impressão estão em CMYK; Os PDFs para visualização online são RGB. Se um PDF usar ambos os espaços de cores, você poderá selecionar um espaço de cores específico escolhendo Forçar como RGB ou Forçar como CMYK. Os PDFs usam ambos os espaços de cores, por exemplo, quando os gráficos de página usam um espaço de cores CMYK, mas as imagens usam RGB. Se você tiver carregado um perfil ICC, seu nome aparecerá no menu Colorspace e você poderá escolhê-lo lá.

   Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

* **Perfil**
de corEscolha uma opção de Perfil de cor:

* **Converta em**
SRGBConverts para SRGB (Azul Verde Vermelho Padrão). SRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

* **Manter**
espaço de cores originalMantém o espaço de cores original.

* **Personalizar de >**
ParaAbrir menus para poder escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Dynamic Media Classic.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para obter detalhes sobre todas as opções de PDF, consulte [opções de upload de PDF](pdfs.md#pdf_upload_options).
