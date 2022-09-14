---
title: "Início rápido: Noções básicas sobre modelo"
description: Uma introdução e o Início rápido para as noções básicas do modelo para ajudá-lo a ativar e executar rapidamente no Adobe Dynamic Media Classic.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Início rápido: Noções básicas do modelo{#quick-start-template-basics}

As Noções básicas sobre o modelo são arquivos de imagem em camadas criados dinamicamente e endereçáveis, como arquivos em camadas em aplicativos de edição de imagens, como o Adobe Photoshop. Ao contrário de um arquivo estático contendo camadas, como um arquivo PSD, um modelo pode incluir parâmetros. Por meio de parâmetros, os diferentes aspectos da imagem podem ser abordados e personalizados.

Um modelo pode conter qualquer número de camadas de imagem e camadas de texto. Você pode converter um arquivo estático contendo camadas, como um arquivo de PSD em camadas, em um modelo e criar modelos no Adobe Dynamic Media Classic. Você pode criar camadas de texto em modelos usando fontes carregadas no Adobe Dynamic Media Classic. Após adicionar texto a um modelo, é possível formatá-lo alterando sua justificação, fontes, tamanho da fonte e cor.

Usando a página Parâmetros , é possível converter qualquer aspecto de um template em um parâmetro endereçável. Ao fazer isso, você pode alterar a imagem em camadas a ser usada ou o valor do texto a ser usado no modelo. Os parâmetros são passados com a string do URL, permitindo alterar qualquer parâmetro para personalizar dinamicamente a imagem de resposta gerada do servidor de imagem.

Consulte também [Noções básicas do modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de treinamento.

Este Início Rápido foi projetado para ajudá-lo a ativar e executar rapidamente com as Noções básicas sobre modelo.

## 1. Faça upload dos arquivos

Comece carregando o arquivo PSD ou de imagem do seu modelo. O Adobe Dynamic Media Classic suporta muitos formatos de arquivo de imagem além do PSD, mas imagens TIFF e PNG sem perdas são recomendadas para modelos, pois permitem transparência.

Se estiver usando um arquivo PSD para criar seu modelo, selecione **[!UICONTROL Create Template]** no **[!UICONTROL Upload Job Options]** ao fazer upload do arquivo PSD. Escolha também uma **[!UICONTROL Layer Naming]** para que a Adobe Dynamic Media Classic saiba como nomear camadas de PSD quando são carregadas no Adobe Dynamic Media Classic.

Se estiver usando arquivos de imagem, você pode recortar as imagens e também criar uma máscara a partir de caminhos de recorte nas imagens, conforme você as carrega.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para carregar um arquivo PSD ou outros arquivos de imagem de seu computador para uma pasta no Adobe Dynamic Media Classic. Consulte [Upload de arquivos de modelo](uploading-template-files.md#uploading_template_files).

## 2. Criar um modelo

Para criar um modelo a partir de um arquivo PSD, selecione **[!UICONTROL Create Template]** ao fazer upload do arquivo. Para criar um modelo a partir de imagens, na barra Navegação global, acesse **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**, insira uma medida de largura e altura para a tela. Ao lado do canto superior direito da página, selecione **[!UICONTROL Designer]** ou **[!UICONTROL Developer]** e arraste as imagens até a página Modelo . Também é possível selecionar as imagens *before* você vai para **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. A página Modelo oferece ferramentas para:

* Adição de camadas de imagem. Para adicionar uma camada, arraste uma imagem para a página Modelo.
* Adição de camadas de texto. Selecione o **[!UICONTROL Text tool]** ícone . Arraste o ponteiro para criar uma caixa para a camada de texto; em seguida, formate o texto com ferramentas na página Texto .
* Alteração do tamanho e da posição das camadas.
* Alteração da ordem das camadas.
* Aplicar efeitos de sombra e brilho a camadas de imagem e texto.

Consulte [Criar um modelo](creating-template.md#creating_a_template).

## 3. Criar parâmetros de modelo

A próxima etapa é parametrizar as propriedades nas camadas para determinar quais propriedades de camada são incluídas na cadeia de caracteres do URL. Os parâmetros permitem usar modelos com o máximo de flexibilidade. Depois de transformar uma propriedade de camada em um parâmetro, é possível alterá-la dinamicamente.

Para parametrizar uma camada, abra o modelo na página Modelo e selecione **[!UICONTROL Parameters]** ao lado de um nome de camada. Na página Parâmetros , selecione a opção ao lado de cada parâmetro que deseja adicionar. Consulte [Criar parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

## 4. Publicar modelos

A publicação do modelo o coloca nos Servidores de imagem da Dynamic Media para que possa ser entregue dinamicamente ao seu site ou aplicativo. A publicação também ativa o URL para chamar o modelo dos Servidores de imagem da Dynamic Media para o site ou aplicativo.

Certifique-se de publicar todas as imagens associadas ao seu modelo.

Para publicar um modelo, marque-o para publicação e, na barra Navegação global, selecione **[!UICONTROL Publish]**. Em seguida, selecione **[!UICONTROL Submit Publish]**. Consulte [Publicar modelos](publishing-templates.md#publishing_templates).

## 5. Vincular um modelo a uma página da Web

O Dynamic Media Classic cria URLs para modelos e ativa os URLs ao publicar modelos nos Dynamic Media Image Servers. Você pode copiar essas cadeias de caracteres do URL da página Visualização do modelo .

Selecione o modelo no Painel de navegação e selecione **[!UICONTROL Preview]** para abrir a página Visualização do modelo . Escolha uma predefinição de imagem para entregar seu modelo e selecione **[!UICONTROL Copy URL]**. Depois de copiar o URL da página de Visualização, você pode usá-lo em seu site ou aplicativo. Consulte [Vincular um modelo a uma página da Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
