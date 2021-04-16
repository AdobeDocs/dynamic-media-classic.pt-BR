---
title: Verificando arquivos de trabalho
description: Saiba como verificar arquivos de trabalho.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
translation-type: tm+mt
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 1%

---

# Verificando arquivos de trabalho{#checking-job-files}

Para monitorar os uploads de arquivos para o Dynamic Media Classic e os arquivos que você publica nos servidores do Dynamic Media Classic, o Dynamic Media Classic oferece a página Trabalhos . Você pode revisar trabalhos de upload e publicação na página Trabalhos, verificar o status dos trabalhos e cancelar trabalhos de publicação nessa página. Você também pode agendar trabalhos de upload e publicação.

Ao fazer upload de ativos, um ícone giratório é exibido ao lado do menu Trabalhos, indicando que uma tarefa está em andamento e o número de arquivos em andamento. Você pode clicar no ícone para ver mais informações sobre o trabalho ativo.

>[!NOTE]
>
>Uma lista de seus trabalhos publicados recentemente também está disponível na página Atividade recente . Clique em **[!UICONTROL Recent]** na barra Navegação global para abrir esta página.

## Sobre a página Trabalhos {#about-the-jobs-page}

Selecione **[!UICONTROL Jobs]** na barra Navegação global para abrir a página Tarefas. Por padrão, as tarefas são listadas começando com as mais recentes.

As tarefas são listadas nessas categorias na guia Histórico da página Trabalhos :

**Tipo** de trabalhoUm ícone indica o tipo de trabalho: Fazer upload e publicar são os tipos de trabalho mais comuns.

**** Nome do trabalhoO nome do trabalho. O nome inclui a parte do nome inserida pelo usuário e a data e hora.

**** IniciadoQuando o trabalho começou.

**** TotalO número de arquivos transferidos.

**W (avisos)** O número de avisos na tarefa (se houver). Avisos indicam problemas com o trabalho que não afetou a conclusão geral do trabalho. Normalmente, esses avisos podem ser ignorados porque eles relatam sobre arquivos ocultos. Por exemplo, os arquivos `.DS_store` (Macintosh) e Thumbs.db (Windows®) contêm informações sobre como exibir arquivos de imagem para usuários. As entradas de aviso relacionadas a esses arquivos, no entanto, podem ser ignoradas porque não se referem à forma como esses arquivos são usados no Dynamic Media Classic. Você pode clicar duas vezes em um nome de trabalho para obter informações detalhadas sobre avisos.

**E (erros)** Lista o número de erros no trabalho (se houver). Você pode clicar duas vezes em um nome de trabalho para obter informações detalhadas sobre erros.

**** DuraçãoQuanto tempo levou para concluir o trabalho.

**** StatusMostra o status da tarefa.

**** Destino: para tarefas de upload, o nome da empresa e a pasta para a qual os arquivos foram carregados. Esta categoria não se aplica a trabalhos de publicação.

**Enviado** porListas que carregaram os ativos.

***Observação **: Você pode cancelar trabalhos de publicação e upload em andamento clicando no botão Cancelar ao lado da barra de progresso.*

## Alteração de exibições na página Trabalhos {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar tarefas ou alterar a visualização da guia Histórico da página Trabalhos :

**** ClassificaçãoSelecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar a opção ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

**** Intervalo de datasSelecione o menu Intervalo de datas e escolha uma opção para restringir a lista de tarefas à data atual, à semana anterior ou ao mês anterior. Escolha Intervalo de datas personalizado e insira um intervalo de datas específico.

**Tipo** de trabalhoSelecione o menu Tipo de trabalho e escolha Publicar ou Fazer upload para restringir a lista e publicar trabalhos ou fazer upload de trabalhos. Escolha Tudo para ver ambos os tipos de trabalhos.

**** MostrarEscolha Mostrar > Meus trabalhos ou Mostrar > Todos os trabalhos para restringir a lista a tarefas que você solicitou ou tarefas que as pessoas em sua empresa solicitaram.

