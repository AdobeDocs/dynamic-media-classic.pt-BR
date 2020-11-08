---
title: '"Start rápido: Noções básicas sobre o modelo"'
seo-title: '"Start rápido: Noções básicas sobre o modelo"'
description: nulo
seo-description: Uma introdução e Start rápido para as noções básicas sobre modelo para ajudá-lo a começar a trabalhar rapidamente.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# Start rápido: Noções básicas sobre o modelo{#quick-start-template-basics}

As noções básicas do modelo são criadas dinamicamente e arquivos de imagem em camadas endereçáveis, como arquivos em camadas em aplicativos de edição de imagens, como o Adobe Photoshop. Ao contrário de um arquivo estático que contém camadas, como um arquivo PSD, um modelo pode incluir parâmetros. Por meio de parâmetros, os diferentes aspectos da imagem podem ser abordados e personalizados.

Um modelo pode conter qualquer número de camadas de imagem e camadas de texto. É possível converter um arquivo estático contendo camadas, como um arquivo PSD em camadas, em um modelo, bem como criar modelos no Dynamic Media Classic. Você pode criar camadas de texto em modelos usando fontes que foram carregadas no Dynamic Media Classic. Depois de adicionar texto a um modelo, é possível formatá-lo alterando sua justificação, fontes, tamanho da fonte e cor.

Usando a tela Parâmetros, é possível converter qualquer aspecto de um modelo em um parâmetro endereçável. Ao fazer isso, você pode alterar qual imagem em camadas usar ou qual valor de texto usar no modelo. Os parâmetros são passados com a string de URL, permitindo que você altere qualquer parâmetro para personalizar dinamicamente a imagem de resposta gerada do servidor de imagem.

**Start rápido**

Este Start rápido foi projetado para começar a funcionar rapidamente com as Informações básicas sobre modelos.

**1. Carregar os arquivos**

Start fazendo upload do arquivo PSD ou de imagem para seu modelo. O Dynamic Media Classic é compatível com vários formatos de arquivo de imagem além do PSD, mas imagens TIFF e PNG sem perdas são recomendadas para modelos, pois permitem transparência.

Se você estiver usando um arquivo PSD para criar seu modelo, selecione a opção Criar modelo na caixa de diálogo Carregar opções de trabalho ao carregar o arquivo PSD. Além disso, escolha uma opção Nomenclatura de camada para informar ao Dynamic Media Classic como nomear camadas PSD quando elas forem carregadas para o Dynamic Media Classic.

Se você estiver usando arquivos de imagem, poderá recortar as imagens e também criar uma máscara a partir de caminhos de recorte nas imagens à medida que as carrega.

Selecione o botão Carregar na barra de navegação global para carregar um arquivo PSD ou outros arquivos de imagem do computador para uma pasta no Dynamic Media Classic. Consulte [Upload de arquivos](uploading-template-files.md#uploading_template_files)de modelo.

**2. Criar um modelo**

Para criar um modelo a partir de um arquivo PSD, selecione a opção Criar modelo ao carregar o arquivo. Para criar um modelo a partir de imagens, escolha Criar > Noções básicas do modelo, insira uma medida de largura e altura para a tela, selecione Designer ou Desenvolvedor e arraste as imagens para a tela Modelo. Você também pode selecionar as imagens antes de escolher Criar > Noções básicas do modelo. A tela Modelo oferta ferramentas para:

* Adicionando camadas de imagem. Para adicionar uma camada, arraste uma imagem para a tela Modelo.
* Adicionar camadas de texto. Selecione a ferramenta Texto e arraste para desenhar uma caixa para a camada de texto; em seguida, formate o texto com ferramentas na tela Texto.
* Alteração do tamanho e da posição das camadas.
* Alteração da ordem das camadas.
* Aplicar efeitos de sombra e brilho a camadas de imagem e texto.

Consulte [Criação de um modelo](creating-template.md#creating_a_template).

**3. Criar parâmetros de modelo**

A próxima etapa é parametrizar as propriedades em camadas para determinar quais propriedades de camada estão incluídas na string de URL. Os parâmetros permitem usar modelos com máxima flexibilidade. Depois de transformar uma propriedade de camada em um parâmetro, é possível alterá-la dinamicamente.

Para parametrizar uma camada, abra o modelo na tela Modelo e selecione o botão Parâmetros ao lado de um nome de camada. Na tela Parâmetros, selecione a opção ao lado de cada parâmetro que deseja adicionar. Consulte [Criação de parâmetros](creating-template-parameters.md#creating_template_parameters)de modelo.

**4. Publicar modelos**

A publicação do seu modelo o coloca em Servidores de Imagem de Mídia Dinâmica para que ele possa ser entregue dinamicamente ao seu site ou aplicativo. A publicação também ativa o URL para chamar o modelo dos Servidores de Imagem de Mídia Dinâmica para seu site ou aplicativo.

Certifique-se de publicar todas as imagens associadas ao seu modelo.

Para publicar um modelo, marque-o para publicação e selecione o botão Publicar na barra Navegação global. Em seguida, selecione o botão Publicar Start. Consulte [Publicação de modelos](publishing-templates.md#publishing_templates).

**5. Vincular um modelo a uma página da Web**

O Dynamic Media Classic cria URLs para modelos e ativa os URLs quando você publica modelos em Servidores de Imagem de Mídia Dinâmica. É possível copiar essas sequências de URL da tela Pré-visualização Modelo.

Selecione seu modelo no Painel de navegação e clique no botão Pré-visualização para abrir a tela Pré-visualização do modelo. Em seguida, escolha uma predefinição de imagem para entregar seu modelo e selecione o botão Copiar URL. Depois de copiar o URL da tela de Pré-visualização, você pode usá-lo em seu site ou aplicativo. Consulte [Vincular um modelo a uma página](linking-template-web-page.md#linking_a_template_to_a_web_page)da Web.
