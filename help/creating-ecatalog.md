---
title: Criar um catálogo eletrônico
description: Saiba como criar um eCatalog no Adobe Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Criação de um catálogo eletrônico {#creating-an-ecatalog}

A criação de um eCatalog implica solicitar as páginas, escolher o layout da página e vincular as páginas, desenhando os Mapas de imagem e inserindo dados de sobreposição e link de hipertexto. Como opção, você pode personalizar o TOC para que os visualizadores vejam nomes de página em vez de números de página no Visualizador de catálogo eletrônico.

## Criar um catálogo eletrônico {#create}

Você pode incluir arquivos de imagem e PDF no seu eCatalog.

Ao criar um eCatalog, o **[!UICONTROL Publish after save]** afeta o conjunto e o conjunto de membros das seguintes maneiras:

| Opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros do conjunto mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um eCatalog:**

1. Comece a criar seu eCatalog com uma destas técnicas:

   * **Selecione os arquivos primeiro** - No Painel Procurar, selecione os arquivos e, em seguida, vá para **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Iniciar a partir da tela Catálogo eletrônico** - Ir para **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Selecione uma pasta na Biblioteca de ativos e arraste os arquivos da pasta até a guia Páginas de pedidos da página eCatalog.

      >[!NOTE]
      >
      >Para exibir os itens na Biblioteca de ativos por nome, em vez de miniatura, selecione a opção Nome para a Exibição da biblioteca de ativos padrão na Configuração pessoal.

1. Selecione um layout geral para seu eCatalog. Selecionar **[!UICONTROL 1 Up]** para páginas únicas, **[!UICONTROL 2 Up]** para páginas espelhadas duplas ou **[!UICONTROL Custom]** para páginas espelhadas de mais de duas páginas. No **[!UICONTROL Change eCatalog Layout]** selecione a caixa de diálogo **[!UICONTROL All Spreads]** e selecione **[!UICONTROL OK]**.
1. Opcionalmente, altere o layout de páginas individuais ou de páginas espelhadas selecionando-as e escolhendo **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** ou **[!UICONTROL Custom]** botão. No **[!UICONTROL Change eCatalog Layout]** selecione a caixa de diálogo **[!UICONTROL Selected Spreads]** e selecione **[!UICONTROL OK]**.
1. Reorganize as páginas conforme necessário com uma dessas técnicas:

   * **Arrastar** - Arraste uma página ou página espelhada para um novo local. A barra vertical mostra onde a página está sendo movida.

   * **Botão Mover para** - Selecione uma página ou página espelhada, selecione **[!UICONTROL Move To]** e escolha a página no menu que deseja que a página apareça antes.

   * **Sequência #** - Na Exibição de lista, insira os números de página nos campos Número da sequência .

1. Quando terminar, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**.
1. Na caixa de diálogo Salvar , selecione uma pasta para armazenar seu eCatalog. No campo Nome do arquivo , insira o nome do conjunto de rotação.
1. Selecionar **[!UICONTROL Save]**.

   Você pode visualizar seu eCatalog, depois de salvá-lo, selecionando **[!UICONTROL Preview]**.

## Editar um catálogo eletrônico {#editing-an-ecatalog}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after save]** afeta o conjunto e o conjunto de membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado. Qualquer novo conjunto de membros adicionado durante a edição manterá o estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto adicionados durante a edição mantêm o estado publicado ou não. |

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um eCatalog:**

1. Selecione a sobreposição do Catálogo eletrônico **[!UICONTROL Edit]** botão.
1. Faça as alterações necessárias.
1. Quando a edição for concluída, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, insira um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um catálogo eletrônico {#deleting-an-ecatalog}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) desse conjunto não são afetados; em vez disso, cada um mantém seu estado publicado ou não publicado.

Consulte também [Publicar ativos manualmente](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um eCatalog:**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais catálogos eletrônicos.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Personalizar o sumário (TOC) {#customizing-the-table-of-contents-toc}

O Adobe Dynamic Media Classic fornece números de página padrão em seu eCatalog na guia Páginas do pedido da tela do eCatalog. Para nomes de página personalizados, você pode alterar os rótulos de página que constituem o sumário (TOC). Recomenda-se renomear a tampa frontal e traseira. Por exemplo, a capa frontal pode ler &quot;Capa&quot; em vez de &quot;Página 0-1&quot;.

Você pode criar um sumário personalizado (TOC) para seu eCatalog manualmente ou importando os nomes de página de um arquivo CSV (somente Mac) ou XML.

>[!NOTE]
>
>Para restaurar os títulos de página padrão, no **[!UICONTROL Order Pages]** guia , selecione **[!UICONTROL TOC Labels]** e selecione **[!UICONTROL Restore Defaults (All)]**.

### Inserção manual de nomes de página {#manually-entering-page-names}

Para inserir manualmente nomes de página, um de cada vez, vá para a guia Páginas do pedido da tela Catálogo eletrônico. Em seguida, no campo número da página , digite um nome para cada página que deseja nomear.

### Importar nomes de página {#importing-page-names}

É recomendável importar nomes de página se você estiver lidando com um eCatalog com muitas páginas. É possível importar os nomes de um arquivo delimitado por tabulação ou XML.

O rótulo TOC é armazenado no campo Dados do usuário de uma imagem; formatar esses dados como uma lista de `name=<value>` ` pairs separated by two question marks “??” `. Por exemplo, para definir um rótulo para um campo TOC chamado `tocEN`, defina os Dados do usuário da imagem como:

`tocEN=&lt;EN_page_label>`

Para definir rótulos separados para campos TOC nomeados `tocEN` e `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Para importar o campo Dados do usuário em um arquivo delimitado por tabulação, inclua os dados do usuário do campo:

| IPSID | Dados do usuário |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Para importar o campo Dados do usuário em um arquivo XML, inclua o atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nomes de página de um arquivo delimitado por tabulação ou XML, selecione a variável **[!UICONTROL TOC Labels]** e selecione **[!UICONTROL Import]**. Na caixa de diálogo Fazer upload de metadados , selecione **[!UICONTROL Browse]** e, em seguida, importe o arquivo CSV (somente Mac) ou o arquivo XML que associa cada página a um nome de página.
