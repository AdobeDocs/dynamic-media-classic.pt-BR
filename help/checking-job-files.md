---
title: Verificando arquivos de trabalho
seo-title: Verificando arquivos de trabalho
description: nulo
seo-description: Saiba como verificar arquivos de trabalho.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---


# Verificando arquivos de trabalho{#checking-job-files}

Para monitorar os uploads de arquivos para o Dynamic Media Classic e os arquivos que você publica nos servidores do Dynamic Media Classic, o Dynamic Media Classic oferta a página Tarefas. Você pode revisar os trabalhos de upload e publicação na página Tarefas, verificar o status dos trabalhos e cancelar os trabalhos de publicação nesta página. Você também pode agendar trabalhos de upload e publicação.

Quando você carrega ativos, um ícone de rotação é exibido ao lado do menu Tarefas, indicando que uma tarefa está em andamento e o número de arquivos em andamento. Você pode clicar no ícone para ver mais informações sobre o trabalho ativo.

>[!NOTE]
>
>Uma lista dos trabalhos publicados recentemente também está disponível na página Atividade recente. Clique em Recente na barra Navegação global para abrir esta página.

## Sobre a página Tarefas {#about-the-jobs-page}

Selecione o botão Tarefas na barra Navegação global para abrir a página Tarefas. Por padrão, os trabalhos são listados começando com os mais recentes.

As tarefas são listadas nessas categorias na guia Histórico da página Tarefas:

**Tipo** de trabalho Um ícone indica o tipo de trabalho: Carregar e publicar são os tipos de trabalho mais comuns.

**Nome** da tarefaO nome da tarefa. O nome inclui a parte digitada pelo usuário do nome e o carimbo de data e hora.

**Iniciado** quando o trabalho começou.

**Total** O número de arquivos transferidos.

**W (avisos)** O número de avisos na tarefa (se houver). Os avisos indicam problemas com o trabalho que não afetaram a conclusão geral do trabalho. Normalmente, esses avisos podem ser ignorados porque relatam sobre arquivos ocultos. Por exemplo, arquivos .DS_store (Macintosh) e arquivos Thumbs.db (Windows) contêm informações sobre como exibir arquivos de imagem para usuários. No entanto, as entradas de aviso referentes a esses arquivos podem ser ignoradas, pois não dizem respeito à forma como esses arquivos são usados no Dynamic Media Classic. Você pode clicar com o duplo em um nome de tarefa para obter informações detalhadas sobre avisos.

**E (erros)** Lista o número de erros no trabalho (se houver). Você pode clicar com o duplo no nome de uma tarefa para obter informações detalhadas sobre erros.

**Duração** Quanto tempo levou para concluir o trabalho.

**Status** Mostra o status da tarefa.

**Destino** Para trabalhos de upload, o nome da empresa e a pasta na qual os arquivos foram carregados. Essa categoria não se aplica a trabalhos de publicação.

**Enviado pelas** Listas que carregaram os ativos.

***Observação **: Você pode cancelar trabalhos de publicação e upload em andamento clicando no botão Cancelar ao lado da barra de progresso.*

## Alterar visualizações na página Tarefas {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar trabalhos ou alterar sua visualização da guia Histórico da página Tarefas:

**Classificação** Selecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar o switch ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

**Intervalo** de datas Selecione o menu Intervalo de datas e escolha uma opção para restringir a lista de trabalhos à data atual, à semana anterior ou ao mês anterior. Escolha Intervalo de datas personalizado para inserir um intervalo de datas específico.

**Tipo** de trabalho Selecione o menu Tipo de trabalho e escolha Publicar ou Fazer upload para restringir a lista de publicar trabalhos ou fazer upload de trabalhos. Escolha Todos para ver os dois tipos de trabalhos.

**Mostrar** Escolha Mostrar > Meus trabalhos ou Mostrar > Todos os trabalhos para restringir a lista aos trabalhos que você solicitou ou aos trabalhos que as pessoas em sua empresa solicitaram.

