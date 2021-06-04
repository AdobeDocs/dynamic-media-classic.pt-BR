---
title: Configuração de publicação
description: As configurações de Configuração de publicação permitem determinar como os ativos são entregues por padrão dos servidores Dynamic Media Classic em sites ou aplicativos da Web.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Administrator
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
source-git-commit: 35c62fb1f4f136c06ccfbfd80f918462e839d931
workflow-type: tm+mt
source-wordcount: '2374'
ht-degree: 0%

---

# Publicar configuração {#publish-setup}

As configurações da página Publicar configuração determinam como os ativos são entregues por padrão dos servidores Dynamic Media Classic para sites ou aplicativos da Web. Se nenhuma configuração for especificada, o servidor do Dynamic Media Classic fornecerá um ativo de acordo com uma configuração padrão em uma página de Configuração de publicação. Por exemplo, uma solicitação para fornecer uma imagem que não inclua um atributo de resolução gera uma imagem com a configuração de Resolução de objeto padrão na página Servidor de imagem.

Os administradores podem alterar as configurações padrão nas páginas Servidor de imagem, Renderizador de imagem e Vinheta para estabelecer configurações padrão para o fornecimento de ativos dos servidores.

Para abrir as páginas de Configuração de publicação, clique em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]**.

>[!NOTE]
>
>As páginas de Configuração da publicação são para uso por desenvolvedores e programadores de sites experientes. O Dynamic Media Classic presume que os usuários que alteram configurações nessas páginas estejam familiarizados com o Dynamic Media Classic, padrões e convenções de protocolo HTTP e tecnologia básica de geração de imagens.

## Servidor de imagem {#image-server}

A página Servidor de imagens estabelece as configurações padrão para o fornecimento de imagens de servidores de imagens. As configurações estão disponíveis nessas cinco categorias (consulte a própria página Servidor de imagens para obter descrições detalhadas das configurações).

Altere essas configurações somente com a assistência de uma pessoa de suporte do Dynamic Media Classic.

* **Gerenciamento de catálogo**  - Essas configurações determinam como o Dynamic Media Classic e o catálogo interagem. Ao contrário da maioria dos servidores da Web, as chamadas de URL do servidor de imagem da Dynamic Media vão para um arquivo manifest-ou de catálogo, em vez de para um arquivo de imagem adequado. O arquivo de catálogo (não confundir com um eCatalog) contém uma lista de todo o conteúdo publicado no servidor de imagem junto com o caminho para cada imagem. Se você tiver uma ID da Digimarc, insira as informações do usuário na seção Informações do usuário da Digimarc .

* **Atributos de solicitação**  - essas configurações impõem limites às imagens que podem ser entregues a partir do servidor. Por exemplo, o *máximo* **[!UICONTROL Reply Image Size Limit]** é **[!UICONTROL Width]** 5000 e **[!UICONTROL Height]** 5000.

* **Atributos de solicitação padrão**  - Essas configurações pertencem à aparência padrão das imagens.

* **Atributos de miniatura comuns**  - Essas configurações pertencem à aparência padrão e ao alinhamento de imagens de miniatura.

* **Padrões para campos de catálogo**  - Essas configurações pertencem à resolução e ao tipo de miniatura padrão de imagens.

* **Atributos de gerenciamento de cores**  - Essas configurações determinam quais perfis de cores ICC são usados.

* **Atributos de compatibilidade**  - Essa configuração permite que parágrafos anteriores e posteriores em camadas de texto sejam tratados como na versão 3.6 para compatibilidade com versões anteriores.

