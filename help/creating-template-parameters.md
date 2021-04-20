---
title: Criação de parâmetros de modelo
description: Saiba como criar parâmetros de modelo.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---


# Criação de parâmetros de modelo{#creating-template-parameters}

Os parâmetros permitem usar modelos com o máximo de flexibilidade; elas permitem personalizar dinamicamente uma imagem de modelo. Você pode decidir quais camadas de texto e imagem devem ser incluídas no modelo e, em cada camada, quais parâmetros devem ser exibidos. Por exemplo, para chamar a atenção para um produto que está à venda, você pode criar uma camada de texto On Sale . Posteriormente, é possível remover essa camada, mas ainda manter o restante da imagem do modelo, removendo o parâmetro Em venda .

Ao criar parâmetros de modelo, você declara quais partes do modelo chamar em uma string de URL. Um URL construído com parâmetros expõe esses itens na string do URL. Com parâmetros expostos, você pode criar resultados personalizados a partir da maneira como a imagem do modelo é construída dinamicamente do Servidor de Imagens. Dessa forma, você pode alterar um modelo dinamicamente, pois pode chamar alguns ou todos os parâmetros em um URL.

Nos parâmetros da camada de texto, também é possível tornar a cadeia de caracteres de texto um campo dinâmico vinculado aos valores em um banco de dados. A capacidade de vincular texto a um banco de dados é útil, por exemplo, em promoções. Você pode personalizar imagens de modelo para fazer com que elas mostrem nomes de clientes ou de clientes. Você também pode, por exemplo, vincular um parâmetro de camada de texto a um banco de dados de preços para mostrar o preço de um item em uma imagem de modelo.

Você pode fazer referência a um parâmetro mais de uma vez. Use a caixa de combinação para cada comando na caixa de diálogo do parâmetro para selecionar qualquer parâmetro que corresponda a esse comando específico. (Por exemplo, todos os parâmetros de tamanho estão disponíveis para o comando size= etc.). Você pode reatribuir a referência do parâmetro a qualquer parâmetro que já esteja na caixa de combinação e renomear para algo que não esteja na caixa de combinação. No último caso, o nome deve ser exclusivo. Caso contrário, um erro indicará que o parâmetro já existe. Quando você exclui uma referência de parâmetro, o parâmetro é removido do URL se não for referenciado em outro lugar. Quando você altera o valor padrão de um parâmetro de texto, todas as referências a esse parâmetro são atualizadas. Você pode ver a atualização na tabela de camadas, na renderização do modelo e na URL. Quando você altera um atributo de camada manipulando alças de redimensionamento ou digitando valores no painel de propriedades, o valor do parâmetro é atualizado e todas as referências ao parâmetro são atualizadas. Por exemplo, se você parametrizou o tamanho de duas camadas usando um parâmetro, ambos os tamanhos de camada são atualizados quando qualquer um dos tamanhos de camada é alterado. Ao visualizar um modelo e alterar um parâmetro, todas as referências a ele são atualizadas.

## Parâmetros de uma camada {#parameterizing-a-layer}

Para cada camada no modelo, siga estas etapas para criar parâmetros do modelo:

1. Na lista Camadas, selecione o botão Parâmetros ao lado do nome da camada para a qual deseja criar parâmetros. A tela Parâmetros é aberta. Ela lista os nomes de cada parâmetro na camada, seu valor e seu tipo.
1. Selecione a opção Ativado ao lado do nome de cada parâmetro que deseja incluir na imagem do modelo.
1. Selecione **Close** para sair da tela Parâmetros.

>[!NOTE]
>
>Você pode renomear parâmetros na tela Parâmetros. Renomear um parâmetro facilita a identificação do parâmetro em cadeias de caracteres de URL e o uso mais fácil como um valor de banco de dados. Para renomear um parâmetro, selecione a opção Ativado , clique em seu nome e insira um novo nome no campo Nome .

Para ver uma lista dos parâmetros criados para o modelo, selecione o botão Resumo dos parâmetros na tela Modelo. A tela Resumo dos parâmetros é aberta. Ela lista o nome de cada camada e, se você tiver criado parâmetros para uma camada, os nomes e valores dos parâmetros.

## Criação de parâmetros de texto dinâmicos {#creating-dynamic-text-parameters}

Para camadas de texto, também é possível tornar a cadeia de caracteres de texto um campo dinâmico vinculado a um valor de banco de dados. Siga estas etapas:

1. Na tela Modelo , selecione o botão Parâmetros ao lado do nome da camada de texto para a qual deseja criar parâmetros de texto dinâmicos. A tela Parâmetros é aberta.
1. Selecione a opção Ativado ao lado do nome do atributo de texto (textAttr).
1. Selecione a guia Texto na tela Parâmetros.
1. Clique no botão Adicionar parâmetro . Um nome de parâmetro padrão é exibido. Você pode substituir esse nome selecionando-o e digitando sobre ele. A string de texto atual se torna o novo nome do parâmetro.
1. Selecione o botão Fechar para fechar a tela Parâmetros.

Para fazer com que o nome do parâmetro use um valor de banco de dados, anexe a seguinte string ao URL do modelo:

```as3
?$_2(parameter name)=(database value)
```

O nome do parâmetro será substituído por nomes em um campo de banco de dados ou código Java indicando, por exemplo, o preço atual de um item ou nome de cliente.
