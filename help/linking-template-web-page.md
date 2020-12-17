---
title: Vincular um modelo a uma página da Web
seo-title: Vincular um modelo a uma página da Web
description: nulo
seo-description: Saiba como vincular um modelo a uma página da Web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Vincular um modelo a uma página da Web{#linking-a-template-to-a-web-page}

Seus sites e aplicativos acessam o conteúdo do Dynamic Media Image Server por meio de sequências de caracteres de URL. Depois de publicar um modelo, o Dynamic Media Classic ativa uma string de URL que faz referência ao modelo em Dynamic Media Image Servers. Você pode colar este URL em um navegador da Web para teste.

Para colocar sequências de caracteres de URL em suas páginas da Web e aplicativos, copie-as do Dynamic Media Classic. Para obter uma string de URL de modelo gerada com uma predefinição de imagem, vá para a tela Pré-visualização ou o painel Procurar (em visualização de detalhes). Em seguida, selecione uma predefinição de imagem e selecione o botão copiar URL.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

## Obtenção de um URL de modelo {#obtaining-a-template-url}

Você pode obter uma string de URL de modelo gerada por uma Predefinição de imagem na tela Pré-visualização de modelo. Depois de copiar o URL, ele chega na Área de transferência para que você possa colá-lo conforme necessário. Siga estas etapas para obter uma string de URL de modelo gerada com uma Predefinição de imagem na tela Pré-visualização de modelo:

1. Clique no botão de Pré-visualização de sobreposição do modelo ou escolha Arquivo > Pré-visualização. A tela Pré-visualização é aberta.
1. Usando os menus da predefinição, escolha a predefinição de imagem com a qual deseja fornecer a imagem do modelo. A tela de Pré-visualização mostra a aparência do modelo quando ele é entregue pelo servidor.
1. Clique no botão Copiar URL para copiar o URL para a Área de transferência.

## Adicionar URLs de modelo à sua página da Web {#adding-template-urls-to-your-web-page}

Para adicionar um modelo à sua página da Web, consulte sua equipe de desenvolvimento de página da Web para modificar a tag `<IMG>` no código da página da Web HTML usando a string do URL do Dynamic Media Classic para fazer uma solicitação aos Dynamic Media Image Servers. O mecanismo de comércio ou o código dinâmico da página da Web insere a imagem do modelo no tamanho e com a especificação de formatação definida pela Predefinição de imagem que você escolher para o modelo.

>[!MORELIKETHIS]
>
>* [Adicionar imagens dinâmicas à sua página da Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

