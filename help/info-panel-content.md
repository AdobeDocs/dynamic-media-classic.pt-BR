---
title: Gerenciamento do conteúdo do painel Informações em eCatalogs
seo-title: Gerenciamento do conteúdo do painel Informações em eCatalogs
description: nulo
seo-description: Saiba como gerenciar o conteúdo do Painel de informações em eCatalogs.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 1%

---


# Gerenciamento do conteúdo do painel Informações em eCatalogs{#managing-info-panel-content-in-ecatalogs}

Além de usar o texto do Mapa de imagem para sobreposições em eCatalogs, você pode usar um Painel de informações para adicionar grandes quantidades de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando o armazenamento em cache programado e o agendamento de atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do Painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se os eCatalogs serão publicados automaticamente.
* O painel Dados do InfoPanel permite especificar um arquivo CSV que contém o texto que você deseja que seja exibido no texto de sobreposição do InfoPanel, bem como os horários de programação para a atualização das informações.
* A caixa de diálogo Importar metadados (acessada da visualização Mapear páginas) permite importar um arquivo TXT delimitado por tabulação que contém as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Datafeed com a opção de arquivo CSV para o texto de sobreposição.
* A visualização Mapear páginas fornece uma opção para visualizar o xml que aparece para mapas de imagem específicos.

## Configurar um modelo de resposta para eCatalogs {#set-up-a-response-template-for-ecatalogs}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel de informações: quantas colunas e linhas, tamanho da fonte, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um deles.

>[!NOTE]
>
>Você também pode configurar o Modelo de resposta na predefinição do visualizador. Para usar o Modelo de resposta na predefinição do visualizador, adicione `fmt=1` ao final do URL do Servidor de informações na predefinição do visualizador.
>
>Consulte [Configuração das predefinições](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)do visualizador do eCatalog.

1. Clique no seu eCatalog com o Duplo para abri-lo na Visualização Detalhe.
1. Clique no painel Configuração do InfoPanel para abri-lo.
1. Selecione um Modelo de Resposta:

   * Selecione uma predefinição no menu Modelo de resposta. O XML para o design de modelo é exibido na caixa Modelo do usuário.
   * Selecione Personalizado para criar seu próprio modelo de resposta. Digite a definição XML do modelo na caixa Modelo do usuário. Você pode usar os modelos predefinidos como uma base para seus próprios modelos.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja exibir se o Dynamic Media Classic encontrar um erro ao recuperar informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de eCatalog, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.
1. Na caixa TTL de Resposta, digite o número de horas que deseja esperar antes de armazenar os dados em cache:

   * Defina um número menor se os dados forem atualizados com frequência ao longo de um dia.
   * Defina um número maior se os dados estiverem relativamente estáveis e não precisarem ser atualizados com frequência ao longo do dia. O padrão é dez horas.

1. Clique em **Publicar**.

## Importar conteúdo de origem para o painel Informações em eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Você pode usar um arquivo de valor separado por vírgulas (CSV) ou um arquivo delimitado por tabulação (TXT) para o texto de origem de um Painel de informações para um eCatalog. Arquivos delimitados por tabulação devem usar a codificação UTF16 (Unicode). Você importa os diferentes tipos de arquivos usando métodos diferentes.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Certifique-se de que os dados delimitados por tabulação e vírgula contenham a quantidade necessária de colunas para o modelo de sobreposição.
* Verifique se o primeiro item ou coluna de dados é o identificador de sobreposição (associado ao valor de rollover_key dos URLs do mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula após o identificador é o item que você deseja substituir no modelo de resposta (portanto, a primeira coluna é substituída em $1$, a segunda coluna em $2$, e assim por diante).

### Importar conteúdo CSV para o eCatalog de um local hospedado externamente {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Clique com o Duplo do mouse no eCatalog para abri-lo na Visualização Detalhe.
1. Clique no painel Dados do InfoPanel para abri-lo.
1. Digite o URL do arquivo CSV na caixa Local do arquivo CSV hospedado externamente. Você pode colar o URL neste campo ou digitar diretamente.
1. (Opcional) Especifique um tempo para atualizar o conteúdo usando os menus Agendar atualização e clique em Adicionar. Você pode selecionar várias vezes para atualização. Cada hora de atualização é exibida na caixa Atualizar horas. (Para remover uma hora, selecione-a e clique em Excluir.)
1. (Opcional) Clique em Executar atualização agora para atualizar imediatamente o conteúdo.

### Importar um arquivo CSV delimitado por tabulação {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Clique com o Duplo do mouse no eCatalog para abri-lo na Visualização Detalhe.
1. Clique no painel Configuração do InfoPanel para abri-lo.
1. **Clique em Carregar conteúdo** S7Info.
1. Clique em **Procurar**, selecione o arquivo TXT delimitado por tabulação, o arquivo CSV ou SSV que deseja usar e clique em **Abrir**.
1. Clique em **Carregar**.

O Dynamic Media Classic envia uma mensagem de email informando se o upload foi bem-sucedido ou não.

## Pré-visualização do texto da chave de sobreposição para um Mapa de imagem {#preview-rollover-key-text-for-an-image-map}

Usando a tela Mapear páginas, é possível visualização com facilidade e rapidez o texto do Painel de informações para os Mapas de imagens em uma página específica do seu eCatalog.

1. Clique no botão Editar de sobreposição do Catálogo.
1. Clique em Mapear páginas.
1. Na parte superior da tabela, no lado direito da tela, escolha Painel de informações no menu Exibir.

   O texto da chave de substituição aparece ao lado de cada Mapa de imagem que contém o texto Painel de informações.

