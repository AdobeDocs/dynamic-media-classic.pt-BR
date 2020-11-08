---
title: Vincular URLs ao aplicativo da Web
seo-title: Vincular URLs ao aplicativo da Web
description: nulo
seo-description: Saiba como vincular URLs ao seu aplicativo da Web.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---


# Vincular URLs ao aplicativo da Web{#linking-urls-to-your-web-application}

Seus sites e aplicativos acessam o conteúdo do Servidor de Imagens do Dynamic Media por meio de sequências de caracteres de URL. Depois de publicar uma imagem, o Dynamic Media Classic ativa uma string de URL que faz referência à predefinição de imagem nos servidores de imagem de mídia dinâmica. Você pode colar esses URLs em um navegador da Web para teste.

Para colocar essas strings de URL em suas páginas da Web e aplicativos, copie-as do Dynamic Media Classic. Para obter uma string de URL gerada com uma Predefinição de imagem, vá para a tela Pré-visualização ou para o Painel de navegação (em visualização de detalhes).

## Obter um URL predefinido de imagem {#obtaining-an-image-preset-url}

Você pode obter uma string de URL gerada por uma Predefinição de imagem a partir de Pré-visualização ou de Visualização Detalhada. Depois de copiar o URL, ele chega na Área de transferência para que você possa colá-lo conforme necessário.

***Observação **: O URL não estará ativo até que você publique o ativo.*

### Obter um URL predefinido de imagem da Pré-visualização {#obtaining-an-image-preset-url-from-preview}

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja pré-visualização.
1. Execute um dos procedimentos a seguir:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Visualização de Grade. Na janela Ativo, selecione um único ativo de imagem e, abaixo da imagem em miniatura, clique em Pré-visualização > Lista de predefinição de imagem.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Visualização de Lista. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, clique em Pré-visualização > Lista de predefinição de imagem.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Visualização Detalhada. Na mesma barra de ferramentas, clique em Pré-visualização > Lista de predefinição de imagem.

1. (Opcional) Na janela Lista Predefinição de imagem, na lista suspensa Codificação de URL para Geração de URL de cópia na parte inferior, selecione a codificação de URL que deseja aplicar ao URL do ativo de imagem quando ele for copiado.
1. Na janela Lista predefinida de imagem, na área superior direita do painel de pré-visualização, clique em Copiar URL para o tipo predefinido selecionado.
1. No canto inferior direito da janela Lista predefinida de imagem, clique em Fechar para retornar à tela Ativos.

### Obter um URL predefinido de imagem no painel Procurar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. No painel Biblioteca de ativos, à esquerda, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja pré-visualização.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Visualização de Grade. Na janela Ativo, selecione um único ativo de imagem.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Visualização Detalhada.
1. Clique em URLs no painel no lado direito da tela para desdobrar a lista das predefinições de imagem.
1. Clique no link Copiar URL ao lado do nome da predefinição de imagem com o URL que você deseja copiar para a área de transferência.

## Sobre strings de URL predefinidos de imagens {#about-image-preset-url-strings}

Uma chamada de URL para Dimensionamento de imagem para Servidores de imagem de mídia dinâmica tem a seguinte sintaxe básica:

*caminho*/*nome do Servidor* de imagens/nome *da* conta/nome *da* imagem?*modifier1*&amp;*modifier2*&amp;...

Em um URL do servidor de imagem do Dynamic Media, as instruções para exibir a imagem ao servidor são exibidas após o ponto de interrogação (?). Por exemplo, esta chamada de URL fornece uma imagem chamada &quot;backpack&quot; com uma largura de 250 pixels:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Um URL de predefinição de imagem contém todas as instruções do modificador para apresentar a imagem no tamanho e especificações de formatação apropriados. Sem uma predefinição de imagem, observe todas as instruções do modificador após o ponto de interrogação (?) nesta string de URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Entretanto, em uma sequência de caracteres de URL gerada com uma predefinição de imagem, o nome da predefinição de imagem aparece no lugar das instruções definidas pela predefinição de imagem. Por exemplo, referindo-se ao URL longo acima, a cadeia de caracteres do URL é:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Os nomes predefinidos de imagem em URLs são delimitados por cifrão ($). Quando um Servidor de Imagem de Mídia Dinâmica encontrar a parte Predefinição de Imagem do URL (o `Large` caso), usando as instruções de tamanho e formatação definidas pela Predefinição de Imagem &quot;Grande&quot;.

## Adicionar imagens dinâmicas à sua página da Web {#adding-dynamic-images-to-your-web-page}

Para adicionar imagens dinâmicas à sua página da Web, a `<IMG>` tag em seu código de página da Web HTML normalmente é modificada usando a string de URL do Dynamic Media Classic para fazer uma solicitação aos Servidores de Imagem de Mídia Dinâmica. Essa string produz a imagem no tamanho e nas especificações de formatação definidos pela Predefinição de imagem.

Por exemplo, em vez da chamada típica para abrir uma imagem estática, como

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

agora você usa a `<IMG>`tag para substituir a referência a uma imagem estática por uma chamada predefinida de imagem para a plataforma Dynamic Media Classic. Uma chamada de amostra tem a seguinte aparência:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

Neste exemplo, um Servidor de Imagem de Mídia Dinâmica &quot;procura&quot; a definição de `$thumbnail$` e gera dinamicamente a imagem apropriada com as especificações de dimensionamento e formatação definidas pela Predefinição de `thumbnail`Imagem. Em uma string de URL, todos os itens, exceto o nome de arquivo de imagem do produto ( `backpack_trns` neste caso), normalmente estão programados para o modelo de página. O único elemento que é inserido automaticamente no modelo de página do servidor de comércio é a ID IPS ou o nome da imagem.
