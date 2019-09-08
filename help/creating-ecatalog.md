---
title: Criação de um ecatalog
seo-title: Criação de um ecatalog
description: 'null'
seo-description: Saiba como criar um ecatalog.
uuid: 2 aff 05 c 2-7052-426 c-b 61 d -7 f 9091 f 7 ace 8
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/ecatalogs
discoiquuid: 28889 c 60-596 a -40 d 2-85 d 4-f 48 a 4 f 86 b 932
translation-type: tm+mt
source-git-commit: 1941567db5c154620bb0dcd12e363d7eebc61b20

---


# Criação de um ecatalog{#creating-an-ecatalog}

A criação de um ecatalog envolve a ordem das páginas, escolha o layout da página e vincula as páginas ao desenhar Mapas de imagem e inserir dados de link de sobreposição e hipertexto. Opcionalmente, você pode personalizar o sumário para que os visualizadores vejam nomes de página em vez de números de página no Visualizador do ecatalog.

## Criação de um ecatalog {#create}

É possível incluir arquivos de imagem e arquivos PDF em seu catálogo.

Quando você cria um ecatalog, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| A opção «Publicar após salvar» selecionada antes de salvar? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |
| Sim | Publicado | Publicado |
| Não | Não publicado | Os membros podem reter seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para criar um ecatalog**

1. Comece a criar seu ecatalog com uma destas técnicas:

   **Selecione os arquivos primeiro** no Painel Procurar, selecione arquivos e clique em Criar &gt; ecatalogs.

   **Comece pela tela ecatalog** clique em Criar &gt; ecatalogs. Selecione uma pasta na Biblioteca de ativos e arraste arquivos da pasta para a guia Páginas de pedido da página ecatalog.

   ***observação**: Para exibir os itens na Biblioteca de ativos por nome em vez de miniatura, selecione a opção Nome para Exibição de biblioteca de ativos padrão na Configuração pessoal. *

1. Selecione um layout geral para o seu catálogo. Clique no botão 1 para cima para páginas únicas, o botão 2 para cima das propagandas de página dupla ou o botão Personalizado para as propagandas de páginas de mais de duas páginas. A caixa de diálogo Alterar layout do ecatalog é exibida. Selecione as opções Todas as páginas espelhadas e clique **em OK**.
1. Opcionalmente, altere o layout de páginas individuais ou páginas espelhadas de página clicando neles e escolhendo o botão 1 para cima, 2 para cima ou para Personalizado. A caixa de diálogo Alterar layout do ecatalog é exibida. Selecione as opções de Planilha selecionada e clique **em OK**.
1. Reorganize as páginas conforme necessário com uma destas técnicas:

   **Arrastar Arrastar** uma página ou página espelhada para um novo local. A barra vertical mostra onde a página está sendo movida.

   **Mover para** botão Selecionar uma página ou página espelhada, clique no botão Mover para e escolha a página no menu que deseja que sua página seja exibida antes.

   **Sequência #** Na exibição de lista, insira números de página nos campos Sequência #.

1. Quando terminar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**.
1. Na caixa de diálogo Salvar, selecione uma pasta para armazenar o ecatalog. No campo Nome do arquivo, digite o nome do conjunto de rotação.
1. Clique **em Salvar**.

   Você pode visualizar o ecatalog depois de salvá-lo, clicando em **Visualizar**.

## Editar um catálogo eletrônico {#editing-an-ecatalog}

Se você editar um conjunto publicado ou um conjunto não publicado, **a opção Publicar depois de salvar** afeta o conjunto e os membros definidos das seguintes maneiras:

| Já foi publicado? | A opção «Publicar após salvar» selecionada antes de salvar sua edição? | Estado de conjunto após salvar | Estado dos membros definidos após salvar |
|--- |--- |--- |--- |
| Sim | Sim | Publicado | Publicado |
| Sim | Não | Publicado | Os membros definidos existentes mantêm seu estado publicado. Todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |
| Não | Sim | Publicado | Publicado |
| Não | Não | Não publicado | Os membros definidos e todos os novos membros definidos durante a edição mantêm seu estado publicado ou não publicado. |

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Para editar um ecatalog**

1. Clique no botão Editar borda **do** ecatalog.
1. Faça as alterações necessárias.
1. Quando terminar de editar, próximo ao canto inferior direito da página, certifique-se de **que Publicar depois de salvar** esteja selecionado (padrão).
1. Clique **em Salvar**, selecione uma pasta de armazenamento, digite um nome para o conjunto e clique **em Salvar**.

## Excluindo um catálogo eletrônico {#deleting-an-ecatalog}

Quando um conjunto é excluído, o próprio conjunto é movido para a lixeira. No entanto, os membros (ou «filhos») dentro desse conjunto não serão afetados; em vez disso, cada um retém seu estado publicado ou não publicado existente.

Consulte também [Publicar manualmente ativos](publishing-files.md#manually_publishing_assets) e [Cancelar a publicação manual de ativos](publishing-files.md#manually_unpublishing_assets).

**Exclusão de um ecatalog**

1. Na Exibição de grade, Exibição de lista ou Exibição de detalhes, selecione um ou mais ecatalogs.
1. Na barra de navegação global, clique **em Arquivo** &gt; **Excluir** &gt; **Excluir**.

## Personalização do sumário (sumário) {#customizing-the-table-of-contents-toc}

O Dynamic Media Classic fornece números de página padrão no seu ecatalog na guia Páginas de pedido da tela ecatalog. Para nomes de página personalizados, é possível alterar os rótulos de páginas que constituem o sumário (sumário). É recomendável renomear a capa frontal e traseira. Por exemplo, a página de capa frontal pode ler «Capa» em vez de «Página 0-1. »

É possível criar um sumário personalizado (TOC) para o seu ecatalog manualmente ou importando os nomes de página de um CSV (somente Mac) ou de um arquivo XML.

>[!NOTE]
>
>Para restaurar títulos de página padrão, clique no botão Rótulos sumários na guia Páginas de pedido e escolha Restaurar padrões (todos).

### Inserir manualmente nomes de página {#manually-entering-page-names}

Para inserir manualmente nomes de página um de cada vez, vá para a guia Páginas de pedido da tela do ecatalog. Em seguida, clique em no campo número da página e insira um nome. Digite um nome para cada página que deseja nomear.

### Importação de nomes de página {#importing-page-names}

A importação de nomes de página é recomendada se você estiver lidando com um ecatalog com várias páginas. É possível importar os nomes de um arquivo delimitado por tabulação ou XML.

O rótulo TOC é armazenado no campo Dados do usuário de uma imagem; formatar esses dados como uma lista de `name=<value>`` pairs separated by two question marks “??” `. Por exemplo, para definir uma etiqueta para um campo TOC chamado toif «, defina os Dados do usuário da imagem como:

Tocen = &lt; EN_ page_ label &gt;

Para definir rótulos separados para os campos TOC chamados tocen e tocfr:

Tocen = &lt; EN_ page_ label &gt;?? Tocfr = &lt; FR_ page_ label &gt;

Para importar o campo Dados do usuário em um arquivo delimitado por tabulação, inclua os dados do campo:

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | Tocen = &lt; EN_ page_ label &gt;?? Tocfr = &lt; FR_ page_ label &gt; |

Para importar o campo Dados do usuário em um arquivo XML, inclua o atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nomes de página de um arquivo delimitado por tabulação ou XML, selecione o botão Rótulos TOC e escolha Importar. A caixa de diálogo Carregar metadados é exibida. Clique no botão Procurar e importe o arquivo CSV (somente Mac) ou o arquivo XML que associa cada página com um nome de página.
