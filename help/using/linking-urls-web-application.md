---
title: Vincular URLs ao aplicativo web
description: Saiba como vincular URLs ao seu aplicativo web a partir do Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Vincular URLs ao aplicativo web{#linking-urls-to-your-web-application}

Seus sites e aplicativos acessam o conteúdo do Dynamic Media Image Server por meio de cadeias de caracteres de URL. Depois de publicar uma imagem, o Adobe Dynamic Media Classic ativa uma cadeia de caracteres de URL que faz referência à Predefinição de imagem nos servidores de imagem da Dynamic Media. Você pode colar esses URLs em um navegador da Web para testes.

Para colocar essas cadeias de caracteres de URL em suas páginas da Web e aplicativos, copie-as do Adobe Dynamic Media Classic. Para obter uma cadeia de caracteres de URL gerada com uma Predefinição de imagem, vá para a tela Visualização ou o Painel de navegação (na Exibição de detalhes).

## Obter um URL de predefinição de imagem {#obtaining-an-image-preset-url}

É possível obter uma cadeia de caracteres de URL gerada por uma Predefinição de imagem a partir da Visualização ou da Exibição de detalhes. Depois de copiar o URL, ele é colocado na Área de transferência para que você possa colá-lo conforme necessário.

>[!NOTE]
>
>O URL não estará ativo até que você publique o ativo.

### Obter um URL de predefinição de imagem a partir da visualização {#obtaining-an-image-preset-url-from-preview}

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta Ativo que contém o ativo de imagem a ser visualizado.
1. Siga um destes procedimentos:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem e, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL List View]**. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. (Opcional) Na Lista de predefinições de imagem, na lista suspensa Codificação de URL para geração de URL de cópia, selecione a codificação de URL a ser aplicada ao URL do ativo de imagem quando ele for copiado.
1. Na janela Lista de predefinições de imagem, na área superior direita do painel de visualização, selecione **[!UICONTROL Copy URL]** para o tipo de predefinição selecionado.
1. No canto inferior direito da janela Lista de predefinições de imagens, selecione **[!UICONTROL Close]** para retornar à tela Ativos.

### Obter um URL de predefinição de imagem no painel Procurar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. No painel Biblioteca de ativos à esquerda, navegue até a pasta Ativo que contém o ativo de imagem que deseja visualizar.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Grid View]**. Na janela Ativo, selecione um único ativo de imagem.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, selecione **[!UICONTROL Detail View]**.
1. Selecionar **[!UICONTROL URLs]** no painel do lado direito da tela, para que você possa abrir a lista de Predefinições de imagem.
1. Selecionar **[!UICONTROL Copy URL]** Link ao lado do nome da Predefinição de imagem com o URL que você deseja copiar para a Área de transferência.

## Sobre strings de URL de predefinição de imagem {#about-image-preset-url-strings}

Uma chamada de URL para dimensionamento de imagem para servidores de imagem Dynamic Media tem a seguinte sintaxe básica:

*caminho*/*nome do Servidor de imagens*/*nome da conta*/*nome da imagem*?*modificador1*&amp;*modificador2*&amp;...

Em um URL do Dynamic Media Image Server, as instruções para o servidor exibir a imagem são exibidas após o ponto de interrogação (?). Por exemplo, essa chamada de URL fornece uma imagem chamada &quot;mochila&quot; com uma largura de 250 pixels:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Um URL de predefinição de imagem contém todas as instruções do modificador para apresentar a imagem nas especificações adequadas de tamanho e formatação. Sem uma Predefinição de imagem, observe todas as instruções do modificador após o ponto de interrogação (?) nesta string de URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

No entanto, em uma cadeia de caracteres de URL gerada com uma Predefinição de imagem, o nome da Predefinição de imagem aparece no lugar das instruções definidas pela Predefinição de imagem. Por exemplo, em referência ao URL longo acima, a cadeia de caracteres do URL é:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Os nomes das predefinições de imagem em URLs são colocados em cifrões ($). Quando um Servidor de imagens do Dynamic Media encontra a parte da Predefinição de imagem do URL (o `Large` nesse caso), usando as instruções de tamanho e formatação definidas pela Predefinição de imagem &quot;Grande&quot;.

## Adicionar imagens dinâmicas à sua página da Web {#adding-dynamic-images-to-your-web-page}

Para adicionar imagens dinâmicas à sua página da Web, `<IMG>` A tag do no código da página da Web do HTML geralmente é modificada usando a string de URL do Adobe Dynamic Media Classic para fazer uma solicitação aos servidores de imagem da Dynamic Media. Essa cadeia de caracteres produz a imagem nas especificações de tamanho e formatação definidas pela Predefinição de imagem.

Por exemplo, em vez da chamada típica para abrir uma imagem estática, como

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Agora você usa o `<IMG>`para substituir a referência a uma imagem estática por uma chamada de Predefinição de imagem para a plataforma Adobe Dynamic Media Classic. Uma chamada de amostra tem esta aparência:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

Neste exemplo, um servidor de imagens Dynamic Media &quot;pesquisa&quot; a definição de `$thumbnail$` e gera dinamicamente a imagem apropriada com as especificações de dimensionamento e formatação definidas pelo `thumbnail`Predefinição de imagem. Em uma string de URL, todos os itens, exceto o nome do arquivo de imagem do produto ( `backpack_trns` nesse caso) normalmente são programados para o modelo de página. O único elemento inserido automaticamente no modelo de página do servidor de comércio é a ID de IPS ou o nome da imagem.
