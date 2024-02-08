---
title: Verificar arquivos de trabalho
description: Saiba como verificar arquivos de trabalho no Adobe Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '1560'
ht-degree: 0%

---

# Verificar arquivos de trabalho{#checking-job-files}

Para monitorar os uploads de arquivos para o Adobe Dynamic Media Classic e os arquivos publicados nos servidores da Adobe Dynamic Media Classic, a Adobe Dynamic Media Classic oferece a página Jobs. Você pode revisar e publicar trabalhos na página Trabalhos, verificar o status dos trabalhos e cancelar trabalhos de publicação nesta página. Você também pode agendar trabalhos de upload e publicação.

Ao fazer upload de ativos, um ícone giratório é exibido ao lado do menu Trabalhos, indicando que um trabalho está em andamento e o número de arquivos em andamento. Você pode selecionar o ícone para ver mais informações sobre o job ativo.

>[!NOTE]
>
>Uma lista de tarefas publicadas recentemente também está disponível na página Atividade recente. Selecionar **[!UICONTROL Recent]** na barra Navegação global.

## Sobre a página Jobs {#about-the-jobs-page}

Selecionar **[!UICONTROL Jobs]** na barra Navegação global, para que a página Trabalhos seja aberta. Por padrão, as tarefas são listadas começando com a mais recente.

Os jobs são listados nestas categorias na guia Histórico da página Jobs:

* **[!UICONTROL Job Type]** - Um ícone indica o tipo de trabalho: Upload e Publish são os tipos mais comuns de trabalho.

* **[!UICONTROL Job Name]** - O nome do trabalho. O nome inclui a parte inserida pelo usuário do nome e a data e hora.

* **[!UICONTROL Started]** - Quando o trabalho começou.

* **[!UICONTROL Total]** - O número de arquivos transferidos.

* **[!UICONTROL W (warnings)]** - O número de avisos na tarefa (se houver). Os avisos indicam problemas com o trabalho que não afetaram a conclusão geral. Normalmente, esses avisos podem ser ignorados, pois eles informam sobre arquivos ocultos. Por exemplo, `.DS_store` arquivos (Mac) e arquivos thumbs.db (Windows®) contêm informações sobre como exibir arquivos de imagem para os usuários. Entradas de aviso relacionadas a esses arquivos, no entanto, podem ser ignoradas, pois não se referem à forma como esses arquivos são usados no Adobe Dynamic Media Classic. Você pode clicar duas vezes em um nome de job para obter informações detalhadas sobre avisos.

* **[!UICONTROL E (errors)]** - Lista o número de erros na tarefa (se houver). Você pode clicar duas vezes em um nome de job para obter informações detalhadas sobre erros.

* **[!UICONTROL Duration]** - Quanto tempo levou para completar o trabalho.

* **[!UICONTROL Status]** - Mostra o status do trabalho.

* **[!UICONTROL Destination]** - Para trabalhos de upload, o nome da empresa e a pasta na qual os arquivos foram carregados. Esta categoria não se aplica a trabalhos de publicação.

* **[!UICONTROL Submitted By]** - Lista quem carregou os ativos.

>[!NOTE]
>
>Você pode cancelar trabalhos de publicação e upload em andamento selecionando o **[!UICONTROL Cancel]** botão ao lado da barra de progresso.

## Alterar exibições na página Trabalhos {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar jobs ou alterar a exibição da guia Histórico da página Jobs:

* **[!UICONTROL Sorting]** - Selecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar a opção ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

* **[!UICONTROL Date Range]** - Selecione o **[!UICONTROL Date Range]** e escolha uma opção para limitar a lista de tarefas à data atual, à semana anterior ou ao mês anterior. Selecionar **[!UICONTROL Custom Date Range]**, em seguida, insira um intervalo de datas específico.

* **[!UICONTROL Job Type]** - Selecione o **[!UICONTROL Job Type]** e escolha **[!UICONTROL Publish]** ou **[!UICONTROL Upload]** para restringir a lista para publicar trabalhos ou fazer upload de trabalhos. Selecionar **[!UICONTROL All]** para ver ambos os tipos de jobs.

