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
role: Profissional
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---


# Gerenciamento do conteúdo do painel Informações em conjuntos de imagens{#managing-info-panel-content-in-image-sets}

Além de usar o texto do Mapa de imagem para suas sobreposições em Conjuntos de imagens, você pode usar um painel de informações para adicionar grandes quantidades de texto de sobreposição, incluindo links. Você também pode gerenciar o InfoPanel usando o armazenamento em cache programado e o agendamento de atualizações de conteúdo.

Você pode gerenciar a configuração e os dados do InfoPanel usando os seguintes recursos no Dynamic Media Classic:

* O painel Configuração do InfoPanel permite especificar o modelo usado para exibir o texto do painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se o Conjunto de imagens é publicado automaticamente.
* O painel Dados do InfoPanel permite que você especifique um arquivo CSV contendo o texto que deseja exibir no texto de sobreposição do painel de informações, bem como os horários de agendamento para atualizar as informações.
* A caixa de diálogo Importar metadados permite importar um arquivo TXT delimitado por tabulação que contém as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel DataFeed do InfoPanel com a opção de arquivo CSV para o texto de sobreposição.

## Configurar um modelo de resposta para Conjuntos de imagens {#set-up-a-response-template-for-image-sets}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir o texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel de informações: quantas colunas e linhas, tamanho da fonte, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um dos seus próprios.

**Para configurar um modelo de resposta**

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição detalhada.
1. Clique em **Configuração do InfoPanel** para expandir o painel.
1. Na lista suspensa Modelo de resposta , siga um destes procedimentos:

   * Selecione Default para usar a resposta padrão. O XML para o design de modelo é exibido, esmaecido, na caixa de texto Modelo de usuário.
   * Selecione Personalizado para criar seu próprio modelo de resposta. Na caixa de texto Modelo do usuário, digite a definição do modelo XML. Você pode usar o modelo padrão já definido na caixa de texto como base para sua própria resposta.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja que apareça se o Dynamic Media Classic encontrar um erro na recuperação de informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de Conjunto de imagens, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.
1. No campo de texto TTL de Resposta , insira o número de horas que você deseja esperar antes de armazenar os dados em cache.

   * Defina um número menor se os dados forem atualizados com frequência ao longo do dia.
   * Defina um número maior se os dados forem relativamente estáveis e não precisarem de atualização com frequência ao longo do dia. O padrão é dez horas.

1. Clique em **Upload** para fazer upload do conteúdo do painel de informações, com base nos valores de rolagem_chave, para s7info.
1. Na caixa de diálogo S7Info Upload , navegue até o arquivo que deseja usar e clique em **Upload**.

   Os formatos de arquivo compatíveis são arquivos delimitados por TAB com codificação UTF-16 e arquivos CSV com codificação ASCII. Para arquivos CSV, caracteres não ASCII devem ser codificados em HTML.

1. No painel Configuração do InfoPanel, clique em **Publicar**.

## Importar conteúdo de origem para o painel Informações em Conjuntos de Imagens {#import-source-content-for-the-info-panel-in-image-sets}

Você pode usar um arquivo CSV (Valor separado por vírgulas) com codificação ASCII (o caractere não ASCII deve ser codificado em HTML) ou um arquivo delimitado por tabulação para o texto de origem de um painel de informações para um Conjunto de imagens. Os arquivos delimitados por tabulação devem usar a codificação UTF-16 (Unicode). Você importa os diferentes tipos de arquivos usando métodos diferentes.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Os dados delimitados por tabulação e vírgulas devem conter a quantidade de colunas necessária para o modelo de sobreposição.
* O primeiro item ou coluna de dados deve ser o identificador de sobreposição (associado ao valor de rolover_key dos URLs do mapa de imagem).
* Certifique-se de que cada item delimitado por tabulação ou por vírgulas depois do identificador seja o item que você deseja substituir no modelo de resposta (então a primeira coluna é substituída em $1$, a segunda em $2$ e assim por diante).

### Importar conteúdo CSV para conjuntos de imagens de um local hospedado externamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição detalhada.
1. Clique em **InfoPanel Datafeed** para abrir o painel.
1. No campo de texto Local do arquivo CSV hospedado externamente (HTTP) , insira o URL para o arquivo CSV.
1. (Opcional) Nos campos Agendar atualização , especifique um horário para atualizar o conteúdo e clique em **Adicionar**.

   É possível selecionar várias vezes para atualização. Cada hora de atualização é exibida na caixa de texto Tempo de atualização . Para remover um horário agendado, selecione-o e clique em **Delete**.

1. (Opcional) Clique em **Executar atualização** para atualizar imediatamente o conteúdo.

