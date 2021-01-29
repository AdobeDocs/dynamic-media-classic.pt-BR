---
title: Configuração de predefinições de imagens
description: Saiba como configurar as predefinições de imagens.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 10%

---


# Configuração de predefinições de imagens{#setting-up-image-presets}

Como uma macro, uma predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos com um nome. Para entender como as predefinições de imagens funcionam, suponha que seu site exija que cada imagem de produto apareça em dois tamanhos diferentes: 500 x 500 pixels e 150 x 150 pixels. Você cria duas predefinições de imagens, uma chamada &quot;Ampliar&quot; para exibir imagens a 500x500 pixels e outra chamada &quot;Miniatura&quot; para exibir imagens a 150 x 150 pixels. Para fornecer imagens nos tamanhos &quot;Ampliar&quot; e &quot;Miniatura&quot;, o Dynamic Media Image Server procura a definição de Predefinição de ampliação de imagem e Predefinição de miniatura de imagem. Em seguida, o servidor gera dinamicamente uma imagem no tamanho e nas especificações de formatação de cada predefinição de imagem.

O Dynamic Media Classic vem com várias predefinições de imagens de &quot;prática recomendada&quot; que já estão configuradas para você usar. Os administradores também podem criar novas predefinições de imagens. Para criar uma predefinição de imagem, é possível criar um start do zero ou start de um existente e salvá-lo com um novo nome.

As imagens que são reduzidas em tamanho quando são entregues dinamicamente de um servidor podem perder nitidez e detalhes. Por esse motivo, cada predefinição de imagem contém controles de formatação para otimizar uma imagem quando ela é entregue em um tamanho específico. Esses controles garantem que suas imagens sejam nítidas e claras quando forem entregues ao seu site ou aplicativo.

## Criando uma predefinição de imagem {#creating-an-image-preset}

Você pode criar suas próprias predefinições de imagens se for um administrador de empresas. Você pode criar novas predefinições de imagens ou start com uma predefinição de imagens padrão fornecida pelo Dynamic Media Classic, editá-los e salvá-los com um novo nome.

**Para criar uma predefinição de imagem**

1. Clique em **Configuração** > **Predefinições de imagem**.

   Você pode navegar até um nome de predefinição de imagem nesta tela para pré-visualização de uma predefinição de imagem existente. Quando você seleciona um nome de Predefinição de imagem, a imagem de amostra na janela Pré-visualização muda de tamanho e aparência.

1. Execute um dos procedimentos a seguir:

   * **Criação de uma**
predefinição de imagemClique em Adicionar.

   * **Edição de uma**
predefinição de imagemNavegue até a predefinição de imagem mais parecida com a que você deseja criar e clique em Editar.

1. Digite um nome para a predefinição de imagem.
1. Insira medidas de Largura e Altura em pixels. Essas medidas determinam o tamanho no qual as imagens são entregues.
1. Preencha a tela Adicionar predefinição ou Editar predefinição. Para obter detalhes, consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

   O Dynamic Media Classic recomenda estas opções de &quot;prática recomendada&quot; para o start:

   * ****
FormatoEscolha JPEG ou outro formato que atenda aos seus requisitos. Todos os navegadores da Web são compatíveis com o formato de imagem JPEG; ele oferece um bom equilíbrio entre arquivos pequenos e qualidade de imagem. No entanto, as imagens no formato JPEG usam um esquema de compactação com perdas que pode apresentar artefatos de imagem indesejados se a configuração de compactação for muito baixa. Por esse motivo, o Dynamic Media Classic recomenda definir a qualidade de compactação (no controle deslizante) como 75. Essa configuração oferece um bom equilíbrio entre a qualidade da imagem e o tamanho pequeno de arquivo.

   * ****
NitidezNão selecione Nitidez (este filtro de nitidez oferta menos controle do que as configurações de Mascaramento com nitidez).

   * **Modo**
de nova amostraEscolha Bi-Cubic.

   * **Opções**
de máscara de nitidez (USM)Insira as configurações mostradas aqui:
   | Tipo predefinido | Tamanho | USM: Valor | USM: Raio | USM: Limiar |
   |--- |--- |--- |--- |--- |
   | Venda cruzada (miniatura) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 3 | 5 |
   | Principal | 350 x 350 | 3 | 3 | 6 |
   | Ampliar | 500 x 500 | 1,2 | 1,2 | 5 |

1. Clique em **Salvar**.

As opções de &quot;prática recomendada&quot; do Dynamic Media Classic para criar predefinições de imagens listadas aqui são recomendações gerais. a nitidez é altamente subjetiva. Estas definições de &quot;melhores práticas&quot; basearam-se numa imagem principal de 2000 x 2000; as configurações para mestres maiores ou menores podem ser diferentes. Se você quiser ajustar as configurações de Mascaramento de nitidez, o Dynamic Media Classic recomenda estes intervalos:

* ****
Valor entre 0,8 e 1,5.

* ****
Raio entre 0,6 e 2.

* ****
Limite De 1 A 6.

Para excluir uma predefinição de imagem, selecione-a na tela Predefinições de imagem e selecione o botão Excluir.

>[!MORELIKETHIS]
>
>* [Criar e editar predefinições de imagens](application-setup.md#creating_and_editing_image_presets)
>* [Opções de predefinição de imagem](application-setup.md#image_preset_options)
>* [Visualizar um ativo de imagem com base em sua predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

