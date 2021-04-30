---
title: Configuração das predefinições do visualizador de catálogo eletrônico
description: Saiba como configurar as Predefinições do visualizador de catálogo eletrônico.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Visualizadores,Predefinições do visualizador,Catálogo eletrônico
role: Business Practitioner
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
translation-type: tm+mt
source-git-commit: 6f3801a71dd2a5f162acacf7d8199dbf8c3520f7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Configuração das predefinições do visualizador de catálogo eletrônico{#setting-up-ecatalog-viewer-presets}

As Predefinições do visualizador de catálogo eletrônico determinam o estilo, o comportamento e a aparência dos visualizadores de catálogo eletrônico. O Dynamic Media Classic fornece predefinições do visualizador de catálogo eletrônico e você também pode criar suas próprias predefinições do visualizador de catálogo eletrônico, se você for um administrador.

Para criar uma predefinição, você pode começar do zero ou começar com uma predefinição do visualizador de catálogo eletrônico fornecida pelo Dynamic Media Classic e salvá-la com um novo nome. Você pode criar suas próprias Predefinições do visualizador de eCatalog para apresentar o material impresso nas cores de sua empresa e definir o tom.

As Predefinições do visualizador de catálogo eletrônico oferecem muitas configurações para ir de página em página, ampliação, pesquisa e escolher &quot;capas&quot;. O aspecto desses controles e a forma como o Visualizador aparece dependem da sua escolha de Predefinições do visualizador de catálogo eletrônico.

Siga estas etapas para criar uma predefinição do visualizador do catálogo eletrônico (você deve ser um administrador):

1. Na barra Navegação global, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na tela Predefinições do visualizador, crie uma Predefinição do visualizador de catálogo eletrônico iniciando de novo ou iniciando em uma Predefinição do visualizador de catálogo eletrônico existente:

   * **Criação de uma predefinição do visualizador de catálogo eletrônico**  - Clique em  **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha Visualizador do catálogo eletrônico e clique em **[!UICONTROL Add]**.

   * **Editar uma predefinição do visualizador de eCatalog**  - Selecione uma predefinição do visualizador do eCatalog e clique em Editar. Clique em **[!UICONTROL Save As]** depois de concluir a criação da predefinição.

1. Na tela Configurar visualizador , digite um nome para sua predefinição do visualizador do catálogo eletrônico.
1. Na tela Configurar visualizador, defina as opções desejadas.

   Clique no ícone **[!UICONTROL Info Tip]** ao lado da opção se quiser ler a descrição.

   A página Visualização exibe o visualizador conforme você atualiza e altera as configurações.

1. (Opcional) Em **[!UICONTROL Info Panel Settings]**, a opção **[!UICONTROL Information Server URL]** pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   |--- |--- |--- |
   | `$1$` | valor de rolover_key | O identificador de item do elemento `<area>` do mapa. |
   | `$2$` | quadro | O número de sequência do quadro exibido no momento no conjunto de imagens. |
   | `$3$` | imageroot | O primeiro elemento de caminho do primeiro item especificado no comando image (normalmente a ID do catálogo de imagens da entrada do catálogo especificando o conjunto de imagens). |

1. (Opcional) Na caixa **[!UICONTROL Info Panel Settings]**, digite o texto que deseja que apareça na caixa **[!UICONTROL Response Template]** se o Dynamic Media Classic encontrar um erro na recuperação de informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de catálogo eletrônico, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar esse Modelo de resposta em vez do modelo definido no próprio Catálogo eletrônico, adicione `fmt=1` ao final do URL do Servidor de informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Clique em **Salvar**.
1. Clique em Padrão se desejar que a predefinição do visualizador do eCatalog que você criou seja aquela usada para exibir eCatalogs em sua página da Web.

Para excluir uma predefinição do visualizador do catálogo eletrônico, selecione-a na tela Predefinições do visualizador e clique em **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)

