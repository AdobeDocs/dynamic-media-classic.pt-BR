---
title: Teste da integração ao visualizar um relatório do Adobe Analytics
seo-title: Teste da integração ao visualizar um relatório do Adobe Analytics
description: 'null'
seo-description: Saiba como testar a integração visualizando um relatório do Adobe Analytics.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 ddc 89 ff-d 2 e 9-42 eb-a 442-aa 6 b 9871 c 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Teste da integração ao visualizar um relatório do Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Depois de criar as variáveis necessárias no Adobe Analytics, vinculá-las aos eventos do Dynamic Media Classic e concluir as etapas de implementação necessárias, em seguida, você deve testar a configuração. Você pode testar e verificar se os dados estão sendo capturados, dentro do próprio Adobe Analytics. Se a configuração funcionar aqui, nenhuma etapa adicional será necessária. Considerando que você siga as etapas acima e vincule seus dados do evento do Dynamic Media Classic a uma ou mais variáveis de tráfego personalizadas, siga este fluxo de trabalho para testar seus dados dentro do Adobe Analytics.

**Para testar a integração, visualize um relatório do Adobe Analytics**

1. Inicie o visualizador do Dynamic Media Classic a partir da sua conta, principalmente uma que transmite a métrica que você deseja capturar e interaja com ela para criar alguns dados de eventos.

   Por exemplo, se quiser medir as visualizações alternativas mais populares em um Conjunto de imagens, visualize um Conjunto de imagens e clique em diferentes imagens miniaturas.

1. Dentro do Adobe Analytics, vá para Tráfego personalizado &gt; Tráfego personalizado 1-10 &gt; [Nome da prop], selecionando seu nome de prop de tráfego nas opções do menu.

   Por exemplo, para acessar o loadasset loadasset em nossa conta de amostra, a escolha de menu apropriada seria Tráfego personalizado &gt; Tráfego personalizado 1-10 &gt; loadasset. Se você tiver mais de dez props personalizados, também poderá visualizar opções de menu adicionais.

1. Exiba o gráfico produzido pelo Adobe Analytics. Observe que isso normalmente é apenas os dados de uma única métrica. Se você também quiser saber com qual ativo esses dados estão associados (por exemplo, qual vídeo está sendo assistido apenas em 50% ou qual imagem em um conjunto é mais popular), certifique-se de capturar os dados do ativo desse evento também.

>[!NOTE]
>
>Todos os dados do visualizador do Dynamic Media Classic são exibidos e reportados nos relatórios de Tráfego personalizado ou nos relatórios de Conversão personalizada do Adobe Analytics.

Para obter mais informações, consulte [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
