---
title: Criação de um eCatalog
seo-title: Criação de um eCatalog
description: nulo
seo-description: Saiba como criar um eCatalog.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---


# Criação de um eCatalog{#creating-an-ecatalog}

A criação de um eCatalog implica ordenar as páginas, escolher o layout da página e vincular as páginas desenhando os Mapas de imagem e inserindo dados de sobreposição e link de hipertexto. Como opção, você pode personalizar o sumário para que os visualizadores vejam os nomes das páginas em vez de os números das páginas no eCatalog Viewer.

## Criação de um eCatalog {#create}

É possível incluir arquivos de imagem e arquivos PDF no eCatalog.

Quando você cria um eCatalog, a opção **Publicar após salvar** afeta o conjunto e define os membros das seguintes maneiras:

| opção &quot;Publicar após salvar&quot; selecionada antes de salvar? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros definidos retêm seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para criar um eCatalog**

1. Comece a criar seu eCatalog com uma destas técnicas:

   **Selecione os arquivos primeiro** No painel Procurar, selecione os arquivos e clique em Criar > eCatálogos.

   **Start da tela** eCatalog Clique em Build > eCatalogs. Selecione uma pasta na Biblioteca de ativos e arraste os arquivos da pasta até a guia Páginas de pedidos da página eCatalog.

   ***observação**: Para visualização os itens na Biblioteca de ativos pelo nome em vez da miniatura, selecione a opção Nome da Visualização da Biblioteca de ativos padrão na Configuração pessoal. *

1. Selecione um layout geral para seu eCatalog. Clique no botão 1 para cima para páginas únicas, no botão 2 para cima para páginas espelhadas de duplo ou no botão Personalizado para páginas espelhadas com mais de duas páginas. A caixa de diálogo Alterar layout do eCatalog é exibida. Selecione as opções Todas as páginas espelhadas e clique em **OK**.
1. Como opção, altere o layout de páginas individuais ou páginas espelhadas clicando nelas e, em seguida, escolha o botão 1 para cima, 2 para cima ou Personalizado. A caixa de diálogo Alterar layout do eCatalog é exibida. Selecione as opções de Páginas espelhadas selecionadas e clique em **OK**.
1. Reorganize as páginas conforme necessário com uma destas técnicas:

   **Arrastar** Arraste uma página ou página espelhada para um novo local. A barra vertical mostra onde a página está sendo movida.

   **botão** Mover paraSelecione uma página ou página espelhada, clique no botão Mover para e escolha a página no menu que deseja que a página apareça antes.

   **Sequência #** Na Visualização da Lista, insira os números de página nos campos Número da sequência.

1. Quando terminar, próximo ao canto inferior direito da página, verifique se a opção **Publicar após salvar** está selecionada (padrão).
1. Clique em **Salvar**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar seu eCatalog. No campo Nome do arquivo, digite o nome do conjunto de spin.
1. Clique em **Salvar**.

   Você pode pré-visualização seu eCatalog, depois de salvá-lo, clicando em **Pré-visualização**.

## Editar um eCatalog {#editing-an-ecatalog}

Dependendo de se você editar um conjunto publicado ou não publicado, a opção **Publicar após salvar** afetará o conjunto e definirá os membros das seguintes maneiras:

| Definir já publicado? | Opção &quot;Publicar após salvar&quot; selecionada antes de salvar sua edição? | Estado do conjunto após salvar | Estado dos membros do conjunto após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros do conjunto existente mantêm seu estado publicado.Qualquer novo conjunto de membros adicionado durante a edição mantém seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros do conjunto existente e quaisquer novos membros do conjunto que você tiver adicionado durante a edição manterão seu estado publicado ou não publicado. |

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para editar um eCatalog**

1. Clique no botão **Editar** de sobreposição do eCatalog.
1. Faça as alterações necessárias.
1. Quando terminar a edição, próximo ao canto inferior direito da página, certifique-se de que a opção **Publicar após salvar** esteja selecionada (padrão).
1. Clique em **Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique em **Salvar**.

## Excluindo um eCatalog {#deleting-an-ecatalog}

Ao excluir um conjunto, o próprio conjunto é movido para a Lixeira. No entanto, os membros (ou &quot;filhos&quot;) dentro desse conjunto não são afetados; em vez disso, cada um deles mantém seu estado publicado ou não publicado.

Consulte também Publicar ativos [manualmente e cancelar](publishing-files.md#manually_publishing_assets) a publicação de ativos [](publishing-files.md#manually_unpublishing_assets)manualmente.

**Para excluir um eCatalog**

1. Na Visualização de grade, Visualização de Lista ou Detalhes, selecione um ou mais eCatálogos.
1. Na barra de navegação global, clique em **Arquivo** > **Excluir** > **Excluir**.

## Personalização do sumário (TOC) {#customizing-the-table-of-contents-toc}

O Dynamic Media Classic fornece números de página padrão em seu eCatalog na guia Páginas de pedido da tela eCatalog. Para nomes de página personalizados, é possível alterar os rótulos de página que constituem o sumário (TOC). É recomendável renomear a tampa frontal e traseira. Por exemplo, a página de capa frontal pode ler &quot;Capa&quot; em vez de &quot;Página 0-1&quot;.

Você pode criar um sumário personalizado (TOC) para seu eCatalog manualmente ou importando os nomes das páginas de um arquivo CSV (somente Mac) ou XML.

>[!NOTE]
>
>Para restaurar os títulos de página padrão, clique no botão Rótulos do sumário na guia Páginas de ordem e escolha Restaurar padrões (Todos).

### Inserção manual de nomes de página {#manually-entering-page-names}

Para inserir manualmente um nome de página de cada vez, vá para a guia Páginas de pedido da tela eCatalog. Em seguida, clique no campo de número da página e insira um nome. Digite um nome para cada página que deseja nomear.

### Importação de nomes de página {#importing-page-names}

A importação de nomes de página é recomendada se você estiver lidando com um eCatalog com muitas páginas. É possível importar os nomes de um arquivo XML ou delimitado por tabulação.

O rótulo do sumário é armazenado no campo Dados do usuário de uma imagem; formate esses dados como uma lista de `name=<value>`` pairs separated by two question marks “??” `. Por exemplo, para definir um rótulo para um campo TOC chamado tocEN &quot;, defina os Dados do usuário da imagem como:

tocEN=&lt;EN_page_label>

Para definir rótulos separados para campos TOC chamados tocEN e tocFR:

tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>

Para importar o campo Dados do usuário em um arquivo delimitado por tabulação, inclua os dados do usuário do campo:

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label> |

Para importar o campo Dados do usuário em um arquivo XML, inclua o atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nomes de páginas de um arquivo XML ou delimitado por tabulação, selecione o botão Rótulos TOC e escolha Importar. A caixa de diálogo Carregar metadados é exibida. Clique no botão Procurar e importe o arquivo CSV (somente Mac) ou o arquivo XML que associa cada página a um nome de página.