* **[!UICONTROL Show]** - Vá para **[!UICONTROL Show]** > **[!UICONTROL My Jobs]** ou **[!UICONTROL Show]** > **[!UICONTROL All Jobs]** para restringir a lista a trabalhos solicitados por você ou trabalhos solicitados por pessoas em sua empresa.

## Exibir, copiar ou imprimir um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique duas vezes no nome de um relatório na página Trabalhos para que a página Detalhes do trabalho seja aberta. Esta página fornece um relatório resumido sobre os arquivos do job. Selecionar **[!UICONTROL View Detail]** assim, você pode ver a Adobe Dynamic Media Classic ID de uma entrada, o caminho de destino e as informações de status. Se você carregou um arquivo PDF ou PostScript que requer fontes que não estão disponíveis no Adobe Dynamic Media Classic, o relatório listará as fontes ausentes.

Você pode copiar essas informações para a Área de transferência.

1. Clique duas vezes no nome de um relatório na página Trabalhos.
1. Na página Detalhes do Job, selecione **[!UICONTROL View Detail]** para obter um relatório detalhado sobre uma entrada.
1. Selecionar **[!UICONTROL Copy to Clipboard]**.

## Lidar com trabalhos recorrentes de upload e publicação {#handling-recurring-upload-and-publish-jobs}

Os trabalhos de upload e publicação recorrentes, criados nas páginas Upload e Publicar, são listados na guia Programado da página Trabalhos. É possível editar e excluir tarefas recorrentes na guia Scheduled.

Selecione o botão Trabalhos na barra Navegação global e, na página Trabalhos, selecione o botão **[!UICONTROL Scheduled]** para poder editar e excluir tarefas recorrentes.

>[!NOTE]
>
>É possível filtrar a lista de trabalhos na **[!UICONTROL Scheduled]** com a guia **[!UICONTROL Job Type]** e **[!UICONTROL Show]** menus. Selecione um tipo de trabalho para restringir a lista para publicar trabalhos de um tipo específico. Selecione um **[!UICONTROL Show]** opção se quiser exibir os trabalhos criados ou os trabalhos criados por todos na empresa.

### Editar, excluir, pausar e retomar tarefas recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione uma tarefa recorrente na página Tarefas e siga estas instruções se desejar editá-la ou excluí-la:

