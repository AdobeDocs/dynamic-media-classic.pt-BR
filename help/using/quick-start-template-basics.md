---
title: "Início rápido: Noções básicas do modelo"
description: Uma introdução e um Início rápido das noções básicas de modelo para ajudar você a começar a usar o Adobe Dynamic Media Classic com rapidez.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# Início rápido: Noções básicas de modelo{#quick-start-template-basics}

Noções básicas de modelo são arquivos de imagem em camadas criados dinamicamente e endereçáveis, como arquivos em camadas em aplicativos de edição de imagens, como o Adobe Photoshop. Diferentemente de um arquivo estático contendo camadas, como um arquivo PSD, um modelo pode incluir parâmetros. Por meio de parâmetros, os diferentes aspectos da imagem podem ser abordados e personalizados.

Um modelo pode conter qualquer número de camadas de imagem e camadas de texto. É possível converter um arquivo estático contendo camadas, como um arquivo de PSD em camadas, em um modelo e criar modelos no Adobe Dynamic Media Classic. É possível criar camadas de texto em modelos usando fontes carregadas no Adobe Dynamic Media Classic. Depois de adicionar texto a um modelo, é possível formatá-lo alterando sua justificação, sua fonte, tamanho da fonte e cor.

Usando a página Parâmetros, você pode converter qualquer aspecto de um modelo em um parâmetro endereçável. Ao fazer isso, você pode alterar qual imagem em camada usar ou qual valor de texto usar no modelo. Os parâmetros são passados com a string do URL, permitindo alterar qualquer parâmetro para personalizar dinamicamente a imagem de resposta gerada no Servidor de imagens.

Veja também o vídeo de treinamento [Noções básicas do modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

Esse Início rápido foi projetado para colocar suas operações em funcionamento rapidamente com os Conceitos básicos sobre modelos.

## 1. Fazer upload dos arquivos

Comece fazendo upload do arquivo PSD ou arquivo de imagem para seu modelo. O Adobe Dynamic Media Classic é compatível com muitos formatos de arquivo de imagem além do PSD, mas imagens TIFF e PNG sem perdas são recomendadas para modelos porque permitem transparência.

Se você estiver usando um arquivo PSD para criar seu modelo, selecione **[!UICONTROL Create Template]** na caixa de diálogo **[!UICONTROL Upload Job Options]** ao carregar o arquivo PSD. Escolha também uma opção **[!UICONTROL Layer Naming]** para que o Adobe Dynamic Media Classic saiba como nomear camadas de PSD quando elas forem carregadas no Adobe Dynamic Media Classic.

Se estiver usando arquivos de imagem, você pode cortar as imagens e também criar uma máscara dos caminhos de recorte nas imagens ao carregá-las.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar um arquivo de PSD ou outros arquivos de imagem do seu computador para uma pasta no Adobe Dynamic Media Classic. Consulte [Carregar arquivos de modelo](uploading-template-files.md#uploading_template_files).

## 2. Criar um modelo

Para criar um modelo a partir de um arquivo PSD, selecione **[!UICONTROL Create Template]** ao carregar o arquivo. Para criar um modelo a partir de imagens, na barra Navegação Global, vá para **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**, insira uma medida de largura e altura para a tela. Próximo ao canto superior direito da página, selecione **[!UICONTROL Designer]** ou **[!UICONTROL Developer]** e arraste imagens para a página Modelo. Você também pode selecionar as imagens *antes* de **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. A página Modelo oferece ferramentas para:

* Adição de camadas de imagem. Para adicionar uma camada, arraste uma imagem para a página Modelo.
* Adicionar camadas de texto. Selecione o ícone **[!UICONTROL Text tool]**. Arraste o ponteiro para criar uma caixa para a camada de texto e formate o texto com as ferramentas na página Texto.
* Alteração do tamanho e da posição das camadas.
* Alteração da ordem das camadas.
* Aplicação de efeitos de sombra e brilho em camadas de imagem e texto.

Consulte [Criar um modelo](creating-template.md#creating_a_template).

## 3. Criar parâmetros de modelo

A próxima etapa é parametrizar as propriedades nas camadas para determinar quais propriedades de camada são incluídas na string do URL. Os parâmetros permitem usar modelos do com o máximo de flexibilidade. Depois de transformar uma propriedade de camada em um parâmetro, é possível alterá-la dinamicamente.

Para parametrizar uma camada, abra o modelo na página Modelo e selecione **[!UICONTROL Parameters]** ao lado do nome de uma camada. Na página Parâmetros, selecione a opção ao lado de cada parâmetro que deseja adicionar. Consulte [Criar parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

## 4. Modelos do Publish

A publicação do modelo o coloca nos Dynamic Media Image Servers para que ele possa ser entregue dinamicamente ao seu site ou aplicativo. A publicação também ativa o URL para chamar o modelo dos Servidores de imagem Dynamic Media para o site ou aplicativo.

Certifique-se de publicar todas as imagens associadas ao modelo.

Para publicar um modelo, marque-o para publicação e, na barra Navegação global, selecione **[!UICONTROL Publish]**. Depois selecione **[!UICONTROL Submit Publish]**. Consulte [modelos do Publish](publishing-templates.md#publishing_templates).

## 5. Vincular um modelo a uma página da Web

O Dynamic Media Classic cria URLs para modelos e ativa os URLs ao publicar modelos nos Dynamic Media Image Servers. Você pode copiar essas cadeias de caracteres de URL da página Visualização de modelo.

Selecione seu modelo no painel Procurar e selecione **[!UICONTROL Preview]** para abrir a página Visualização de Modelo. Escolha uma Predefinição de imagem para fornecer seu modelo e clique no botão **[!UICONTROL Copy URL]**. Depois de copiar o URL da página de Visualização, você pode usá-lo no site ou no aplicativo. Consulte [Vincular um modelo a uma página da Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
