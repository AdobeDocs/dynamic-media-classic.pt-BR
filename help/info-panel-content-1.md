---
title: Gerenciamento do conteúdo do painel Informações em conjuntos de imagens
description: Saiba como gerenciar o conteúdo do Painel de informações em Conjuntos de imagens.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Visualizadores,Conjuntos de imagens
role: Business Practitioner
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Gerenciamento do conteúdo do painel Informações em conjuntos de imagens{#managing-info-panel-content-in-image-sets}

Além de usar o texto do Mapa de imagem para suas sobreposições em Conjuntos de imagens, você pode usar um painel de informações para adicionar grandes quantidades de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando o armazenamento em cache programado e o agendamento de atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se o Conjunto de imagens é publicado automaticamente.
* O painel Dados do InfoPanel permite que você especifique um arquivo CSV contendo o texto que deseja que apareça no texto de sobreposição do painel de informações e os horários de agendamento para a atualização das informações.
* A caixa de diálogo Importar metadados permite importar um arquivo TXT delimitado por tabulação que contém as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel do feed de dados do InfoPanel com a opção de arquivo CSV para o texto de sobreposição.

## Configurar um modelo de resposta para Conjuntos de imagens {#set-up-a-response-template-for-image-sets}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir o texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel de informações: quantas colunas e linhas, tamanho da fonte, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um dos seus próprios.

**Para configurar um template de resposta:**

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição detalhada.
1. Clique em **[!UICONTROL InfoPanel Setup]**.
1. Na lista suspensa Modelo de resposta , siga um destes procedimentos:

   * Para usar a resposta padrão, selecione **[!UICONTROL Default]**. O XML para o design de modelo é exibido, esmaecido, na caixa de texto Modelo de usuário.
   * Para criar seu próprio modelo de resposta, selecione **[!UICONTROL Custom]**. Na caixa de texto Modelo do usuário, digite a definição do modelo XML. Você pode usar o modelo padrão já definido na caixa de texto como base para sua própria resposta.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja que apareça se o Dynamic Media Classic encontrar um erro na recuperação de informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de Conjunto de imagens, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.
1. No campo de texto TTL de Resposta , insira o número de horas que você deseja esperar antes de armazenar os dados em cache.

   * Defina um número menor se os dados forem atualizados com frequência ao longo do dia.
   * Defina um número maior se os dados forem relativamente estáveis e não precisarem de atualização com frequência ao longo do dia. O padrão é dez horas.

1. Clique em **[!UICONTROL Upload]** para fazer upload do conteúdo do painel de informações, com base nos valores de rolover_key, para s7info.
1. Na caixa de diálogo S7Info Upload , navegue até o arquivo que deseja usar e clique em **[!UICONTROL Upload]**.

   Os formatos de arquivo compatíveis são arquivos delimitados por TAB com codificação UTF-16 e arquivos CSV com codificação ASCII. Para arquivos CSV, caracteres não ASCII devem ser codificados em HTML.

1. No painel Configuração do InfoPanel, clique em **[!UICONTROL Publish]**.

## Importar conteúdo de origem para o painel Informações em Conjuntos de Imagens {#import-source-content-for-the-info-panel-in-image-sets}

Você pode usar um arquivo CSV (Valor separado por vírgulas) com codificação ASCII (o caractere não ASCII deve ser codificado em HTML) ou um arquivo delimitado por tabulação para o texto de origem de um painel de informações para um Conjunto de imagens. Os arquivos delimitados por tabulação devem usar a codificação UTF-16 (Unicode). Você importa os diferentes tipos de arquivos usando métodos diferentes.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Os dados delimitados por tabulação e vírgulas podem conter quantas colunas forem necessárias para o modelo de sobreposição.
* O primeiro item ou coluna de dados é o identificador de sobreposição (associado ao valor de rolagem_key dos URLs do mapa de imagem).
* Certifique-se de que cada item delimitado por tabulação ou por vírgulas depois do identificador seja o item que você deseja substituir no template de resposta. Assim, a primeira coluna é substituída por $1$, a segunda em $2$ e assim por diante).

### Importar conteúdo CSV para conjuntos de imagens de um local hospedado externamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição detalhada.
1. Clique em **[!UICONTROL InfoPanel Datafeed]**.
1. No campo de texto Local do arquivo CSV hospedado externamente (HTTP) , insira o URL para o arquivo CSV.
1. (Opcional) Nos campos Agendar atualização , especifique um horário para atualizar o conteúdo e clique em **[!UICONTROL Add]**.

   É possível selecionar várias vezes para atualização. Cada hora de atualização é exibida na caixa de texto Tempo de atualização . Para remover um horário agendado, selecione-o e clique em **[!UICONTROL Delete]**.

1. (Opcional) Clique em **[!UICONTROL Run Update]** para atualizar imediatamente o conteúdo.
