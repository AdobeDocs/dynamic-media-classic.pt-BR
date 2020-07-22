---
title: Configuração de publicação
seo-title: Configuração de publicação
description: nulo
seo-description: As configurações da tela Publicar configuração determinam como os ativos são entregues por padrão dos servidores Dynamic Media Classic para sites ou aplicativos.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# Configuração de publicação {#publish-setup}

As configurações da tela Publicar configuração determinam como os ativos são entregues por padrão dos servidores Dynamic Media Classic para sites ou aplicativos. Se nenhuma configuração for especificada, o servidor Dynamic Media Classic fornecerá um ativo de acordo com uma configuração padrão em uma tela de configuração de publicação. Por exemplo, uma solicitação para fornecer uma imagem que não inclui um atributo de resolução gera uma imagem com a configuração Resolução de objeto padrão na tela Servidor de imagens.

Os administradores podem alterar as configurações padrão nas telas Servidor de imagens, Renderizador de imagens e Vignette para estabelecer as configurações padrão para fornecer ativos dos servidores.

Para abrir as telas Instalação de publicação, clique em Configuração > Configuração do aplicativo > Configuração de publicação.

>[!NOTE]
>
>As telas de configuração de publicação são para uso por desenvolvedores e programadores experientes do site. O Dynamic Media Classic supõe que os usuários que mudam as configurações nessas telas estejam familiarizados com o Dynamic Media Classic, os padrões e convenções de protocolo HTTP e a tecnologia básica de geração de imagens.

## Servidor de imagens {#image-server}

A tela Servidor de imagens estabelece as configurações padrão para a entrega de imagens dos servidores de imagens. As configurações estão disponíveis nessas cinco categorias (consulte a tela do Servidor de imagens para obter descrições detalhadas das configurações).

Altere essas configurações somente com a ajuda de um suporte do Dynamic Media Classic.

**Gerenciamento** de catálogo Essas configurações determinam como o Dynamic Media Classic e o catálogo interagem. Ao contrário da maioria dos servidores da Web, as chamadas de URL do Dynamic Media Image Server vão para um arquivo manifest-or de catálogo em vez de um arquivo de imagem propriamente dito. O arquivo de catálogo (não confundir com um eCatalog) contém uma lista de todo o conteúdo publicado no servidor de imagem juntamente com o caminho para cada imagem. Se você tiver uma ID Digimarc, insira as informações do usuário na seção Informações do usuário Digimarc.

**Atributos** de solicitação Essas configurações impõem limites às imagens que podem ser entregues do servidor.

**Atributos** de solicitação padrão Essas configurações pertencem à aparência padrão das imagens.

**Atributos** de miniatura comuns Essas configurações pertencem à aparência padrão e ao alinhamento das imagens em miniatura.

**Padrões para campos** de catálogo Essas configurações pertencem à resolução e ao tipo de miniatura padrão das imagens.

**Atributos** de gerenciamento de cores Essas configurações determinam quais perfis de cor ICC são usados.

**Atributos** de compatibilidade Essa configuração permite que os parágrafos à esquerda e à direita em camadas de texto sejam tratados como na versão 3.6 para compatibilidade com versões anteriores.

**Suporte** à Localização Essas configurações permitem gerenciar vários atributos de localidade. Ela também permite que você especifique uma string de mapa de localidade para que você possa definir quais idiomas deseja suportar para as várias dicas de ferramentas nos Visualizadores.

Por exemplo, se você for uma marca multinacional que vende em diferentes países, é possível garantir que cada país tenha seu próprio Visualizador específico para localidades. Para realizar essa funcionalidade, especifique uma string de mapa de localidade. Em seguida, edite o texto da dica de ferramenta em uma predefinição do Visualizador adicionando as strings de texto traduzidas para o idioma desejado.

>[!NOTE]
> Para configurar as opções de suporte à Localização, entre em contato com o suporte técnico do Adobe Dynamic Media Classic ou envie um email para s7support@adobe.com solicitando ajuda de configuração.