## Exibição, cópia e impressão de um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique com o Duplo no nome de um relatório na página Tarefas para abrir a página Detalhes da Ordem de Produção. Esta página fornece um relatório de resumo sobre os arquivos no trabalho. Clique em Detalhes da Visualização para ver a Dynamic Media Classic ID de uma entrada, o caminho de destino e as informações de status. Se você carregou um arquivo PDF ou PostScript que requer fontes que não estão disponíveis no Dynamic Media Classic, o relatório lista as fontes ausentes.

É possível copiar essas informações para a Área de transferência.

1. Clique com o Duplo no nome de um relatório na página Tarefas para abrir a página Detalhes da Ordem de Produção.
1. Clique em Detalhes da Visualização para obter um relatório detalhado sobre uma entrada.
1. Clique em Copiar para a área de transferência.

## Manuseando trabalhos recorrentes de upload e publicação {#handling-recurring-upload-and-publish-jobs}

Os trabalhos recorrentes de upload e publicação criados nas páginas de upload e publicação são listados na guia Agendado da página de Tarefas. É possível editar e excluir trabalhos recorrentes na guia Agendado.

Selecione o botão Tarefas na barra Navegação global e, na página Tarefas, selecione a guia Agendado para editar e excluir trabalhos recorrentes.

>[!NOTE]
>
>Você pode filtrar a lista de trabalho na guia Agendado com os menus Tipo de trabalho e Mostrar. Escolha um Tipo de Trabalho para restringir a lista para publicar trabalhos de um tipo específico. Escolha uma opção Mostrar para exibir trabalhos criados ou criados por todos na sua empresa.

### Editar, excluir, pausar e retomar trabalhos recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione uma tarefa recorrente na página Tarefas e siga estas instruções para editá-la ou excluí-la:

**Edição de um trabalho** recorrente Selecione o botão Editar e insira as informações do agendamento na caixa de diálogo Editar trabalho programado. Se desejar que a tarefa ocorra novamente em um intervalo de sua escolha, escolha Repetir > Personalizado.

Consulte [Criação de um intervalo](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)de tempo de trabalho de upload ou publicação personalizado.

**Excluindo um trabalho** recorrente Selecione o botão Excluir.

**Pausando (e retomando) um trabalho** recorrente Na coluna Ativo, desmarque uma caixa de seleção para pausar um trabalho; marque uma caixa de seleção para retomar um trabalho que foi pausado.

### Criação de um intervalo de tempo de trabalho de upload ou publicação personalizado {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo de tempo personalizado para um upload (via FTP) ou um trabalho de publicação, escolha Repetir > Personalizado na página Carregar ou Publicar. Em seguida, insira números e curingas na caixa Regra para descrever um intervalo de tempo para que os trabalhos de upload ou publicação sejam repetidos.

A sintaxe para descrever intervalos de tempo de upload e publicação personalizados na caixa Regra é:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por exemplo, `0 15 10 * * ?` agenda uma tarefa às 10:15.00 todos os dias.

As tabelas a seguir e a lista explicam como descrever um intervalo de tempo na caixa Regra.

Esta tabela mostra os incrementos de tempo, seus valores permitidos e os curingas suportados por eles:

| Incrementos de tempo | Valores permitidos | Comentários | Caracteres curinga suportados |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | , - * / |
| Minutos | 0-59 |  | , - * / |
| Horas | 0-23 | Observe o uso de um relógio de 24 horas. | , - * / |
| Dia do mês | 1-31 | Não é possível especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um ? caractere curinga. | , - * / ? L C |
| Mês | 1-12 ou Jan, Fev, Mar, Abr, Maio, Jun, Jul, Ago, Set, Set, Out, Nov, Dez | Os valores distinguem maiúsculas de minúsculas. | , - * / |
| Dia da semana | Seg, Ter, Qua, Qui, Sex, Sáb, Dom | Os valores distinguem maiúsculas de minúsculas. Não é possível especificar um valor numérico para &quot;dia do mês&quot; e &quot;dia da semana&quot;. Um desses campos deve usar um ? caractere curinga. | , - * / ? L C # |
| Ano (opcional) | Vazio ou 1970-2099 |  | , - * / |


