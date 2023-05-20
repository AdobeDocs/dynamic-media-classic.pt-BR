---
title: Criar parâmetros de modelo
description: Saiba como criar parâmetros de modelo no Adobe Dynamic Media Classic.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Criar parâmetros de modelo{#creating-template-parameters}

Os parâmetros permitem usar modelos com o máximo de flexibilidade; eles permitem personalizar dinamicamente uma imagem de modelo. É possível decidir quais camadas de texto e imagem serão incluídas no modelo e, em cada camada, quais parâmetros serão exibidos. Por exemplo, para chamar a atenção para um produto que está à venda, você pode criar uma camada de texto À venda. Posteriormente, é possível remover essa camada, mas manter o restante da imagem de modelo removendo o parâmetro Ao vender.

Ao criar parâmetros de modelo, você declara quais partes do modelo chamar em uma cadeia de caracteres de URL. Um URL construído com parâmetros expõe esses itens na cadeia de caracteres do URL. Com os parâmetros expostos, você pode criar resultados personalizados a partir da maneira como a imagem de modelo é construída dinamicamente a partir do Servidor de imagens. Dessa forma, você pode alterar um modelo dinamicamente, pois pode chamar alguns ou todos os seus parâmetros em um URL.

Em parâmetros de camada de texto, também é possível transformar a cadeia de caracteres de texto em um campo dinâmico vinculado a valores em um banco de dados. Poder vincular texto a um banco de dados é útil, por exemplo, em promoções. É possível personalizar imagens de modelo para que elas mostrem os nomes do cliente ou do cliente. Você também pode vincular um parâmetro de camada de texto a um banco de dados de preços para mostrar o preço de um item em uma imagem de modelo.

É possível consultar um parâmetro mais de uma vez. Use a caixa de combinação para cada comando na caixa de diálogo de parâmetros para selecionar qualquer parâmetro que corresponda a esse comando específico. Por exemplo, todos os parâmetros de tamanho estão disponíveis para o `size=` comando. Você pode reatribuir a referência de parâmetro a qualquer parâmetro que já esteja na caixa de combinação e renomear para algo que não esteja na caixa de combinação. No último caso, o nome deve ser exclusivo. Caso contrário, um erro informa que o parâmetro existe. Ao excluir uma referência de parâmetro, o parâmetro é removido do URL se não for referenciado em nenhum outro lugar. Quando você altera o valor padrão de um parâmetro de texto, todas as referências a esse parâmetro são atualizadas. Você pode ver a atualização na tabela de camadas, na renderização do modelo e no URL. Quando você altera um atributo de camada manipulando alças de redimensionamento ou digitando valores no painel de propriedades, o valor do parâmetro é atualizado e todas as referências ao parâmetro são atualizadas. Por exemplo, se você tiver parametrizado o tamanho de duas camadas usando um parâmetro, ambos os tamanhos de camada serão atualizados quando qualquer um dos tamanhos for alterado. Quando você visualiza um modelo e altera um parâmetro, todas as referências a esse parâmetro são atualizadas.

Consulte também [Noções básicas de modelo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de treinamento.

## Parametrizar uma camada {#parameterizing-a-layer}

Para cada camada do modelo, siga estas etapas para criar parâmetros do modelo:

1. Na lista Camadas, selecione o botão Parâmetros ao lado do nome da camada para a qual deseja criar parâmetros. A tela Parâmetros é aberta. Ela lista os nomes de cada parâmetro na camada, seu valor e seu tipo.
1. Selecione a opção Ativado ao lado do nome de cada parâmetro que você deseja incluir na imagem de modelo.
1. Selecionar **[!UICONTROL Close]** para sair da tela Parâmetros.

>[!NOTE]
>
>Você pode renomear parâmetros na tela Parâmetros. Renomear um parâmetro facilita a identificação do parâmetro em cadeias de caracteres de URL e o uso como um valor de banco de dados. Para renomear um parâmetro, selecione seu **[!UICONTROL On]** selecione seu nome e insira um novo nome no campo Nome.

Para ver uma lista dos parâmetros criados para o modelo, selecione o botão Resumo de Parâmetros na tela Modelo. A tela Resumo de Parâmetros é aberta. Ela lista o nome de cada camada e, se você tiver criado parâmetros para uma camada, os nomes e valores dos parâmetros.

## Criar parâmetros de texto dinâmicos {#creating-dynamic-text-parameters}

Para camadas de texto, também é possível transformar a sequência de texto em um campo dinâmico vinculado a um valor de banco de dados. Siga estas etapas:

1. Na tela Modelo, selecione o botão Parâmetros ao lado do nome da camada de texto para a qual deseja criar parâmetros de texto dinâmicos. A página Parâmetros é aberta.
1. Selecione o **[!UICONTROL On]** opção ao lado do nome do atributo text (textAttr).
1. Selecione o **[!UICONTROL Text]** na tela Parâmetros.
1. Selecionar **[!UICONTROL Add Parameter]**. Um nome de parâmetro padrão é exibido. Você pode substituir esse nome selecionando-o e digitando sobre ele. A sequência de texto atual se torna o novo nome do parâmetro.
1. Selecionar **[!UICONTROL Close]** para fechar a página Parâmetros.

Para fazer com que o nome do parâmetro use um valor de banco de dados, anexe a seguinte string ao URL do Modelo:

```as3
?$_2(parameter name)=(database value)
```

O nome do parâmetro é substituído por nomes em um campo de banco de dados ou código Java™ indicando, por exemplo, o preço atual de um item ou um nome de cliente.
