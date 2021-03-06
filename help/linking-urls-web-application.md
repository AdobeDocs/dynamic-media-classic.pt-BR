---
title: Vincular URLs ao aplicativo da Web
description: Saiba como vincular URLs ao seu aplicativo da Web a partir do Adobe Dynamic Media Classic.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Vincular URLs ao aplicativo da Web{#linking-urls-to-your-web-application}

Seus sites e aplicativos da Web acessam o conteúdo do Dynamic Media Image Server por meio de cadeias de caracteres de URL. Depois de publicar uma imagem, o Adobe Dynamic Media Classic ativa uma string de URL que faz referência à Predefinição de imagem nos Servidores de imagem Dynamic Media. Você pode colar esses URLs em um navegador da Web para testes.

Para colocar essas cadeias de caracteres de URL em suas páginas da Web e aplicativos, copie-as do Adobe Dynamic Media Classic. Para obter uma string de URL gerada com uma Predefinição de imagem, vá para a tela Visualização ou o Painel de navegação (na Exibição de detalhes).

## Obter um URL de predefinição de imagem {#obtaining-an-image-preset-url}

Você pode obter uma string de URL gerada por uma Predefinição de imagem a partir de Visualização ou da Exibição de detalhes. Depois de copiar o URL, ele chega à Área de transferência para que você possa colá-lo conforme necessário.

>[!NOTE]
>
>O URL não fica ativo até que você publique o ativo.

### Obter um URL de predefinição de imagem na Visualização {#obtaining-an-image-preset-url-from-preview}

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja visualizar.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem e, em seguida, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. (Opcional) Na Lista predefinida de imagem, na lista suspensa Codificação de URL para Geração de URL de Cópia, selecione a codificação de URL que deseja aplicar ao URL do ativo de imagem quando ele for copiado.
1. Na janela Lista de predefinições de imagens, na área superior direita do painel de visualização, selecione **[!UICONTROL Copy URL]** para o tipo de predefinição selecionado.
1. No canto inferior direito da janela Lista de predefinições de imagens, selecione **[!UICONTROL Close]** para retornar à tela Ativos.

### Obter um URL de predefinição de imagem no painel Procurar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja visualizar.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**.
1. Selecione **[!UICONTROL URLs]** no painel no lado direito da tela, para que você possa abrir a lista de Predefinições de imagem.
1. Selecione **[!UICONTROL Copy URL]** link ao lado do nome da Predefinição de imagem com o URL que você deseja copiar para a Área de transferência.

## Sobre as cadeias de caracteres do URL da predefinição de imagem {#about-image-preset-url-strings}

Uma chamada de URL para dimensionamento de imagem em servidores de imagem da Dynamic Media tem a seguinte sintaxe básica:

*caminho*/*nome do Servidor de imagens*/*nome da conta*/*nome* da imagem?*modifier1*&amp;*modifier2*&amp;...

Em um URL de servidor de imagem do Dynamic Media, as instruções para o servidor exibir a imagem são exibidas após o ponto de interrogação (?). Por exemplo, esta chamada de URL fornece uma imagem chamada &quot;backpack&quot; a uma largura de 250 pixels:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Um URL de predefinição de imagem contém todas as instruções do modificador para apresentar a imagem no tamanho e especificações de formatação adequados. Sem uma predefinição de imagem, observe todas as instruções do modificador após o ponto de interrogação (?) nesta cadeia de caracteres do URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

No entanto, em uma string de URL gerada com uma Predefinição de imagem, o nome da Predefinição de imagem aparece no lugar das instruções definidas pela Predefinição de imagem. Por exemplo, referindo-se ao URL longo acima, a cadeia de caracteres do URL é:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Nomes de predefinições de imagens em URLs são colocados em cifrões ($). Quando um servidor de imagem do Dynamic Media encontra a parte da Predefinição de imagem do URL (o `Large` neste caso), usando as instruções de tamanho e formatação definidas pela Predefinição de imagem &quot;Grande&quot;.

## Adicionar imagens dinâmicas à página da Web {#adding-dynamic-images-to-your-web-page}

Para adicionar imagens dinâmicas à sua página da Web, a tag `<IMG>` no código da página da Web HTML normalmente é modificada usando a Adobe Dynamic Media Classic URL string para fazer uma solicitação para Servidores de Imagem Dynamic Media. Essa string produz a imagem no tamanho e nas especificações de formatação definidos pela Predefinição de imagem.

Por exemplo, em vez da chamada típica para abrir uma imagem estática como

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Agora você usa a tag `<IMG>`para substituir a referência a uma imagem estática por uma chamada de Predefinição de imagem para a plataforma Adobe Dynamic Media Classic. Um exemplo de chamada tem esta aparência:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

Neste exemplo, um Dynamic Media Image Server &quot;procura&quot; a definição de `$thumbnail$` e gera dinamicamente a imagem apropriada com as especificações de dimensionamento e formatação definidas pela `thumbnail`Predefinição de imagem. Em uma string de URL, todos os itens, exceto o nome do arquivo da imagem do produto ( `backpack_trns` neste caso) normalmente são conectados ao modelo da página. O único elemento inserido automaticamente no modelo de página do seu servidor de comércio é a ID do IPS ou o nome da imagem.