Esta tabela descreve os caracteres curingas permitidos na caixa Regra e como usá-los:

| Caractere curinga | Nome | O que ela descreve |
|--- |--- |--- |
| * | Asterisco | Todos os valores (por exemplo, &quot;a cada minuto&quot;). |
| ? | Ponto de interrogação | Nenhum valor específico (por exemplo, &quot;qualquer minuto dentro da hora especificada&quot;). |
| , | Vírgula | Valores adicionais (por exemplo, &quot;segunda e quarta-feira&quot;). |
| - | Hífen | Intervalo de valores (por exemplo, &quot;de segunda a sexta-feira&quot;). |
| / | Barra para frente | Incrementos (por exemplo, &quot;a cada 15 minutos&quot;). |
| L | Capital L | Último &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível apenas para esses campos). Por exemplo, se o mês for janeiro, um valor L para o campo &quot;dia do mês&quot; programará a ordem de produção para 31 de janeiro.Para o campo &quot;dia da semana&quot;, você pode informar esse caractere sozinho para agendar a ordem de produção no sábado. Você pode usá-lo com um número (por exemplo, 6L) para especificar a última sexta-feira do mês.Não especifique L com os curingas de vírgula ou hífen. |
| # | Sinal de número | &quot;Nth&quot; dia da semana do mês (disponível apenas para o campo &quot;dia da semana&quot;).Por exemplo, 6#3 no campo &quot;dia da semana&quot; especifica a terceira sexta-feira do mês. O 6 denota &quot;Sexta-feira&quot; (o sexto dia da semana) e o 3 denota a terceira ocorrência do mês. |
| C | # Capital C | Primeiro calendário &quot;dia do mês&quot; ou &quot;dia da semana&quot; (disponível apenas para estes campos). Por exemplo, especificar um valor de 1C para &quot;dia do mês&quot; agendará o primeiro dia do calendário que ocorre no quinto dia ou depois dele.Para o campo &quot;dia da semana&quot;, a especificação de 1C agendará o primeiro dia do calendário que ocorre no domingo ou depois dele |

Esta lista fornece exemplos de descrição de intervalos de tempo na caixa Regra:

* 0 0 12 * * ?: Nove todos os dias
* 0 15 10 ? * *: 22:15 todo dia
* 0 0/5 14 * * ?: A cada 5 minutos entre as 14:00 e 14:55 da tarde todos os dias
* 0 0/5 14,18 * * * ?: A cada 5 minutos, entre 14:00 e 14:55, todos os dias, e a cada 5 minutos, entre 18:00 e 18:55, todos os dias
* 0 10,44 14 ? 3: Que às 14:10 e 14:44 toda quarta-feira em março
* 0 15 10 ? *: Seg-Sex às 10h15 todos os dias da semana
* 0 15 10 20 * ?: Às 10h15 do dia 20 de cada mês
* 0 15 10 L * ?: Às 10h15 do último dia de cada mês
* 0 15 10 ? * 6L: Às 10h15 da última sexta-feira de cada mês
* 0 15 10 * * 6#3: Às 10h15 da terceira sexta-feira de cada mês

## Usar um trabalho de upload ou publicação como disparador {#using-an-upload-or-publish-job-as-a-trigger}

Ao fazer upload de ativos via FTP ou executar um trabalho de publicação, você pode agendar um trabalho subsequente para começar assim que o upload for concluído. (Se outras tarefas estiverem programadas para começar nesse momento, a tarefa agendada aqui será colocada em fila atrás delas.) A nova ordem de produção envia uma notificação para o endereço especificado, para que o código nesse local possa ser acionado. Esse trabalho de upload de continuação recebe o mesmo nome do trabalho de upload atual, mas com o prefixo _Pub.

Para fazer um trabalho de upload ou publicação disparar outro trabalho, selecione Avançado na página Carregar ou Publicar. Em seguida, insira o URL no campo de texto Notificação HTTP.
