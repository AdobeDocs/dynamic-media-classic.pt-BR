---
title: Gerenciar o conteúdo do painel Informações em catálogos eletrônicos
description: Saiba como gerenciar o conteúdo do Painel de informações em Catálogos eletrônicos no Adobe Dynamic Media Classic.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Gerenciar o conteúdo do painel Informações em catálogos eletrônicos{#managing-info-panel-content-in-ecatalogs}

Além de usar o texto do Mapa de imagem para suas sobreposições em eCatalogs, você pode usar um Painel de informações para adicionar grandes quantidades de texto sobreposto, incluindo links. Você também pode gerenciar o InfoPanel usando o armazenamento em cache programado e o agendamento de atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Adobe Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do Painel de Informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se os catálogos eletrônicos são publicados automaticamente.
* O painel Datafeed do InfoPanel permite que você especifique um arquivo CSV contendo o texto que deseja que apareça no texto de sobreposição do InfoPanel e os horários de agendamento para a atualização das informações.
* A caixa de diálogo Importar metadados (acessada da exibição Páginas de mapa) permite importar um arquivo TXT delimitado por tabulação que contém as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Datafeed com a opção de arquivo CSV para o texto de sobreposição.
* A exibição Páginas de mapa fornece uma opção para visualizar o xml que aparece para mapas de imagem específicos.

## Configurar um modelo de resposta para eCatalogs {#set-up-a-response-template-for-ecatalogs}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir o texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel de informações: quantas colunas e linhas, tamanho da fonte, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um dos seus próprios.

>[!NOTE]
>
>Você também pode configurar o Modelo de resposta na Predefinição do visualizador. Para usar o Modelo de resposta na Predefinição do visualizador, adicione `fmt=1` ao final do URL do servidor de informações na Predefinição do visualizador.
>
>Consulte [Configurar predefinições do visualizador do catálogo eletrônico](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Clique duas vezes no seu eCatalog para que ele seja aberto na Exibição detalhada.
1. Selecione o painel **[!UICONTROL InfoPanel Setup]**.
1. Selecione um Modelo de Resposta:

   * Selecione uma predefinição no menu Modelo de resposta. O XML para o design de modelo é exibido na caixa Modelo do usuário .
   * Para criar seu próprio modelo de resposta, selecione **[!UICONTROL Custom]**. Digite a definição do modelo XML na caixa Modelo do usuário. Você pode usar os modelos predefinidos como base para os seus próprios.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja que apareça se o Adobe Dynamic Media Classic encontrar um erro na recuperação de informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de catálogo eletrônico, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.
1. Na caixa TTL de resposta, digite o número de horas que deseja aguardar antes de armazenar os dados em cache:

   * Defina um número menor se os dados forem atualizados com frequência ao longo de um dia.
   * Defina um número maior se os dados forem relativamente estáveis e não precisarem de atualização com frequência ao longo do dia. O padrão é dez horas.

1. Selecione **[!UICONTROL Publish]**.

## Importar conteúdo de origem para o painel Informações em Catálogos eletrônicos {#import-source-content-for-the-info-panel-in-ecatalogs}

Você pode usar um arquivo de valor separado por vírgulas (CSV) ou um arquivo delimitado por tabulação (TXT) para o texto de origem de um Painel de informações para um eCatalog. Os arquivos delimitados por tabulação devem usar a codificação UTF16 (Unicode). Você importa os diferentes tipos de arquivos usando métodos diferentes.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Verifique se os dados delimitados por tabulação e por vírgulas contêm a quantidade de colunas necessária para o modelo de sobreposição.
* Certifique-se de que o primeiro item ou coluna de dados seja o identificador de sobreposição (associado ao valor de rolagem_chave dos URLs do mapa de imagem).
* Certifique-se de que cada item delimitado por tabulação ou por vírgulas depois do identificador seja o item que você deseja substituir no template de resposta. Assim, a primeira coluna é substituída por $1$, a segunda em $2$ e assim por diante.

### Importar conteúdo CSV para catálogos eletrônicos de um local hospedado externamente {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Clique duas vezes no Catálogo eletrônico para que ele seja aberto na Exibição de detalhes.
1. Selecione o painel **[!UICONTROL InfoPanel Datafeed]**.
1. Insira o URL do arquivo CSV na caixa Local do arquivo CSV hospedado externamente . Você pode colar o URL neste campo ou digitar diretamente.
1. (Opcional) Especifique um horário para atualizar o conteúdo usando os menus Agendar atualização e selecione **[!UICONTROL Add]**. É possível selecionar várias vezes para atualização. Cada hora de atualização é exibida na caixa Atualizar horas . (Para remover uma hora, selecione-a e selecione **[!UICONTROL Delete]**.)
1. (Opcional) Selecione **[!UICONTROL Run Update Now]** para atualizar imediatamente o conteúdo.

### Importar um arquivo CSV ou delimitado por tabulação {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Clique duas vezes no eCatalog para que ele seja aberto na Exibição de detalhes.
1. Selecione o painel **[!UICONTROL InfoPanel Setup]**.
1. Selecione **[!UICONTROL Upload S7Info Content]**.
1. Selecione **[!UICONTROL Browse]**, selecione o arquivo TXT delimitado por tabulação, CSV ou SSV que deseja usar e selecione **[!UICONTROL Open]**.
1. Selecione **[!UICONTROL Upload]**.

O Adobe Dynamic Media Classic envia uma mensagem de email informando se o upload foi bem-sucedido ou não.

## Visualizar texto da chave de substituição para um Mapa de imagem {#preview-rollover-key-text-for-an-image-map}

Usando a tela Mapear páginas, você pode exibir de forma fácil e rápida o texto do Painel de informações para os Mapas de imagem em uma página específica do seu eCatalog.

1. Selecione o botão **[!UICONTROL Edit]** de sobreposição do Catálogo.
1. Selecione **[!UICONTROL Map Pages]**.
1. Na parte superior da tabela, no lado direito da tela, escolha **[!UICONTROL Info Panel]** no menu Exibir.

   O texto da chave de substituição aparece ao lado de cada Mapa de imagem que contém o texto Painel de informações.