* **Suporte à localização**  - Essas configurações permitem gerenciar vários atributos de localidade. Ela também permite especificar uma sequência de mapa de localidade para que você possa definir quais idiomas deseja suportar para as várias dicas de ferramentas em Visualizadores.

   Por exemplo, se você for uma marca multinacional que vende em diferentes países, é possível garantir que cada país tenha seu próprio Visualizador específico da localidade. Para realizar essa funcionalidade, especifique uma string de mapa de localidade. Em seguida, edite o texto da dica de ferramenta em uma predefinição do Visualizador, adicionando as sequências de texto traduzidas para o idioma desejado.

   >[!NOTE]
   > Para configurar as opções de Suporte de localização, [use o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) No seu caso de suporte, solicite ajuda para a configuração.

   Para obter mais informações sobre como configurar o **Suporte de localização**, consulte [Considerações ao configurar a localização de ativos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerações ao configurar a localização de ativos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Se você quiser configurar as opções de Suporte de localização no Dynamic Media Classic, como o campo Mapa de localidade , [use o Admin Console para criar um caso de suporte.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) No seu caso de suporte, solicite ajuda para a configuração.

Uma maneira comum de usar o Dynamic Media Classic é gerenciar a imagem do produto em sites de comércio eletrônico. As empresas internacionais enfrentam o desafio de que os ativos para produtos similares pareçam diferentes de país para país. Normalmente, as diferenças são para algumas partes da mídia geral. Enfrentar essas diferenças copiando todos os ativos para cada um dos países e sobrescrevendo apenas as diferenças é um tremendo esforço e contradiz a metáfora única de ativos principais. Essas diferenças para os ativos podem durar, desde vídeos específicos do país com diferentes faixas de áudio, até diferenças sutis, mas importantes, em um cabo de alimentação usado com o produto. O Dynamic Media Classic usa um mecanismo de pesquisa básico. Você define uma ordem de sufixos de ativos na qual o Servidor de imagens está procurando, começando pelo local necessário.

#### Como os ativos são localizados

A localidade de uma solicitação IS (Image Serving) é identificada com o seguinte comando IS/IR (Image Rendering):

`locale=`

Esse comando aceita uma sequência de caracteres de ID de localidade (locId) que não diferencia maiúsculas de minúsculas. Normalmente, o ID da localidade é uma string de 2 a 6 caracteres composta por letras e &quot;_&quot;.

O IS suporta cadeias ASCII imprimíveis arbitrariamente. O comando `locale=` tem um escopo global, o que significa que ele é aplicado a toda a solicitação, incluindo todas as solicitações IS e IR aninhadas, modelos referenciados e camadas de imagem. Várias localidades por solicitação, como uma localidade diferente para cada camada, não são suportadas. No entanto, é concebível permitir substituições explícitas em solicitações aninhadas.

Se `locale=` não for especificado, `attribute::DefaultLocale` será passado para os mecanismos de tradução. A validação de entrada limitada é aplicada ao valor `locale=`. Valores vazios `locale=` são permitidos. Como `locale=` tem um escopo global, `attribute::DefaultLocale` é fornecido pelo catálogo principal para toda a solicitação.

Alguns dos benefícios de usar `locale=` e `attribute::DefaultLocale` incluem o seguinte:

* Compartilhar conteúdo para várias localidades.
* Acesse conteúdo específico da localidade usando ids genéricas.
* Permita flexibilidade em torno de convenções de nomenclatura e do gerenciamento de conteúdo específico de localidades, como prefixo de localidade versus sufixo, ou conteúdo específico de localidade em um catálogo separado.
* Suporte ao acesso a versões específicas do local.
* Objetos agregados, como conjuntos de imagens, às vezes podem conter referências genéricas a conteúdos potencialmente específicos da localidade.
* Suporta todo o conteúdo gerenciado por catálogos que precisam de localização, incluindo imagens, conjuntos de imagens, vinhetas, materiais e registros de configuração do visualizador.
* Minimize as alterações no banco de dados IPS e nos mecanismos de manifesto IS.
* O suporte para conteúdo estático, como vídeos e capas, é adicionado quando o RFC IS-63 é implementado.
* A localidade padrão é configurável.

#### Cenários do aplicativo

| Aplicativo | Cenário |
|--- |--- |
| Localização do visualizador | Depois que os catálogos de conteúdo estático são implementados, a localização é controlada inteiramente com o parâmetro locale=, anexado a todas as solicitações feitas ao IS. Registros de configuração, capas, telas iniciais e assim por diante podem ter variantes específicas da localidade ou não. O conteúdo correto é fornecido pelo IS, sem que o visualizador precise saber qual conteúdo está localizado e quais são suas IDs. |
| Imagens e vídeo | As empresas multinacionais têm frequentemente uma combinação de conteúdos genéricos e específicos para cada localidade. Com esse mecanismo, uma referência a uma imagem ou vídeo pode ser genérica e o IS serve o conteúdo específico da localidade, se estiver disponível. |
| Conjuntos de imagens e Conjuntos de mídia | O conjunto de imagens inteiro pode ser diferente para algumas localidades, como quando um eCatalog é diferente, com a tradução de um genérico para um conjunto de imagens específico da localidade manipulado pelo visualizador. Mais comumente, as IDs individuais em um conjunto genérico podem se referir a conteúdos localizados. Por exemplo, a maioria das fotos de um equipamento pode ser a mesma em todos os idiomas, exceto a foto do Painel de controle do Campaign. O IS traduz IDs automaticamente, de modo que não há necessidade de gerar conjuntos de imagens específicos para localidades. |

#### Implementação da localização de ativos

O Dynamic Media Classic e o Image Serving têm uma interface que permite a localização de imagens e conteúdo estático.

Sem localização, um URL de servidor de imagem tem a seguinte aparência:

`https://server/is/image/company/image`

Com a localização, um URL de servidor de imagem adiciona o parâmetro `locale=` ao caminho, como no seguinte:

`https://server/is/image/company/image?locale=de_DE`

Ao receber a chamada http pelo Servidor de imagem, o parâmetro `locale=` é analisado pelo campo localeMap encontrado no grupo **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

O campo Mapa de localidade contém uma lista de entradas que são separadas usando o símbolo da barra vertical (|).

Cada entrada consiste em uma lista de valores separada por vírgulas. O primeiro valor é o valor de pesquisa passado pelo parâmetro `locale=`. Os valores restantes são valores de sufixo/substituição que são tentados até que um resulte em uma imagem existente.

Se um valor de sufixo ou um valor de substituição for aplicado depende da configuração Local Global em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

>[!NOTE]
>
>A configuração Local global só é possível ao defini-la por meio da API, não dentro da interface do Dynamic Media Classic.

**Exemplo de sufixo:**

| URL | localeMap IDs | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observe que não há um GlobalLocale definido. O parâmetro de localidade de_DE corresponde à primeira entrada no localeMap. O primeiro valor correspondente _DE é adicionado como um sufixo ao asset image_DE e é feita uma tentativa de encontrá-lo no Servidor de imagens. Se for encontrado no servidor, ele será retornado. Caso contrário, o segundo valor &quot; é usado como um sufixo, resultando no retorno da própria imagem. |

**Exemplo de substituição:**

| URL | IDs do GlobalLocale e do LocaleMap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | No exemplo de substituição acima, GlobalLocale é definido como main. O parâmetro de localidade de_DE corresponde à primeira entrada no localeMap. A substring GlobalLocale é encontrada e substituída pelo primeiro valor correspondente `de` no localeMap: `image-de-01`. Se for encontrado no Servidor de imagem, ele será retornado. Caso contrário, o segundo valor será substituído, resultando em `image-main-01`. |

Se nenhuma localidade estiver definida no URL, o Servidor de imagem pega a DefaultLocale, se estiver definida, e a aplica ao URL.

Se um parâmetro de local desconhecido ou vazio for fornecido com `locale=`, o localeMap será verificado para procurar o valor vazio &quot;começando com&quot;. É importante ter uma localidade padrão aplicada para localidades desconhecidas.

#### Sobre defaultImage

O Servidor de Imagens tenta as opções para a localidade solicitada, uma após a outra. Se nenhuma correspondência for encontrada, as opções de local serão aplicadas a defaultImage e a versão correspondente será retornada. Portanto, cada localidade deve incluir uma opção para a imagem sem localização ou as versões de defaultImage localizadas são disponibilizadas no Dynamic Media Classic.

#### Cenários para localizar o localeMap

Suponha que você deseja oferecer suporte às seguintes localidades:

`en, en_us, en_uk, de, de_at, de_de, fr`

Você mapeia essas localidades para os sufixos `_E`, `_G` e `_F`, para inglês, alemão e francês, respectivamente. Para todos os exemplos, a ID da imagem de entrada genérica é `myImg`.

##### Comportamento padrão para localizar o localeMap

As IDs de localidade são mapeadas para seus sufixos correspondentes. Se nenhuma ID específica da localidade for encontrada no catálogo, a ID genérica será tentada. Observe os valores de locSuffix vazios que são mapeados para a ID genérica.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | IDs de saída a serem pesquisadas |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Todos os outros | - |

##### LocaleMap quando a localidade é desconhecida

Você pode mapear localidades desconhecidas para IDs específicas ou para IDs genéricas. Por exemplo, você pode mapear localidades desconhecidas para IDs em inglês ou, se elas não existirem, para as IDs genéricas.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | IDs de saída a serem pesquisadas |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Todos os outros | myImg_E,myImg |

Você também pode ter um locSuffix dedicado, como U, apenas para localidades desconhecidas, e forçar para a imagem padrão se nenhum `_U` existir, como no seguinte:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou você pode mapear diretamente para a ID genérica, como no seguinte:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Encontrar o localeMap usando uma pesquisa em várias camadas

Geralmente é desejável agrupar localidades, como a Europa, o Oriente Médio e a América do Norte, para atender aos padrões regionais, como a exposição da pele. Você pode obter esse efeito usando uma pesquisa em várias camadas.

Neste exemplo, suponhamos que você queira oferecer suporte a coleções para uso do Oeste e do Oriente Médio. Ambas as coleções são baseadas na coleção de imagens genérica e ambas adicionam ou modificam algumas imagens. Ambas as coleções são posteriormente refinadas para localidades específicas, como `m1, m2` para duas variantes do Oriente Médio, e `w1, w2,` e `w3` para três localidades Ocidentais, exceto que as imagens são compartilhadas para `w1` e `w3`. Localidades desconhecidas são mapeadas somente para a coleção genérica e não têm acesso a imagens específicas de localidade. O mapa a seguir seria:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | IDs de saída a serem pesquisadas |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Todos os outros | mylmg |

##### LocaleMap ao pesquisar por IDs específicas

Algumas convenções de nomenclatura de imagem não suportam IDs de imagem genéricas. As IDs genéricas da solicitação devem ser mapeadas para uma ID específica no catálogo. No entanto, há instâncias em que a ID específica exata não é conhecida.

Usando o primeiro exemplo como base, as imagens para todos os idiomas podem ter os sufixos `_1`, `_2` ou `_3`. As imagens específicas às localidades francesas podem ter os sufixos `_22` ou `_23`. E as imagens específicas para localidades alemãs podem ter os sufixos `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | IDs de saída a serem pesquisadas |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2, myImg_3 |
| Todos os outros | myImg_1, myImg_2, myImg_3 |

##### Considerações importantes ao implementar o suporte de localização

* A localização é limitada a chamadas de ativos com base em ID e não pode ser usada em chamadas de ativos com base em caminho. Portanto, ao chamar vídeos com a localidade, eles devem ser chamados de company/assetID; nenhum caminho completo para o vídeo. Não é possível usar o rtmp com localização, pois esse método é para ser usado somente com chamadas de vídeo baseadas em caminho.
* Não é possível usar um Conjunto de mídias mistas que contenha um único vídeo quando o localeMap está ativo, caso contrário, a chamada para o conteúdo do conjunto falhará. Para contornar esse problema, você pode adicionar um único vídeo a um Conjunto de vídeos adaptáveis. Em seguida, adicione o Conjunto de vídeos adaptáveis a um Conjunto de mídias mistas.
* Certas solicitações não estão localizadas, como solicitações para o conteúdo de um Conjunto de vídeos adaptáveis. Portanto, se você pretende usar os Conjuntos de vídeos adaptáveis com localização, coloque o Conjunto de vídeos adaptáveis em um Conjunto de mídias mistas. Em seguida, chame o conjunto em um visualizador de Mídia mista com o parâmetro `locale=` .

## Renderizador de imagem {#image-renderer}

A página Renderizador de imagem estabelece as configurações padrão para o fornecimento de Conjuntos de imagens a partir dos servidores de renderização de imagem. As configurações estão disponíveis nessas cinco categorias (consulte a própria página Servidor de imagens para obter descrições detalhadas das configurações):

* **Gerenciamento de catálogo**  - Essas configurações determinam como o Dynamic Media Classic e o arquivo de catálogo interagem. As chamadas de URL do servidor de renderização do Dynamic Media Classic são feitas ao catálogo, que, por sua vez, chama para fornecer imagens do servidor. Altere essas configurações somente com a assistência de uma pessoa de suporte do Dynamic Media Classic.

* **Atributos da sessão**  - Essas configurações estabelecem parâmetros de erro, o URL para URLs de imagem relativa e se a sobreposição de objeto é permitida.

* **Atributos de material padrão**  - Essas configurações estabelecem configurações padrão de resolução e nitidez para imagens.

* **Atributos de imagem de resposta**  - Essas configurações pertencem à aparência padrão das imagens.

* **Atributos de gerenciamento de cores**  - Essas configurações pertencem às configurações de cores padrão das imagens.

## Vinheta {#vignette}

A página Vinheta oferece configurações para estabelecer a aparência padrão das vinhetas (consulte a própria página para obter descrições detalhadas das opções).
