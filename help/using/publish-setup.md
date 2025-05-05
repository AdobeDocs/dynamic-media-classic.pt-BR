---
title: Configuração do Publish
description: As configurações do Publish permitem determinar como os ativos são entregues por padrão dos servidores da Adobe Dynamic Media Classic para sites ou aplicativos.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2318'
ht-degree: 0%

---

# Configuração do Publish {#publish-setup}

As configurações da página Configuração do Publish determinam como os ativos são entregues por padrão dos servidores da Adobe Dynamic Media Classic para sites ou aplicativos. Se nenhuma configuração for especificada, o servidor do Adobe Dynamic Media Classic fornecerá um ativo de acordo com uma configuração padrão em uma página de Configuração do Publish. Por exemplo, uma solicitação para fornecer uma imagem que não inclui um atributo de resolução produz uma imagem com a configuração Resolução de objeto padrão na página Servidor de imagens.

Os administradores podem alterar as configurações padrão nas páginas Servidor de imagens, Renderizador de imagens e Vinheta para estabelecer configurações padrão para fornecer ativos dos servidores.

Para abrir as páginas da Instalação do Publish, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]**.

>[!NOTE]
>
>As páginas de configuração do Publish são para desenvolvedores e programadores experientes de sites. O Adobe Dynamic Media Classic presume que os usuários que alteram as configurações nessas páginas estão familiarizados com o Adobe Dynamic Media Classic, os padrões e convenções de protocolo HTTP e a tecnologia básica de geração de imagens.

## Servidor de imagens {#image-server}

A página Servidor de imagens estabelece configurações padrão para fornecer imagens de Servidores de imagens. As configurações estão disponíveis nessas cinco categorias (consulte a própria página Servidor de imagens para obter descrições detalhadas das configurações).

Altere essas configurações somente com a assistência de um suporte técnico da Adobe Dynamic Media Classic.

* **[!UICONTROL Catalog Management]**: essas configurações determinam como o Adobe Dynamic Media Classic e o catálogo interagem. Diferentemente da maioria dos servidores da Web, as chamadas de URL do Dynamic Media Image Server são direcionadas a um arquivo de manifesto ou catálogo, e não a um arquivo de imagem. O arquivo de catálogo (que não deve ser confundido com um eCatalog) contém uma lista de todo o conteúdo publicado no Servidor de imagens. Ele também contém o caminho para cada imagem. Se você tiver uma ID da Digimarc, insira as informações de usuário na seção Informações de usuário da Digimarc.

* **[!UICONTROL Request Attributes]**: essas configurações impõem limites às imagens que podem ser entregues do servidor. Por exemplo, o *máximo* **[!UICONTROL Reply Image Size Limit]** é **[!UICONTROL Width]** 5000 e **[!UICONTROL Height]** 5000.

* **[!UICONTROL Default Request Attributes]**: Essas configurações pertencem à aparência padrão das imagens.

* **[!UICONTROL Common Thumbnail Attributes]**: Essas configurações pertencem à aparência e ao alinhamento padrão das imagens em miniatura.

* **[!UICONTROL Defaults for Catalog Fields]**: essas configurações pertencem à resolução e ao tipo de miniatura padrão das imagens.

* **[!UICONTROL Color Management Attributes]**: estas configurações determinam quais perfis de cores ICC são usados.

* **[!UICONTROL Compatibility Attributes]**: essa configuração permite que parágrafos à esquerda e à direita em camadas de texto sejam tratados como estavam na versão 3.6 para compatibilidade com versões anteriores.

