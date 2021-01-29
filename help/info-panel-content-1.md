---
title: Gerenciamento do conteúdo do painel Informações em conjuntos de imagens
description: Saiba como gerenciar o conteúdo do Painel de informações em Conjuntos de imagens.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Gerenciamento do conteúdo do painel Informações em conjuntos de imagens{#managing-info-panel-content-in-image-sets}

Além de usar o texto do Mapa de imagem para sobreposições em Conjuntos de imagens, você pode usar um painel de informações para adicionar grandes quantidades de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando o armazenamento em cache programado e o agendamento de atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se o Conjunto de imagens será publicado automaticamente.
* O painel Dados do Painel de Informações permite que você especifique um arquivo CSV que contém o texto que deseja que seja exibido no texto de sobreposição do painel de informações, bem como os horários de agendamento para a atualização das informações.
* A caixa de diálogo Importar metadados permite importar um arquivo TXT delimitado por tabulação que contém as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Dados do InfoPanel com a opção de arquivo CSV para o texto de sobreposição.

## Configurar um modelo de resposta para Conjuntos de Imagens {#set-up-a-response-template-for-image-sets}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel de informações: quantas colunas e linhas, tamanho da fonte, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um deles.

**Para configurar um modelo de resposta**

1. Clique com o duplo do mouse em seu Conjunto de imagens para abri-lo na Visualização Detalhe.
1. Clique em **Configuração do InfoPanel** para desdobrar o painel.
1. Na lista suspensa Modelo de resposta, execute um dos procedimentos a seguir:

   * Selecione Padrão para usar a resposta padrão. O XML para o design de modelo é exibido, esmaecido, na caixa de texto Modelo do usuário.
   * Selecione Personalizado para criar seu próprio modelo de resposta. Na caixa de texto Modelo do usuário, digite a definição XML do modelo. Você pode usar o modelo padrão que já está definido na caixa de texto como uma base para sua própria resposta.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja que seja exibido se o Dynamic Media Classic encontrar um erro ao recuperar informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de Conjunto de imagens, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.
1. No campo de texto TTL de resposta, informe o número de horas que você deseja esperar antes de armazenar os dados em cache.

   * Defina um número menor se os dados forem atualizados com frequência ao longo do dia.
   * Defina um número maior se os dados estiverem relativamente estáveis e não precisarem ser atualizados com frequência ao longo do dia. O padrão é dez horas.

1. Clique em **Carregar** para fazer upload do conteúdo do painel de informações, com base nos valores de roll_key, para s7info.
1. Na caixa de diálogo S7Info Upload, navegue até o arquivo que deseja usar e clique em **Carregar**.

   Os formatos de arquivo suportados são arquivos delimitados por TAB com codificação UTF-16 e arquivos CSV com codificação ASCII. Para arquivos CSV, caracteres que não sejam ASCII devem ser codificados em HTML.

1. No painel Configuração do InfoPanel, clique em **Publicar**.

## Importar conteúdo de origem para o painel Informações em Conjuntos de imagens {#import-source-content-for-the-info-panel-in-image-sets}

Você pode usar um arquivo CSV (Valor separado por vírgulas) com codificação ASCII (caractere não ASCII deve ser codificado em HTML) ou um arquivo delimitado por tabulação para o texto de origem de um painel de informações de um Conjunto de imagens. Os arquivos delimitados por tabulação devem usar a codificação UTF-16 (Unicode). Você importa os diferentes tipos de arquivos usando métodos diferentes.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Os dados delimitados por tabulação e vírgulas devem conter quantas colunas forem necessárias para o modelo de sobreposição.
* O primeiro item ou coluna de dados deve ser o identificador de sobreposição (associado ao valor de rollover_key dos URLs do mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula após o identificador é o item que você deseja substituir no modelo de resposta (portanto, a primeira coluna é substituída em $1$, a segunda coluna em $2$, e assim por diante).

### Importar conteúdo CSV para conjuntos de imagens de um local hospedado externamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Clique com o duplo do mouse no Conjunto de imagens para abri-lo na Visualização Detalhe.
1. Clique em **InfoPanel Datafeed** para desdobrar o painel.
1. No campo de texto Local do arquivo CSV hospedado externamente (HTTP), insira o URL para o arquivo CSV.
1. (Opcional) Nos campos Agendar atualização, especifique um horário para atualizar o conteúdo e clique em **Adicionar**.

   Você pode selecionar várias vezes para atualização. Cada hora de atualização é exibida na caixa de texto Atualizar horas. Para remover um horário agendado, selecione-o e clique em **Excluir**.

1. (Opcional) Clique em **Executar Atualização** para atualizar imediatamente o conteúdo.

