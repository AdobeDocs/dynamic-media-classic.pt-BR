---
title: Configuração das predefinições do eCatalog Viewer
seo-title: Configuração das predefinições do eCatalog Viewer
description: nulo
seo-description: Saiba como configurar as predefinições do visualizador do eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Configuração das predefinições do eCatalog Viewer{#setting-up-ecatalog-viewer-presets}

As predefinições do visualizador do eCatalog determinam o estilo, o comportamento e a aparência dos visualizadores do eCatalog. O Dynamic Media Classic fornece predefinições do visualizador de eCatalog e você pode criar suas próprias predefinições do visualizador de eCatalog, bem como se você for um administrador.

Para criar uma nova predefinição, você pode start do zero ou start com uma predefinição do visualizador do eCatalog fornecida pelo Dynamic Media Classic e salvá-la com um novo nome. Você pode criar suas próprias predefinições do visualizador do eCatalog para apresentar o material impresso nas cores da empresa e definir o tom.

O eCatalog Viewer Presets oferta muitas configurações para ir de página em página, aumentar o zoom, pesquisar e escolher &quot;capas&quot;. A aparência desses controles e a aparência do próprio visualizador dependem da sua escolha de Predefinições do visualizador de eCatalog.

Siga estas etapas para criar uma predefinição do visualizador do eCatalog (você deve ser um administrador):

1. Clique em **Configuração** > Predefinições **do visualizador**.
1. Na tela Predefinições do visualizador, crie uma predefinição do visualizador do eCatalog iniciando novamente ou iniciando a partir de uma predefinição existente do visualizador do eCatalog:

   * **Criação de uma predefinição** do visualizador do eCatalogClick Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha o eCatalog Viewer e clique em 
**Adicionar**.

   * **Editando uma predefinição** do visualizador do eCatalogSelecione uma predefinição do visualizador do eCatalog e clique em Editar. Clique em 
**Salvar como** após terminar de criar a predefinição.

1. Na tela Configurar visualizador, digite um nome para sua predefinição do visualizador do eCatalog.
1. Na tela Configurar visualizador, defina as opções desejadas.

   Clique no ícone Dica de informações adjacente à opção para ver sua descrição.

   A tela pré-visualização exibe o visualizador à medida que você atualiza e altera as configurações.

1. (Opcional) Nas Configurações do painel Informações, a opção URL do Servidor de Informações pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   |--- |--- |--- |
   | `$1$` | valor de rollover_key | O identificador de item do `<area>` elemento do mapa. |
   | `$2$` | quadro | O número de sequência do quadro exibido no momento no conjunto de imagens. |
   | `$3$` | imageroot | O primeiro elemento de caminho do primeiro item especificado no comando image (normalmente a ID do catálogo de imagens da entrada do catálogo que especifica o conjunto de imagens). |

1. (Opcional) Na caixa Configurações do painel Informações, na caixa Modelo de resposta, digite o texto que deseja exibir se o Dynamic Media Classic encontrar um erro ao recuperar informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de eCatalog, mas nenhum identificador de sobreposição, essa mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar esse Modelo de Resposta em vez do modelo definido no próprio eCatalog, adicione &quot;fmt=1&quot; ao final do URL do Servidor de Informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Clique em **Salvar**.
1. Clique em Padrão se desejar que a predefinição do visualizador de eCatalog que você criou seja a usada para exibir eCatalogs na sua página da Web.

Para excluir uma predefinição do visualizador do eCatalog, selecione-a na tela Predefinições do visualizador e clique em **Excluir**.

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)

