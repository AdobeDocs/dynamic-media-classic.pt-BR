---
title: Como parametrizar um modelo no Dynamic Media Classic
seo-title: Como parametrizar um modelo no Dynamic Media Classic
description: nulo
seo-description: Saiba como parametrizar um modelo no Dynamic Media Classic
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Como parametrizar um modelo no Dynamic Media Classic{#parameterizing-a-template-in-scene}

Depois de carregar um modelo do Illustrator salvo como Dynamic Media Classic FXG no Scene7 Publishing System, você pode definir seus elementos variáveis. Faça isso parametrizando elementos variáveis nas telas Criação e Visualização da Publicação do Modelo. O Dynamic Media Classic oferece ferramentas para definir parâmetros de texto e objeto em camadas e suas respectivas propriedades. Você também pode criar diferentes versões de um modelo.

A parametrização de um modelo FXG permite personalizar a variabilidade de texto, imagens e gráficos no modelo. Por exemplo, você pode parametrizar uma linha de texto para que os usuários finais possam modificar o texto por meio de uma interface de usuário da Web. É possível definir campos de texto vazios como variáveis para que os usuários finais possam preencher esses campos com texto personalizado. Você também pode parametrizar os atributos e propriedades dos elementos de design na tela Construtor de publicação do modelo do Dynamic Media Classic.

>[!NOTE]
>
>A parametrização do modelo no Dynamic Media Classic não é necessária se você planeja usar a manipulação de DOM.

## Definição de parâmetros em modelos FXG {#defining-parameters-in-fxg-templates}

Siga estas etapas no Dynamic Media Classic para definir parâmetros para um modelo FXG:

1. Na janela Procurar, selecione o arquivo FXG.
1. Clique em **Criar** e escolha Publicação **de** modelo ou clique no botão **Editar** do arquivo.

   A tela Publicação de modelo é aberta.

1. Selecione LRCo\FXG\Welcome_Summit_10 (arquivo FXG) e clique em **Criar** &gt; Publicação **de** modelo.</p>

   ![](assets/wp_fxg_edit.png)

1. No painel Camadas na tela Publicação de modelo, selecione a camada com os elementos que deseja parametrizar.

   >[!NOTE]
   >
   >Clique no ícone de olho ligado e desligado para garantir que você selecione o objeto desejado.

1. No painel Propriedades, clique em um parâmetro na coluna Nome (para parametrizar o texto) ou na coluna Parâmetro (para parametrizar objetos).

   * **Texto** Clique no campo de texto (role até a parte inferior da lista Propriedades para encontrá-lo). A caixa de diálogo Parâmetros é exibida. Selecione o texto que deseja parametrizar e clique em **Adicionar**. É possível criar vários parâmetros a partir da mesma propriedade de texto selecionando partes diferentes do texto e adicionando parâmetros para cada parte. Para alterar o nome do parâmetro, clique nele, insira um novo nome e clique em **Fechar**.

   * **Objetos** Clique em uma caixa na coluna Parâmetro. A caixa de diálogo Editar parâmetro é exibida. Digite um nome e clique em **OK**.
   Para personalizar vários atributos ao mesmo tempo com o mesmo valor, use o mesmo nome de parâmetro para cada atributo. Por exemplo, se o modelo tem um retângulo e uma estrela, você pode digitar `newcolor` como o nome do Parâmetro para o atributo de cor SolidColor de cada um. Sempre que o `newcolor` valor é alterado, tanto o retângulo quanto a estrela são alterados para a nova cor.

1. Especifique um valor padrão para o atributo no campo Valor ou Dados. Defina todas as propriedades do objeto selecionado para especificar a aparência exata que deseja.
1. (Opcional) Repita as etapas 3 a 5 para todos os objetos ou camadas que você deseja parametrizar.
1. Clique em **Salvar** ou **Salvar como**.
1. Clique em **Visualizar** para abrir a janela Visualização FXG e ver os parâmetros criados com seus valores padrão.

## Mostrar ou ocultar um objeto ou camada no modelo FXG {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Objetos e camadas ocultos não são visíveis na visualização ou na saída, mas não são excluídos do arquivo. Você pode torná-los visíveis novamente, conforme desejado. Visibilidade é um atributo que você pode fazer variável. Clicar no ícone de olho ativado ou desativado define o valor padrão para a visibilidade de um objeto ou camada.

1. No painel Objetos, clique no ícone de olho ao lado de um objeto ou nome de camada para ocultá-lo no arquivo.
1. Clique novamente para tornar o objeto visível.

## Criar diferentes versões de um modelo {#create-different-versions-of-a-template}

Você pode editar atributos para criar diferentes versões do modelo para diferentes usos.

Na tela Publicação de modelo, clique em Salvar como para salvar o arquivo como um novo modelo FXG sem substituir o modelo FXG original.

## Uso de texto traçado {#using-stroked-text}

O texto com marcadores é um exemplo de como você pode parametrizar atributos. O Dynamic Media Classic suporta estes recursos de texto traçado:

* Largura do traço
* Padrão de traço tracejado
* Diferentes estilos de junção
* Diferentes estilos de extremidade de cap
* Superimposição de traço
* Manuseio de cores separadas para traçado, incluindo suporte a cores especiais

Esta tabela descreve os atributos que suportam o texto traçado.

| Atributo | Descrição |
|--- |--- |
| s7:fill `<Boolean>`(somente S7FXG) | Especifica se o preenchimento está ativado para texto. O padrão é verdadeiro. |
| s7:stroke `<Boolean>` (apenas S7FXG) | Especifica se o pressionamento está ativado para texto. O padrão é falso. |
| s7:weight `<number>` (somente S7FXG) | Especifica a espessura do traçado do texto em pontos. O padrão é 1 ponto. |
| s7:juntas `<string>` (mitre, arredondada, bisel) (apenas S7FXG) | Especifica o tipo de junção do traçado. O padrão é arredondado. |
| s7:caps `<string>` (none, round, square) (S7FXG apenas) | Especifica o tipo de cap do traçado. O padrão é arredondado. |
| s7:miterLimit `<number>` (somente S7FXG) | Especifica o limite do mitre quando a junção é de mitre para o traçado. O padrão é 4. |
| s7:strokeOverprint `<Boolean>` (somente S7FXG) | Especifica se a superimposição está ativada para traçado. O padrão é falso. |
| s7:strokeColorName (apenas S7FXG) | Igual a s7:colorName, exceto que define o nome da cor para o traçado. |
| s7:strokeColorValue (somente S7FXG) | Igual a s7:colorValue, exceto que define o valor da cor que está sendo usada para o traçado. |
| s7:strokeColorspace (somente S7FXG) | Igual a s7:color space, exceto que define o espaço de cores do traçado. |
| flm:dashPattern `<array>` (apenas S7FXG) | Por padrão, não há padrões para traços e espaços. Este atributo define o padrão de traço/espaço do traçado. O primeiro valor é o traço do traço. A segunda é a diferença entre os traços. É possível estender a matriz para vários valores da mesma maneira, com valores alternativos sendo especificados como traço e intervalo. |

## Uso de texto distorcido {#using-warped-text}

O texto distorcido permite modificar a aparência do texto com efeitos como onda, sinalizador, estiramento e assim por diante.

O texto distorcido é compatível com objetos RichText. O texto pode ser vertical ou horizontal e pode ser texto de ponto, texto de área e texto de tipo em caminho. O objeto de texto inteiro deve ser selecionado antes que o texto distorcido possa ser aplicado.

O texto distorcido pode ser criado no Adobe Illustrator.

Ao distorcer o texto, você pode definir os seguintes atributos:

* Estilo
* Direção
* Curvatura
* Distorção horizontal
* Distorção vertical

Cada atributo contém um conjunto de valores.

| Atributo | Valores | Padrão |
|--- |--- |--- |
| Estilos7:estilowarp | nonearcarcLowerarcUpperarchbulgesHellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | none |
| Direções7:warpDirection | horizontal vertical | horizontal |
| Bordas7:warpBend | -1 a 1 | 0.5 |
| Distorções Horizontais7:distorçãoHorizontalDistorçãoDistorçãoDistorções Horizontais | -1 a 1 | 0 |
| Distorções de círculo7:distorçãoVerticalDistorçãoDistorçãoVertical | -1 a 1 | 0 |

>[!NOTE]
>
>Para `inflate` e `fishEye`, alterar o `s7:warpDirection` sinalizador entre horizontal e vertical não tem efeito na saída.

Para obter mais informações sobre como criar e usar texto distorcido, consulte a documentação do Adobe Illustrator.

>[!MORELIKETHIS]
>
>* [Criar o modelo inicial no Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Carregar arquivos para Publicação de modelo](upload-files-template-publishing.md#upload_files_for_template-publishing)

