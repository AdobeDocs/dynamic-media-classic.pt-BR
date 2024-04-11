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
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Configurar Predefinições do Visualizador de eCatalog{#setting-up-ecatalog-viewer-presets}

As predefinições do visualizador do eCatalog determinam o estilo, o comportamento e a aparência dos visualizadores do eCatalog. O Adobe Dynamic Media Classic fornece Predefinições do Visualizador de eCatalog e você pode criar suas próprias Predefinições do Visualizador de eCatalog, caso seja um administrador.

Para criar uma predefinição, você pode começar do zero ou começar com uma Predefinição do visualizador do eCatalog fornecida pela Adobe Dynamic Media Classic e salvá-la com um novo nome. Você pode criar suas próprias Predefinições do visualizador de eCatalog para apresentar o material impresso nas cores da empresa e definir o tom.

As predefinições do visualizador do eCatalog oferecem muitas configurações para ir de página a página, aplicar zoom, pesquisar e escolher &quot;capas&quot;. A aparência desses controles e a forma como o Visualizador é exibido dependem da sua escolha de Predefinições do visualizador do eCatalog.

Siga estas etapas para criar uma Predefinição do visualizador do eCatalog (você deve ser um administrador):

1. Na barra de Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na tela Predefinições do visualizador, crie uma Predefinição do visualizador do eCatalog iniciando de novo ou a partir de uma Predefinição do visualizador do eCatalog existente:

   * **Criar uma predefinição do visualizador de eCatalog** - Selecionar **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha eCatalog Viewer e, em seguida, selecione **[!UICONTROL Add]**.

   * **Editar uma predefinição do visualizador de eCatalog** - Selecione uma Predefinição do visualizador de eCatalog e, em seguida, **[!UICONTROL Edit]**. Selecionar **[!UICONTROL Save As]** após concluir a criação da predefinição.

1. No `Configure Viewer` digite um nome para a Predefinição do visualizador do eCatalog.
1. No `Configure Viewer` defina as opções desejadas.

   selecione o **[!UICONTROL Info Tip]** ícone ao lado da opção se desejar ler sua descrição.

   A página Visualizar exibe o visualizador à medida que você atualiza e altera as configurações.

1. (Opcional) Na **[!UICONTROL Info Panel Settings]**, o **[!UICONTROL Information Server URL]** pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   | --- | --- | --- |
   | `$1$` | valor rollover_key | O identificador de item do `<area>` elemento do mapa. |
   | `$2$` | quadro | O número sequencial do quadro mostrado no momento no conjunto de imagens. |
   | `$3$` | raiz da imagem | O primeiro elemento de caminho do primeiro item especificado no comando image (normalmente a ID do catálogo de imagens da entrada do catálogo especificando o conjunto de imagens). |

1. (Opcional) Na **[!UICONTROL Info Panel Settings]**, no **[!UICONTROL Response Template]** digite o texto que deseja exibir se o Adobe Dynamic Media Classic encontrar um erro ao recuperar informações de um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de eCatalog, mas nenhum identificador de rollover, essa mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar esse Modelo de resposta em vez do modelo definido no próprio eCatalog, adicione `fmt=1` até o final do URL do Servidor de Informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Selecionar **[!UICONTROL Save]**.
1. Selecionar **[!UICONTROL Default]** para que a Predefinição do visualizador do eCatalog criada seja a usada para exibir eCatalogs na sua página da Web.

Para excluir uma Predefinição do visualizador de eCatalog, selecione-a na tela Predefinições do visualizador e **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)
