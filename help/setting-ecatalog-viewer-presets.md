---
title: Configuração das predefinições do visualizador de catálogo eletrônico
description: Saiba como configurar as Predefinições do visualizador de catálogo eletrônico.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Visualizadores,Predefinições do visualizador,Catálogo eletrônico
role: Profissional
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Configuração das predefinições do visualizador de catálogo eletrônico{#setting-up-ecatalog-viewer-presets}

As Predefinições do visualizador de catálogo eletrônico determinam o estilo, o comportamento e a aparência dos visualizadores de catálogo eletrônico. O Dynamic Media Classic fornece predefinições do visualizador de catálogo eletrônico e você também pode criar suas próprias predefinições do visualizador de catálogo eletrônico, se você for um administrador.

Para criar uma nova predefinição, você pode começar do zero ou começar com uma predefinição do visualizador de catálogo eletrônico fornecida pelo Dynamic Media Classic e salvá-la com um novo nome. Você pode criar suas próprias Predefinições do visualizador de eCatalog para apresentar o material impresso nas cores de sua empresa e definir o tom.

As Predefinições do visualizador de catálogo eletrônico oferecem muitas configurações para ir de página em página, ampliação, pesquisa e escolher &quot;capas&quot;. A aparência desses controles e a aparência do próprio Visualizador dependem da escolha das Predefinições do visualizador de catálogo eletrônico.

Siga estas etapas para criar uma predefinição do visualizador do catálogo eletrônico (você deve ser um administrador):

1. Clique em **Configurar** > **Predefinições do visualizador**.
1. Na tela Predefinições do visualizador, crie uma Predefinição do visualizador de catálogo eletrônico iniciando de novo ou iniciando em uma Predefinição do visualizador de catálogo eletrônico existente:

   * **Criando um Visualizador de Catálogo Eletrônico**
Predefinido Clique em Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha Visualizador do catálogo eletrônico e clique em 
**Adicionar**.

   * **Editando uma**
predefinição do visualizador de catálogo eletrônicoSelecione uma predefinição do visualizador de catálogo eletrônico e clique em Editar. Clique em 
**Salve** assim que terminar de criar a predefinição.

1. Na tela Configurar visualizador , digite um nome para sua predefinição do visualizador do catálogo eletrônico.
1. Na tela Configurar visualizador, defina as opções desejadas.

   Clique no ícone Dica de informações , adjacente à opção para ver sua descrição.

   A tela de visualização exibe o visualizador conforme você atualiza e altera as configurações.

1. (Opcional) Nas Configurações do painel Informações, a opção URL do servidor de informações pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   |--- |--- |--- |
   | `$1$` | valor de rolover_key | O identificador de item do elemento `<area>` do mapa. |
   | `$2$` | quadro | O número de sequência do quadro exibido no momento no conjunto de imagens. |
   | `$3$` | imageroot | O primeiro elemento de caminho do primeiro item especificado no comando image (normalmente a ID do catálogo de imagens da entrada do catálogo especificando o conjunto de imagens). |

1. (Opcional) Nas Configurações do painel Informações, na caixa Modelo de resposta, digite o texto que deseja que apareça se o Dynamic Media Classic encontrar um erro na recuperação de informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de catálogo eletrônico, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar esse Modelo de resposta em vez do modelo definido no próprio eCatalog, adicione &quot;fmt=1&quot; ao final do URL do Servidor de informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Clique em **Salvar**.
1. Clique em Padrão se desejar que a predefinição do visualizador do eCatalog que você criou seja aquela usada para exibir eCatalogs em sua página da Web.

Para excluir uma predefinição do visualizador do catálogo eletrônico, selecione-a na tela Predefinições do visualizador e clique em **Excluir**.

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)

