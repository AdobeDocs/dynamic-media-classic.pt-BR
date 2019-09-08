---
title: Fazer upload dos arquivos PDF
seo-title: Fazer upload dos arquivos PDF
description: 'null'
seo-description: Saiba como carregar os arquivos PDF associados a um ecatalog.
uuid: 9 e 178 bb 2-ac 09-427 a-b 61 a-aad 4 e 87 a 5837
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0097 cba 5-c 886-4115-bc 35-7 ae 7 a 500202 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Fazer upload dos arquivos PDF{#uploading-the-pdf-files}

Geralmente, os arquivos Adobe PDF são a fonte de um ecatalog; esses arquivos contêm todas as informações da imagem, bem como fontes e gráficos vetoriais. Também é possível criar um ecatalog com imagens. Depois de preparar os arquivos PDF para upload, selecione o botão Carregar na barra Navegação global para começar a fazer upload dos pdfs.

## Preparação de arquivos PDF {#preparing-your-pdf-files}

Prepare seus arquivos PDF antes de carregá-los no Sistema de publicação Scene 7:

* Coloque todos os arquivos na mesma pasta do computador ou rede para facilitar o carregamento dos arquivos.
* Nomeie os arquivos em ordem alfanumérica por página. A ordenação das páginas facilitará colocar as páginas na ordem correta depois que os arquivos são carregados.
* Examine as páginas de PDF para verificar se eles contêm marcas de corte, metas de registro ou barras de cores. Essas marcas determinam onde recortar o papel quando documentos são impressos; devem ser removidos antes que seu ecatalog seja colocado na Web. O Dynamic Media Classic fornece opções para recortar marcas quando você carrega arquivos PDF.
* Se quiser que os visualizadores pesquisem seu ecatalog por palavra-chave, descubra se os arquivos PDF são «nivelados. » Não é possível extrair palavras de pesquisa de arquivos PDF nivelados. Para descobrir se um PDF é nivelado, tente selecionar o texto dentro dele. Se não for possível selecionar o texto, o PDF será nivelado e os visualizadores não poderão pesquisar por palavra-chave no seu catálogo.
* Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. Por padrão, o SPS pode detectar de forma inteligente essas imagens CMYK e convertê-las usando um perfil de cores CMYK interno. No entanto, se você quiser usar um perfil de cores personalizado para converter imagens CMYK, poderá fazê-lo.

   Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

## Opções recomendadas de upload de Pdf {#best-practice-pdf-upload-options}

Para obter informações detalhadas sobre os diferentes métodos de upload, consulte [Upload de arquivos](uploading-files.md#uploading_your_files).

Selecione os arquivos que deseja carregar e, em seguida, selecione estas *Práticas de* PDF recomendadas:

**Cortar** Selecione o menu Cortar e escolha Manual se as páginas contiverem marcas de corte, marcas de registro ou outras marcas. Insira o número de pixels para cortar dos lados superior, direito, inferior e esquerdo das páginas. As marcas de corte geralmente são definidas para uma margem de meia polegada. Supondo que você escolha 150 como a resolução de pixel por polegada (a configuração recomendada), digitar 75, 75, 75, 75 nas caixas de texto Superior, Direita, Inferior e Esquerda corta uma metade da margem das margens (a 150 ppi, metade de uma polegada equivale a 75 pixels).

**Processando** Selecione o menu Processamento e escolha Rasterizar. O arquivo PDF deve ser rasterizado para que todas as páginas e imagens possam ser exibidas no ecatalog.

**Extrair palavras de pesquisa (opcional)** Selecione essa opção se quiser que os visualizadores possam pesquisar por palavra-chave em seu ecatalog.

**Gerar automaticamente o ecatalog de várias páginas PDF (opcional)** Selecione esta opção para criar automaticamente um ecatalog ao carregar. Você pode ir diretamente para a tela ecatalog e começar a trabalhar em seu ecatalog sem precisar selecionar primeiro arquivos PDF e selecionar o comando Build. O ecatalog é nomeado após seu arquivo PDF.

**Resolução** Dynamic Media Classic recomenda 150 pixels por polegada.

**O Colorspace** Dynamic Media Classic recomenda escolher Detectar automaticamente. Geralmente, os pdfs criados para saída impressa estão em CMYK; Os pdfs para visualização online são RGB. Se um PDF usar ambos os espaços de cor, você pode selecionar um espaço de cores específico escolhendo Forçar como RGB ou Forçar como CMYK. Os pdfs usam espaços de cor, por exemplo, quando gráficos de página usam um espaço de cores CMYK, mas imagens usam RGB. Se você carregou um perfil ICC, seu nome aparece no menu Espaço colorido e você pode escolhê-lo lá.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

**Opção Perfil** de cor escolha uma opção Perfil de cor:

**Converter
em SRGB** converte para SRGB (Vermelho vermelho padrão). O SRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter Espaço original de cor** retém o espaço de cores original.

**Personalizado de &gt; Para** abrir menus para que você possa escolher um espaço de cores Converter de e Converter para. É possível escolher um espaço de cor padrão do Photoshop ou um espaço de cores carregado no SPS.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para obter detalhes sobre todas as opções de PDF, consulte [Opções de upload de PDF](pdfs.md#pdf_upload_options).

