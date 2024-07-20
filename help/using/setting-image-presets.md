---
title: Configurar predefinições da imagem
description: Saiba como configurar predefinições de imagem no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 1%

---

# Configurar predefinições da imagem{#setting-up-image-presets}

Como uma macro, uma Predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos com um nome. Para entender como as Predefinições de imagem funcionam, suponha que seu site exija que cada imagem de produto seja exibida em dois tamanhos diferentes: 500 × 500 pixels e 150 × 150 pixels. Você cria duas Predefinições de imagem, uma chamada &quot;Ampliar&quot; para exibir imagens a 500x500 pixels e outra chamada &quot;Miniatura&quot; para exibir imagens a 150 × 150 pixels. Para fornecer imagens no tamanho &quot;Ampliar&quot; e &quot;Miniatura&quot;, um Servidor de imagens do Dynamic Media pesquisa a definição de &quot;Ampliar predefinição de imagem&quot; e &quot;Predefinição de imagem em miniatura&quot;. Em seguida, o servidor gera dinamicamente uma imagem com as especificações de tamanho e formatação de cada Predefinição de imagem.

O Adobe Dynamic Media Classic vem com várias Predefinições de imagem de &quot;prática recomendada&quot; que já estão configuradas para você usar. Os administradores também podem criar Predefinições de imagem. Para criar uma Predefinição de imagem, comece do zero ou a partir de uma predefinição existente e salve com um novo nome.

Imagens com tamanho reduzido quando são entregues dinamicamente de um servidor podem perder nitidez e detalhes. Por esse motivo, cada Predefinição de imagem contém controles de formatação para otimizar uma imagem quando ela é entregue em um tamanho específico. Esses controles garantem que suas imagens sejam nítidas e claras quando forem entregues ao seu site ou aplicativo.

## Criar uma predefinição de imagem {#creating-an-image-preset}

Você poderá criar suas próprias Predefinições de imagem se for um Administrador da empresa. É possível criar Predefinições de imagem ou começar com uma Predefinição de imagem padrão fornecida pelo Adobe Dynamic Media Classic, editá-la e salvá-la com um novo nome.

**Para criar uma Predefinição de Imagem:**

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

   É possível navegar até o nome de uma Predefinição de imagem nessa tela para visualizar uma Predefinição de imagem existente. Quando você seleciona um nome de Predefinição de imagem, a imagem de amostra na janela Visualização muda de tamanho e aparência.

1. Siga um destes procedimentos:

   * **Criar uma Predefinição de Imagem**: Selecione **[!UICONTROL Add]**.
   * **Editar uma Predefinição de Imagem**: Navegue até a Predefinição de Imagem mais parecida com a que você deseja criar e selecione **[!UICONTROL Edit]**.

1. Insira um nome para a Predefinição de imagem.
1. Insira as medidas de Largura e Altura em pixels. Essas medidas determinam o tamanho em que as imagens são entregues.
1. Preencha a tela Adicionar predefinição ou Editar predefinição. Para obter detalhes, consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

   A Adobe Dynamic Media Classic recomenda que essas opções de &quot;práticas recomendadas&quot; comecem:

   * **[!UICONTROL Format]**: Escolha JPEG ou outro formato que atenda aos seus requisitos. Todos os navegadores da Web são compatíveis com o formato de imagem JPEG; ele oferece um bom equilíbrio entre arquivos pequenos e qualidade de imagem. No entanto, as imagens de JPEG usam um esquema de compactação com perdas que pode apresentar artefatos de imagem indesejados se a configuração de compactação for muito baixa. Por esse motivo, a Adobe Dynamic Media Classic recomenda definir a qualidade de compactação (no controle deslizante) como 75. Essa configuração oferece um bom equilíbrio entre a qualidade da imagem e o tamanho pequeno de arquivo.

   * **[!UICONTROL Sharpening]**: Não selecione Nitidez (este filtro de nitidez oferece menos controle do que as configurações de **[!UICONTROL Unsharp Masking]**).

   * **[!UICONTROL Resample Mode]**: Escolha **[!UICONTROL Bi-Cubic]**.

   * **[!UICONTROL Unsharp Masking]** (USM): insira as seguintes configurações:

   | Tipo de predefinição | Tamanho | USM: Quantidade | USM: Raio | USM: Limite |
   | --- | --- | --- | --- | --- |
   | Venda cruzada (miniminiminiatura) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 × 150 | 1,1 | 1 | 5 |
   | Principal | 350 × 350 | 1 | 1 | 6 |
   | Ampliar | 500 × 500 | 1,2 | 1,2 | 5 |

1. Selecione **[!UICONTROL Save]**.

As opções de &quot;prática recomendada&quot; do Adobe Dynamic Media Classic para criar Predefinições de imagem listadas aqui são recomendações gerais; a nitidez é altamente subjetiva. Essas configurações de &quot;práticas recomendadas&quot; foram baseadas em uma imagem primária de 2000 × 2000; as configurações para arquivos primários maiores ou menores podem ser diferentes. Se você quiser ajustar as configurações Tirar nitidez da máscara, a Adobe Dynamic Media Classic recomenda estes intervalos:

* **[!UICONTROL Amount]**: Entre `.8` e `1.5`.

* **[!UICONTROL Radius]**: Entre `.6` e `2`.

* **[!UICONTROL Threshold]**: De `1` até `6`.

Para excluir uma Predefinição de imagem, selecione-a na tela Predefinições de imagem e selecione **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Criar e editar Predefinições de Imagem](application-setup.md#creating_and_editing_image_presets)
>* [Opções de predefinição de imagem](application-setup.md#image_preset_options)
>* [Visualizar um ativo de imagem com base em sua Predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