Para obter mais informações sobre como configurar o suporte **à** Localização, consulte [Considerações ao configurar a localização de ativos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerações ao configurar a localização de ativos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Se você quiser configurar opções de suporte à Localização no Dynamic Media Classic, como o campo Mapa de localidade, entre em contato com o Suporte técnico do Adobe Dynamic Media Classic. Ou envie um email para s7support@adobe.com solicitando ajuda para a configuração.

Uma maneira comum de usar o Dynamic Media Classic é gerenciar a imagem do produto em sites de comércio eletrônico. As empresas internacionais enfrentam o desafio de que os ativos para produtos similares pareçam diferentes de país para país. Normalmente, as diferenças são para uma parte muito pequena da mídia geral. Abordar essas diferenças copiando todos os ativos para cada um dos países e sobrescrevendo apenas as diferenças é um tremendo esforço e contradiz a única metáfora principal dos ativos. Tais diferenças para ativos podem durar, desde vídeos específicos do país com diferentes faixas de áudio, até diferenças sutis, mas importantes, em um cabo de alimentação que é usado com o produto. O Dynamic Media Classic usa um mecanismo de pesquisa básico. Você define uma ordem de sufixos de ativos na qual o Servidor de imagens está olhando, começando pela localidade desejada.

**Como os ativos são localizados**

A localidade de uma solicitação IS (Image Serving) é identificada com o seguinte comando IS/IR (Image Rendering):

`locale=`

Este comando aceita uma cadeia de caracteres de ID de localidade (locId) que não diferencia maiúsculas de minúsculas. Normalmente, a ID de localidade é uma string de 2 a 6 caracteres composta por letras e &quot;_&quot;.

O IS oferece suporte a strings ASCII imprimíveis arbitrárias.O `locale=` comando tem um escopo global, o que significa que é aplicado a toda a solicitação, incluindo todas as solicitações IS e IR aninhadas, modelos referenciados e camadas de imagem. Não há suporte para várias localidades por solicitação, como uma localidade diferente para cada camada. No entanto, é possível permitir substituições explícitas em solicitações aninhadas.

Se não `locale=` for especificado, `attribute::DefaultLocale` será passado para os mecanismos de conversão. A validação de entrada limitada é aplicada ao `locale=` valor. São permitidos `locale=` valores vazios. Como `locale=` tem um escopo global, `attribute::DefaultLocale` é fornecido pelo catálogo principal para toda a solicitação.

Alguns dos benefícios do uso `locale=` e `attribute::DefaultLocale` incluem:

* Compartilhe conteúdos para várias localidades.
* Acesse conteúdos específicos da localidade usando IDs genéricas.
* Permita flexibilidade para nomear convenções e o gerenciamento de conteúdo específico da localidade, como prefixo da localidade versus sufixo, ou conteúdo específico da localidade em um catálogo separado.
* Suporte ao acesso direto a versões específicas da localidade.
* Objetos de Agregação, como conjuntos de imagens, podem conter referências genéricas a conteúdos potencialmente específicos para localidades.
* Suporta todo o conteúdo gerenciado por catálogos que podem precisar de localização, incluindo imagens, conjuntos de imagens, vinhetas, materiais e registros de configuração do visualizador.
* Minimize as alterações no banco de dados IPS e nos mecanismos de manifesto IS.
* O suporte para conteúdo estático, como vídeos e capas, será adicionado quando o RFC IS-63 for implementado.
* A localidade padrão é configurável.

**Cenários de aplicativo**

| Aplicativo | Cenário |
|--- |--- |
| localização do visualizador | Depois que os catálogos de conteúdo estático são implementados, a localização é controlada inteiramente com o parâmetro locale=, anexado a todas as solicitações feitas ao IS. Registros de configuração, capas, telas de apresentação e assim por diante podem ter variantes específicas da localidade ou não. O conteúdo correto é fornecido pelo IS sem que o visualizador precise saber qual conteúdo está localizado e quais são suas IDs. |
| Imagens e vídeo | Muitas vezes, as empresas multinacionais têm uma mistura de conteúdos genéricos e locais específicos. Com esse mecanismo, uma referência a uma imagem ou vídeo pode ser genérica e o IS serve o conteúdo específico da localidade, se disponível. |
| Conjuntos de imagens e conjuntos de mídia | O conjunto de imagens inteiro pode ser diferente para algumas localidades, como quando um eCatalog é completamente diferente, com a tradução de um genérico para um conjunto de imagens específico da localidade manipulado pelo visualizador.Mais comumente, as IDs individuais em um conjunto genérico podem se referir ao conteúdo localizado. Por exemplo, a maioria das fotos de um equipamento pode ser a mesma em todos os idiomas, exceto na foto do painel de controle. O IS traduz IDs automaticamente, portanto não há necessidade de gerar conjuntos de imagens específicos para localidades. |

**Implementação da localização de ativos**

O Dynamic Media Classic e o Image Server têm uma interface que permite localizações de imagens e conteúdo estático.

Sem localização, um URL do Servidor de imagens é semelhante ao seguinte:

`https://server/is/image/company/image`

Com a localização, um URL do Servidor de imagens adiciona o `locale=` parâmetro ao caminho, como a seguir:

`https://server/is/image/company/image?locale=de_DE`

Ao receber a chamada http pelo Servidor de imagens, o `locale=` parâmetro é analisado pelo campo localeMap encontrado em **Configuração** > Configuração **do** aplicativo > Configuração **** de publicação > Servidor **de** imagens > Grupo de suporte à **** Localização.

O campo Mapa de localidade contém uma lista de entradas que são separadas usando o símbolo de barra vertical (|).

Cada entrada consiste em uma lista de valores separada por vírgulas. O primeiro valor é o valor de pesquisa transmitido pelo `locale=` parâmetro. Os valores restantes são valores de sufixo/substituição que são tentados subsequentemente até que um resulte em uma imagem existente.

Se um valor de sufixo ou um valor de substituição for aplicado depende da configuração Local global em **Configuração** > Configuração **** do aplicativo > Configuração **de** publicação > Servidor **de** imagem > Grupo de suporte **à** Localização.

>[!NOTE]
>
>A configuração Local global só é possível no momento quando você a define pela API, e não pela interface do Dynamic Media Classic.

**Exemplo de sufixo**

| URL | localeMap IDs | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observe que não há nenhum GlobalLocale definido. O parâmetro de localidade de_DE corresponde à primeira entrada no localeMap. O primeiro valor correspondente _DE é adicionado como um sufixo ao asset image_DE e é feita uma tentativa de encontrá-lo no Image Server. Se for encontrado no servidor, ele será retornado. Caso contrário, o segundo valor &quot;&quot; será usado como um sufixo, resultando no retorno da própria imagem. |

**Exemplo de substituição**

| URL | IDs GlobalLocale e localeMap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | No exemplo de substituição acima, GlobalLocale é definido como main. O parâmetro de localidade de_DE corresponde à primeira entrada no localeMap. A substring GlobalLocale é encontrada e substituída pelo primeiro valor correspondente de no localeMap: image-de-01. Se for encontrado no Servidor de imagens, ele será retornado. Caso contrário, o segundo valor será substituído, resultando em image-main-01. |

Se nenhuma localidade estiver definida no URL, o Servidor de imagens pega a Localidade padrão, se estiver definida, e a aplica ao URL.

Se um parâmetro de localidade desconhecido ou vazio for fornecido com `locale=`, o localeMap será verificado em busca do valor vazio &quot;começando com&quot;. É importante configurar esta opção para que tenha uma localidade padrão aplicada a localidades desconhecidas.

**Sobre o defaultImage**

O Servidor de imagens tenta as opções para a localidade solicitada, uma após a outra. Se nenhuma correspondência for encontrada, as opções de localidade serão aplicadas à defaultImage e a versão correspondente será retornada. Portanto, cada localidade deve incluir uma opção para a imagem sem localização, ou as versões de imagem padrão localizadas devem ser disponibilizadas no Dynamic Media Classic.

**Cenários para localizar o localeMap**

Suponha que você queira suportar as seguintes localidades:

`en, en_us, en_uk, de, de_at, de_de, fr`

Você mapeia essas localidades para os sufixos `_E`, `_G`e `_F`, para inglês, alemão e francês, respectivamente. Para todos os exemplos, a ID de imagem de entrada genérica é `myImg`.

*Comportamento padrão para localizar localeMap*

As IDs de localidade são mapeadas para seus sufixos correspondentes. Se nenhuma ID específica da localidade for encontrada no catálogo, a ID genérica será tentada. Observe os valores locSuffix vazios que mapeiam para a ID genérica.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | IDs de saída para pesquisar |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos os outros | - |

*Encontrar o localeMap quando a localidade é desconhecida*

Você pode mapear localidades desconhecidas para IDs específicas ou para IDs genéricas. No nosso exemplo, é possível mapear localidades desconhecidas para as IDs em inglês ou, se elas não existirem, para as IDs genéricas.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | IDs de saída para pesquisar |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos os outros | myImg_E,myImg |

Você também pode ter um locSuffix dedicado, como U, apenas para localidades desconhecidas, e forçar para a imagem padrão se não `_U` existir, como a seguir:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou você pode mapear diretamente para a ID genérica, como a seguir:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Como localizar o localeMap usando uma pesquisa em várias camadas*

Muitas vezes, é desejável agrupar localidades, como a Europa, o Oriente Médio e a América do Norte, para atender a padrões regionais, como a exposição da pele. Você pode atingir esse efeito usando uma pesquisa em várias camadas.

Para este exemplo, suponha que você queira suportar coleções para uso no Oriente Médio e Ocidental. Ambas as coleções são baseadas na coleção de imagens genérica e ambas adicionam ou modificam algumas imagens. Ambas as coleções são posteriormente refinadas para localidades específicas, como `m1, m2` para duas variantes do Oriente Médio, e `w1, w2,` e `w3` para três localidades Ocidentais, exceto que as imagens são compartilhadas para `w1` e `w3`. As localidades desconhecidas são mapeadas apenas para a coleção genérica e não têm acesso a imagens específicas da localidade. A seguir está o mapa:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | IDs de saída para pesquisar |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Todos os outros | mylmg |

*LocaleMap ao procurar IDs específicas*

Algumas convenções de nomenclatura de imagem podem não suportar IDs de imagem genéricas. As IDs genéricas da solicitação devem ser mapeadas para uma ID específica no catálogo. No entanto, pode haver casos em que a ID específica exata não seja conhecida.

Usando o primeiro exemplo como base, as imagens para todos os idiomas podem ter os sufixos `_1`, `_2`ou `_3`. As imagens que são específicas para localidades francesas podem ter os sufixos `_22` ou o `_23` sufixo. E as imagens que são específicas para localidades alemãs podem ter os sufixos `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | IDs de saída para pesquisar |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Todos os outros | myImg_1, myImg_2, myImg_3 |

**Considerações importantes ao implementar o suporte à localização**

* A Localização é limitada a chamadas de ativos baseadas em ID e não pode ser usada em chamadas de ativos baseadas em caminho. Portanto, ao chamar vídeos com a localidade, eles devem ser chamados de empresa/assetID; nenhum caminho completo para o vídeo. Isso significa que você não pode usar rtmp com localização, pois esse método é usado somente com chamadas de vídeo baseadas em caminho.
* Não é possível usar um Conjunto de mídia mista que contenha um único vídeo quando localeMap está ativo, caso contrário, a chamada para o conteúdo do conjunto falhará. Para contornar esse problema, adicione um único vídeo a um Conjunto de vídeos adaptáveis. Em seguida, adicione o Conjunto de vídeos adaptáveis a um Conjunto de mídia mista.
* Determinadas solicitações não estão localizadas, como solicitações para o conteúdo de um Conjunto de vídeos adaptáveis. Portanto, se você pretende usar Conjuntos de vídeo adaptáveis com localização, você deve colocar o Conjunto de vídeos adaptáveis em um Conjunto de mídia mista. Em seguida, chame o conjunto para um visualizador de Mídia mista com o `locale=` parâmetro.

## Renderizador de imagem {#image-renderer}

A tela do renderizador de imagens estabelece as configurações padrão para fornecer Conjuntos de imagens dos servidores de renderização de imagens. As configurações estão disponíveis nessas cinco categorias (consulte a tela do Servidor de imagens para obter descrições detalhadas das configurações):

**Gerenciamento** de catálogo Essas configurações determinam como o Dynamic Media Classic e o arquivo de catálogo interagem. As chamadas de URL do Dynamic Media Classic Render Server são feitas no catálogo, que, por sua vez, chama para fornecer imagens do servidor. Altere essas configurações somente com a ajuda de uma pessoa de suporte do Dynamic Media Classic.

**Atributos** da sessão Essas configurações estabelecem parâmetros de erro, o URL para URLs de imagem relativos e se a sobreposição de objetos é permitida.

**Atributos** de material padrão Essas configurações estabelecem a resolução padrão e as configurações de nitidez das imagens.

**Atributos** de imagem de resposta Essas configurações pertencem à aparência padrão das imagens.

**Atributos** de gerenciamento de cores Essas configurações pertencem às configurações de cores padrão das imagens.

## Vinheta {#vignette}

A tela Vinheta oferta as configurações para estabelecer a aparência padrão das vinhetas (consulte a própria tela para obter descrições detalhadas das opções).
