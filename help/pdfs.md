---
title: Trabalhar com pdfs
seo-title: Trabalhar com pdfs
description: 'null'
seo-description: Saiba como trabalhar com pdfs no Dynamic Media Classic.
uuid: 26 d 70 d 28-9393-49 b 1-9051-d 70456 deca 67
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 5 a 073 de 3-6 b 1 d -4 c 3 e -8 c 03-9182 f 9 f 3874 a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Trabalhar com pdfs{#working-with-pdfs}

Os arquivos PDF (Portable Document Format) são usados com mais frequência no Dynamic Media Classic para criar ecatalogs. Quando você carrega um arquivo PDF, o Dynamic Media Classic rasteriza, ou faz rips, as páginas por padrão para que as páginas possam ser usadas para criar mídia avançada.

## Opções de upload de PDF {#pdf-upload-options}

Quando você carrega um arquivo PDF, pode formatá-lo de várias maneiras. Recorte suas páginas, extraia palavras de pesquisa, digite uma resolução de pixels por polegada e escolha um espaço de cores. Os arquivos PDF geralmente contêm uma margem de aparagem, marcas de corte, marcas de registro e outras marcas da impressora. É possível recortar essas marcas dos lados das páginas enquanto você carrega um arquivo PDF.

As opções para fazer upload de arquivos PDF estão localizadas na tela Carregar em Opções de PDF.

**Processamento**

As opções de Processamento são as seguintes:

**Rasterizar** (Padrão) Rila as páginas no arquivo PDF e converte gráficos vetoriais em imagens bitmap. Escolha essa opção para criar um ecatalog.

**Extrair palavras de pesquisa** Extrai palavras do arquivo PDF para que o arquivo possa ser pesquisado por palavra-chave em um Visualizador do ecatalog.

**Extrair links** extrai links dos arquivos PDF e os divide em Mapas de imagem usados em um Visualizador do ecatalog.

**O arquivo de geração automática de catálogo com várias páginas PDF** cria automaticamente um ecatalog a partir do arquivo PDF. O ecatalog é nomeado após o arquivo PDF carregado. Essa opção estará disponível apenas se você rasterizar o arquivo PDF enquanto o carrega.

**Resolução**

Determina a configuração de resolução. Essa configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

**Espaço da cor**

Selecione o menu Espaço de cor e escolha um espaço de cor para o arquivo PDF. A maioria dos arquivos PDF possuem imagens coloridas RGB e CMYK. O espaço de cores RGB é preferível à exibição online.

**Detectar Retém automaticamente** o espaço de cores do arquivo PDF.

**Forçar como RGB** converte para o espaço de cores RGB.

**Forçar como CMYK** converte para o espaço de cores CMYK.

**Forçar como escala de cinza** para o espaço de cor em Tons de cinza.

**Perfil de cor**

Escolha uma opção Perfil de cor:

**Converter em srgb** converte para srgb (Azul vermelho padrão). O srgb é o espaço de cores recomendado para exibir imagens em páginas da Web.

**Manter Espaço original de cor** retém o espaço de cores original.

**Personalizado de &gt; Para** abrir menus para que você possa escolher um espaço de cores Converter de e Converter para. É possível escolher um espaço de cor padrão do Photoshop ou um espaço de cores carregado no SPS.

Consulte [Perfis ICC](icc-profiles.md#icc_profiles).

## Recortar o espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para cortar automaticamente pixels de espaço em branco de um arquivo PDF enquanto o carrega, selecione o menu Cortar e escolha Aparar.
1. Especifique as seguintes opções:

   **Aparar com base em** Escolher se deseja cortar com base em cor ou transparência:

   **Cor** Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto do PDF com a cor que representa melhor a cor de espaço em branco que você deseja cortar.

   **Opção Transparência** escolha a opção Transparência.

   **Tolerância** Arraste o controle deslizante para especificar uma tolerância de 0 a 1:

   **Aparar com base em cor** Especifique 0 para cortar os pixels apenas se eles corresponderem exatamente à cor selecionada no canto do PDF. Números mais próximos a 1 permitem mais diferença de cor.

   **Aparar com base na transparência** especificada 0 para cortar pixels apenas se eles forem totalmente transparentes; os números mais próximos a 1 permitem mais transparência.

## Recortar dos lados das páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Você pode remover manualmente as marcas da impressora das laterais de um arquivo PDF enquanto o carrega.

1. Selecione o menu Cortar e escolha Manual.
1. Insira as configurações de pixel nas caixas de texto Superior, Direito, Inferior e Esquerda para cortar das páginas superior, inferior e lateral das páginas.

A quantidade de cortes da página depende da configuração PX/Polegada da resolução que você inserir para o arquivo PDF. Por exemplo, se você digitar 150 (o padrão) como a configuração PX/Polegada Resolução e cortar 75 pixels dos lados das páginas, uma meia polegada será cortada porque, a 150 pixels por polegada, 75 pixels equivale a meia polegada.
