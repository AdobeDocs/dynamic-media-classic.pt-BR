---
title: Verificar arquivos de trabalho
description: Saiba como verificar arquivos de trabalho no Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Gerenciamento de ativos
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# Verificar arquivos de trabalho{#checking-job-files}

Para monitorar os uploads de arquivos para o Dynamic Media Classic e os arquivos que você publica nos servidores do Dynamic Media Classic, o Dynamic Media Classic oferece a página Trabalhos . Você pode revisar trabalhos de upload e publicação na página Trabalhos, verificar o status dos trabalhos e cancelar trabalhos de publicação nessa página. Você também pode agendar trabalhos de upload e publicação.

Ao fazer upload de ativos, um ícone giratório é exibido ao lado do menu Trabalhos, indicando que uma tarefa está em andamento e o número de arquivos em andamento. Você pode selecionar o ícone para ver mais informações sobre o trabalho ativo.

>[!NOTE]
>
>Uma lista de seus trabalhos publicados recentemente também está disponível na página Atividade recente . Selecione **[!UICONTROL Recent]** na barra Navegação global.

## Sobre a página Trabalhos {#about-the-jobs-page}

Selecione **[!UICONTROL Jobs]** na barra Navegação global para que a página Trabalhos seja aberta. Por padrão, as tarefas são listadas começando com as mais recentes.

As tarefas são listadas nessas categorias na guia Histórico da página Trabalhos :

* **[!UICONTROL Job Type]** - Um ícone indica o tipo de trabalho: Fazer upload e publicar são os tipos de trabalho mais comuns.

* **[!UICONTROL Job Name]** - O nome da tarefa. O nome inclui a parte do nome inserida pelo usuário e a data e hora.

* **[!UICONTROL Started]** - Quando o trabalho começou.

* **[!UICONTROL Total]** - O número de arquivos transferidos.

* **[!UICONTROL W (warnings)]** - O número de avisos na tarefa (se houver). Avisos indicam problemas com o trabalho que não afetou a conclusão geral do trabalho. Normalmente, esses avisos podem ser ignorados porque eles relatam sobre arquivos ocultos. Por exemplo, os arquivos `.DS_store` (Macintosh) e Thumbs.db (Windows®) contêm informações sobre como exibir arquivos de imagem para usuários. As entradas de aviso relacionadas a esses arquivos, no entanto, podem ser ignoradas porque não se referem à forma como esses arquivos são usados no Dynamic Media Classic. Você pode clicar duas vezes em um nome de trabalho para obter informações detalhadas sobre avisos.

* **[!UICONTROL E (errors)]** - Lista o número de erros no trabalho (se houver). Você pode clicar duas vezes em um nome de trabalho para obter informações detalhadas sobre erros.

* **[!UICONTROL Duration]** - Quanto tempo levou para concluir o trabalho.

* **[!UICONTROL Status]** - Mostra o status da tarefa.

* **[!UICONTROL Destination]** - Para trabalhos de upload, o nome da empresa e a pasta para a qual os arquivos foram carregados. Esta categoria não se aplica a trabalhos de publicação.

* **[!UICONTROL Submitted By]** - Lista quem fez upload dos ativos.

>[!NOTE]
>
>Você pode cancelar tarefas de publicação e upload em andamento selecionando o botão **[!UICONTROL Cancel]** ao lado da barra de progresso.

## Alterar exibições na página Trabalhos {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar tarefas ou alterar a visualização da guia Histórico da página Trabalhos :

* **[!UICONTROL Sorting]** - Selecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar a opção ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

* **[!UICONTROL Date Range]** - Selecione o  **[!UICONTROL Date Range]** menu e escolha uma opção para restringir a lista de tarefas à data atual, à semana anterior ou ao mês anterior. Selecione **[!UICONTROL Custom Date Range]** e insira um intervalo de datas específico.

* **[!UICONTROL Job Type]** - Selecione o  **[!UICONTROL Job Type]** menu e escolha  **[!UICONTROL Publish]** ou  **[!UICONTROL Upload]** para restringir a lista para publicar trabalhos ou fazer upload de trabalhos. Selecione **[!UICONTROL All]** para ver ambos os tipos de tarefas.

