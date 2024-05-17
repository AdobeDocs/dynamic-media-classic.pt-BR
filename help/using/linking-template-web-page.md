---
title: Vincular um modelo a uma página da Web
description: Saiba como vincular um modelo a uma página da Web no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Vincular um modelo a uma página da Web{#linking-a-template-to-a-web-page}

Seus sites e aplicativos acessam o conteúdo do Dynamic Media Image Server por meio de cadeias de caracteres de URL. Depois de publicar um modelo, o Adobe Dynamic Media Classic ativa uma cadeia de caracteres de URL que faz referência ao modelo nos Dynamic Media Image Servers. Você pode colar esse URL em um navegador da Web para testar o.

Para inserir strings de URL em suas páginas da Web e aplicativos, copie-as do Adobe Dynamic Media Classic. Para obter uma cadeia de caracteres de URL de modelo gerada com uma Predefinição de imagem, vá para a tela Visualização ou o painel Procurar (na Exibição de detalhes). Em seguida, selecione uma Predefinição de imagem e o botão Copiar URL.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Obter um URL de modelo {#obtaining-a-template-url}

Você pode obter uma cadeia de caracteres de URL de modelo gerada por uma Predefinição de imagem na tela Visualização de modelo. Depois de copiar o URL, ele é colocado na Área de transferência para que você possa colá-lo conforme necessário. Para obter uma string de URL de modelo gerada com uma Predefinição de imagem a partir da página Visualização de modelo, faça o seguinte:

1. Selecione a sobreposição do modelo **[!UICONTROL Preview]** ou vá para **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Usando os menus da Predefinição, escolha a Predefinição de imagem com a qual deseja fornecer a imagem de modelo. A página Visualizar mostra a aparência do modelo quando ele é entregue pelo servidor.
1. Selecionar **[!UICONTROL Copy URL]** para que você possa copiar o URL para a Área de transferência.

## Adicionar URLs de modelo à sua página da Web {#adding-template-urls-to-your-web-page}

Para adicionar um modelo à página da Web, consulte a equipe de desenvolvimento da página da Web para modificar a `<IMG>` no código da página da Web do HTML. Use a string do URL do Adobe Dynamic Media Classic para fazer uma solicitação aos Dynamic Media Image Servers. O mecanismo de comércio ou o código dinâmico da página da Web insere a imagem de modelo no tamanho e com a especificação de formatação definida pela Predefinição de imagem escolhida para o modelo.

>[!MORELIKETHIS]
>
>* [Adicionar imagens dinâmicas à sua página da Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
