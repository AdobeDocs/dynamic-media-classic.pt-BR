---
title: Vincular um modelo a uma página da Web
seo-title: Vincular um modelo a uma página da Web
description: 'null'
seo-description: Saiba como vincular um modelo a uma página da Web.
uuid: f 111 ef 06-4 afc -454 c -86 ce -5 d 640236 d 40 b
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/template_ basics
discoiquuid: 989 dba 07-448 a -45 b 1-b 157-af 50 abb 5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vincular um modelo a uma página da Web{#linking-a-template-to-a-web-page}

Seus sites e aplicativos acessam o conteúdo do Servidor de imagem do Dynamic Media por meio de strings de URL. Depois de publicar um modelo, o Dynamic Media Classic ativa uma sequência de caracteres de URL que referencia o modelo nos servidores de imagem do Dynamic Media. Você pode colar esse URL em um navegador da Web para teste.

Para colocar strings de URL em suas páginas e aplicativos da Web, copie-os do Sistema de publicação Scene 7. Para obter uma sequência de URL do modelo gerada com uma predefinição de imagem, vá para a tela Visualizar ou o Painel Procurar (na exibição Detalhe). Em seguida, selecione uma Predefinição de imagem e selecione o botão Copiar URL.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Obtenção de um URL de modelo {#obtaining-a-template-url}

É possível obter uma sequência de URL de modelo gerada por uma Predefinição de imagem na tela Visualização do modelo. Depois de copiar o URL, ele chega à área de transferência para que você possa colá-lo conforme necessário. Siga estas etapas para obter uma sequência de URL de modelo gerada com uma Predefinição de imagem na tela Visualização do modelo:

1. Clique no botão de visualização de rolagem do modelo ou escolha Arquivo &gt; Visualizar. A tela Visualizar é aberta.
1. Usando os menus Predefinidos, escolha a Predefinição de imagem com a qual você deseja entregar a imagem de modelo. A tela Visualizar mostra como é a aparência do modelo quando ele é entregue a partir do servidor.
1. Clique no botão Copiar URL para copiar o URL para a área de transferência.

## Adicionar urls de modelo à sua página da Web {#adding-template-urls-to-your-web-page}

Para adicionar um modelo à sua página da Web, consulte sua equipe de desenvolvimento de página da Web para modificar a `<IMG>` tag no código de sua página HTML usando a string de URL clássica do Dynamic Media para fazer uma solicitação aos servidores de imagem do Dynamic Media. O mecanismo de comércio ou o código dinâmico da página da Web insere a imagem de modelo em tamanho e com a especificação de formatação definida pela predefinição de imagem escolhida para o modelo.

>[!MORELIKETHIS]
>
>* [Adicionar imagens dinâmicas à sua página da Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

