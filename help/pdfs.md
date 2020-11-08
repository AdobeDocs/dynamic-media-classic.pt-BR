---
title: Como trabalhar com PDFs
seo-title: Como trabalhar com PDFs
description: nulo
seo-description: Saiba como trabalhar com PDFs no Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Como trabalhar com PDFs{#working-with-pdfs}

Os arquivos PDF (Portable Documento Format) são usados com mais frequência no Dynamic Media Classic para criar eCatalogs. Quando você carrega um arquivo PDF, o Dynamic Media Classic rasteriza ou remove as páginas por padrão para que as páginas possam ser usadas para criar mídia avançada.

## Opções de upload de PDF {#pdf-upload-options}

Ao carregar um arquivo PDF, você pode formatá-lo de várias maneiras. Você corta suas páginas, extrai palavras de pesquisa, digita uma resolução de pixels por polegada e escolhe um espaço de cor. Os arquivos PDF geralmente contêm uma margem de aparagem, marcas de corte, marcas de registro e marcas de outra impressora. É possível recortar essas marcas dos lados das páginas ao carregar um arquivo PDF.

As opções para fazer upload de arquivos PDF estão localizadas na tela Fazer upload em Opções de PDF.

**Processamento**

As opções de Processamento são as seguintes:

**Rasterizar** (Padrão) Limpa as páginas no arquivo PDF e converte gráficos vetoriais em imagens de bitmap. Escolha essa opção para criar um eCatalog.

**Extrair palavras** de pesquisa Extrai palavras do arquivo PDF para que o arquivo possa ser pesquisado por palavra-chave em um eCatalog Viewer.

**Extrair links** extrai links dos arquivos PDF e os converte em mapas de imagem usados em um eCatalog Viewer.

**Gerar eCatalog automaticamente com PDF** de várias páginas cria automaticamente um eCatalog a partir do arquivo PDF. O eCatalog recebe o nome do arquivo PDF que você carregou. Essa opção só estará disponível se você rasterizar o arquivo PDF ao carregá-lo.

**Resolução**

Determina a configuração de resolução. Essa configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

**Espaço da cor**

Selecione o menu Espaço de cor e escolha um espaço de cor para o arquivo PDF. A maioria dos arquivos PDF tem imagens coloridas RGB e CMYK. O espaço de cores RGB é preferível para visualização online.

**Detectar automaticamente** retém o espaço de cor do arquivo PDF.

**Forçar como RGB** converte para o espaço de cores RGB.

**Forçar como CMYK** converte para o espaço de cores CMYK.

**Forçar como conversão em escala de cinza** no espaço de cores em escala de cinza.

**Perfil de cores**

Escolha uma opção de Perfil de cor:

**Converter em sRGB** converte em sRGB (Padrão Vermelho Verde Azul). O sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter espaço** de cor original Mantém o espaço de cor original.

**Os menus Personalizado de > Para** abre para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores padrão do Photoshop ou um espaço de cores carregado no Dynamic Media Classic.

Consulte perfis [](icc-profiles.md#icc_profiles)ICC.

## Recortar espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para recortar automaticamente pixels de espaço em branco de um arquivo PDF ao carregá-lo, selecione o menu Recortar e escolha Aparar.
1. Especifique as seguintes opções:

   **ApararCom** base emEscolha se deseja cortar com base na cor ou na transparência:

   **Cor** Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto do PDF com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

   **Transparência** Escolha a opção Transparência.

   **Tolerância** Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

   **Aparar com base na cor** Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PDF. Números próximos a 1 permitem mais diferenças de cor.

   **Aparar com base na transparência** Especifique 0 para cortar pixels somente se eles forem totalmente transparentes. números mais próximos de 1 permitem mais transparência.

## Recortar das laterais das páginas do PDF {#cropping-from-the-sides-of-pdf-pages}

É possível remover manualmente as marcas da impressora das laterais das páginas em um arquivo PDF ao carregá-lo.

1. Selecione o menu Cortar e escolha Manual.
1. Insira as configurações de pixel nas caixas de texto Superior, Direita, Inferior e Esquerda para cortar da parte superior, inferior e laterais das páginas.

A quantidade de páginas cortadas depende da configuração Resolution PX/Inch inserida para o arquivo PDF. Por exemplo, se você digitar 150 (o padrão) como a configuração Resolução PX/Polegada e cortar 75 pixels das laterais das páginas, meia polegada será cortada porque, a 150 pixels por polegada, 75 pixels equivale a meia polegada.
