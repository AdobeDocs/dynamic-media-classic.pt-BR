---
title: Verificação de arquivos de trabalho
seo-title: Verificação de arquivos de trabalho
description: 'null'
seo-description: Saiba como verificar os arquivos de trabalho.
uuid: 8241 a 894-3014-4 a 5 c -96 ef -71 f 3 aaa 3716 a
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/upload_ and_ publish_ assets
discoiquuid: d 53 ae 5 dd -8 daf -4 d 87-b 9 a 6-3039 ruim 30538
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Verificação de arquivos de trabalho{#checking-job-files}

Para monitorar carregamentos de arquivos no Sistema de publicação do Scene 7 e arquivos que você publica nos servidores do Dynamic Media Classic, o SPS oferece a página Tarefas. Você pode revisar o upload e publicar trabalhos na página Tarefas, verificar o status das tarefas e cancelar trabalhos de publicação nesta página. Você também pode programar o upload e a publicação de tarefas.

Quando você carrega ativos, um ícone de rotação aparece ao lado do menu Tarefas, indicando que um trabalho está em andamento e o número de arquivos em andamento. Você pode clicar no ícone para ver mais informações sobre o trabalho ativo.

>[!NOTE]
>
>Uma lista de trabalhos publicados recentemente também está disponível na página Atividade recente. Clique em Recente na barra Navegação global para abrir esta página.

## Sobre a página de Tarefas {#about-the-jobs-page}

Selecione o botão Tarefas na barra Navegação global para abrir a página Tarefas. Por padrão, as tarefas são listadas começando com o mais recente.

As tarefas são listadas nessas categorias na guia Histórico da página Tarefas:

**Tipo de trabalho** Um ícone indica o tipo de trabalho: O upload e a publicação são os tipos de trabalho mais comuns.

**Nome** do trabalho O nome da tarefa. O nome inclui a parte inserida pelo usuário do nome e o carimbo de data e hora.

**Iniciada** quando a tarefa começou.

**Total** O número de arquivos transferidos.

**W (avisos)** O número de avisos no trabalho (se houver). Os avisos indicam problemas com a tarefa que não afetava a conclusão geral do trabalho. Normalmente, esses avisos podem ser ignorados porque eles relatam arquivos ocultos. Por exemplo, arquivos. DS_ store (Macintosh) e Thumbs. db (Windows) contêm informações sobre como exibir arquivos de imagem para usuários. No entanto, as entradas de aviso referentes a esses arquivos podem ser ignoradas porque elas não pertencem à forma como esses arquivos são usados no Dynamic Media Classic. Você pode clicar duas vezes em um nome de serviço para obter informações detalhadas sobre avisos.

**E (Erros)** Lista o número de erros no trabalho (se houver). Você pode clicar duas vezes em um nome de serviço para obter informações detalhadas sobre erros.

**Duração Por** quanto tempo levou para concluir o trabalho.

**Status** Mostra o status da tarefa.

**Destino** para fazer upload de trabalhos, o nome e a pasta da empresa aos quais os arquivos foram carregados. Esta categoria não se aplica a publicar trabalhos.

**Enviado por** lista que carregou os ativos.

***Observação**: Você pode cancelar a publicação em andamento e fazer upload de tarefas clicando no botão Cancelar próximo à barra de progresso.*

## Alteração de exibições na página de Tarefas {#changing-views-on-the-jobs-page}

Use essas técnicas para classificar tarefas ou alterar a exibição da guia Histórico da página Tarefas:

**Classificação** Selecione um nome de coluna para classificar a lista por uma coluna específica. Você pode selecionar a alternância ao lado do nome da coluna para classificar em ordem decrescente ou crescente.

**Intervalo** de datas Selecione o menu Intervalo de datas e escolha uma opção para restringir a lista de tarefas à data atual, à semana anterior ou ao mês anterior. Escolha o Intervalo de datas personalizado para inserir um intervalo de datas específico.

**Tipo de trabalho** Selecione o menu Tipo de trabalho e escolha Publicar ou Fazer upload para restringir a lista para publicar trabalhos ou fazer upload de tarefas. Escolha Todos para ver ambos os tipos de tarefas.

**Mostrar** escolha Mostrar &gt; Meus trabalhos ou Mostrar &gt; Todos os trabalhos para restringir a lista a trabalhos ordenados ou trabalhos que as pessoas na sua empresa ordenaram.

## Exibir, copiar ou imprimir um relatório de Detalhes do trabalho {#viewing-copying-or-printing-a-job-details-report}

Clique duas vezes no nome de um relatório na página Tarefas para abrir a página Detalhes do trabalho. Esta página fornece um relatório resumido sobre os arquivos na tarefa. Clique em Exibir detalhe para ver a ID de SPS de uma entrada, o caminho de destino e as informações de status. Se você carregou um arquivo PDF ou postscript que requer fontes que não estão disponíveis no SPS, o relatório lista as fontes ausentes.

Você pode copiar essas informações para a Área de transferência.

1. Clique duas vezes no nome de um relatório na página Tarefas para abrir a página Detalhes do trabalho.
1. Clique em Exibir detalhe para obter um relatório detalhado sobre uma entrada.
1. Clique em Copiar para a área de transferência.

## Manipulação de trabalhos de upload e publicação recorrentes {#handling-recurring-upload-and-publish-jobs}

Os trabalhos de upload e publicação recorrentes criados nas páginas Carregar e Publicar são listados na guia Programada da página Tarefas. Você pode editar e excluir trabalhos recorrentes na guia Programada.

Selecione o botão Tarefas na barra Navegação global e, na página Tarefas, selecione a guia Programada para editar e excluir trabalhos recorrentes.

>[!NOTE]
>
>Você pode filtrar a lista de tarefas na guia Programado com os menus Tipo de trabalho e Mostrar. Escolha um Tipo de trabalho para restringir a lista para publicar trabalhos de um tipo específico. Escolha uma opção Mostrar para exibir trabalhos criados por todos na empresa.

### Editar, excluir, pausar e retomar trabalhos recorrentes {#editing-deleting-pausing-and-resuming-recurring-jobs}

Selecione uma tarefa recorrente na página Tarefas e siga estas instruções para editar ou excluí-la:

**Edição de um trabalho recorrente** Selecione o botão Editar e insira informações de programação na caixa de diálogo Editar trabalho programado. Se você quiser que a tarefa ocorra novamente em um intervalo de sua escolha, escolha Repetir &gt; Personalizado.

Consulte [Criar um intervalo de tempo de trabalho ou um intervalo de tempo de trabalho personalizado](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Excluir um trabalho recorrente** Selecione o botão Excluir.

**Pausar (e retomar) um trabalho recorrente** na coluna Ativa, desmarcar uma caixa de seleção para pausar um trabalho; selecione uma caixa de seleção para retomar uma tarefa pausada.

### Criação de um intervalo de tempo de trabalho de upload ou publicação personalizado {#creating-a-custom-upload-or-publish-job-time-interval}

Para criar um intervalo de tempo personalizado para um upload (via FTP) ou um trabalho de publicação, escolha Repetir &gt; Personalizado na página Carregar ou Publicar. Em seguida, insira números e curingas na caixa Regra para descrever um intervalo de tempo para o upload ou publicação de trabalhos para recorrerem novamente.

A sintaxe para descrever intervalos de tempo de upload personalizado e de publicação na caixa Regra é:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Por exemplo, `0 15 10 * * ?` programe um trabalho a 10:15.00 todos os dias.

As tabelas a seguir explicam como descrever um intervalo de tempo na caixa Regra.

Esta tabela mostra os incrementos de tempo, os valores permitidos e os curingas que eles suportam:

| Incrementos de tempo | Valores permitidos | Comentários | Curingas suportadas |
|--- |--- |--- |--- |
| Segundos | 0-59 |  | , - * / |
| Minutos | 0-59 |  | , - * / |
| Horas | 0-23 | Observe o uso de um relógio de 24 horas. | , - * / |
| Dia do mês | 1-31 | Não é possível especificar um valor numérico para o «dia do mês» e o «dia da semana. » Um desses campos deve usar a? caractere curinga. | , - * / ? L C |
| Mês | 1-12 ou Jan, Feb, Mar, Apr, maio, Jun, Jul, Aug, Sep, Sep, Out, Nov, Dez | Os valores distinguem maiúsculas de minúsculas. | , - * / |
| Dia da semana | Maria, Terça, Entregue, Thu, Sex, Sat, Sun | Os valores distinguem maiúsculas de minúsculas. Não é possível especificar um valor numérico para o «dia do mês» e o «dia da semana. » Um desses campos deve usar a? caractere curinga. | , - * / ? L C # |
| Ano (opcional) | Vazio ou 1970-2099 |  | , - * / |


Esta tabela descreve os caracteres curinga permitidos na caixa Regra e como usá-los:

| Caractere curinga | Nome | O que ele descreve |
|--- |--- |--- |
| * | Asterisco | Todos os valores (por exemplo, «cada minuto»). |
| ? | Ponto de interrogação | Nenhum valor específico (por exemplo, «qualquer minuto dentro da hora especificada»). |
| , | Vírgula | Valores adicionais (por exemplo, «segunda-feira e quarta-feira»). |
| - | Hífen | Intervalo de valores (por exemplo, «segunda-feira a sexta-feira»). |
| / | Barra posterior | Incrementos (por exemplo, «a cada 15 minutos»). |
| L | Capital L | Último «dia do mês» ou «dia da semana» (disponível apenas para esses campos). Por exemplo, se o mês for janeiro, um valor L para o campo "dia do mês" programará o trabalho para January 1 de janeiro. No campo "dia do semana", você pode inserir este caractere sozinho para agendar o trabalho no sábado. Você pode usá-lo com um número (por exemplo, 6 L) para especificar a última sexta-feira do mês. Não especifique L com as curingas ou hífen. |
| # | Sinal de número | Dia da semana «Enth» do mês (disponível apenas para o campo «dia do semana»). Por exemplo, 6 # 3 no campo «dia do semana» especifica o terceiro sexta-feira do mês. O 6 denota «Sexta-feira» (o sexto dia da semana) e o 3 indica a terceira ocorrência no mês. |
| C | # Capital C | Primeiro calendário «dia do mês» ou «dia da semana» (disponível apenas para esses campos). Por exemplo, especificar um valor de 1 C para "dia do mês" agendará o primeiro dia do calendário em ou depois do quinto. Para o campo "dia do semana", especificar 1 C agendará o primeiro dia no calendário que ocorre em ou depois do domingo |

Esta lista fornece exemplos de descrição de intervalos de tempo na caixa Regra:

* 0 0 12 * *?: Dia todo dia
* 0 15 10 ? * *: 1h:1am am todos os dias
* 0 0/5 14 * *?: A cada 5 minutos entre 2:00 e 2:55 pm todos os dias
* 0 0/5 14,18 * *?: A cada 5 minutos entre 2:00 e 2:55 pm todos os dias e a cada 5 minutos entre 6:00 e 6:55 pm todos os dias
* 0 10,44 14 ? 3: Entregue às 2:10 pm e 2:44 pm a cada quarta-feira em março
* 0 15 10 ? *: J-Sex às 10h every 5 am todos os dias úteis
* 0 15 10 20 *?: Às 1am h on am am no 20 º dia de cada mês
* 0 15 10 L *?: Às 1h on 5 am no último dia de cada mês
* 0 15 10 ? * 6 L: Às 1am h Friday 5 am na última sexta-feira de cada mês
* 0 15 10 * * 6 # 3: Às 10h Friday 5 am no terceiro sexta-feira de cada mês

## Uso de um serviço de upload ou publicação como disparador {#using-an-upload-or-publish-job-as-a-trigger}

Quando você carrega ativos via FTP ou executa um trabalho de publicação, é possível agendar uma tarefa subsequente para iniciar assim que o carregamento for concluído. (Se outras tarefas estiverem programadas para começar nesse momento, o trabalho agendado aqui é colocado em fila por trás delas.) O novo serviço envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse serviço de carregamento de seguidores recebe o mesmo nome do trabalho de upload atual, mas com o prefixo_ Pub.

Para fazer com que um upload ou publicação de um trabalho seja acionado, selecione Avançado na página Carregar ou Publicar. Em seguida, insira o URL no campo de texto Notificação HTTP.