* **[!UICONTROL Show]** - Acesse  **[!UICONTROL Show]** >  **[!UICONTROL My Jobs]** ou  **[!UICONTROL Show]** >  **[!UICONTROL All Jobs]** para restringir a lista aos trabalhos solicitados ou aos trabalhos solicitados pelas pessoas em sua empresa.

## Exibir, copiar ou imprimir um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique duas vezes no nome de um relatório na página Trabalhos para que a página Detalhes do trabalho seja aberta. Esta página fornece um relatório de resumo sobre os arquivos na tarefa. Selecione **[!UICONTROL View Detail]** para visualizar a Dynamic Media Classic ID, o caminho de destino e as informações de status de uma entrada. Se você tiver carregado um arquivo PDF ou PostScript que requer fontes que não estão disponíveis no Dynamic Media Classic, o relatório listará as fontes ausentes.

Você pode copiar essas informações para a Área de transferência.

1. Clique duas vezes no nome de um relatório na página Trabalhos .
1. Na página Detalhes do trabalho , selecione **[!UICONTROL View Detail]** para obter um relatório detalhado sobre uma entrada.
1. Selecione **[!UICONTROL Copy to Clipboard]**.

## Gerenciar trabalhos recorrentes de upload e publicação {#handling-recurring-upload-and-publish-jobs}

Os trabalhos recorrentes de upload e publicação criados nas páginas Upload e Publicação são listados na guia Scheduled da página Jobs . É possível editar e excluir tarefas recorrentes na guia Scheduled .

Selecione o botão Trabalhos na barra Navegação Global e, na página Trabalhos, selecione a guia **[!UICONTROL Scheduled]** para poder editar e excluir tarefas recorrentes.

>[!NOTE]
>
>Você pode filtrar a lista de tarefas na guia **[!UICONTROL Scheduled]** com os menus **[!UICONTROL Job Type]** e **[!UICONTROL Show]**. Selecione um tipo de trabalho para restringir a lista para publicar trabalhos de um tipo específico. Selecione uma opção **[!UICONTROL Show]** se desejar exibir tarefas criadas ou tarefas criadas por todos na empresa.

### Editar, excluir, pausar e retomar tarefas recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione um trabalho recorrente na página Trabalhos e siga estas instruções se desejar editá-lo ou excluí-lo:

