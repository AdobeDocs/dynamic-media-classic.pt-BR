---
title: Configuração de predefinições de imagens
seo-title: Configuração de predefinições de imagens
description: 'null'
seo-description: Saiba como configurar predefinições de imagens.
uuid: 90530948-dee 9-41 bd-b 39 e -684140446 abc
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/image_ sizing
discoiquuid: 1 ec 39 fe 5-7 b 2 a -4034-9570-6 b 5595 f 97052
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Configuração de predefinições de imagens{#setting-up-image-presets}

Como uma macro, uma predefinição de imagem é uma coleção predefinida de comandos de tamanho e formatação salvos com um nome. Para compreender como as Predefinições de imagens funcionam, suponha que o site da Web exija que cada imagem do produto seja exibida em dois tamanhos diferentes: 500 x 500 pixels e 150 x 150 pixels. Você cria duas predefinições de imagens, uma chamada «Ampliar» para exibir imagens com 500 x 500 pixels e outra chamada «Miniatura» para exibir imagens a 150 x 150 pixels. Para fornecer imagens no tamanho «Ampliar» e «Miniatura», um Servidor de imagem do Dynamic Media analisa a definição da Predefinição de imagem ampliada e da predefinição de imagem em miniatura. Em seguida, o servidor gera dinamicamente uma imagem nas especificações de tamanho e formatação de cada predefinição de imagem.

O Dynamic Media Classic apresenta várias «práticas recomendadas» que já estão configuradas para você usar. Os administradores também podem criar novas predefinições de imagens. Para criar uma predefinição de imagem, você pode começar do zero ou pode começar de uma existente e salvá-la com um novo nome.

Imagens que são reduzidas em tamanho quando são entregues dinamicamente a partir de um servidor podem perder nitidez e detalhes. Por esse motivo, cada Predefinição de imagem contém controles de formatação para otimizar uma imagem quando ela é entregue em um tamanho específico. Esses controles garantem que suas imagens sejam nítidas e claras quando são entregues ao seu site ou aplicativo.

## Criar uma predefinição de imagem {#creating-an-image-preset}

Você pode criar suas próprias Predefinições de imagens se for um administrador da empresa. Você pode criar novas Predefinições de imagens ou iniciar com uma predefinição de imagem padrão que o Dynamic Media Classic fornece, editá-la e salvá-la com um novo nome.

**Para criar uma predefinição de imagem**

1. Clique **em Configuração** &gt; **Predefinições de imagens**.

   Você pode navegar até um nome de Predefinição de imagem nesta tela para visualizar uma predefinição de imagem existente. Quando um nome de Predefinição de imagem é selecionado, a imagem de amostra na janela Visualizar muda o tamanho e a aparência.

1. Execute um dos procedimentos a seguir:

   **Criando uma
predefinição de imagem** Clique em Adicionar.

   **Editando uma predefinição** de imagem Navegue até a predefinição de imagem que você deseja criar e clique em Editar.

1. Insira um nome para a Predefinição de imagem.
1. Insira medições de Largura e Altura em pixels. Essas medições determinam o tamanho em que as imagens são entregues.
1. Preencha a tela Adicionar predefinição ou Editar predefinição. Para obter detalhes, consulte [Opções de predefinição de imagens](application-setup.md#image_preset_options).

   O Dynamic Media Classic recomenda que as opções de «práticas recomendadas» sejam iniciadas:

   **Formatar** escolha JPEG ou outro formato que atenda às suas necessidades. Todos os navegadores da Web suportam o formato de imagem JPEG; oferece um bom equilíbrio entre tamanhos pequenos de arquivos e qualidade de imagem. No entanto, as imagens de formato JPEG usam um esquema de compactação com perdas que pode inserir artefatos de imagem indesejados se a configuração de compactação for muito baixa. Por esse motivo, o Dynamic Media Classic recomenda definir a qualidade de compactação (no controle deslizante) para 75. Essa configuração oferece um bom equilíbrio entre qualidade de imagem e tamanho de arquivo pequeno.

   **Nitidez** não selecione Nitidez (esse filtro de nitidez oferece menos controle do que as configurações de Máscara de nitidez).

   **Modo de reamostragem** selecione Bi-Cubic.

   **Opções de máscara unsharp (USM)** Insira as configurações mostradas aqui:

   | Tipo de predefinido | Tamanho | USM: Quantia | USM: Raio | USM: Limite |
   |--- |--- |--- |--- |--- |
   | Venda cruzada (mini-miniatura) | 75 x 75 | 1.5 | 0.8 | 5 |
   | Miniatura | 150 x 150 | 1.1 | 1 | 5 |
   | Principal | 350 x 350 | 1 | 1 | 6 |
   | Ampliar | 500 x 500 | 1.2 | 1.2 | 5 |

1. Clique **em Salvar**.

As opções de «práticas recomendadas» do Dynamic Media para criar predefinições de imagens listadas aqui são recomendações gerais; a nitidez é altamente subjetiva. Essas configurações de «práticas recomendadas» foram baseadas em uma imagem mestre de 2000 x 2000; as configurações para estres maiores ou menores podem ser diferentes. Se você quiser ajustar as configurações de Máscara de nitidez, o Dynamic Media Classic recomenda estes intervalos:

**Quantidade** entre .8 e 1.5.

**Raio** entre .6 e 2.

**Limite** de 1-6.

Para excluir uma predefinição de imagem, selecione-a na tela Predefinições de imagens e selecione o botão Excluir.

>[!MORELIKETHIS]
>
>* [Criar e editar predefinições de imagens](application-setup.md#creating_and_editing_image_presets)
>* [Opções de predefinição de imagens](application-setup.md#image_preset_options)
>* [Visualização de um ativo de imagem com base na predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

