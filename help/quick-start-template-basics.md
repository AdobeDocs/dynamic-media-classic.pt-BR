---
title: '" Início rápido: Noções básicas para o modelo "'
seo-title: '" Início rápido: Noções básicas para o modelo "'
description: 'null'
seo-description: Uma introdução e Início rápido às noções básicas do modelo para ajudá-lo a começar a usar rapidamente.
uuid: 16 d 78 cbb-f 762-4263-aea 9-5712 eb 933693
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/template_ basics
discoiquuid: dd 0 fbb 39-3 f 6 a -496 b-a 9 b 6-63 b 11 dcb 823 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Início rápido: Noções básicas para o modelo{#quick-start-template-basics}

As noções básicas de modelo são arquivos de imagem criados dinamicamente e arquivos de imagem que podem ser acessados como arquivos em camadas nos aplicativos de edição de imagens, como o Adobe Photoshop. Diferentemente de um arquivo estático contendo camadas, como um arquivo PSD, um modelo pode incluir parâmetros. Por meio dos parâmetros, os diferentes aspectos da imagem podem ser abordados e personalizados.

>[!NOTE]
>
>Você também pode criar modelos de designs baseados em layout usando Publicação modelo e arquivos do Adobe Illustrator e do Adobe indesign. Consulte [Publicação](quick-start-template-publishing.md) de modelo.

Um modelo pode conter qualquer número de camadas de imagem e camadas de texto. É possível converter um arquivo estático contendo camadas, como um arquivo PSD em camadas, em um modelo, bem como criar modelos no Dynamic Media Classic. É possível criar camadas de texto em modelos usando fontes que você carregou no SPS. Depois de adicionar texto a um modelo, é possível formatá-lo alterando sua justificação, fontes, tamanho da fonte e cor.

Usando a tela Parâmetros, é possível converter qualquer aspecto de um modelo em um parâmetro endereçável. Dessa forma, você pode alterar a imagem em camadas a ser usada ou qual valor de texto usar no modelo. Os parâmetros são passados com a sequência de caracteres do URL, permitindo alterar qualquer parâmetro para personalizar dinamicamente a imagem de resposta gerada do servidor de imagem.

**Início rápido**

Este Início rápido foi criado para começar a usar rapidamente as Noções básicas de modelo.

**1. Carregar os arquivos**

Comece carregando o arquivo PSD ou o arquivo de imagem para seu modelo. O Dynamic Media Classic oferece suporte a muitos formatos de arquivo de imagem além do PSD, mas as imagens TIFF e PNG sem perdas são recomendadas para modelos, pois permitem transparência.

Se estiver usando um arquivo PSD para criar seu modelo, selecione a opção Criar modelo na caixa de diálogo Fazer upload das opções de trabalho ao carregar o arquivo PSD. Escolha também uma opção de Nomenclatura de camada para informar o Dynamic Media Classic como nomear camadas PSD quando eles forem carregados no Sistema de publicação Scene 7.

Se você estiver usando arquivos de imagem, poderá recortar as imagens e criar uma máscara de traçados de recorte nas imagens enquanto os carrega.

Selecione o botão Carregar na barra Navegação global para carregar um arquivo PSD ou outros arquivos de imagem do seu computador para uma pasta no SPS. Consulte [Carregar arquivos de modelo](uploading-template-files.md#uploading_template_files).

**2. Criar um modelo**

Para criar um modelo a partir de um arquivo PSD, selecione a opção Criar modelo ao carregar o arquivo. Para criar um modelo a partir de imagens, escolha Criar &gt; Noções básicas de modelo, insira uma medida de largura e altura para a tela, selecione Designer ou Desenvolvedor e arraste imagens até a tela Modelo. Você também pode selecionar as imagens antes de escolher Build &gt; Noções básicas do modelo. A tela Modelo oferece ferramentas para:

* Adicionar camadas de imagens. Para adicionar uma camada, arraste uma imagem para a tela Modelo.
* Adicionar camadas de texto. Selecione a ferramenta Texto e arraste para desenhar uma caixa para a camada de texto; em seguida, formate o texto com ferramentas na tela Texto.
* Alteração do tamanho e da posição das camadas.
* Alteração da ordem das camadas.
* Aplicar efeitos de sombra e brilho a camadas de imagens e texto.

Consulte [Criar um modelo](creating-template.md#creating_a_template).

**3. Criar parâmetros de modelo**

A próxima etapa é exemplificar as propriedades em camadas para determinar quais propriedades de camada são incluídas na sequência de caracteres do URL. Os parâmetros permitem que você use modelos com flexibilidade máxima. Depois de colocar uma propriedade de camada em um parâmetro, é possível alterá-la dinamicamente.

Para colorir uma camada, abra o modelo na tela Modelo e selecione o botão Parâmetros próximo ao nome da camada. Na tela Parâmetros, selecione a opção ao lado de cada parâmetro que você deseja adicionar. Consulte [Criar parâmetros de modelo](creating-template-parameters.md#creating_template_parameters).

**4. Publicar modelos**

Publicar seu modelo o coloca em servidores de imagem do Dynamic Media para que ele possa ser fornecido dinamicamente em seu site ou aplicativo. A publicação também ativa o URL para chamar o modelo de Servidores de imagem do Dynamic Media a seu site ou aplicativo.

Certifique-se de publicar todas as imagens associadas ao seu modelo.

Para publicar um modelo, marque-o para publicar e selecione o botão Publicar na barra Navegação global. Em seguida, selecione o botão Iniciar publicação. Consulte [Publicação de modelos](publishing-templates.md#publishing_templates).

**5. Vincular um modelo a uma página da Web**

O Dynamic Media Classic cria urls para modelos e ativa os urls quando você publica modelos em servidores de imagem do Dynamic Media. É possível copiar essas sequências de URL da tela Visualização do modelo.

Selecione o modelo no Painel Procurar e clique no botão Visualizar para abrir a tela Visualização do modelo. Em seguida, escolha uma Predefinição de imagem para entregar seu modelo e selecionar o botão Copiar URL. Depois de copiar o URL da tela Visualizar, você pode usá-lo em seu site ou aplicativo. Consulte [Vincular um modelo a uma página da Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
