---
title: Verificar arquivos de trabalho
description: Saiba como verificar arquivos de trabalho no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1573'
ht-degree: 0%

---

# Verificar arquivos de trabalho{#checking-job-files}

Para monitorar os uploads de arquivos para o Adobe Dynamic Media Classic e os arquivos publicados nos servidores da Adobe Dynamic Media Classic, a Adobe Dynamic Media Classic oferece a página Jobs. Você pode revisar, fazer upload e publicar trabalhos na página Trabalhos, verificar o status dos trabalhos e cancelar trabalhos de publicação nesta página. Você também pode agendar trabalhos de upload e publicação.

Ao fazer upload de ativos, um ícone giratório é exibido ao lado do menu Trabalhos, indicando que um trabalho está em andamento e o número de arquivos em andamento. Você pode selecionar o ícone para ver mais informações sobre o job ativo.

>[!NOTE]
>
>Uma lista de tarefas publicadas recentemente também está disponível na página Atividade recente. Selecione **[!UICONTROL Recent]** na barra de Navegação Global.

## Sobre a página Jobs {#about-the-jobs-page}

Selecione **[!UICONTROL Jobs]** na barra de Navegação Global para que a página Trabalhos seja aberta. Por padrão, as tarefas são listadas começando com a mais recente.

Os jobs são listados nestas categorias na guia Histórico da página Jobs:

* **[!UICONTROL Job Type]**: Um ícone indica o tipo de trabalho: Carregar e Publicar são os tipos de trabalho mais comuns.

* **[!UICONTROL Job Name]**: O nome do trabalho. O nome inclui a parte inserida pelo usuário do nome e a data e hora.

* **[!UICONTROL Started]**: Quando o trabalho começou.

* **[!UICONTROL Total]**: O número de arquivos transferidos.

* **[!UICONTROL W (warnings)]**: O número de avisos no trabalho (se houver). Os avisos indicam problemas com o trabalho que não afetaram a conclusão geral. Normalmente, esses avisos podem ser ignorados, pois eles informam sobre arquivos ocultos. Por exemplo, os arquivos `.DS_store` (Mac) e Thumbs.db (Windows®) contêm informações sobre como exibir arquivos de imagem para os usuários. Entradas de aviso relacionadas a esses arquivos, no entanto, podem ser ignoradas, pois não se referem à forma como esses arquivos são usados no Adobe Dynamic Media Classic. Você pode clicar duas vezes em um nome de job para obter informações detalhadas sobre avisos.

* **[!UICONTROL E (errors)]**: lista o número de erros no trabalho (se houver). Você pode clicar duas vezes em um nome de job para obter informações detalhadas sobre erros.

* **[!UICONTROL Duration]**: Quanto tempo levou para concluir o trabalho.

* **[!UICONTROL Status]**: mostra o status do trabalho.

* **[!UICONTROL Destination]**: Para trabalhos de carregamento, o destino é o nome da empresa e a pasta na qual os arquivos foram carregados. Esta categoria não se aplica a trabalhos de publicação.

* **[!UICONTROL Submitted By]**: lista quem carregou os ativos.

>[!NOTE]
>
>Você pode cancelar trabalhos de publicação e carregamento em andamento selecionando o botão **[!UICONTROL Cancel]** ao lado da barra de progresso.

## Alterar exibições na página Trabalhos {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar jobs ou alterar a exibição da guia Histórico da página Jobs:

* **[!UICONTROL Sorting]**: Selecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar a opção ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

* **[!UICONTROL Date Range]**: Selecione o menu **[!UICONTROL Date Range]** e escolha uma opção para limitar a lista de trabalhos à data atual, à semana anterior ou ao mês anterior. Selecione **[!UICONTROL Custom Date Range]** e insira um intervalo de datas específico.

* **[!UICONTROL Job Type]**: Selecione o menu **[!UICONTROL Job Type]** e escolha **[!UICONTROL Publish]** ou **[!UICONTROL Upload]** para restringir a lista para publicar trabalhos ou carregar trabalhos. Selecione **[!UICONTROL All]** para ver os dois tipos de trabalhos.

* **[!UICONTROL Show]**: Vá para **[!UICONTROL Show]** > **[!UICONTROL My Jobs]** ou **[!UICONTROL Show]** > **[!UICONTROL All Jobs]** para restringir a lista a trabalhos que você solicitou ou trabalhos que as pessoas da sua empresa solicitaram.

