---
title: Configuração das predefinições do visualizador do ecatalog
seo-title: Configuração das predefinições do visualizador do ecatalog
description: 'null'
seo-description: Saiba como configurar Predefinições do ecatalog Viewer.
uuid: aca 66 bc 5-8491-4 d 81-9 a 06-1 d 3531860 a 14
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6 c 123 f 85-3 bc 4-4392-a 7 fb -55618127 c 65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuração das predefinições do visualizador do ecatalog{#setting-up-ecatalog-viewer-presets}

As Predefinições do visualizador do ecatalog determinam o estilo, o comportamento e a aparência dos visualizadores ecatalog. O Dynamic Media Classic fornece Predefinições do visualizador do ecatalog e também é possível criar suas próprias Predefinições do visualizador do ecatalog, caso você seja um administrador.

Para criar uma nova predefinição, comece do zero ou comece com uma Predefinição do visualizador do ecatalog do Dynamic Media fornecida e salve-a com um novo nome. Você pode criar suas próprias Predefinições do visualizador do ecatalog para apresentar material impresso em suas cores da empresa e definir o tom.

As Predefinições do Visualizador do ecatalog oferecem várias configurações para ir de página à página, ampliar, pesquisar e escolher «capas». » A aparência desses controles depende da escolha das Predefinições do ecatalog Viewer.

Siga estas etapas para criar uma Predefinição do visualizador do ecatalog (você deve ser um administrador):

1. Clique **em Configuração** &gt; **Predefinições do visualizador**.
1. Na tela Predefinições do visualizador, crie uma Predefinição do visualizador ecatalog começando pela inicialização ou iniciando de uma Predefinição do visualizador ecatalog existente:

   **Criando uma Predefinição do visualizador do ecatalog** Clique em Adicionar. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma, escolha o ecatalog Viewer e clique **em Adicionar**.

   **Editando uma Predefinição do visualizador do ecatalog** Selecione uma Predefinição do visualizador do ecatalog e clique em Editar. Clique **em Salvar como** depois de concluir a criação da predefinição.

1. Na tela Configurar visualizador, insira um nome para a Predefinição do Visualizador do ecatalog.
1. Na tela Configurar visualizador, defina as opções desejadas.

   Clique no ícone Dica de informações adjacente à opção para ver sua descrição.

   A tela de visualização exibe o visualizador à medida que você atualiza e altera as configurações.

1. (Opcional) Nas Configurações do painel Informações, a opção URL do servidor de informações pode incluir os seguintes tokens especiais, que o visualizador substitui:

   | Token | Substituído por | Notas |
   |--- |--- |--- |
   | `$1$` | valor rollover_ key | O identificador do item do `<area>` elemento do mapa. |
   | `$2$` | quadro | O número da sequência do quadro exibido no momento no conjunto de imagens. |
   | `$3$` | imageroot | O primeiro elemento de caminho do primeiro item especificado no comando da imagem (normalmente a ID do catálogo de imagens da entrada do catálogo que especifica o conjunto de imagens). |

1. (Opcional) Nas Configurações do painel Informações, na caixa Modelo de resposta, digite o texto que deseja exibir se o Dynamic Media Classic encontrar um erro ao recuperar as informações para um mapa de imagem. Por exemplo, se o sistema receber um nome de empresa e um nome de ecatalog, mas sem identificador de rolagem, esta mensagem será exibida para o usuário.

>[!NOTE]
>
>Para usar este Modelo de resposta em vez do modelo definido no próprio ecatalog, adicione «fmt = 1» ao final do URL do servidor de informações. Por exemplo: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Clique **em Salvar**.
1. Clique em Padrão se desejar que a Predefinição do visualizador ecatalog que você criou seja aquela usada para exibir o ecatalogs em sua página da Web.

Para excluir uma predefinição do visualizador do ecatalog, selecione-a na tela Predefinições do visualizador e clique **em Excluir**.

>[!MORELIKETHIS]
>
>* [Predefinições do visualizador](application-setup.md#viewer_presets)

