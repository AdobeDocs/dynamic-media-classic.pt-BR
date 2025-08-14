---
title: Exibição do Trabalho em Detalhes
description: Saiba como trabalhar na Exibição de detalhes no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Exibição do Trabalho em Detalhes{#working-in-detail-view}

Você pode trabalhar com e aprender sobre um ativo abrindo-o na Exibição de detalhes. Na Exibição detalhada, você pode ver o tamanho do ativo, os atributos, os derivados e os metadados. Você também pode ver se e quando o ativo foi publicado e obter o URL dos ativos publicados. Dependendo do tipo de ativo, é possível visualizá-lo em tamanhos diferentes, ampliá-lo e executar operações de nitidez, corte e outras operações de formatação.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Exibição detalhada](/help/using/assets/image_0.img.png)
*Exibição detalhada com o painel Biblioteca de ativos oculto na exibição à esquerda.*

>[!NOTE]
>
>Para abrir a pasta onde o ativo está armazenado, selecione o caminho da pasta na parte superior do painel Informações.

## Abra um ativo na Exibição de detalhes {#open-an-asset-in-detail-view}

É possível exibir um ativo na Exibição de detalhes para examinar, visualizar ou trabalhar detalhadamente nele.

1. No painel Procurar, execute um dos procedimentos a seguir:

   * Selecione o ativo. Próximo ao canto superior direito do Adobe Dynamic Media Classic, selecione o ícone **[!UICONTROL Detail View]**.
   * Clique duas vezes no ativo.
   * Selecione o ativo e vá para **[!UICONTROL File]** > **[!UICONTROL Details]**.

>[!NOTE]
>
>É possível paginar de ativo a ativo na mesma pasta da Exibição de detalhes. Basta clicar em **[!UICONTROL Previous Asset]** ou **[!UICONTROL Next Asset]**. Esses botões estão no canto superior direito da Exibição de detalhes.

## Obter informações na Exibição de detalhes {#getting-information-in-detail-view}

A Exibição de detalhes fornece informações sobre um ativo ou arquivo. Essas informações são exibidas sobre um item: a pasta onde ele está armazenado, seu nome de arquivo, a data em que o item foi carregado para o Adobe Dynamic Media Classic e seu histórico de publicação. Também é possível exibir e editar metadados e adicionar palavras-chave para um ativo na Exibição de detalhes.

É possível obter um URL do ativo na Exibição de detalhes; no entanto, o URL não estará ativo até que você publique o ativo. Para imagens, a Exibição de detalhes também fornece uma lista de ativos e metadados criados e derivados, como Destinos de zoom e Conjuntos de imagens.

## Trabalhar com ativos na Exibição de detalhes {#working-with-assets-in-detail-view}

A Exibição de detalhes oferece ferramentas para trabalhar com o ativo que você abriu. As ferramentas disponíveis dependem do tipo de ativo com o qual você está trabalhando, mas a Exibição de detalhes sempre oferece estas funções:

* **itens para publicação**: selecione o ícone **[!UICONTROL `Publish`]** à esquerda do nome ou vá para **[!UICONTROL File]** > **[!UICONTROL Publish]** ou **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

* **Renomear o ativo**: selecione o nome e insira um novo nome.

* **Editar e adicionar metadados**: selecione o painel Metadados e altere conforme desejado. Consulte [Exibir, adicionar e exportar metadados](/help/using/viewing-adding-exporting-metadata.md).

* **Editar e adicionar palavras-chave**: selecione Palavras-chave e adicione-as ou remova-as conforme desejado. Consulte [Adicionar ou editar palavras-chave](/help/using/viewing-adding-exporting-metadata.md).

* **Excluir o ativo**: Vá para **[!UICONTROL File]** > **[!UICONTROL Delete]**.

Para arquivos discretos (imagens, conjuntos de imagens e fontes, por exemplo), é possível exibir o histórico de publicação e edição e verificar os detalhes da tarefa na Exibição detalhada.

Esta tabela mostra quais outras opções estão disponíveis com diferentes tipos de ativos na Exibição de detalhes.

| Tipo de ativo | Editar/ajustar | Visualizar |
| --- | --- | --- |
| Imagens | Adicionar Mapas de Imagem<br>Adicionar Destinos de Zoom<br>Cortar<br>Nitidez<br>Criar modos de exibição ajustados | Sim; Predefinições de zoom e imagem |
| Imagens de revestimento de gabinete e janela | Não | Miniatura |
| eCatalogs | Editar | Sim<br>O Painel de Informações também está disponível |
| Fontes | Editar informações da fonte | Não |
| Arquivos FXG | Editar | Sim |
| Perfis ICC | Editar informações de perfil | Não |
| Arquivos Illustrator | Não (a menos que convertido em FXG) | Não |
| Conjuntos de imagem | Editar | Sim |
| Arquivos do InDesign | Não (a menos que convertido em FXG) | Não |
| Arquivos do PDF | Não | Não |
| Arquivos do PSD | Sim para camadas individuais | Sim para camadas individuais |
| Conjuntos de rotação | Editar | Sim |
| Arquivos do SVG | Não | Não |
| Modelos | Editar | Sim |
| Vídeos | Não | Sim |
| Vinhetas e vinhetas fundidas | Não | A imagem é mostrada<br>Você pode exibir o conteúdo e a estrutura dos elementos renderizáveis da vinheta no formato XML |
| Arquivos XML | Não | O conteúdo é mostrado |
| Arquivos ZIP | Não | O conteúdo não é exibido |

>[!MORELIKETHIS]
>
>* [Exibir, adicionar e exportar metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
