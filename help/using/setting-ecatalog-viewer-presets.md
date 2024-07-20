---
title: Configurar Predefinições do Visualizador de eCatalog
description: Saiba como configurar Predefinições do visualizador do eCatalog no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Configurar Predefinições do Visualizador de eCatalog{#setting-up-ecatalog-viewer-presets}

As predefinições do visualizador do eCatalog determinam o estilo, o comportamento e a aparência dos visualizadores do eCatalog. O Adobe Dynamic Media Classic fornece Predefinições do Visualizador de eCatalog e você pode criar suas próprias Predefinições do Visualizador de eCatalog, caso seja um administrador.

Para criar uma predefinição, você pode começar do zero ou começar com uma Predefinição do visualizador do eCatalog fornecida pela Adobe Dynamic Media Classic e salvá-la com um novo nome. Você pode criar suas próprias Predefinições do visualizador de eCatalog para apresentar o material impresso nas cores da empresa e definir o tom.

As predefinições do visualizador do eCatalog oferecem muitas configurações para ir de página a página, aplicar zoom, pesquisar e escolher &quot;capas&quot;. A aparência desses controles e a forma como o Visualizador é exibido dependem da sua escolha de Predefinições do visualizador do eCatalog.

Siga estas etapas para criar uma Predefinição do visualizador do eCatalog (você deve ser um administrador):

1. Na barra de Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na tela Predefinições do visualizador, crie uma Predefinição do visualizador do eCatalog iniciando de novo ou a partir de uma Predefinição do visualizador do eCatalog existente:

   * **Criar uma Predefinição do Visualizador de eCatalog**: selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha Visualizador de eCatalog e selecione **[!UICONTROL Add]**.

   * **Editar uma Predefinição do Visualizador de eCatalog**: selecione uma Predefinição do Visualizador de eCatalog e, em seguida, selecione **[!UICONTROL Edit]**. Selecione **[!UICONTROL Save As]** depois de concluir a criação da predefinição.

1. Na página `Configure Viewer`, digite um nome para a Predefinição do Visualizador de eCatalog.
1. Na página `Configure Viewer`, defina as opções desejadas.

   selecione o ícone **[!UICONTROL Info Tip]** ao lado da opção se desejar ler sua descrição.

   A página Visualizar exibe o visualizador à medida que você atualiza e altera as configurações.

1. (Opcional) Em **[!UICONTROL Info Panel Settings]**, a opção **[!UICONTROL Information Server URL]** pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   | --- | --- | --- |
   | `$1$` | valor rollover_key | O identificador de item do elemento `<area>` do mapa. |
   | `$2$` | quadro | O número sequencial do quadro mostrado no momento no conjunto de imagens. |
   | `$3$` | raiz da imagem | O primeiro elemento de caminho do primeiro item especificado no comando image (normalmente a ID do catálogo de imagens da entrada do catálogo especificando o conjunto de imagens). |

1. (Opcional) No **[!UICONTROL Info Panel Settings]**, na caixa **[!UICONTROL Response Template]**, digite o texto que você deseja exibir se o Adobe Dynamic Media Classic encontrar um erro ao recuperar informações para um Mapa de Imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de eCatalog, mas nenhum identificador de rollover, essa mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar esse Modelo de Resposta em vez do modelo definido no próprio eCatalog, adicione `fmt=1` ao final da URL do Servidor de Informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Selecione **[!UICONTROL Save]**.
1. Selecione **[!UICONTROL Default]** para que a Predefinição do visualizador de eCatalog criada seja a usada para exibir eCatalogs na sua página da Web.

Para excluir uma Predefinição do visualizador de eCatalog, selecione-a na tela Predefinições do visualizador e selecione **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Predefinições do Visualizador](application-setup.md#viewer_presets)