## Exibir, copiar ou imprimir um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique duas vezes no nome de um relatório na página Trabalhos para que a página Detalhes do trabalho seja aberta. Esta página fornece um relatório resumido sobre os arquivos do job. Selecione **[!UICONTROL View Detail]** para que você possa ver a Adobe Dynamic Media Classic ID de uma entrada, o caminho de destino e as informações de status. Se você carregou um arquivo PDF ou PostScript que requer fontes que não estão disponíveis no Adobe Dynamic Media Classic, o relatório listará as fontes ausentes.

Você pode copiar essas informações para a Área de transferência.

1. Clique duas vezes no nome de um relatório na página Trabalhos.
1. Na página Detalhes do Trabalho, selecione **[!UICONTROL View Detail]** para obter um relatório detalhado sobre uma entrada.
1. Selecione **[!UICONTROL Copy to Clipboard]**.

## Lidar com trabalhos recorrentes de upload e publicação {#handling-recurring-upload-and-publish-jobs}

Os trabalhos de upload e publicação recorrentes, criados nas páginas Upload e Publicar, são listados na guia Programado da página Trabalhos. É possível editar e excluir tarefas recorrentes na guia Scheduled.

Selecione o botão Trabalhos na barra de Navegação Global e, na página Trabalhos, selecione a guia **[!UICONTROL Scheduled]** para poder editar e excluir trabalhos recorrentes.

>[!NOTE]
>
>Você pode filtrar a lista de trabalhos na guia **[!UICONTROL Scheduled]** com os menus **[!UICONTROL Job Type]** e **[!UICONTROL Show]**. Selecione um tipo de trabalho para restringir a lista para publicar trabalhos de um tipo específico. Selecione uma opção de **[!UICONTROL Show]** para exibir os trabalhos criados por você ou os trabalhos criados por todos na sua empresa.

### Editar, excluir, pausar e retomar tarefas recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione uma tarefa recorrente na página Tarefas e siga estas instruções se desejar editá-la ou excluí-la:

* **Editar um trabalho recorrente**: selecione o botão **[!UICONTROL Edit]** e insira as informações de agendamento na caixa de diálogo Editar Trabalho Agendado. Se você quiser que o trabalho se repita em um intervalo de sua escolha, vá para **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Consulte [Criar um intervalo de tempo de trabalho de carregamento ou publicação personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Excluindo um trabalho recorrente**: selecione o botão **[!UICONTROL Delete]**.

* **Pausando (e retomando) um trabalho recorrente**: na coluna Ativo, desmarque uma caixa de seleção para pausar um trabalho; marque uma caixa de seleção para retomar um trabalho pausado.

### Criar um intervalo de tempo de trabalho personalizado de carregamento ou publicação {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo personalizado para um carregamento (por meio do FTP) ou um trabalho de publicação, na página Carregar ou Publicar, vá para **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Em seguida, insira números e curingas na caixa Regra descrevendo um intervalo de tempo para que os trabalhos de upload ou publicação voltem a ocorrer.

A sintaxe para descrever os intervalos de tempo personalizados de upload e publicação na caixa Regra é:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por exemplo, `0 15 10 * * ?` agenda um trabalho às 10:15.00 todos os dias.

As tabelas e a lista a seguir explicam como descrever um intervalo de tempo na caixa Regra.

Esta tabela mostra os incrementos de tempo, seus valores permitidos e os curingas suportados por eles:

| Incrementos de tempo | Valores permitidos | Comentários | Caracteres curinga compatíveis |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | `,: * /` |
| Minutes | 0-59 |  | `,: * /` |
| Horas | 0-23 | Observe o uso de um relógio de 24 horas. | `,: * /` |
| Dia do mês | 1-31 | Você não pode especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um caractere curinga `?`. | `,: * / ? L C` |
| Month | 1-12 ou Jan, Fev, Mar, Abr, maio, Jun, Jul, Ago, Set, Set, Out, Nov, Dez | Os valores diferenciam maiúsculas de minúsculas. | `,: * /` |
| Dia da semana | Seg, Ter, Qua, Qui, Sex, Sáb, Sol | Os valores diferenciam maiúsculas de minúsculas. Você não pode especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um caractere curinga `?`. | `,: * / ? L C #` |
| Ano (opcional) | Vazio ou 1970-2099 |  | `,: * /` |


Esta tabela descreve os caracteres curingas permitidos na caixa Regra e como usá-los:

| Caractere curinga | Nome | O que ele descreve |
| --- | --- | --- |
| `*` | Asterisco | Todos os valores (por exemplo, &quot;a cada minuto&quot;). |
| `?` | Ponto de interrogação | Nenhum valor específico (por exemplo, &quot;qualquer minuto dentro da hora especificada&quot;). |
| `,` | Vírgula | Outros valores (por exemplo, &quot;segunda e quarta-feira&quot;). |
| `-` | Hífen | Intervalo de valores (por exemplo, &quot;de segunda a sexta-feira&quot;). |
| `/` | Barra inclinada | Incrementos (por exemplo, &quot;a cada 15 minutos&quot;). |
| `L` | L maiúsculo | Último &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível somente para esses campos). Por exemplo, se o mês for janeiro, um valor L para o campo &quot;dia do mês&quot; agendará o trabalho para 31 de janeiro. Para o campo &quot;dia da semana&quot;, você pode inserir esse caractere sozinho para agendar o trabalho no sábado. Você pode usá-lo com um número (por exemplo, `6L`) para especificar a última sexta-feira do mês. Não especifique `L` com os curingas de vírgula ou hífen. |
| `#` | Sinal numérico | Dia da semana &quot;enésimo&quot; do mês (disponível somente para o campo &quot;dia da semana&quot;). Por exemplo, `6#3` no campo &quot;dia da semana&quot; especifica a terceira sexta-feira do mês. O `6` denota &quot;sexta-feira&quot; (o sexto dia da semana) e o `3` denota a terceira ocorrência no mês. |
| `C` | # Maiúscula C | Primeiro &quot;dia do mês&quot; ou &quot;dia da semana&quot; do calendário (disponível somente para esses campos). Por exemplo, especificar um valor de `1C` para &quot;dia do mês&quot; agenda o primeiro dia no calendário que ocorre no quinto dia ou depois dele. Para o campo &quot;dia da semana&quot;, especificar `1C` agenda o primeiro dia no calendário que ocorre no domingo ou depois. |

Esta lista fornece exemplos de descrição de intervalos de tempo na caixa Regra:

* `0 0 12 * * ?` : ao meio-dia todos os dias
* `0 15 10 ? * *` : 10:15 am todos os dias
* `0 0/5 14 * * ?`: a cada 5 minutos entre 2:00 e 2:55 pm todos os dias
* `0 0/5 14,18 * * ?` : a cada 5 minutos entre 2:00 e 2:55 pm todos os dias e a cada 5 minutos entre 6:00 e 6:55 pm todos os dias
* `0 10,44 14 ? 3` : quarta-feira às 14h10 e 14h20 todas as quartas-feiras de março:10:44
* `0 15 10 ? *` : segunda a sexta às 10:15, todos os dias da semana
* `0 15 10 20 * ?` : Às 10:15 da manhã do dia 20 de cada mês
* `0 15 10 L * ?` : Às 10:15 da manhã, no último dia de cada mês
* `0 15 10 ? * 6L` : Às 10:15 da última sexta-feira de cada mês
* `0 15 10 * * 6#3` : Às 10:15 da terceira sexta-feira de cada mês

## Usar um trabalho de upload ou publicação como acionador {#using-an-upload-or-publish-job-as-a-trigger}

Ao fazer upload de ativos por FTP ou executar um trabalho de publicação, você pode agendar um trabalho subsequente para começar quando o upload estiver concluído. (Se outros trabalhos estiverem programados para começar, o trabalho programado aqui será enfileirado atrás deles.) O novo trabalho envia uma notificação para o endereço especificado, para que o código nesse local possa ser acionado. Esse trabalho de upload complementar recebe o mesmo nome do trabalho de upload atual, mas com o prefixo _Pub.

Para fazer um trabalho de carregamento ou publicação acionar outro trabalho, selecione **[!UICONTROL Advanced]** na página Carregar ou Publicar. Em seguida, insira o URL no campo de texto Notificação HTTP.
