---
title: Configuração de predefinições de imagens
description: Saiba como configurar Predefinições de imagem.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 10%

---

# Configuração de predefinições de imagens{#setting-up-image-presets}

Como uma macro, uma Predefinição de imagem é uma coleção predefinida de comandos de dimensionamento e formatação salvos em um nome. Para entender como as Predefinições de imagem funcionam, suponha que o site exija que cada imagem de produto seja exibida em dois tamanhos diferentes: 500 x 500 pixels e 150 x 150 pixels. Você cria duas Predefinições de imagem, uma chamada &quot;Enlarge&quot; para exibir imagens a 500x500 pixels e outra chamada &quot;Thumbnail&quot; para exibir imagens a 150 x 150 pixels. Para entregar imagens no tamanho &quot;Ampliar&quot; e &quot;Miniatura&quot;, um Servidor de Imagens do Dynamic Media procura a definição da Predefinição de Imagem Ampliada e da Predefinição de Imagem em Miniatura. Em seguida, o servidor gera dinamicamente uma imagem no tamanho e nas especificações de formatação de cada Predefinição de imagem.

O Adobe Dynamic Media Classic vem com várias Predefinições de imagem de &quot;prática recomendada&quot; que já estão configuradas para você usar. Os administradores também podem criar novas Predefinições de imagem. Para criar uma predefinição de imagem, você pode começar do zero ou começar com uma predefinição existente e salvá-la com um novo nome.

As imagens que são reduzidas quando são entregues dinamicamente de um servidor podem perder nitidez e detalhes. Por esse motivo, cada Predefinição de imagem contém controles de formatação para otimizar uma imagem quando ela é entregue em um tamanho específico. Esses controles garantem que suas imagens sejam nítidas e claras quando forem entregues ao seu site ou aplicativo.

## Criação de uma predefinição de imagem {#creating-an-image-preset}

Você pode criar suas próprias Predefinições de imagem se for um administrador da empresa. Você pode criar novas Predefinições de imagem ou começar com uma Predefinição de imagem padrão fornecida pelo Adobe Dynamic Media Classic, editá-la e salvá-la com um novo nome.

**Para criar uma predefinição de imagem:**

1. Clique em **Configurar** > **Predefinições de imagem**.

   Você pode navegar até um nome de predefinição de imagem nessa tela para visualizar uma predefinição de imagem existente. Quando você seleciona um nome de Predefinição de imagem, a imagem de amostra na janela Visualização muda de tamanho e aparência.

1. Siga um destes procedimentos:

   * **Criando uma**
predefinição de imagem Clique em Adicionar.

   * **Editar uma**
predefinição de imagemNavegue até a predefinição de imagem mais parecida com aquela que você deseja criar e clique em Editar.

1. Insira um nome para a predefinição de imagem.
1. Insira as medições de Largura e Altura em pixels. Essas medidas determinam o tamanho no qual as imagens são entregues.
1. Preencha a tela Adicionar predefinição ou Editar predefinição . Para obter detalhes, consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

   O Adobe Dynamic Media Classic recomenda estas opções de &quot;prática recomendada&quot; para iniciar:

   * ****
FormatoEscolha JPEG ou outro formato que atenda aos seus requisitos. Todos os navegadores da Web são compatíveis com o formato de imagem JPEG; ele oferece um bom equilíbrio entre arquivos pequenos e qualidade de imagem. No entanto, as imagens no formato JPEG usam um esquema de compactação com perdas que pode apresentar artefatos de imagem indesejados se a configuração de compactação for muito baixa. Por esse motivo, o Adobe Dynamic Media Classic recomenda definir a qualidade de compactação (no controle deslizante) como 75. Essa configuração oferece um bom equilíbrio entre a qualidade da imagem e o tamanho pequeno de arquivo.

   * ****
Nitidez Não selecione Nitidez (este filtro de nitidez oferece menos controle do que as configurações Tirar nitidez da máscara).

   * **Modo**
de amostraEscolha Bi-Cubic.

   * **Tirar nitidez das**
opções de Mascaramento (USM)Insira as configurações mostradas aqui:
   | Tipo de predefinição | Tamanho | USM: Valor | USM: Raio | USM: Limite |
   |--- |--- |--- |--- |--- |
   | Venda cruzada (miniatura) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1.1. | 1 | 5 |
   | Principal | 350 x 350 | 1 | 1 | 6 |
   | Ampliar | 500 x 500 | 1.2. | 1.2. | 5 |

1. Clique em **Salvar**.

As opções de &quot;prática recomendada&quot; do Adobe Dynamic Media Classic para criar Predefinições de imagem listadas aqui são recomendações gerais; a nitidez é altamente subjetiva. Essas configurações de &quot;práticas recomendadas&quot; foram baseadas em uma imagem principal de 2000 x 2000; as configurações para mestres maiores ou menores podem ser diferentes. Se você quiser ajustar as configurações de Tirar nitidez do mascaramento, o Adobe Dynamic Media Classic recomenda esses intervalos:

* ****
Valor entre 0,8 e 1,5.

* ****
Raio entre 0,6 e 2.

* ****
ThresholdFrom 1-6.

Para excluir uma predefinição de imagem, selecione-a na tela Predefinições de imagem e selecione o botão Excluir.

>[!MORELIKETHIS]
>
>* [Criar e editar predefinições de imagens](application-setup.md#creating_and_editing_image_presets)
>* [Opções de predefinição de imagem](application-setup.md#image_preset_options)
>* [Visualização de um ativo de imagem com base em sua Predefinição de imagem](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

