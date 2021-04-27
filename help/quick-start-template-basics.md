---
title: '"Início rápido: Noções básicas sobre modelo"'
description: Uma introdução e o Início rápido para as noções básicas do modelo para ajudá-lo a ativar e executar rapidamente.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Início rápido: Noções básicas do modelo{#quick-start-template-basics}

As Noções básicas sobre o modelo são arquivos de imagem em camadas criados dinamicamente e endereçáveis, como arquivos em camadas em aplicativos de edição de imagens, como o Adobe Photoshop. Ao contrário de um arquivo estático contendo camadas, como um arquivo PSD, um modelo pode incluir parâmetros. Por meio de parâmetros, os diferentes aspectos da imagem podem ser abordados e personalizados.

Um modelo pode conter qualquer número de camadas de imagem e camadas de texto. Você pode converter um arquivo estático contendo camadas, como um arquivo PSD em camadas, em um modelo, bem como criar modelos no Dynamic Media Classic. Você pode criar camadas de texto em modelos usando fontes carregadas no Dynamic Media Classic. Após adicionar texto a um modelo, é possível formatá-lo alterando sua justificação, fontes, tamanho da fonte e cor.

Usando a tela Parâmetros , é possível converter qualquer aspecto de um modelo em um parâmetro endereçável. Ao fazer isso, você pode alterar a imagem em camadas a ser usada ou o valor do texto a ser usado no modelo. Os parâmetros são passados com a string do URL, permitindo alterar qualquer parâmetro para personalizar dinamicamente a imagem de resposta gerada do servidor de imagem.

**Início rápido**

Este Início Rápido foi projetado para entrar em operação rapidamente com as Noções básicas sobre Modelo.

**1. Fazer upload dos arquivos**

Comece carregando o arquivo PSD ou o arquivo de imagem para seu modelo. O Dynamic Media Classic é compatível com vários formatos de arquivo de imagem, além do PSD, mas imagens TIFF e PNG sem perdas são recomendadas para modelos, pois permitem transparência.

Se você estiver usando um arquivo PSD para criar seu modelo, selecione a opção Criar modelo na caixa de diálogo Upload de opções de trabalho quando fizer upload do arquivo PSD. Escolha também uma opção de Nomenclatura de Camada para informar ao Dynamic Media Classic como nomear camadas de PSD quando elas forem carregadas no Dynamic Media Classic.

Se estiver usando arquivos de imagem, você pode recortar as imagens e também criar uma máscara a partir de caminhos de recorte nas imagens, conforme você as carrega.

Selecione o botão Fazer upload na barra de navegação global para fazer upload de um arquivo PSD ou outros arquivos de imagem de seu computador para uma pasta no Dynamic Media Classic. Consulte [Upload de arquivos de modelo](uploading-template-files.md#uploading_template_files).

**2. Criar um modelo**

Para criar um modelo a partir de um arquivo PSD, selecione a opção Criar modelo ao fazer upload do arquivo. Para criar um modelo a partir de imagens, escolha Criar > Noções básicas do modelo, insira uma medida de largura e altura para a tela, selecione Designer ou Desenvolvedor e arraste as imagens para a tela Modelo . Você também pode selecionar as imagens antes de escolher Criar > Noções básicas do modelo. A tela Modelo oferece ferramentas para:

* Adição de camadas de imagem. Para adicionar uma camada, arraste uma imagem para a tela Modelo .
* Adição de camadas de texto. Selecione a ferramenta Texto e arraste para desenhar uma caixa para a camada de texto; em seguida, formate o texto com ferramentas na tela Texto .
* Alteração do tamanho e da posição das camadas.
* Alteração da ordem das camadas.
* Aplicar efeitos de sombra e brilho a camadas de imagem e texto.

Consulte [Criação de um modelo](creating-template.md#creating_a_template).

**3. Criar parâmetros de modelo**

A próxima etapa é parametrizar as propriedades nas camadas para determinar quais propriedades de camada são incluídas na cadeia de caracteres do URL. Os parâmetros permitem usar modelos com o máximo de flexibilidade. Depois de transformar uma propriedade de camada em um parâmetro, é possível alterá-la dinamicamente.

Para parametrizar uma camada, abra o modelo na tela Modelo e selecione o botão Parâmetros ao lado do nome da camada. Na tela Parâmetros, selecione a opção ao lado de cada parâmetro que deseja adicionar. Consulte [Criação de parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

**4. Publicar modelos**

A publicação do modelo o coloca nos Servidores de imagem da Dynamic Media para que possa ser entregue dinamicamente ao seu site ou aplicativo. A publicação também ativa o URL para chamar o modelo dos Servidores de imagem da Dynamic Media para o site ou aplicativo.

Certifique-se de publicar todas as imagens associadas ao seu modelo.

Para publicar um modelo, marque-o para publicar e selecione o botão Publicar na barra de navegação global. Em seguida, clique em **[!UICONTROL Submit Publish]**. Consulte [Publicação de modelos](publishing-templates.md#publishing_templates).

**5. Vincular um modelo a uma página da Web**

O Dynamic Media Classic cria URLs para modelos e ativa os URLs quando você publica modelos nos Dynamic Media Image Servers. Você pode copiar essas cadeias de caracteres do URL da tela Visualização do modelo .

Selecione o modelo no Painel de navegação e clique no botão Visualizar para abrir a tela Visualização do modelo . Em seguida, escolha uma Predefinição de imagem para entregar seu modelo e selecione o botão Copiar URL . Depois de copiar o URL da tela de Visualização, você pode usá-lo em seu site ou aplicativo. Consulte [Vincular um modelo a uma página da Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
