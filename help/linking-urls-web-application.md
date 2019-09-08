---
title: Vincular urls ao aplicativo da Web
seo-title: Vincular urls ao aplicativo da Web
description: 'null'
seo-description: Saiba como vincular urls ao aplicativo da Web.
uuid: 1179 bdd 3-9 b 39-47 f 9-945 d -1 c 1 ca 186 bf 96
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/image_ sizing
discoiquuid: 71299640-676 d -49 b 7-841 d -6118 f 31044 e 8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vincular urls ao aplicativo da Web{#linking-urls-to-your-web-application}

Seus sites e aplicativos acessam o conteúdo do Servidor de imagem do Dynamic Media por meio de strings de URL. Depois de publicar uma imagem, o Dynamic Media Classic ativa uma sequência de caracteres de URL que faz referência à Predefinição de imagem nos servidores de imagem do Dynamic Media. Você pode colar esses urls em um navegador da Web para teste.

Para colocar essas sequências de URL em suas páginas e aplicativos da Web, copie-os do Sistema de publicação Scene 7. Para obter uma sequência de caracteres de URL gerada com uma predefinição de imagem, vá para a tela Visualizar ou o Painel Procurar (na exibição Detalhe).

## Obtenção de um URL predefinido de imagem {#obtaining-an-image-preset-url}

É possível obter uma string de URL gerada por uma Predefinição de imagem na Visualização ou na Exibição de detalhes. Depois de copiar o URL, ele chega à área de transferência para que você possa colá-lo conforme necessário.

***Observação**: O URL não estará ativo até que você publique o ativo.*

### Obter um URL predefinido de imagem da visualização {#obtaining-an-image-preset-url-from-preview}

1. No painel Biblioteca de ativos do lado esquerdo, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja visualizar.
1. Execute um dos procedimentos a seguir:

   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Exibição de grade. Na janela Ativo, selecione um único ativo de imagem e depois abaixo da imagem em miniatura, clique em Visualizar &gt; Lista predefinida de imagens.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Exibição de lista. Na janela Ativo, selecione um único ativo de imagem e, à direita da imagem em miniatura, clique em Visualizar &gt; Lista predefinida de imagens.
   * Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Exibição de detalhes. Na mesma barra de ferramentas, clique em Visualizar &gt; Lista de predefinições de imagens.

1. (Opcional) Na janela Lista de predefinição de imagem, na lista suspensa Codificação de URL da lista suspensa Geração de URL de cópia na parte inferior, selecione a codificação de URL que deseja aplicar ao URL do ativo de imagem quando ele for copiado.
1. Na janela Lista de predefinições de imagens, na área superior direita do painel de visualização, clique em Copiar URL para o tipo predefinido selecionado.
1. No canto inferior direito da janela Lista de predefinições de imagens, clique em Fechar para retornar à tela Ativos.

### Obter um URL predefinido de imagem no painel Procurar {#obtaining-an-image-preset-url-from-the-browse-panel}

1. No painel Biblioteca de ativos do lado esquerdo, navegue até as pastas Ativos que contêm o ativo de imagem que você deseja visualizar.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Exibição de grade. Na janela Ativo, selecione um único ativo de imagem.
1. Acima da janela Ativos, no lado direito da barra de ferramentas, clique em Exibição de detalhes.
1. Clique em urls no painel no lado direito da tela para desdobrar a lista de Predefinições de imagens.
1. Clique em Copiar link URL ao lado do nome da Predefinição de imagem com o URL que você deseja copiar para a Área de transferência.

## Sobre strings de URL predefinidas de imagens {#about-image-preset-url-strings}

Uma chamada de URL para dimensionamento de imagem para servidores de imagem do Dynamic Media tem a seguinte sintaxe básica:

*caminho*/*nome do servidor de imagem*/*nome da conta*/*nome da imagem*?*modifier 1*&amp;*modifier 2*&amp;…

Em um URL do servidor de imagem do Dynamic Media, instruções para o servidor para exibir a imagem aparecem depois do ponto de interrogação (?). Por exemplo, essa chamada de URL fornece uma imagem chamada «backpack» em uma largura de 250 pixels:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Um URL predefinido de imagem contém todas as instruções modificadoras para a apresentação da imagem nas especificações de tamanho e formatação adequadas. Sem uma predefinição de imagem, observe todas as instruções modificadoras após o ponto de interrogação (?) nesta string de URL:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

No entanto, em uma sequência de caracteres de URL gerada com uma predefinição de imagem, o nome da predefinição de imagem aparece no lugar das instruções definidas pela predefinição de imagem. Por exemplo, se refere ao URL longo acima, a string do URL é:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Os nomes de predefinição de imagens em urls são inscritos em cifrão ($). Quando um servidor de imagem do Dynamic Media encontra a parte Predefinida de imagem do URL (neste `Large` caso), usando as instruções de tamanho e formatação definidas pela Predefinição de imagem «Grande».

## Adicionar imagens dinâmicas à sua página da Web {#adding-dynamic-images-to-your-web-page}

Para adicionar imagens dinâmicas à sua página da Web, a `<IMG>` tag em seu código de página HTML normalmente é modificada usando a string de URL clássica do Dynamic Media para fazer uma solicitação aos servidores de imagem do Dynamic Media. Essa string produz a imagem nas especificações de tamanho e formatação definidas pela Predefinição de imagem.

Por exemplo, em vez da chamada típica para abrir uma imagem estática, como

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

agora você usa a `<IMG>`tag para substituir a referência a uma imagem estática por uma chamada de Predefinição de imagem para a plataforma do Dynamic Media Classic. Uma chamada de amostra é desta forma:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

Neste exemplo, um Servidor de imagem do Dynamic Media «procura» a definição `$thumbnail$` de e gera dinamicamente a imagem apropriada com as especificações de dimensionamento e de formatação definidas pela Predefinição `thumbnail`de imagem. Em uma sequência de caracteres de URL, todos os itens, exceto o nome de arquivo de imagem do produto ( `backpack_trns` nesse caso), normalmente são impressos para o modelo de página. O único elemento inserido automaticamente no modelo de página do seu servidor de comércio é a ID do IPS ou o nome da imagem.
