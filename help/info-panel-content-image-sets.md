---
title: Gerenciar conteúdo do Painel de informações em Conjuntos de imagens
description: Saiba como gerenciar o conteúdo do Painel de informações em Conjuntos de imagens no Adobe Dynamic Media Classic.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Gerenciar conteúdo do Painel de informações em Conjuntos de imagens{#managing-info-panel-content-in-image-sets}

Além de usar o texto do Mapa de imagem para sobreposições em Conjuntos de imagens, você pode usar um painel de informações para adicionar quantidades maiores de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando o cache cronometrado e programando atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Adobe Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, é possível especificar se o Conjunto de imagens é publicado automaticamente.
* O painel Data Feed do InfoPanel permite especificar um arquivo CSV contendo o texto que você deseja exibir no texto de sobreposição do painel de informações e programar horários para atualizar as informações.
* A caixa de diálogo Importar metadados permite importar um arquivo TXT delimitado por tabulação contendo as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Feed de dados do InfoPanel com a opção de arquivo CSV para o texto de sobreposição.

## Configurar um modelo de resposta para conjuntos de imagens {#set-up-a-response-template-for-image-sets}

É possível selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como as informações são apresentadas no Painel Informações: quantas colunas e linhas, tamanho da fonte, etc. Você pode selecionar um modelo de resposta predefinido ou criar um de sua preferência.

**Para configurar um modelo de resposta para Conjuntos de imagens:**

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição de detalhes.
1. Selecionar **[!UICONTROL InfoPanel Setup]**.
1. Na lista suspensa Modelo de resposta, execute um dos procedimentos a seguir:

   * Para usar a resposta padrão, selecione **[!UICONTROL Default]**. O XML do design do modelo aparece esmaecido na caixa de texto Modelo do usuário.
   * Para criar seu próprio modelo de resposta, selecione **[!UICONTROL Custom]**. Na caixa de texto Modelo de Usuário, digite a definição XML do modelo. Você pode usar o template padrão que já está definido na caixa de texto como base para sua própria resposta.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja exibir se o Adobe Dynamic Media Classic encontrar um erro ao recuperar informações de um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de Conjunto de imagens, mas nenhum identificador de substituição, esta mensagem será exibida para o usuário.
1. No campo de texto TTL de Resposta, informe o número de horas que deseja aguardar antes de armazenar os dados em cache.

   * Defina um número menor se os dados forem atualizados com frequência ao longo do dia.
   * Defina um número mais alto se os dados estiverem relativamente estáveis e não exigirem atualização com frequência ao longo do dia. O padrão é dez horas.

1. Selecionar **[!UICONTROL Upload]** para carregar o conteúdo do painel info, com base nos valores rollover_key, para s7info.
1. Na caixa de diálogo Upload S7Info, navegue até o arquivo que deseja usar e selecione **[!UICONTROL Upload]**.

   Os formatos de arquivo compatíveis são arquivos delimitados por TAB com codificação UTF-16 e arquivos CSV com codificação ASCII. Para arquivos CSV, os caracteres não ASCII devem ser codificados em HTML.

1. No painel Configuração do InfoPanel, selecione **[!UICONTROL Publish]**.

## Importar conteúdo de origem para o Painel Informações em Conjuntos de imagens {#import-source-content-for-the-info-panel-in-image-sets}

Você pode usar um arquivo CSV (Valor separado por vírgulas) com codificação ASCII (o caractere não ASCII deve ser codificado em HTML) ou um arquivo delimitado por tabulação para o texto de origem de um painel de informações de um Conjunto de imagens. Os arquivos delimitados por tabulação devem usar a codificação UTF-16 (Unicode). Importe os diferentes tipos de arquivo usando métodos diferentes.

Ao formatar o conteúdo original, lembre-se das seguintes diretrizes:

* Os dados delimitados por tabulação e vírgula podem conter quantas colunas forem necessárias para o modelo de sobreposição.
* O primeiro item ou coluna de dados é o identificador de rollover (associado ao valor rollover_key dos URLs do mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula após o identificador é o item que você deseja substituir no modelo de resposta. Assim, a primeira coluna é substituída por $1$, a segunda coluna por $2$ e assim por diante).

### Importar conteúdo de CSV para conjuntos de imagens de um local hospedado externamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição de detalhes.
1. Selecionar **[!UICONTROL InfoPanel Datafeed]**.
1. No campo de texto Localização do arquivo CSV hospedado externamente (HTTP), insira o URL do arquivo CSV.
1. (Opcional) Nos campos Agendar atualização, especifique um horário para atualizar o conteúdo e selecione **[!UICONTROL Add]**.

   Você pode selecionar várias vezes para atualização. Cada hora de atualização aparece na caixa de texto Atualizar horas. Para remover um horário agendado, selecione-o e, em seguida, **[!UICONTROL Delete]**.

1. (Opcional) Selecione **[!UICONTROL Run Update]** para atualizar imediatamente o conteúdo.
