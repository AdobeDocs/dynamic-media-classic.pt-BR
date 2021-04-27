---
title: Como trabalhar com PDFs
description: Saiba como trabalhar com PDFs no Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Trabalhar com PDFs{#working-with-pdfs}

Os arquivos PDF (Portable Document Format) são usados com mais frequência no Dynamic Media Classic para criar catálogos eletrônicos. Ao fazer upload de um arquivo PDF, o Dynamic Media Classic rasteriza ou extrai as páginas por padrão, para que as páginas possam ser usadas para criar mídia avançada.

## Opções de upload de PDF {#pdf-upload-options}

Ao carregar um arquivo PDF, você pode formatá-lo de várias maneiras. Você recorta suas páginas, extrai palavras de pesquisa, digita uma resolução de pixels por polegada e escolhe um espaço de cores. Os arquivos PDF geralmente contêm uma margem de corte, marcas de corte, marcas de registro e outras marcas de impressora. É possível recortar essas marcas das laterais das páginas ao carregar um arquivo PDF.

As opções para fazer upload de arquivos PDF estão na página Fazer upload em Opções de PDF.

### Opções de processamento

**Rasterizar**  - (Padrão) Ripsa as páginas no arquivo PDF e converte gráficos vetoriais em imagens bitmap. Para criar um eCatalog, escolha essa opção.

**Extrair palavras de pesquisa**  - Extrai palavras do arquivo PDF para que o arquivo possa ser pesquisado por palavras-chave em um visualizador de eCatalog.

**Extrair links**  - Extrai links dos arquivos PDF e os converte em mapas de imagens usados em um visualizador de eCatalog.

**Gerar catálogo eletrônico automaticamente com PDF de várias páginas**  - Cria automaticamente um catálogo eletrônico a partir do arquivo PDF. O eCatalog é nomeado após o arquivo PDF que você carregou. (Essa opção só estará disponível se você rasterizar o arquivo PDF ao carregá-lo.)

### Resolução

Determina a configuração de resolução. Essa configuração determina quantos pixels são exibidos por polegada no arquivo PDF. O padrão é 150.

### Opções de Espaço de cor

Selecione o menu Espaço de cores e escolha um espaço de cores para o arquivo PDF. A maioria dos arquivos PDF tem imagens coloridas RGB e CMYK. O espaço de cores RGB é preferível para visualização online.

* **Detectar automaticamente**  - Mantém o espaço de cores do arquivo PDF.

* **Forçar como RGB**  - Converte para o espaço de cores RGB.

* **Forçar como CMYK**  - Converte para o espaço de cores CMYK.

* **Forçar como escala de cinza**  - Converte para o espaço de cores da escala de cinza.

### Opções de perfil de cor

* **Converter em sRGB**  - Converte em sRGB (Azul Verde Vermelho Padrão). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

* **Manter espaço de cor original**  - Mantém o espaço de cor original.

* **Personalizado de > Para**  - abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Você pode escolher um espaço de cores Photoshop padrão ou um espaço de cores carregado no Dynamic Media Classic.

Consulte também [Perfis ICC](/help/icc-profiles.md#icc_profiles).

## Recortar espaço em branco de um arquivo PDF {#cropping-white-space-from-a-pdf-file}

1. Para cortar automaticamente pixels de espaço em branco de um arquivo PDF à medida que você o carrega, selecione o menu Recortar e escolha Aparar.
1. Especifique as seguintes opções:

   * **Aparar com base em**  - Escolha se deseja recortar com base na cor ou na transparência:

   * **Cor**  - Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto do PDF com a cor que melhor representa a cor do espaço em branco que deseja recortar.

   * **Transparência**  - Escolha a opção Transparência.

   * **Tolerância**  - Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

   * **Aparar com base na cor**  - Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto do PDF. Os números mais próximos de 1 permitem mais diferenças de cor.

   * **Aparar com base na transparência**  - Especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos de 1 permitem mais transparência.

## Recortar das laterais das páginas PDF {#cropping-from-the-sides-of-pdf-pages}

Você pode remover manualmente as marcas da impressora das laterais das páginas em um arquivo PDF à medida que você o carrega.

1. No menu Cortar, clique em **[!UICONTROL Manual]**.
1. Insira as configurações de pixel nas caixas de texto Superior, Direita, Inferior e Esquerda para cortar da parte superior, inferior e laterais das páginas.

A quantidade de páginas cortadas depende da configuração de Resolução PX/Inch inserida para o arquivo PDF. Por exemplo, se você digitar 150 (padrão) como a configuração Resolução PX/Polegada e cortar 75 pixels das laterais das páginas, meia polegada será cortada; a 150 pixels por polegada, 75 pixels é igual a meia polegada.