* **Editar uma tarefa recorrente** - Selecione o **[!UICONTROL Edit]** e especifique as informações de programação na caixa de diálogo Editar Job Programado. Se quiser que o job seja repetido em um intervalo de sua escolha, vá para **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Consulte [Criar um intervalo de tempo de trabalho personalizado de carregamento ou publicação](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Exclusão de uma tarefa recorrente** - Selecione o **[!UICONTROL Delete]** botão.

* **Pausa (e retomada) de uma tarefa recorrente** - Na coluna Ativo, desmarque uma caixa de seleção para pausar um trabalho; marque uma caixa de seleção para retomar um trabalho que foi pausado.

### Criar um intervalo de tempo de trabalho personalizado de carregamento ou publicação {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo personalizado para um upload (por meio do FTP) ou um trabalho de publicação, na página Fazer upload ou publicar, vá para **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Em seguida, insira números e curingas na caixa Regra descrevendo um intervalo de tempo para que os trabalhos de upload ou publicação voltem a ocorrer.

A sintaxe para descrever os intervalos de tempo personalizados de upload e publicação na caixa Regra é:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por exemplo, `0 15 10 * * ?` O programa um trabalho às 10h15 todos os dias.

As tabelas e a lista a seguir explicam como descrever um intervalo de tempo na caixa Regra.

Esta tabela mostra os incrementos de tempo, seus valores permitidos e os curingas suportados por eles:

| Incrementos de tempo | Valores permitidos | Comentários | Caracteres curinga compatíveis |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | `, - * /` |
| Minutes | 0-59 |  | `, - * /` |
| Horas | 0-23 | Observe o uso de um relógio de 24 horas. | `, - * /` |
| Dia do mês | 1-31 | Você não pode especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um `?` caractere curinga. | `, - * / ? L C` |
| Month | 1-12 ou Jan, Fev, Mar, Abr, maio, Jun, Jul, Ago, Set, Set, Out, Nov, Dez | Os valores diferenciam maiúsculas de minúsculas. | `, - * /` |
| Dia da semana | Seg, Ter, Qua, Qui, Sex, Sáb, Sol | Os valores diferenciam maiúsculas de minúsculas. Você não pode especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um `?` caractere curinga. | `, - * / ? L C #` |
| Ano (opcional) | Vazio ou 1970-2099 |  | `, - * /` |


Esta tabela descreve os caracteres curingas permitidos na caixa Regra e como usá-los:

| Caractere curinga | Nome | O que ele descreve |
| --- | --- | --- |
| `*` | Asterisco | Todos os valores (por exemplo, &quot;a cada minuto&quot;). |
| `?` | Ponto de interrogação | Nenhum valor específico (por exemplo, &quot;qualquer minuto dentro da hora especificada&quot;). |
| `,` | Vírgula | Outros valores (por exemplo, &quot;segunda e quarta-feira&quot;). |
| `-` | Hífen | Intervalo de valores (por exemplo, &quot;de segunda a sexta-feira&quot;). |
| `/` | Barra inclinada | Incrementos (por exemplo, &quot;a cada 15 minutos&quot;). |
| `L` | L maiúsculo | Último &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível somente para esses campos). Por exemplo, se o mês for janeiro, um valor L para o campo &quot;dia do mês&quot; agendará o trabalho para 31 de janeiro. Para o campo &quot;dia da semana&quot;, você pode inserir esse caractere sozinho para agendar o trabalho no sábado. Você pode usá-lo com um número (por exemplo, `6L`) para especificar a última sexta-feira do mês. Não especificar `L` com os curingas de vírgula ou hífen. |
| `#` | Sinal numérico | Dia da semana &quot;enésimo&quot; do mês (disponível somente para o campo &quot;dia da semana&quot;). Por exemplo, `6#3` no campo &quot;dia da semana&quot; especifica a terceira sexta-feira do mês. A variável `6` significa &quot;sexta-feira&quot; (o sexto dia da semana) e o `3` indica a terceira ocorrência do mês. |
| `C` | # Maiúscula C | Primeiro &quot;dia do mês&quot; ou &quot;dia da semana&quot; do calendário (disponível somente para esses campos). Por exemplo, especificar um valor de `1C` para &quot;dia do mês&quot; agenda o primeiro dia no calendário que ocorre no quinto dia ou depois dele. Para o campo &quot;dia da semana&quot;, especificando `1C` programa o primeiro dia do calendário que ocorre no domingo ou depois. |

Esta lista fornece exemplos de descrição de intervalos de tempo na caixa Regra:

* `0 0 12 * * ?` : Meio-dia todos os dias
* `0 15 10 ? * *` : 10:15 todos os dias
* `0 0/5 14 * * ?`: a cada 5 minutos entre 14h e 14h55 todos os dias
* `0 0/5 14,18 * * ?` : a cada 5 minutos entre 14h e 14h55 todos os dias e a cada 5 minutos entre 18h e 18h55 todos os dias
* `0 10,44 14 ? 3` : Qua às 14h10 e 14h44 toda quarta-feira de março
* `0 15 10 ? *` : Segunda a sexta às 10h15, todos os dias da semana
* `0 15 10 20 * ?` : Às 10h15 do dia 20 de cada mês
* `0 15 10 L * ?` : Às 10h15 do último dia de cada mês
* `0 15 10 ? * 6L` : Às 10h15 da última sexta-feira de cada mês
* `0 15 10 * * 6#3` : Às 10h15 da terceira sexta-feira de cada mês

## Usar um trabalho de upload ou publicação como acionador {#using-an-upload-or-publish-job-as-a-trigger}

Ao fazer upload de ativos por FTP ou executar um trabalho de publicação, você pode agendar um trabalho subsequente para começar quando o upload estiver concluído. (Se outros trabalhos estiverem programados para começar, o trabalho programado aqui será enfileirado atrás deles.) O novo trabalho envia uma notificação para o endereço especificado, para que o código nesse local possa ser acionado. Esse trabalho de upload complementar recebe o mesmo nome do trabalho de upload atual, mas com o prefixo _Pub.

Para fazer um trabalho de upload ou publicação acionar outro trabalho, selecione **[!UICONTROL Advanced]** na página Fazer upload ou publicar. Em seguida, insira o URL no campo de texto Notificação HTTP.
