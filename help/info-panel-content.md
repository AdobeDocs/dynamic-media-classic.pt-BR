---
title: Gerenciando conteúdo do painel Informações no ecatalogs
seo-title: Gerenciando conteúdo do painel Informações no ecatalogs
description: 'null'
seo-description: Saiba como gerenciar o conteúdo do Painel Informações no ecatalogs.
uuid: 5 aa 634 f 9-0874-4 bb 5-a 3 d 9-8 ce 4 d 5577941
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/ecatalogs
discoiquuid: be 277831-77 cc -4011-ae 30-e 75 c 18 eec 99 b
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gerenciando conteúdo do painel Informações no ecatalogs{#managing-info-panel-content-in-ecatalogs}

Além de usar o texto do Mapa de imagem para sobreposições no ecatalogs, você pode usar um Painel de informações para adicionar quantidades maiores de texto de sobreposição, incluindo links. Você também pode gerenciar o infopanel usando atualizações de conteúdo de cache e programação cronometradas.

Você pode gerenciar sua configuração e dados do infopanel usando os seguintes recursos no Dynamic Media Classic:

* O painel de Configuração do infopanel permite especificar o modelo usado para exibir o texto do Painel Informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se o ecatalogs é publicado automaticamente.
* O painel de Datafeel do infopanel permite especificar um arquivo CSV que contém o texto que você deseja que apareça no texto de sobreposição do infopanel, bem como horários de agendamento para atualizar as informações.
* A caixa de diálogo Importar metadados (acessada na exibição Mapear páginas) permite importar um arquivo TXT delimitado por tabulação contendo as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Datafeed com a opção de arquivo CSV para o texto de sobreposição.
* A exibição de Páginas do mapa fornece uma opção para visualizar o xml que aparece para mapas de imagem específicos.

## Configurar um modelo de resposta para o ecatalogs {#set-up-a-response-template-for-ecatalogs}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel Informações: quantas colunas e linhas, tamanho da face de tipos, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um dos seus próprios.

>[!NOTE]
>
>Você também pode configurar o Modelo de resposta na Predefinição do visualizador. Para usar o Modelo de resposta na Predefinição do visualizador, adicione `fmt=1` ao final do URL do servidor de informações na Predefinição do visualizador.
>
>Consulte [Configuração das predefinições](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)do visualizador do ecatalog.

1. Clique duas vezes em seu ecatalog para abri-lo na Exibição de detalhes.
1. Clique no painel Configuração do infopanel para abri-lo.
1. Selecione um Modelo de Resposta:

   * Selecione uma predefinição no menu Modelo de resposta. O XML para o design de modelo aparece na caixa Modelo de usuário.
   * Selecione Personalizado para criar seu próprio modelo de resposta. Digite a definição XML de modelo na caixa Modelo de usuário. Você pode usar os modelos predefinidos como base para os seus próprios.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja exibir se o Dynamic Media Classic encontrar um erro ao recuperar as informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de ecatalog, mas sem identificador de rolagem, esta mensagem será exibida para o usuário.
1. Na caixa TTL de resposta, digite o número de horas que deseja esperar antes de armazenar os dados em cache:

   * Defina um número menor se os dados forem atualizados frequentemente durante um dia.
   * Defina um número maior se os dados forem relativamente estáveis e não precisarem atualizar frequentemente durante o dia. O padrão é dez horas.

1. Clique **em Publicar**.

## Importar conteúdo de origem para o Painel Informações no ecatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Você pode usar um arquivo de valor separado por vírgula (CSV) ou arquivo delimitado por tabulação (TXT) para o texto de origem de um Painel Info para um ecatalog. Os arquivos delimitados por tabulação devem usar a codificação UTF 16 (Unicode). Você importa os diferentes tipos de arquivo usando diferentes métodos.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Certifique-se de que os dados delimitados por tabulação e vírgula contêm quantas colunas forem necessárias para o modelo de sobreposição.
* Certifique-se de que o primeiro item ou coluna de dados é o identificador de rolagem (associado ao valor rollover_ key dos urls do mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula depois do identificador é o item que você deseja substituir no modelo de resposta (para que a primeira coluna seja substituída em $ 1 $, a segunda coluna até $ 2 $ e assim por diante).

### Importar conteúdo CSV para o ecatalogs a partir de um local externo hospedado {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Clique duas vezes no ecatalog para abri-lo na Exibição de detalhes.
1. Clique no painel Dados do infopanel para abri-lo.
1. Digite o URL do arquivo CSV na caixa Local do arquivo CSV externamente hospedado. É possível colar o URL nesse campo ou digitar diretamente.
1. (Opcional) Especifique um horário para atualizar o conteúdo usando os menus Agendar atualização e clique em Adicionar. É possível selecionar várias vezes para atualizar. Cada hora de atualização aparece na caixa Atualizar horas. (Para remover um horário, selecione-o e clique em Excluir.)
1. (Opcional) Clique em Executar atualização agora para atualizar o conteúdo imediatamente.

### Importar um arquivo delimitado por tabulação ou CSV {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Clique duas vezes no ecatalog para abri-lo na Exibição de detalhes.
1. Clique no painel Configuração do infopanel para abri-lo.
1. **Clique em Carregar conteúdo** S 7 informando.
1. Clique **em Procurar**, selecione o arquivo TXT delimitado por tabulação, arquivo CSV ou SSV que deseja usar e clique **em Abrir**.
1. Clique em **Carregar**.

O Dynamic Media Classic envia uma mensagem de email para avisá-lo se o upload foi realizado com sucesso ou não.

## Visualizar texto-chave de sobreposição para um Mapa de imagem {#preview-rollover-key-text-for-an-image-map}

Usando a tela Mapear páginas, você pode exibir com facilidade o texto do Painel Informações para os Mapas de imagem em uma página específica do seu ecatalog.

1. Clique no botão Editar borda do catálogo.
1. Clique em Mapa de páginas.
1. Na parte superior da tabela no lado direito da tela, escolha Painel Informações no menu Exibir.

   O texto de sobreposição é exibido ao lado de cada Mapa de imagem que contém o texto do Painel Informações.

