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
autotag-review: '2026-05-13T19:52:27.080Z'
TQID: 'https://experienceleague.adobe.com/c1Un6UFrYZh-tqwPp98shMiTUEEMhkEn1vmxEl2rVq0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 334
ht-degree: 0%

---

# Vincular um modelo a uma página da Web{#linking-a-template-to-a-web-page}

Seus sites e aplicativos acessam o conteúdo do Servidor de imagens do Dynamic Media por meio de cadeias de caracteres de URL. Depois de publicar um modelo, o Adobe Dynamic Media Classic ativa uma cadeia de caracteres de URL que faz referência ao modelo nos servidores de imagem do Dynamic Media. Você pode colar esse URL em um navegador da Web para testar o.

Para inserir strings de URL em suas páginas da Web e aplicativos, copie-as do Adobe Dynamic Media Classic. Para obter uma cadeia de caracteres de URL de modelo gerada com uma Predefinição de imagem, vá para a tela Visualização ou o painel Procurar (na Exibição de detalhes). Em seguida, selecione uma Predefinição de imagem e o botão Copiar URL.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Obter um URL de modelo {#obtaining-a-template-url}

Você pode obter uma cadeia de caracteres de URL de modelo gerada por uma Predefinição de imagem na tela Visualização de modelo. Depois de copiar o URL, ele é colocado na Área de transferência para que você possa colá-lo conforme necessário. Para obter uma string de URL de modelo gerada com uma Predefinição de imagem a partir da página Visualização de modelo, faça o seguinte:

1. Selecione o botão de substituição **[!UICONTROL Preview]** do modelo ou vá para **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Usando os menus da Predefinição, escolha a Predefinição de imagem com a qual deseja fornecer a imagem de modelo. A página Visualizar mostra a aparência do modelo quando ele é entregue pelo servidor.
1. Selecione **[!UICONTROL Copy URL]** para poder copiar a URL para a Área de Transferência.

## Adicionar URLs de modelo à sua página da Web {#adding-template-urls-to-your-web-page}

Para adicionar um modelo à sua página da Web, consulte sua equipe de desenvolvimento de página da Web para modificar a tag `<IMG>` no código da página da Web do HTML. Use a string do URL do Adobe Dynamic Media Classic para fazer uma solicitação aos servidores de imagem do Dynamic Media. O mecanismo de comércio ou o código dinâmico da página da Web insere a imagem de modelo no tamanho e com a especificação de formatação definida pela Predefinição de imagem escolhida para o modelo.

>[!MORELIKETHIS]
>
>* [Adicionar imagens dinâmicas à sua página da Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
