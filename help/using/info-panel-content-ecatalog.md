---
title: Gerenciar conteúdo do Painel de Informações em eCatalogs
description: Saiba como gerenciar o conteúdo do Painel de informações em eCatalogs no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Gerenciar conteúdo do Painel de Informações em eCatalogs{#managing-info-panel-content-in-ecatalogs}

Além de usar o texto do Mapa de imagem para suas sobreposições em eCatalogs, você pode usar um Painel de informações para adicionar quantidades maiores de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando um armazenamento em cache cronometrado e programando atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Adobe Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do Painel de Informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se os eCatalogs serão publicados automaticamente.
* O painel Feed de dados do InfoPanel permite especificar um arquivo CSV contendo o texto que você deseja exibir no texto de sobreposição do InfoPanel e agendar tempos para atualizar as informações.
* A caixa de diálogo Importar metadados (acessada na visualização Mapear páginas ) permite importar um arquivo TXT delimitado por tabulação contendo as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Feed de dados com a opção de arquivo CSV para o texto de sobreposição.
* A exibição Mapear páginas fornece uma opção para visualizar o xml que aparece para Mapas de imagem específicos.

## Configurar um modelo de resposta para eCatalogs {#set-up-a-response-template-for-ecatalogs}

É possível selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como as informações são apresentadas no Painel Informações: quantas colunas e linhas, tamanho da fonte, etc. Você pode selecionar um Modelo de resposta predefinido ou criar um de sua preferência.

>[!NOTE]
>
>Você também pode configurar o Modelo de resposta na Predefinição do visualizador. Para usar o modelo de resposta na predefinição do visualizador, adicione `fmt=1` ao final do URL do Servidor de Informações na Predefinição do visualizador.
>
>Consulte [Configurar Predefinições do Visualizador de eCatalog](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Clique duas vezes no eCatalog para abri-lo na Exibição de detalhes.
1. Selecione o **[!UICONTROL InfoPanel Setup]** painel.
1. Selecione um Modelo de Resposta:

   * Selecione uma predefinição no menu Modelo de resposta. O XML do design do modelo aparece na caixa Modelo do usuário.
   * Para criar seu próprio Modelo de resposta, selecione **[!UICONTROL Custom]**. Digite a definição XML do modelo na caixa Modelo do Usuário. Você pode usar os modelos predefinidos como base para os seus próprios modelos.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja exibir se o Adobe Dynamic Media Classic encontrar um erro ao recuperar informações de um Mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de eCatalog, mas nenhum identificador de rollover, essa mensagem será exibida para o usuário.
1. Na caixa Resposta TTL, informe o número de horas que deseja aguardar antes de armazenar os dados em cache:

   * Defina um número menor se os dados forem atualizados com frequência ao longo de um dia.
   * Defina um número mais alto se os dados estiverem relativamente estáveis e não exigirem atualizações frequentes ao longo do dia. O padrão é dez horas.

1. Selecionar **[!UICONTROL Publish]**.

## Importar conteúdo de origem para o Painel de Informações em eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Você pode usar um arquivo de valores separados por vírgula (CSV) ou um arquivo delimitado por tabulação (TXT) para o texto de origem de um Painel de informações para um eCatalog. Os arquivos delimitados por tabulação devem usar a codificação UTF16 (Unicode). É possível importar os diferentes tipos de arquivo usando métodos diferentes.

Ao formatar o conteúdo original, lembre-se das seguintes diretrizes:

* Verifique se os dados delimitados por tabulação e vírgula contêm quantas colunas forem necessárias para o modelo de sobreposição.
* Verifique se o primeiro item ou coluna de dados é o identificador de substituição (associado ao valor rollover_key dos URLs do Mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula após o identificador é o item que você deseja substituir no Modelo de resposta. Assim, a primeira coluna é substituída por $1$, a segunda coluna por $2$ e assim por diante.

### Importar conteúdo CSV para eCatalogs de um local hospedado externamente {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Clique duas vezes no eCatalog para abri-lo na Exibição de detalhes.
1. Selecione o **[!UICONTROL InfoPanel Data feed]** painel.
1. Insira o URL do arquivo CSV na caixa Local do arquivo CSV hospedado externamente. Você pode colar o URL nesse campo ou digitá-lo diretamente.
1. (Opcional) Especifique um horário para atualizar o conteúdo usando o menu Agendar atualização e selecione **[!UICONTROL Add]**. Você pode selecionar várias vezes para atualização. Cada hora de atualização aparece na caixa Atualizar horas. (Para remover um horário, selecione-o e, em seguida, **[!UICONTROL Delete]**.)
1. (Opcional) Selecione **[!UICONTROL Run Update Now]** para que você possa atualizar o conteúdo imediatamente.

### Importar um arquivo CSV ou delimitado por tabulação {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Clique duas vezes no eCatalog para abri-lo na Exibição de detalhes.
1. Selecione o **[!UICONTROL InfoPanel Setup]** painel.
1. Selecionar **[!UICONTROL Upload S7Info Content]**.
1. Selecionar **[!UICONTROL Browse]**, selecione o arquivo TXT delimitado por tabulação, CSV ou SSV que deseja usar e selecione **[!UICONTROL Open]**.
1. Selecionar **[!UICONTROL Upload]**.

O Adobe Dynamic Media Classic envia uma mensagem de email informando se o upload foi bem-sucedido ou não.

## Visualizar texto da chave de sobreposição para um Mapa de imagem {#preview-rollover-key-text-for-an-image-map}

Usando a tela Mapear páginas, você pode visualizar de maneira fácil e rápida o texto do Painel de informações dos Mapas de imagem em uma página específica do seu eCatalog.

1. Selecione a sobreposição do catálogo **[!UICONTROL Edit]** botão.
1. Selecionar **[!UICONTROL Map Pages]**.
1. Na parte superior da tabela, no lado direito da tela, escolha **[!UICONTROL Info Panel]** no menu Mostrar.

   O texto da chave de substituição é exibido ao lado de cada Mapa de imagem que contém o texto Painel de informações.
