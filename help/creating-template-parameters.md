---
title: Criação de parâmetros de modelo
seo-title: Criação de parâmetros de modelo
description: 'null'
seo-description: Saiba como criar parâmetros de modelo.
uuid: d 17168 a 8-4776-4761-b 022-8258 d 5997604
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/template_ basics
discoiquuid: d 263 f 041-5 a 0 d -4 c 4 f -9266-aeff 51 a 5 a 7 e 2
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Criação de parâmetros de modelo{#creating-template-parameters}

Os parâmetros permitem que você use modelos com flexibilidade máxima; permitem personalizar dinamicamente uma imagem de modelo. Você pode decidir quais camadas de texto e imagem devem ser incluídas no modelo e em cada camada, quais parâmetros serão exibidos. Por exemplo, para chamar a atenção para um produto que está à venda, você pode criar uma camada de texto na venda. Posteriormente, você pode remover essa camada, mas ainda reter o restante da imagem do modelo, removendo o parâmetro On Sales.

Ao criar parâmetros de modelo, você declara quais partes do modelo serão chamadas em uma sequência de caracteres de URL. Um URL criado com parâmetros expõe esses itens na string do URL. Com parâmetros expostos, é possível criar resultados personalizados da forma como a imagem do modelo é construída dinamicamente a partir do Servidor de imagens. Dessa forma, é possível alterar um modelo dinamicamente, pois você pode chamar alguns ou todos os parâmetros em um URL.

Em parâmetros de camada de texto, você também pode tornar a sequência de texto um campo dinâmico vinculado a valores em um banco de dados. A capacidade de vincular texto a um banco de dados é útil, por exemplo, em promoções. Você pode personalizar as imagens modelo para que elas mostrem nomes de cliente ou cliente. Por exemplo, você pode vincular um parâmetro de camada de texto a um banco de dados de preços para mostrar o preço de um item em uma imagem de modelo.

Você pode consultar um parâmetro mais de uma vez. Use a caixa de combinação para cada comando na caixa de diálogo do parâmetro para selecionar qualquer parâmetro que corresponda a esse comando específico. (Por exemplo, todos os parâmetros de tamanho estão disponíveis para o tamanho = comando, etc). É possível reatribuir a referência do parâmetro a qualquer parâmetro existente na caixa de combo e renomear a algo que não consta na caixa de combinação. No último caso, o nome deve ser exclusivo. Caso contrário, um erro declara que o parâmetro já existe. Quando uma referência de parâmetro é excluída, o parâmetro é removido do URL se não for referenciado em outro lugar. Quando você alterar o valor padrão para um parâmetro de texto, todas as referências a esse parâmetro serão atualizadas. É possível visualizar a atualização na tabela de camadas, na renderização do modelo e no URL. Ao alterar um atributo de camada manipulando redimensionar alças ou digitar valores no painel de propriedades, o valor do parâmetro será atualizado e todas as referências à atualização do parâmetro serão atualizadas. Por exemplo, se você tiver parâmetros com o tamanho de duas camadas usando um parâmetro, ambos os tamanhos de camada serão atualizados quando qualquer um dos tamanhos de camada for alterado. Quando você visualiza um modelo e altera um parâmetro, todas as referências a esse parâmetro são atualizadas.

## Parâmetro de uma camada {#parameterizing-a-layer}

Para cada camada no modelo, siga estas etapas para criar parâmetros de modelo:

1. Na lista Camadas, selecione o botão Parâmetros ao lado do nome da camada para a qual deseja criar parâmetros. A tela Parâmetros é aberta. Ele lista os nomes de cada parâmetro na camada, seu valor e seu tipo.
1. Selecione a opção Ativar ao lado do nome de cada parâmetro que você deseja incluir na imagem do modelo.
1. Selecione **Fechar** para sair da tela Parâmetros.

>[!NOTE]
>
>É possível renomear parâmetros na tela Parâmetros. Renomear um parâmetro facilita a identificação do parâmetro em sequências de caracteres de URL e facilita a utilização como um valor de banco de dados. Para renomear um parâmetro, selecione a opção Ativado, clique no seu nome e digite um novo nome no campo Nome.

Para ver uma lista dos parâmetros criados para o modelo, selecione o botão Resumo do parâmetro na tela Modelo. A tela Resumo do parâmetro é aberta. Ele lista o nome de cada camada e, caso tenha criado parâmetros para uma camada, os nomes e valores de parâmetros.

## Criação de parâmetros de texto dinâmico {#creating-dynamic-text-parameters}

Para camadas de texto, também é possível tornar a string de texto um campo dinâmico vinculado a um valor de banco de dados. Siga estas etapas:

1. Na tela Modelo, selecione o botão Parâmetros próximo ao nome da camada de texto para a qual deseja criar parâmetros de texto dinâmicos. A tela Parâmetros é aberta.
1. Selecione a opção Ativar ao lado do nome do atributo de texto (textparam).
1. Selecione a guia Texto na tela Parâmetros.
1. Clique no botão Adicionar parâmetro. Um nome de parâmetro padrão aparece. Você pode substituir esse nome selecionando-o e digitando-o sobre ele. A string de texto atual se torna o novo nome do parâmetro.
1. Selecione o botão Fechar para fechar a tela Parâmetros.

Para fazer com que o nome do parâmetro use um valor de banco de dados, acrescente a seguinte sequência à URL do modelo:

```as3
?$_2(parameter name)=(database value)
```

O nome do parâmetro será substituído pelos nomes em um campo de banco de dados ou código Java que indica, por exemplo, o preço atual de um item ou um nome de cliente.
