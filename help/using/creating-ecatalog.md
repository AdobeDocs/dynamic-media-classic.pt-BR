---
title: Criar um eCatalog
description: Saiba como criar um eCatalog no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Criação de um eCatalog {#creating-an-ecatalog}

A criação de um eCatalog implica ordenar as páginas, escolher o layout de página e vincular as páginas desenhando Mapas de imagem. Também requer a inserção de dados de sobreposição e link de hipertexto. Como opção, você pode personalizar o índice para que os visualizadores vejam os nomes das páginas em vez dos números das páginas no Visualizador de eCatalog.

## Criar um eCatalog {#create}

Você pode incluir arquivos de imagem e arquivos PDF no eCatalog.

Ao criar um eCatalog, a variável **[!UICONTROL Publish after a save]** opção afeta os membros set e set das seguintes maneiras:

| A opção &quot;Publicar após salvar&quot; foi selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos mantêm seu estado publicado ou não publicado. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um eCatalog:**

1. Comece a criar seu eCatalog com uma destas técnicas:

   * **Selecione os arquivos primeiro**: No painel Procurar, selecione os arquivos e vá para **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Iniciar na tela eCatalog**: Vá para **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Selecione uma pasta na Biblioteca de ativos. Arraste os arquivos da pasta para a guia Ordenar páginas da página eCatalog.

     >[!NOTE]
     >
     >Para exibir os itens na Biblioteca de ativos por nome em vez de miniatura, selecione a opção Nome para Exibição da biblioteca de ativos padrão em Configuração pessoal.

1. Selecione um layout geral para o eCatalog. Selecionar **[!UICONTROL 1 Up]** para páginas únicas, **[!UICONTROL 2 Up]** para páginas espelhadas duplas ou **[!UICONTROL Custom]** para páginas espelhadas superiores a duas. No **[!UICONTROL Change eCatalog Layout]** , selecione a **[!UICONTROL All Spreads]** e selecione **[!UICONTROL OK]**.
1. Opcionalmente, altere o layout de páginas individuais ou de páginas espelhadas selecionando-as e, em seguida, escolhendo **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** ou **[!UICONTROL Custom]** botão. No **[!UICONTROL Change eCatalog Layout]** , selecione a **[!UICONTROL Selected Spreads]** e selecione **[!UICONTROL OK]**.
1. Reordene as páginas conforme necessário com uma destas técnicas:

   * **Arrastando**: arraste uma página ou página espelhada para um novo local. A barra vertical mostra para onde a página está sendo movida.

   * **Botão Mover para**: selecione uma página ou página espelhada, selecione **[!UICONTROL Move To]** e escolha a página no menu que deve aparecer antes da sua página.

   * **Sequence #**: Na Exibição de Lista, insira números de página nos campos de Número de Sequência.

1. Quando terminar, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar o eCatalog. No campo Nome do arquivo, digite o nome do conjunto de rotação.
1. Selecionar **[!UICONTROL Save]**.

   Você pode visualizar seu eCatalog, depois de salvá-lo, selecionando **[!UICONTROL Preview]**.

## Editar um eCatalog {#editing-an-ecatalog}

Se você editar um conjunto publicado ou não, a variável **[!UICONTROL Publish after a save]** opção afeta os membros set e set das seguintes maneiras:

| Conjunto já publicado? | A opção &quot;Publicar após salvar&quot; foi selecionada antes de salvar a edição? | Estado do conjunto após salvar | Estado dos membros definidos após salvar |
| --- | --- | --- | --- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existentes mantêm seu estado publicado. Qualquer novo membro do conjunto adicionado durante sua edição manterá seu estado publicado ou não. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existentes e os novos membros do conjunto adicionados durante a edição mantêm seus estados publicado ou não. |

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um eCatalog:**

1. Selecione a sobreposição do eCatalog **[!UICONTROL Edit]** botão.
1. Faça as alterações necessárias.
1. Ao concluir a edição, próximo ao canto inferior direito da página, verifique se **[!UICONTROL Publish after a save]** está selecionada (padrão).
1. Selecionar **[!UICONTROL Save]**, selecione uma pasta de armazenamento, digite um nome para o conjunto e selecione **[!UICONTROL Save]**.

## Excluir um eCatalog

Quando você exclui um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicação manual de ativos](publishing-files.md#manually_publishing_assets) e [Cancelamento de publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para excluir um eCatalog:**

1. Na Exibição em Grade, Exibição em Lista ou Exibição de Detalhes, selecione um ou mais eCatalogs.
1. Na Barra de navegação global, acesse **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Personalizar o sumário {#customizing-the-table-of-contents-toc}

O Adobe Dynamic Media Classic fornece números de página padrão em seu eCatalog na guia Ordenar páginas da tela eCatalog. Para nomes de página personalizados, é possível alterar os rótulos de página que constituem o índice. É recomendável renomear a tampa frontal e traseira. Por exemplo, a folha de rosto pode ler &quot;Capa&quot; em vez de &quot;Página 0-1&quot;.

Você pode criar um sumário personalizado (TOC) para seu eCatalog manualmente. Ou você pode importar os nomes de página de um arquivo CSV (somente Mac) ou XML.

>[!NOTE]
>
>Para restaurar títulos de página padrão, no campo **[!UICONTROL Order Pages]** selecione **[!UICONTROL TOC Labels]** e selecione **[!UICONTROL Restore Defaults (All)]**.

### Inserção manual de nomes de página {#manually-entering-page-names}

Insira manualmente os nomes de página, um de cada vez, acessando a guia Ordenar páginas da tela do eCatalog. Em seguida, no campo Número da página, digite um nome para cada página que deseja nomear.

### Importar nomes de página {#importing-page-names}

A importação de nomes de página é recomendada se você estiver lidando com um eCatalog com muitas páginas. Você pode importar os nomes de um arquivo XML ou delimitado por tabulação.

O rótulo do índice é armazenado no campo Dados do usuário de uma imagem; formate esses dados como uma lista de `name=<value>` ` pairs separated by two question marks "??" `. Por exemplo, para definir um rótulo para um campo de índice chamado `tocEN`, defina os Dados do usuário da imagem como:

`tocEN=&lt;EN_page_label>`

Para definir rótulos separados para campos de índice denominados `tocEN` e `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Para importar o campo Dados do usuário em um arquivo delimitado por tabulação, inclua os dados do usuário do campo:

| IPSID | Dados do usuário |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Para importar o campo Dados do Usuário em um arquivo XML, inclua o atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nomes de página de um arquivo XML ou delimitado por tabulação, selecione o **[!UICONTROL TOC Labels]** e selecione **[!UICONTROL Import]**. Na caixa de diálogo Fazer upload de metadados, selecione **[!UICONTROL Browse]** e importe o arquivo CSV (somente Mac) ou o arquivo XML que associa cada página a um nome de página.