## Exibição, cópia e impressão de um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique duas vezes no nome de um relatório na página Trabalhos para abrir a página Detalhes do trabalho . Esta página fornece um relatório de resumo sobre os arquivos na tarefa. Clique em Exibir detalhes para ver a Dynamic Media Classic ID de uma entrada, o caminho de destino e as informações de status. Se você tiver carregado um arquivo PDF ou PostScript que requer fontes que não estão disponíveis no Dynamic Media Classic, o relatório listará as fontes ausentes.

Você pode copiar essas informações para a Área de transferência.

1. Clique duas vezes no nome de um relatório na página Trabalhos para abrir a página Detalhes do trabalho .
1. Clique em Exibir detalhe para obter um relatório detalhado sobre uma entrada.
1. Clique em Copiar para a área de transferência.

## Lidar com trabalhos recorrentes de upload e publicação {#handling-recurring-upload-and-publish-jobs}

Os trabalhos recorrentes de upload e publicação criados nas páginas Upload e Publicação são listados na guia Scheduled da página Jobs . É possível editar e excluir tarefas recorrentes na guia Scheduled .

Selecione o botão Trabalhos na barra Navegação global e, na página Trabalhos, selecione a guia Agendado para editar e excluir trabalhos recorrentes.

>[!NOTE]
>
>Você pode filtrar a lista de tarefas na guia Scheduled com os menus Job Type e Show . Escolha um Tipo de Trabalho para restringir a lista e publicar trabalhos de um tipo específico. Escolha uma opção Mostrar para exibir tarefas criadas ou tarefas criadas por todos na empresa.

### Editar, excluir, pausar e retomar trabalhos recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione um trabalho recorrente na página Tarefas e siga estas instruções para editá-lo ou excluí-lo:

**Edição de um** trabalho recorrenteSelecione o botão Editar e insira informações de programação na caixa de diálogo Editar Trabalho Programado. Se desejar que o trabalho ocorra em um intervalo de sua escolha, escolha Repetir > Personalizado.

Consulte [Criação de um intervalo de tempo de trabalho personalizado de upload ou publicação](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Excluindo um** trabalho recorrenteSelecione o botão Excluir.

**Pausando (e retomando) um** trabalho recorrente Na coluna Ativo , desmarque uma caixa de seleção para pausar um trabalho; marque uma caixa de seleção para retomar um trabalho pausado.

### Criação de um intervalo de tempo de trabalho personalizado de upload ou publicação {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo de tempo personalizado para um upload (via FTP) ou um trabalho de publicação, escolha Repetir > Personalizado na página Fazer upload ou Publicar . Em seguida, insira números e curingas na caixa Regra para descrever um intervalo de tempo para que os trabalhos de upload ou publicação sejam repetidos.

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

* 0 0 12 * * ?: Nove todos os dias
* 0 15 10 ? * *: 10:15 todos os dias
* 0 0/5 14 * * ?: A cada 5 minutos entre 2:00 e 2:55 PM todos os dias
* 0 0/5 14,18 * * * ?: A cada 5 minutos entre 2:00 e 2:55 PM todos os dias e a cada 5 minutos entre 6:00 e 6:55 pm todos os dias
* 10,44 14 ? 3: Queijo às 14h10 e 14h44 toda quarta-feira em março
* 0 15 10 ? *: Seg-Sex às 10h15 todos os dias da semana
* 15 10 20 * ?: Às 10h15 do dia 20 de cada mês
* 15 10 L * ?: Às 10h15 do último dia de cada mês
* 0 15 10 ? * 6L: Às 10h15 da última sexta-feira de cada mês
* 0 15 10 * * 6#3: Às 10h15 da terceira sexta-feira de cada mês

## Usar um trabalho de upload ou publicação como acionador {#using-an-upload-or-publish-job-as-a-trigger}

Ao fazer upload de ativos via FTP ou executar um trabalho de publicação, você pode agendar um trabalho subsequente para começar quando o upload for concluído. (Se outras tarefas estiverem programadas para começar então, a tarefa agendada aqui estará na fila atrás delas.) A nova tarefa envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse trabalho de upload de seguimento recebe o mesmo nome do trabalho de upload atual, mas com o prefixo _Pub.

Para fazer com que um trabalho de upload ou publicação acione outro trabalho, selecione Avançado na página Upload ou Publish . Em seguida, insira o URL no campo de texto Notificação HTTP .
