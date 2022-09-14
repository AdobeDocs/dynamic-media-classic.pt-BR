---
title: Trabalhar na exibição de detalhes
description: Saiba como trabalhar na Exibição de detalhes no Adobe Dynamic Media Classic.
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Trabalhar na exibição de detalhes{#working-in-detail-view}

Você pode trabalhar com e aprender sobre um ativo abrindo-o na Exibição de detalhes. Na Exibição de detalhes, você verá o tamanho do ativo, atributos, derivados e metadados. Você também pode ver se e quando o ativo foi publicado e pode obter o URL dos ativos publicados. Dependendo do tipo de ativo, é possível visualizá-lo em tamanhos diferentes, ampliar e executar operações de nitidez, recorte e outras operações de formatação.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Exibição de detalhes](/help/assets/image_0.img.png)
*Exibição de detalhes com o painel Biblioteca de ativos oculta da exibição no lado esquerdo.*

>[!NOTE]
>
>Para abrir a pasta onde o ativo está armazenado, você pode selecionar o caminho da pasta na parte superior do painel Informações.

## Abra um ativo na Exibição de detalhes {#open-an-asset-in-detail-view}

Para examinar, visualizar ou trabalhar em um ativo detalhadamente, você pode exibi-lo na Exibição de detalhes.

1. No painel Procurar, siga um destes procedimentos:

   * Selecione o ativo. Ao lado do canto superior direito da Adobe Dynamic Media Classic, selecione o **[!UICONTROL Detail View]** ícone .
   * Clique duas vezes no ativo.
   * Selecione o ativo e vá para **[!UICONTROL File]** > **[!UICONTROL Details]**.

>[!NOTE]
>
>Você pode criar uma página de ativo para ativo na mesma pasta na Exibição de detalhes selecionando **[!UICONTROL Previous Asset]** ou **[!UICONTROL Next Asset]**. Esses botões estão no canto superior direito na Exibição de detalhes.

## Obter informações na Exibição de detalhes {#getting-information-in-detail-view}

A Exibição de detalhes fornece informações sobre um ativo ou arquivo. Ele mostra estas informações sobre um item: a pasta onde está armazenado, seu nome de arquivo, a data em que o item foi carregado no Adobe Dynamic Media Classic e seu histórico de publicação. Você também pode exibir e editar metadados e adicionar palavras-chave a um ativo na Exibição de detalhes.

Você pode obter um URL de ativo na Exibição de detalhes; no entanto, o URL não fica ativo até que você publique o ativo. Para imagens, a Exibição de detalhes também fornece uma lista de ativos e metadados de criação e derivados, como destinos de zoom e Conjuntos de imagens.

## Trabalhar com ativos na Exibição de detalhes {#working-with-assets-in-detail-view}

A Exibição de detalhes oferece ferramentas para trabalhar com o ativo que você abriu. As ferramentas disponíveis dependem do tipo de ativo com o qual você está trabalhando, mas a Exibição de detalhes sempre oferece estas funções:

* **itens para publicar** - Selecione o **[!UICONTROL Publish]** à esquerda do nome ou vá para **[!UICONTROL File]** > **[!UICONTROL Publish]** ou **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

* **Renomear o ativo** - Selecione o nome e insira um novo nome.

* **Editar e adicionar metadados** - Selecione o painel Metadados e altere conforme desejado. Consulte [Exibir, adicionar e exportar metadados](/help/viewing-adding-exporting-metadata.md).

* **Editar e adicionar palavras-chave** - Selecione Palavras-chave e adicione ou remova-as conforme desejado. Consulte [Adicionar ou editar palavras-chave](/help/viewing-adding-exporting-metadata.md).

* **Excluir o ativo** - Ir para **[!UICONTROL File]** > **[!UICONTROL Delete]**.

Para arquivos discretos — imagens, conjuntos de imagens e fontes, por exemplo — é possível visualizar o histórico de publicação e edição e verificar os detalhes da tarefa, na Exibição de detalhes.

Esta tabela mostra quais outras opções estão disponíveis com diferentes tipos de ativos na Exibição de detalhes.

| Tipo de ativo | Editar/ajustar | Visualizar |
| --- | --- | --- |
| Imagens | Adicionar mapas de imagem<br>Adicionar metas de zoom<br>Cortar<br>Nitidez<br>Criar visualizações ajustadas | Sim; Predefinições de zoom e imagem |
| Imagens de capa de gabinete e de janela | Não | Miniatura |
| Catálogos eletrônicos | Editar | Sim<br>O Painel Informações também está disponível |
| Fontes | Editar informações de fonte | Não |
| Arquivos FXG | Editar | Sim |
| Perfis ICC | Editar informações de perfil | Não |
| Arquivos Illustrator | Não (exceto quando convertido em FXG) | Não |
| Conjuntos de imagens | Editar | Sim |
| Arquivos InDesign | Não (exceto quando convertido em FXG) | Não |
| Arquivos PDF | Não | Não |
| Arquivos PSD | Sim para camadas individuais | Sim para camadas individuais |
| Conjuntos de rotação | Editar | Sim |
| Arquivos SVG | Não | Não |
| Modelos | Editar | Sim |
| Vídeos | Não | Sim |
| Vinhetas e vinhetas renderizadas | Não | A imagem é mostrada<br>Você pode exibir o conteúdo e a estrutura dos elementos renderizáveis da vinheta no formato XML |
| Arquivos XML | Não | O conteúdo é mostrado |
| Arquivos ZIP | Não | O conteúdo não é mostrado |

>[!MORELIKETHIS]
>
>* [Exibir, adicionar e exportar metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

