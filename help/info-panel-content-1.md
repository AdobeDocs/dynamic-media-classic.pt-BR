---
title: Gerenciando conteúdo do painel Informações em Conjuntos de imagens
seo-title: Gerenciamento do conteúdo do painel de informações em Conjuntos de imagens
description: 'null'
seo-description: Saiba como gerenciar o conteúdo do Painel Informações em Conjuntos de imagens.
uuid: ed 7 b 4344-f 180-41 fc-a 95 a -62 a 9767 dc 056
contentOwner: rbrough
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
content-type: reference
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/image_ sets
discoiquuid: ba 5 d 1 fb 1-af 54-471 c-a 471-853 ace 7 f 72 fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gerenciando conteúdo do painel Informações em Conjuntos de imagens{#managing-info-panel-content-in-image-sets}

Além de usar o texto do Mapa de imagem para sobreposições em Conjuntos de imagens, você pode usar um painel de informações para adicionar quantidades maiores de texto de sobreposição, incluindo links. Você também pode gerenciar o infopanel usando atualizações de conteúdo de cache e programação cronometradas.

Você pode gerenciar sua configuração e dados do infopanel usando os seguintes recursos no Sistema de publicação Scene 7:

* O painel de Configuração do infopanel permite especificar o modelo usado para exibir o texto do painel de informações, uma resposta padrão para erros e o número de horas em que as informações são armazenadas em cache. Além disso, você pode especificar se o Conjunto de imagens é publicado automaticamente.
* O painel Datafanel Datafeed permite especificar um arquivo CSV que contém o texto que você deseja que apareça no texto de sobreposição do painel Informações, bem como horários de agendamento para atualizar as informações.
* A caixa de diálogo Importar metadados permite importar um arquivo TXT delimitado por tabulação contendo as informações de texto de sobreposição. Você pode usar essa opção TXT ou o painel Datafanel Datafeed com a opção de arquivo CSV para o texto de sobreposição.

## Configurar um modelo de resposta para Conjuntos de imagens {#set-up-a-response-template-for-image-sets}

Você pode selecionar um dos três modelos de resposta predefinidos para exibir texto em um Painel de informações. Esses modelos de resposta predefinidos determinam como suas informações são apresentadas no Painel Informações: quantas colunas e linhas, tamanho da face de tipos, fonte e assim por diante. Você pode selecionar um modelo de resposta predefinido ou criar um dos seus próprios.

**Configuração de um modelo de resposta**

1. Clique duas vezes em seu Conjunto de imagens para abri-lo na Exibição de detalhes.
1. Clique **em Configurações do infopanel** para desdobrar o painel.
1. Na lista suspensa Modelo de resposta, execute um dos procedimentos a seguir:

   * Selecione Padrão para usar a resposta padrão. O XML para o design de modelo aparece, esmaecido, na caixa de texto Modelo de usuário.
   * Selecione Personalizado para criar seu próprio modelo de resposta. Na caixa de texto Modelo de usuário, digite a definição XML modelo. Você pode usar o modelo padrão que já está definido na caixa de texto como base para sua própria resposta.

1. (Opcional) Na caixa Resposta padrão, digite o texto que deseja exibir se o Dynamic Media Classic encontrar um erro ao recuperar as informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de conjunto de imagens, mas sem identificador de rolagem, esta mensagem será exibida para o usuário.
1. No campo de texto TTL de resposta, digite o número de horas que deseja esperar antes de armazenar os dados em cache.

   * Defina um número mais baixo se os dados forem atualizados com frequência durante o dia.
   * Defina um número maior se os dados forem relativamente estáveis e não exigir atualização frequente durante o dia. O padrão é dez horas.

1. Clique **em Carregar** para carregar o conteúdo do painel de informações, com base nos valores rollover_ key, para s 7 informações.
1. Na caixa de diálogo S 7 Info Upload, navegue até o arquivo que deseja usar e clique em **Carregar**.

   Formatos de arquivo suportados são arquivos delimitados por TAB com codificação UTF -16 e arquivos CSV com codificação ASCII. Para arquivos CSV, caracteres não ASCII devem ser codificados por HTML.

1. No painel Configuração do infopanel, clique **em Publicar**.

## Importar conteúdo de origem para o Painel Informações em Conjuntos de imagens {#import-source-content-for-the-info-panel-in-image-sets}

É possível usar um arquivo CSV (valores separados por vírgula) com codificação ASCII (caracteres não ASCII devem ser codificados por HTML) ou um arquivo delimitado por tabulação para o texto de origem de um painel de informações para um conjunto de imagens. Os arquivos delimitados por tabulação devem usar a codificação UTF -16 (Unicode). Você importa os diferentes tipos de arquivo usando diferentes métodos.

Ao formatar o conteúdo de origem, lembre-se das seguintes diretrizes:

* Os dados delimitados por tabulação e vírgula devem conter quantas colunas forem necessárias para o modelo de sobreposição.
* O primeiro item ou coluna de dados deve ser o identificador de rolagem (associado ao valor rollover_ key dos urls do mapa de imagem).
* Verifique se cada item delimitado por tabulação ou vírgula depois do identificador é o item que você deseja substituir no modelo de resposta (para que a primeira coluna seja substituída em $ 1 $, a segunda coluna até $ 2 $ e assim por diante).

### Importar conteúdo CSV em Conjuntos de imagens a partir de um local externo hospedado {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Clique duas vezes no Conjunto de imagens para abri-lo na Exibição de detalhes.
1. Clique **em infopanel Datafeed** para desdobrar o painel.
1. No campo de texto Local hospedado externamente (HTTP), insira o URL para o arquivo CSV.
1. (Opcional) Nos campos Agendar atualização, especifique um tempo para atualizar o conteúdo e clique **em Adicionar**.

   É possível selecionar várias vezes para atualizar. Cada hora de atualização aparece na caixa de texto Atualizar horas. Para remover um horário agendado, selecione-o e clique **em Excluir**.

1. (Opcional) Clique **em Executar atualização** para atualizar imediatamente o conteúdo.