* **[!UICONTROL Localization Support]**: essas configurações permitem gerenciar vários atributos de localidade. Também permite especificar uma sequência de mapa de localidade para que você possa definir quais idiomas deseja suportar para as várias dicas de ferramentas em Visualizadores.

  Por exemplo, se você for uma marca multinacional que vende em diferentes países, é possível garantir que cada país tenha seu próprio Visualizador específico de localidade. Para obter essa funcionalidade, especifique uma string de mapa de local. Em seguida, edite o texto da dica de ferramenta na predefinição do Visualizador. Basta adicionar as cadeias de texto traduzidas para o idioma desejado.

  >[!NOTE]
  > Para configurar as opções de Suporte à Localização, [use o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/br/enterprise/using/support-for-experience-cloud.html) No seu caso de suporte, solicite ajuda para a instalação.

  Para obter mais informações sobre a configuração do **[!UICONTROL Localization Support]**, consulte [Considerações ao configurar a localização de ativos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerações ao configurar a localização de ativos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Se você quiser configurar as opções de Suporte à localização no Adobe Dynamic Media Classic, como o campo Mapa de localidade, [use o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/br/enterprise/using/support-for-experience-cloud.html) No seu caso de suporte, solicite ajuda para a instalação.

Uma maneira comum de usar o Adobe Dynamic Media Classic é gerenciar as imagens do produto em sites de e-Commerce. As empresas internacionais enfrentam o desafio de que os ativos para produtos semelhantes pareçam diferentes de país para país. Geralmente, as diferenças se referem a algumas partes da mídia geral. Resolver essas diferenças copiando todos os ativos para cada um dos países e substituindo apenas as diferenças é um esforço tremendo e contradiz a metáfora do ativo principal individual. Essas diferenças nos recursos podem variar, desde vídeos específicos de cada país com faixas de áudio diferentes até diferenças sutis, mas importantes, em um cabo de alimentação usado com o produto. O Adobe Dynamic Media Classic usa um mecanismo básico de pesquisa. Você define uma ordem de sufixos de ativos que o Servidor de imagens procura, começando pelo local necessário.

#### Como os ativos são localizados

O local de uma solicitação IS (Servidor de imagens) é identificado com o seguinte comando IS/IR (Renderização de imagens):

`locale=`

Este comando aceita uma sequência de caracteres de ID de localidade (locId) que não diferencia maiúsculas de minúsculas. A ID de localidade geralmente é uma cadeia de 2 a 6 caracteres composta por letras e &quot;`_`&quot;.

IS suporta strings ASCII imprimíveis arbitrárias. O comando `locale=` tem um escopo global, o que significa que ele é aplicado a toda a solicitação, incluindo todas as solicitações IS e IR aninhadas, modelos referenciados e camadas de imagem. Não há suporte para várias localidades por solicitação, como uma localidade diferente para cada camada. No entanto, é concebível permitir substituições explícitas em solicitações aninhadas.

Se `locale=` não for especificado, `attribute::DefaultLocale` será passado para os mecanismos de tradução. Validação de entrada limitada aplicada ao valor `locale=`. São permitidos valores `locale=` vazios. Como `locale=` tem um escopo global, `attribute::DefaultLocale` é fornecido pelo catálogo principal para toda a solicitação.

Alguns dos benefícios de usar o `locale=` e o `attribute::DefaultLocale` incluem:

* Compartilhar conteúdo para várias localidades.
* Acesse o conteúdo específico do local usando ids genéricas.
* Permita flexibilidade em convenções de nomenclatura e no gerenciamento de conteúdo específico da localidade, como prefixo de localidade versus sufixo ou conteúdo específico da localidade em um catálogo separado.
* Acesso de suporte a versões específicas do local.
* Objetos agregados, como Conjuntos de imagens, às vezes podem conter referências genéricas a conteúdos potencialmente específicos do local.
* Suporta todo o conteúdo gerenciado por catálogos que precisam de localização, incluindo imagens, Conjuntos de imagens, vinhetas, materiais e registros de configuração do visualizador.
* Minimize as alterações no banco de dados do IPS e nos mecanismos de manifesto do IS.
* O suporte para conteúdo estático, como vídeos e capas, é adicionado quando o RFC IS-63 é implementado.
* O local padrão é configurável.

#### Cenários de aplicação

| Aplicativo | Cenário |
| --- | --- |
| Localização do visualizador | Depois que os catálogos de conteúdo estático são implementados, a localização é controlada totalmente com o parâmetro locale=, anexado a todas as solicitações feitas no IS. Registros de configuração, capas, telas iniciais e assim por diante podem ter variantes específicas do local ou não. O conteúdo correto é fornecido pelo IS sem que o visualizador precise saber qual conteúdo está localizado e quais são suas IDs. |
| Imagens e vídeo | As empresas multinacionais geralmente têm uma combinação de conteúdos genéricos e específicos do local. Com esse mecanismo, uma referência a uma imagem ou vídeo pode ser genérica, e o IS serve o conteúdo específico do local, se disponível. |
| Conjuntos de imagens e conjuntos de mídia | O conjunto de imagens inteiro pode ser diferente para algumas localidades, como quando um eCatalog é diferente, com a tradução de um conjunto de imagens genérico para um conjunto específico de localidade manipulada pelo visualizador. Normalmente, as IDs individuais em um conjunto genérico podem se referir a conteúdos localizados. Por exemplo, a maioria das fotos de um equipamento pode ser a mesma em todos os idiomas, exceto na foto do Painel de controle do Campaign. O é capaz de traduzir IDs automaticamente, de modo que não há necessidade de gerar Conjuntos de imagens específicos do local. |

#### Implementar a localização de ativos

O Adobe Dynamic Media Classic e o Servidor de imagens têm uma interface que permite a localização de imagens e conteúdo estático.

Sem localização, um URL do servidor de imagens é semelhante ao seguinte:

`https://server/is/image/company/image`

Com a localização, uma URL do Servidor de imagens adiciona o parâmetro `locale=` ao caminho, como no exemplo a seguir:

`https://server/is/image/company/image?locale=de_DE`

No recebimento da chamada http pelo Servidor de imagens, o parâmetro `locale=` é analisado por meio do campo `localeMap` encontrado no grupo **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

O campo Mapa de localidade contém uma lista de entradas separadas usando o símbolo da barra vertical (|).

Cada entrada consiste em uma lista de valores separados por vírgulas. O primeiro valor é o valor de pesquisa passado pelo parâmetro `locale=`. Os valores restantes são valores de sufixo/substituição que são tentados até que um resulte em uma imagem existente.

A aplicação de um valor de sufixo ou de um valor de substituição depende da configuração Local Global no grupo **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

>[!NOTE]
>
>A configuração de Local global só é possível ao defini-la por meio da API, não na interface do Adobe Dynamic Media Classic.

**Exemplo de sufixo:**

| URL | IDs do localeMap | Resultado | Notas |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Observe que não há GlobalLocale definido. O parâmetro de localidade de_DE corresponde à primeira entrada no `localeMap`. O primeiro valor _DE correspondente é adicionado como um sufixo ao ativo image_DE e é feita uma tentativa de encontrá-lo no Servidor de imagens. Se encontrado no servidor, é retornado. Caso contrário, o segundo valor &quot;&quot; será usado como um sufixo, resultando na imagem propriamente dita ser retornada. |

**Exemplo de substituição:**

| URL | `GlobalLocale` e `localeMap` IDs | Resultado | Notas |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | No exemplo de substituição acima, GlobalLocale está definido como main. O parâmetro de localidade de_DE corresponde à primeira entrada no `localeMap`. A subcadeia de caracteres GlobalLocale foi encontrada e substituída pelo primeiro valor correspondente `de` em `localeMap`: `image-de-01`. Se for encontrada no Servidor de imagens, ela será retornada. Caso contrário, o segundo valor é substituído, resultando em `image-main-01`. |

Se nenhum local for definido no URL, o Servidor de imagens usará o Local padrão, se estiver definido, e o aplicará ao URL.

Se um parâmetro de localidade desconhecido ou vazio for fornecido com `locale=`, então `localeMap` é verificado para o valor vazio &quot;começando com&quot;. É importante ter um local padrão aplicado para locais desconhecidos.

#### Sobre defaultImage

O Servidor de imagens tenta as opções para o local solicitado, um após o outro. Se nenhuma correspondência for encontrada, as opções de local serão aplicadas a defaultImage e a versão correspondente será retornada. Portanto, cada localidade deve incluir uma opção para a imagem sem localização ou as versões localizadas de defaultImage são disponibilizadas no Adobe Dynamic Media Classic.

#### Cenários para localizar o localeMap

Suponha que você deseja oferecer suporte às seguintes localidades:

`en, en_us, en_uk, de, de_at, de_de, fr`

Você mapeia essas localidades para os sufixos `_E` (inglês), `_G` (alemão) e `_F` (francês). Para todos os exemplos, a ID da imagem de entrada genérica é `myImg`.

##### Comportamento padrão para localizar localeMap

As IDs de localidade são mapeadas para seus sufixos correspondentes. Se nenhuma ID específica da localidade for encontrada no catálogo, a ID genérica será tentada. Observe os valores de locSuffix vazios que são mapeados para a ID genérica.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | IDs de saída para pesquisar |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos os outros | : |

##### Localizar o localeMap quando o locale é desconhecido

Você pode mapear localidades desconhecidas para IDs específicas ou para IDs genéricas. Por exemplo, você pode mapear locais desconhecidos para as IDs em inglês ou, se eles não existirem, para as IDs genéricas.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | IDs de saída para pesquisar |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos os outros | myImg_E, myImg |

Você também pode ter um locSuffix dedicado, tal como U, apenas para localidades desconhecidas, e forçar para a imagem padrão se nenhum `_U` existir, como no seguinte:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou você pode mapear diretamente para a ID genérica, como no seguinte:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Localizar o localeMap usando uma pesquisa de várias camadas

Muitas vezes é desejável agrupar locais, como Europeu, Oriente Médio e América do Norte, para abordar padrões regionais, como a exposição da pele. Você pode obter esse efeito usando uma pesquisa em várias camadas.

Por exemplo, suponha que você queira oferecer suporte a coleções para uso no Oeste e no Oriente Médio. Ambas as coleções se baseiam na coleção de imagens genérica e adicionam ou modificam algumas imagens. Ambas as coleções são então refinadas para localidades específicas. Por exemplo, `m1, m2` para duas variantes do oriente médio e `w1, w2,` e `w3` para três localidades ocidentais, exceto que as imagens são compartilhadas para `w1` e `w3`. Locais desconhecidos são mapeados somente para a coleção genérica e não têm acesso a imagens específicas do local. O mapa seria mostrado a seguir:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | IDs de saída para pesquisar |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Todos os outros | mylmg |

##### Localizar o localeMap procurando IDs específicas

Algumas convenções de nomenclatura de imagem não oferecem suporte a IDs de imagem genéricas. As IDs genéricas da solicitação devem ser mapeadas para uma ID específica no catálogo. No entanto, há instâncias em que a ID específica exata não é conhecida.

Usando o primeiro exemplo como base, imagens para todas as linguagens podem ter os sufixos `_1`, `_2` ou `_3`. Imagens específicas para localidades francesas podem ter os sufixos `_22` ou `_23`. E as imagens específicas para localidades alemãs podem ter os sufixos `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | IDs de saída para pesquisar |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Todos os outros | myImg_1, myImg_2, myImg_3 |

##### Considerações importantes ao implementar o suporte à localização

* A localização é limitada a chamadas de ativos baseadas em ID e não pode ser usada em chamadas de ativos baseadas em caminho. Portanto, ao chamar vídeos com localidade, ele deve ser chamado como company/assetID; sem caminho completo para o vídeo. Você não pode usar `RTMP` com localização porque esse método deve ser usado somente com chamadas de vídeo baseadas em caminho.
* Não é possível usar um Conjunto de mídias mistas que contenha um único vídeo quando o localeMap está ativo, caso contrário, a chamada para o conteúdo do conjunto falhará. Para contornar esse problema, você pode adicionar um único vídeo a um Conjunto de vídeos adaptados. Em seguida, adicione o Conjunto de vídeos adaptados a um Conjunto de mídias mistas.
* Determinadas solicitações não são localizadas, como solicitações para o conteúdo de um Conjunto de vídeos adaptados. Portanto, se você pretende usar Conjuntos de vídeos adaptados com localização, coloque o Conjunto de vídeos adaptados em um Conjunto de mídias mistas. Em seguida, chame o conjunto em um visualizador de Mídia mista com o parâmetro `locale=`.

## Renderizador de imagem {#image-renderer}

A página Renderizador de imagem estabelece configurações padrão para fornecer Conjuntos de imagens de servidores de renderização de imagem. As configurações estão disponíveis nestas cinco categorias (consulte a própria página Servidor de imagens para obter descrições detalhadas das configurações):

* **[!UICONTROL Catalog Management]**: essas configurações determinam como o Adobe Dynamic Media Classic e o arquivo de catálogo interagem. As chamadas de URL do servidor de renderização do Adobe Dynamic Media Classic são feitas para o catálogo, que, por sua vez, chama para fornecer imagens do servidor. Altere essas configurações somente com a assistência de um suporte técnico da Adobe Dynamic Media Classic.

* **[!UICONTROL Session Attributes]**: Essas configurações estabelecem parâmetros de erro, a URL para URLs de imagens relativas e se a sobreposição de objetos é permitida.

* **[!UICONTROL Default Material Attributes]**: Essas configurações estabelecem as configurações padrão de resolução e nitidez de imagens.

* **[!UICONTROL Response Image Attributes]**: Essas configurações pertencem à aparência padrão das imagens.

* **[!UICONTROL Color Management Attributes]**: Essas configurações pertencem às configurações de cores padrão das imagens.

## Vinheta {#vignette}

A página de Vinheta oferece configurações para estabelecer a aparência padrão das vinhetas (consulte a própria página para obter descrições detalhadas das opções).