* **Editar um trabalho recorrente**  - Selecione o  **[!UICONTROL Edit]** botão e insira as informações da programação na caixa de diálogo Editar Trabalho Programado. Se desejar que o trabalho ocorra novamente em um intervalo de sua escolha, vá para **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Consulte [Criar um intervalo de tempo de trabalho de upload ou publicação personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Excluindo um trabalho recorrente**  - Selecione o  **[!UICONTROL Delete]** botão .

* **Pausa (e retomada) de um trabalho recorrente**  - Na coluna Ativo , desmarque uma caixa de seleção para pausar um trabalho; marque uma caixa de seleção para retomar um trabalho pausado.

### Criar um intervalo de tempo de trabalho de upload ou publicação personalizado {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo de tempo personalizado para um upload (via FTP) ou um trabalho de publicação, na página Upload or Publish , acesse **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Em seguida, insira números e curingas na caixa Regra que descreve um intervalo de tempo para que os trabalhos de upload ou publicação sejam repetidos.

A sintaxe para descrever intervalos de tempo de upload e publicação personalizados na caixa Regra é:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por exemplo, `0 15 10 * * ?` agende uma tarefa às 10:15.00 todos os dias.

As tabelas e a lista a seguir explicam como descrever um intervalo de tempo na caixa Regra.

Esta tabela mostra os incrementos de tempo, seus valores permitidos e os curingas suportados por eles:

| Incrementos de tempo | Valores permitidos | Comentários | Caracteres curinga compatíveis |
|--- |--- |--- |--- |
| Seconds | 0-59 |  | `, - * /` |
| Minutes | 0-59 |  | `, - * /` |
| Horas | 0-23 | Observe o uso de um relógio de 24 horas. | `, - * /` |
| Dia do mês | 1-31 | Não é possível especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um caractere curinga `?`. | `, - * / ? L C` |
| Mês | 1-12 ou Jan, Fev, Mar, Abr, maio, junho, julho, agosto, Set, Set, Out, nov, Dez | Os valores diferenciam maiúsculas de minúsculas. | `, - * /` |
| Dia da semana | Seg, Ter, Qua, Qui, Sex, Sáb, Dom | Os valores diferenciam maiúsculas de minúsculas. Não é possível especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um caractere curinga `?`. | `, - * / ? L C #` |
| Ano (opcional) | Empty ou 1970-2099 |  | `, - * /` |


Esta tabela descreve os caracteres curingas permitidos na caixa Regra e como usá-los:

| Caractere curinga | Nome | O que ele descreve |
|--- |--- |--- |
| `*` | Asterisco | Todos os valores (por exemplo, &quot;a cada minuto&quot;). |
| `?` | Ponto de interrogação | Nenhum valor específico (por exemplo, &quot;qualquer minuto dentro da hora especificada&quot;). |
| `,` | Vírgula | Outros valores (por exemplo, &quot;Segunda-feira e Quarta-feira&quot;). |
| `-` | Hífen | Intervalo de valores (por exemplo, &quot;de segunda a sexta-feira&quot;). |
| `/` | Barra | Incrementos (por exemplo, &quot;a cada 15 minutos&quot;). |
| `L` | Capital L | Último &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível somente para esses campos). Por exemplo, se o mês for janeiro, um valor L para o campo &quot;dia do mês&quot; programará a tarefa para 31 de janeiro. Para o campo &quot;dia da semana&quot;, você pode inserir esse caractere sozinho para agendar o trabalho no sábado. Você pode usá-lo com um número (por exemplo, `6L`) para especificar a última sexta-feira do mês. Não especifique `L` com os curingas de vírgula ou hífen. |
| `#` | Sinal numérico | &quot;Nono&quot; dia da semana do mês (disponível somente para o campo &quot;dia da semana&quot;). Por exemplo, `6#3` no campo &quot;dia da semana&quot; especifica a terceira sexta-feira do mês. O `6` indica &quot;sexta-feira&quot; (o sexto dia da semana) e o `3` indica a terceira ocorrência no mês. |
| `C` | # Capital C | Primeiro calendário &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível apenas para estes campos). Por exemplo, especificar um valor de `1C` para &quot;dia do mês&quot; agende o primeiro dia no calendário que ocorre em ou após o quinto dia. Para o campo &quot;dia da semana&quot;, a especificação de `1C` agende o primeiro dia no calendário que ocorre no domingo ou depois dele |

Essa lista fornece exemplos de descrição dos intervalos de tempo na caixa Regra:

* `0 0 12 * * ?` : Nove todos os dias
* `0 15 10 ? * *` : 10:15 todos os dias
* `0 0/5 14 * * ?`: A cada 5 minutos entre 2:00 e 2:55 PM todos os dias
* `0 0/5 14,18 * * ?` : A cada 5 minutos entre 2:00 e 2:55 PM todos os dias e a cada 5 minutos entre 6:00 e 6:55 pm todos os dias
* `0 10,44 14 ? 3` : Queijo às 14h10 e 14h44 toda quarta-feira em março
* `0 15 10 ? *` : Seg-Sex às 10h15 todos os dias da semana
* `0 15 10 20 * ?` : Às 10h15 do dia 20 de cada mês
* `0 15 10 L * ?` : Às 10h15 do último dia de cada mês
* `0 15 10 ? * 6L` : Às 10h15 da última sexta-feira de cada mês
* `0 15 10 * * 6#3` : Às 10h15 da terceira sexta-feira de cada mês

## Usar um trabalho de upload ou publicação como acionador {#using-an-upload-or-publish-job-as-a-trigger}

Ao fazer upload de ativos via FTP ou executar um trabalho de publicação, você pode agendar um trabalho subsequente para começar quando o upload for concluído. (Se outras tarefas estiverem programadas para começar então, a tarefa agendada aqui estará na fila atrás delas.) A nova tarefa envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse trabalho de upload de seguimento recebe o mesmo nome do trabalho de upload atual, mas com o prefixo _Pub.

Para fazer com que um trabalho de upload ou publicação acione outro trabalho, selecione **[!UICONTROL Advanced]** na página Upload or Publish . Em seguida, insira o URL no campo de texto Notificação HTTP .
