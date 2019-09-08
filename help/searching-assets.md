---
title: Pesquisar ativos
seo-title: Pesquisar ativos
description: 'null'
seo-description: Saiba como pesquisar ativos.
uuid: 058209 bc-bac 4-4 d 5 c -8261-e 242 a 543 beaf
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/managing_ assets
discoiquuid: effef 4 e 7-37 c 5-42 e 2-9266-asu 026 cad 628
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Pesquisar ativos{#searching-assets}

Para localizar ativos de arquivos no Sistema de publicação Scene 7, é possível exibir ativos por tipo, classificar ativos no Painel Procurar, realizar uma pesquisa simples, realizar uma pesquisa avançada e filtrar ativos.

>[!NOTE]
>
>A tela de Configuração pessoal oferece opções para escolher como você deseja realizar pesquisas. Por exemplo, você pode escolher um tipo de pesquisa padrão e escolher se deseja incluir campos definidos pelo usuário em pesquisas. Para obter mais informações, consulte [Configuração pessoal](personal-setup.md#personal_setup).

## Exibir ativos por tipo {#viewing-assets-by-type}

Para ver apenas arquivos de determinado tipo conforme você navega, abra o menu suspenso Mostrar na Biblioteca de ativos e escolha um tipo de arquivo. Somente ativos do tipo escolhido aparecem na Biblioteca de ativos.

## Classificação de arquivos no painel Procurar {#sorting-files-in-the-browse-panel}

Para classificar o conteúdo de uma pasta ou de resultados de pesquisa no Painel Procurar, selecione o menu Classificar e escolha uma opção. As opções são Nome, Tamanho, Tipo, Data criada e Última modificação.

Você pode escolher Crescente ou Decrescente para classificar os ativos em ordem crescente ou decrescente pelos critérios escolhidos.

Na Exibição de lista, você pode ordenar clicando em um nome de coluna.

## Realizar uma pesquisa simples {#conducting-a-simple-search}

Use o campo Pesquisar para realizar pesquisas simples. Você pode pesquisar por itens por nome ou pesquisar itens cujos metadados contêm uma palavra-chave.

Para realizar uma pesquisa simples:

1. Selecione a pasta na Biblioteca de ativos para pesquisar em uma pasta específica e em suas subpastas
1. Clique na Biblioteca de ativos e escolha uma opção que descreva a amplitude ou ampla amplitude da pesquisa. Você pode escolher Em Todos os arquivos e pastas, Dentro da pasta selecionada ou nas Pastas e subpastas selecionadas.
1. Insira um termo de pesquisa.
1. Clique em Ir ou pressione Enter.

   Os resultados da pesquisa aparecem no Painel Procurar.

>[!NOTE]
>
>O Dynamic Media Classic monitora pesquisas. Para executar uma pesquisa pela segunda vez, selecione o botão Pesquisar e escolha o nome de uma pesquisa na parte inferior do menu Pesquisar.

## Realizar uma pesquisa avançada {#conducting-an-advanced-search}

Clique em Pesquisa avançada na Biblioteca de ativos para pesquisar usando muitos critérios, incluindo valores em campos de metadados.

Especifique qualquer um dos seguintes critérios na pesquisa:

**Filtre por Tipo de ativo** limitar sua pesquisa a um tipo de ativo somente escolhendo um tipo de ativo no menu.

**Arquivos e pastas** Escolha onde deseja pesquisar: Em todos os arquivos e pastas, na pasta selecionada ou nas pastas e subpastas selecionadas.

**Todos os estados** de publicação Pesquisa por arquivos marcados como prontos para publicação não estão marcados para publicação ou todos os arquivos.

**Condições** Se você especificar os critérios de metadados para a pesquisa, selecione se a pesquisa deve corresponder a todas as condições (uma pesquisa ALL) ou qualquer condição (uma pesquisa OU).

**Especificar critérios de pesquisa de metadados** Crie um ou mais campos de pesquisa para pesquisar metadados. Para criar campos de pesquisa:

1. Abra a lista Exibição de metadados (à esquerda do menu Adicionar um campo) e escolha uma Exibição de metadados. Você pode escolher Exibição compacta, IPTC, XMP ou uma exibição de seu administrador configurado.
1. Selecione o menu Adicionar um campo e escolha um nome de campo na lista suspensa.
1. Escolha uma opção Contém (Contém, Não contém, Começa com, Termina com ou Igual).
1. Para campos numéricos, escolha um valor ou insira um intervalo de datas personalizado.
1. (Opcional) Repita as etapas de 1a 4 para criar mais campos de pesquisa.

Você pode clicar no botão Remover campo de pesquisa para remover um campo de pesquisa.

Clique em Pesquisar para iniciar a pesquisa. Os resultados da pesquisa aparecem no Painel Procurar. Você pode alterar qualquer condição de pesquisa e clicar em Pesquisar para executar a pesquisa novamente.

Clique em Limpar para limpar os critérios de pesquisa e iniciar uma nova pesquisa. Clique em Fechar quando terminar de pesquisar para fechar o painel Pesquisar.

## Filtrar ativos usando metadados {#filter-assets-using-metadata}

Filtre ativos na guia Filtros da Biblioteca de ativos. Para filtrar ativos, use valores de metadados como critérios. Depois de escolher um campo de metadados que deseja usar para filtragem, a guia Filtros lista todos os valores de metadados inseridos no campo escolhido e o número de ativos atribuídos a cada valor. Por exemplo, em uma operação de filtro no campo metadados do Criador, a guia Filtros lista todos os nomes inseridos no campo metadados do Criador para diferentes ativos e para cada nome, o número de ativos atribuídos ao nome. Em seguida, clique em um valor de metadados para ver todos os ativos atribuídos a esse valor. No exemplo, clique no valor de metadados Jimmy para ver todos os ativos nos quais o nome Jimmy foi inserido no campo metadados do Criador. É possível filtrar usando mais de um campo de metadados como um critério de filtragem.

É possível salvar operações de filtro para executá-las várias vezes.

>[!NOTE]
>
>Somente os campos de metadados na Exibição de metadados padrão podem ser usados para operações de filtro. A tela Exibições de metadados mostra o nome da Exibição de metadados padrão.

Consulte [Exibições de metadados](application-setup.md#metadata_views).

### Executar uma operação de filtro {#running-a-filter-operation}

Siga estas etapas para localizar ativos filtrando os valores de metadados:

1. Clique na guia Filtros na Biblioteca de ativos.

   Os critérios da operação de filtro anterior aparecem no painel Filtros. O painel Filtros é dividido em painéis, com cada painel representando um campo de metadados. Use os painéis para escolher quais campos de metadados serão filtrados e dentro de cada campo para escolher um valor de metadados para a operação de filtro.

   Para executar uma operação de filtro criada e salva, clique no botão Selecionar predefinição e escolha o nome da operação no menu.

   Consulte [Salvar, repetir e excluir operações de filtro](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Clique no botão Campo em um painel, siga estas instruções para exibir o menu de filtragem e criar a operação de filtro:

   **Escolha
um campo de metadados** Selecione o nome do campo no menu de filtragem.

   ***observação**: Somente os nomes dos campos de metadados na Exibição de metadados padrão aparecem no menu de filtragem.*

   Consulte [Exibições de metadados](application-setup.md#metadata_views).

   **Adicionar um campo de metadados** Escolha Adicionar um painel. Depois que o painel aparecer no painel Filtros, clique no botão Campo e escolha o nome de um campo de metadados no menu de filtragem.

   **Remover um campo de metadados** Escolher Remover esse painel no menu de filtragem.

   Ao escolher um campo de metadados, seu painel lista:

   * Todos os valores de metadados inseridos no campo.
   * Para cada valor de metadados, o número de ativos fornecidos pelo valor.

1. Repita a Etapa 2 quantas vezes forem necessárias para listar todos os campos de metadados para a operação de filtro nos painéis.
1. Em cada painel, selecione um valor de metadados para filtrar. Não é possível selecionar mais de um valor de metadados em cada painel.

   Os ativos que correspondem a todos os valores selecionados aparecem no painel Procurar.

   >[!NOTE]
   >
   >Para remover temporariamente um campo da operação de filtro, clique em Cancelar seleção de tudo. Essa opção está localizada na parte superior de cada painel, acima dos valores de metadados.

1. (Opcional) Para salvar a operação de filtro e ser capaz de executá-la depois, clique no botão Selecionar predefinição, escolha Salvar atual como novas predefinições e insira um nome na caixa de diálogo Salvar.

### Salvar, repetir e excluir operações de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instruções na guia Filtros para salvar, repetir e excluir as operações de filtro:

**Salvar uma operação de filtro** clique no botão Selecionar predefinido, escolha Salvar atual como novas predefinições e insira um nome na caixa de diálogo Salvar.

**Repita uma operação de filtro** Clique no botão Selecionar predefinição e escolha o nome de uma operação de filtro no menu. O menu lista as operações de filtro salvas.

**Excluir uma operação de filtro no menu Selecionar predefinição** 
Execute a operação de filtro. Em seguida, clique no botão Selecionar predefinido e escolha Excluir predefinição no menu.

## Uso do servidor de metadados {#using-the-metadata-server}

O servidor de metadados é uma API pública que pode ser usada para pesquisar ativos por metadados por meio de solicitações http.

Para configurar o servidor de metadados, clique em Configuração &gt; Configuração do aplicativo &gt; Configuração de publicação &gt; Servidor de metadados.

A tela Publicação do servidor de metadados é aberta. Esta tela permite definir as seguintes opções:

**Publicar** instantaneamente Avisa qualquer alteração de metadados quando efetuada, incluindo novos ativos, alterações de palavras-chave e assim por diante.

**Pacote XMP** publica o pacote XMP. Este pacote não é usado para pesquisa, mas fornece a XMP/XMP mais atualizada

**As palavras-chave** publicam suas palavras-chave para o servidor de metadados para uso em pesquisas.

**Campos de publicação do servidor de metadados** Selecione os campos a serem incluídos nos metadados. Isso permite determinar a quantidade de informações sobre os ativos disponíveis ao público. Esses campos também são exibidos em Exibições de metadados, mas só podem ser alterados no servidor de metadados.

Clique **em Publicar agora** para iniciar o trabalho. Uma confirmação é exibida, informando que a tarefa foi iniciada.

>[!MORELIKETHIS]
>
>* [Noções básicas de navegação](navigation-basics.md#navigation_basics)
>* [Exibição, adição e exportação de metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

