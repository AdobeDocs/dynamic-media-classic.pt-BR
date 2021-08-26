---
title: Vincular um modelo a uma página da Web
description: Saiba como vincular um modelo a uma página da Web no Adobe Dynamic Media Classic.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Vincular um modelo a uma página da Web{#linking-a-template-to-a-web-page}

Seus sites e aplicativos da Web acessam o conteúdo do Dynamic Media Image Server por meio de cadeias de caracteres de URL. Depois de publicar um modelo, o Adobe Dynamic Media Classic ativa uma string de URL que faz referência ao modelo em Servidores de imagem da Dynamic Media. Você pode colar este URL em um navegador da Web para testes.

Para colocar cadeias de caracteres de URL em suas páginas da Web e aplicativos, copie-as do Adobe Dynamic Media Classic. Para obter uma cadeia de caracteres de URL de modelo gerada com uma Predefinição de imagem, vá para a tela Visualização ou o Painel de navegação (na Exibição de detalhes). Em seguida, selecione uma Predefinição de imagem e selecione o botão copiar URL.

>[!NOTE]
>
>O URL não fica ativo até que você publique o ativo.

## Obter um URL de modelo {#obtaining-a-template-url}

Você pode obter uma string de URL do modelo gerada por uma Predefinição de imagem na tela Visualização do modelo . Depois de copiar o URL, ele chega à Área de transferência para que você possa colá-lo conforme necessário. Para obter uma string de URL do modelo gerada com uma Predefinição de imagem da página Visualização do modelo, faça o seguinte:

1. Selecione o botão **[!UICONTROL Preview]** de sobreposição do modelo ou vá para **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Usando os menus da predefinição, escolha a predefinição de imagem com a qual deseja fornecer a imagem do modelo. A página Visualização mostra a aparência do modelo quando ele é entregue a partir do servidor.
1. Selecione **[!UICONTROL Copy URL]** para poder copiar o URL para a Área de transferência.

## Adicionar URLs de modelo à sua página da Web {#adding-template-urls-to-your-web-page}

Para adicionar um modelo à sua página da Web, consulte a equipe de desenvolvimento da página da Web para modificar a tag `<IMG>` no código da página da Web HTML. Use a cadeia de caracteres de URL clássica do Adobe Dynamic Media para fazer uma solicitação para os servidores de imagem da Dynamic Media. O mecanismo de comércio ou o código dinâmico da página da Web insere a imagem do modelo no tamanho e com a especificação de formatação definida pela Predefinição de imagem escolhida para o modelo.

>[!MORELIKETHIS]
>
>* [Adicionar imagens dinâmicas à página da Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

