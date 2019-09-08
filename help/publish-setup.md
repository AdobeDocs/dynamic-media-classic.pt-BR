---
title: Publicação de publicação
seo-title: Publicação de publicação
description: 'null'
seo-description: As configurações de tela de Configuração de publicação determinam como os ativos são fornecidos por padrão dos servidores do Dynamic Media Classic a sites ou aplicativos.
uuid: 196 f 25 c 8-abf 5-4 c 5 d -8 f 6 f-bc 70007 a 0301
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: cba 59093-28 b 6-4490-b 838-d 942 b 72 ad 1 ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Publicação de publicação {#publish-setup}

As configurações de tela de Configuração de publicação determinam como os ativos são fornecidos por padrão dos servidores do Dynamic Media Classic a sites ou aplicativos. Se nenhuma configuração for especificada, o servidor do Dynamic Media Classic fornecerá um ativo de acordo com uma configuração padrão em uma tela de Configuração de publicação. Por exemplo, uma solicitação para entregar uma imagem que não inclui um atributo de resolução gera uma imagem com a configuração Resolução padrão de objetos na tela Servidor de imagens.

Os administradores podem alterar as configurações padrão nas telas do Servidor de imagem, do Renderizador de imagens e da Vigneta para estabelecer configurações padrão para a disponibilização de ativos de servidores.

Para abrir as telas de Configuração de publicação, clique em Configuração &gt; Configuração do aplicativo &gt; Configuração de publicação.

>[!NOTE]
>
>As telas de Configuração de publicação são usadas por desenvolvedores e programadores de sites experientes. O Dynamic Media Classic supõe que os usuários que mudam configurações nessas telas estejam familiarizados com o Sistema de publicação Scene 7, normas de protocolo HTTP e convenções e tecnologia básica de geração de imagens.

## Servidor de imagens {#image-server}

A tela Servidor de imagens estabelece configurações padrão para a entrega de imagens de servidores de imagem. As configurações estão disponíveis nessas cinco categorias (consulte a tela Servidor de imagens para obter descrições detalhadas das configurações).

Altere essas configurações somente com a assistência de uma pessoa de suporte do Dynamic Media Classic.

**Gerenciamento de catálogo** Estas configurações determinam como o Sistema de publicação Scene 7 e o catálogo interagem. Ao contrário da maioria dos servidores Web, as chamadas URL do servidor de imagem do Dynamic Media vão para um arquivo de manifest ou catálogo, em vez de um arquivo de imagem apropriado. O arquivo de catálogo (não confundir com um ecatalog) contém uma lista de todo o conteúdo publicado no servidor de imagens junto com o caminho para cada imagem. Se você tiver uma ID da Digimarc, digite as informações do usuário na seção Informações do usuário Digimarc.

**Atributos de solicitação** Estas configurações impõem limites em imagens que podem ser entregues a partir do servidor.

**Atributos de solicitação padrão** Estas configurações pertencem à aparência padrão das imagens.

**Atributos de miniatura comuns** Estas configurações pertencem à aparência padrão e ao alinhamento das imagens em miniatura.

**Padrões para campos de catálogo** Essas configurações pertencem à resolução e ao tipo de miniatura padrão das imagens.

**Atributos de gerenciamento de cores** Estas configurações determinam quais perfis de cor ICC são usados.

**Atributos de compatibilidade** Essa configuração permite que os parágrafos à esquerda e à direita em camadas de texto sejam tratados como na versão 3.6 para compatibilidade retroativa.

**Suporte à localização** Estas configurações permitem gerenciar vários atributos de localidade. Ela também permite especificar uma string de mapa de localidade para que você possa definir quais idiomas deseja suportar para as várias dicas de ferramentas nos Visualizadores.

Por exemplo, se você for uma marca multinacional que vende em países diferentes, você pode garantir que cada país tenha seu próprio Visualizador específico de localidade. Para obter essa funcionalidade, especifique uma string de mapa de localidade. Em seguida, edite o texto da dica de ferramenta na predefinição do visualizador adicionando as strings de texto traduzidas para o idioma desejado.

>[!NOTE]
> Para configurar opções de Suporte a localização, entre em contato com o Suporte técnico da Adobe Dynamic Media Classic ou envie um email para s7support@adobe.com solicitando a ajuda de configuração.

Para obter mais informações sobre como configurar o Suporte **a localização**, consulte [Considerações ao configurar a localização de ativos](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerações ao configurar a localização de ativos {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Se desejar configurar opções de Suporte de localização no Sistema de publicação Scene 7, como o campo Mapa de localidade, entre em contato com o Suporte técnico do Adobe Dynamic Media Classic. Ou envie um email para s7support@adobe.com solicitando a ajuda de configuração.

Uma maneira comum de usar o Sistema de publicação do Scene 7 (SPS) é gerenciar a imagem de produto em sites de comércio eletrônico. As empresas internacionais enfrentam o desafio que os ativos para produtos semelhantes parecem diferentes de país para país. Normalmente, as diferenças são para uma pequena parte da mídia geral. Resolver essas diferenças copiando todos os ativos para cada um dos países e sobrescrever apenas as diferenças é um enorme esforço e contradiz a única metálise do ativo mestre. Essas diferenças para os ativos podem ser endura, de vídeos específicos do país com faixas de áudio diferentes, para sutis, mas diferenças importantes em uma cord de energia usada com o produto. O Dynamic Media Classic usa um mecanismo de pesquisa básico. Você define uma ordem de sufixos de ativos no qual o Servidor de imagens está procurando, começando pela localidade necessária.

**Como os ativos são localizados**

A localidade para uma solicitação IS (Serviço de imagem) é identificada com o comando IS/IR (Renderização de imagens) a seguir:

`locale=`

Esse comando aceita uma string de ID de localidade (locid) que não faz distinção entre maiúsculas e minúsculas. A ID de localidade normalmente é uma sequência de 2-6 caracteres compostos de letras e «_».

A IS suporta sequências de caracteres ASCII arbitrários arbitrários. O `locale=` comando tem um escopo global, o que significa que é aplicado à solicitação inteira, incluindo todas as solicitações IS e IR aninhadas, modelos referenciados e camadas de imagem. Vários localidades por solicitação, como uma localidade diferente para cada camada, não são compatíveis. No entanto, é possível permitir substituições explícitas em solicitações aninhadas.

Se `locale=` não for especificado, `attribute::DefaultLocale` será passado para os mecanismos de tradução. A validação de entrada limitada é aplicada ao `locale=` valor. Valores vazios `locale=` são permitidos. Como `locale=` tem um escopo global, `attribute::DefaultLocale` é fornecido pelo catálogo principal para toda a solicitação.

Alguns dos benefícios do uso `locale=` e `attribute::DefaultLocale` inclusão do seguinte:

* Compartilhar conteúdo para várias localidades.
* Acesse conteúdo específico da localidade usando ids genéricas.
* Permita flexibilidade em relação às convenções de nomenclatura e ao gerenciamento de conteúdo específico da localidade, como o prefixo de localidade e o sufixo, ou conteúdo específico da localidade em um catálogo separado.
* Suporte direto a versões específicas de localidades.
* Objetos agregados, como conjuntos de imagens, podem conter referências genéricas a conteúdo potencialmente específico da localidade.
* Suporta todo o conteúdo gerenciado por catálogos que podem precisar de localização, incluindo imagens, conjuntos de imagens, vinhetas, materiais e registros de configuração do visualizador.
* Minimize as alterações nos mecanismos de banco de dados IPS e manifest IS.
* O suporte para conteúdos estáticos, como vídeos e capas, será adicionado quando a RFC IS -63 for implementada.
* A localidade padrão é configurável.

**Cenários do aplicativo**

| Aplicativo | Cenário |
|--- |--- |
| Localização do visualizador | Depois que catálogos de conteúdo estáticos são implementados, a localização é controlada totalmente com o parâmetro locale =, anexado a todas as solicitações feitas ao IS. Os registros de configuração, capas, telas de apresentação e assim por diante podem ter variantes específicos para localidades ou não. O conteúdo correto é fornecido pela IS sem o visualizador precisar saber qual conteúdo está localizado e quais são as IDs. |
| Imagens e vídeo | As empresas multinacionais muitas vezes possuem uma combinação de conteúdo genérico e específico de localidades. Com esse mecanismo, uma referência a uma imagem ou vídeo pode ser genérica, e o IS disponibiliza o conteúdo específico da localidade se estiver disponível. |
| Conjuntos de imagens e conjuntos de mídia | Todo o conjunto de imagens pode ser diferente para alguns locais—como quando um ecatalog é completamente diferente—com a tradução de um conjunto genérico para um conjunto de imagens específico de localidade manipulado pelo visualizador. Mais comumente, IDs individuais em um conjunto genérico podem se referir a conteúdo localizado. Por exemplo, a maioria das fotos de um applília pode ser a mesma em todos os idiomas, exceto a foto do painel de controle. A IS traduz automaticamente IDs, portanto não há necessidade de gerar conjuntos de imagens específicos de localidades. |

**Implementação da localização de ativos**

O Scene 7 Publishing and Image Serving tem uma interface que permite as localizações de imagens e conteúdo estático.

Sem localização, um URL do servidor de imagens é semelhante ao seguinte:

`https://server/is/image/company/image`

Com a localização, um URL do servidor de imagens adiciona o `locale=` parâmetro ao caminho, como segue:

`https://server/is/image/company/image?locale=de_DE`

Ao receber a chamada http pelo Servidor de imagens, o `locale=` parâmetro é analisado por meio do campo localemap encontrado em **Configuração** &gt; Configuração **do aplicativo** &gt; Configuração **de publicação** &gt; **Servidor de imagens** &gt; **Grupo de suporte** de localização.

O campo Mapa de localidade contém uma lista de entradas separadas usando o símbolo de barra vertical (|).

Cada entrada consiste em uma lista de valores separada por vírgulas. O primeiro valor é o valor de pesquisa passado pelo `locale=` parâmetro. Os valores restantes são valores de sufixo/substituição que são subsequentemente tentados até que um resultado resulte em uma imagem existente.

Se um valor de sufixo ou um valor de substituição for aplicado depende da configuração Local global em **Configuração** &gt; Configuração **do aplicativo** &gt; Configuração **de publicação** &gt; **Servidor de imagens** &gt; **Grupo de suporte** de localização.

>[!NOTE]
>
>Atualmente, a configuração Local global só é possível quando você o define por meio da API, não na interface do Sistema de publicação Scene 7.

**Exemplo de sufixo**

| URL | IDs do localemap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observe que não há globalocale definido. O parâmetro de localidade de_ DE é correspondente à primeira entrada no localemap. O primeiro valor correspondente_ DE é adicionado como um sufixo para o ativo image_ DE e é feita uma tentativa de encontrá-la no Servidor de imagens. Se for encontrado no servidor, ele será retornado. Caso contrário, o segundo valor «» será usado como um sufixo, resultando na própria imagem sendo retornada. |

**Exemplo de substituição**

| URL | Globalocale e IDs do localemap | Resultado |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | No exemplo de substituição acima, globalocale está definido como principal. O parâmetro de localidade de_ DE é correspondente à primeira entrada no localemap. A subsequência de caracteres globalocale é encontrada e substituída pelo primeiro valor correspondente de no localemap: image-de -01. Se for encontrado no Servidor de imagens, ele será retornado. Caso contrário, o segundo valor será substituído, resultando na imagem principal -01. |

Se nenhuma localidade for definida no URL, o servidor de imagem assumirá o defaultlocale, se for definido, e o aplicará ao URL.

Se um parâmetro de localidade desconhecido ou vazio for `locale=`fornecido, o localemap será apagado pelo valor vazio «começando com». É importante configurar isso para ter uma localidade padrão aplicada para localidades desconhecidas.

**Sobre a defaultimage**

O Servidor de imagens tenta as opções para a localidade solicitada, uma após a outra. Se nenhuma correspondência for encontrada, as opções de local serão aplicadas à defaultimage e a versão correspondente será retornada. Portanto, cada localidade deve incluir uma opção para a imagem sem localização, ou versões defaultimage localizadas devem ser disponibilizadas no Sistema de publicação Scene 7.

**Cenários para encontrar o localemap**

Suponha que você queira oferecer suporte às seguintes localidades:

`en, en_us, en_uk, de, de_at, de_de, fr`

Você mapeia essas localidades para os sufixos `_E`, `_G`e `_F`para inglês, alemão e francês, respectivamente. Para todos os exemplos, a ID de imagem de entrada genérica é `myImg`.

*Comportamento padrão para encontrar o localemap*

As IDs de localidade são mapeadas para seus sufixos correspondentes. Se nenhuma ID de localidade específica for encontrada no catálogo, a ID genérica será tentada. Observe os valores vazios de locsufix que mapeiam para a ID genérica.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale = | IDs de saída para pesquisar |
|--- |--- |
| en, en_ us, en_ uk | Myimg_ E, myimg |
| de, de_ de, de_ at | Myimg_ D, myimg |
| fr | Myimg_ F, myimg |
| Todos os outros | - |

*Localizar o localemap quando a localidade for desconhecida*

É possível mapear localidades desconhecidas para IDs específicas ou para IDs genéricas. Por exemplo, é possível mapear localidades desconhecidas para as IDs em inglês, ou se elas não existem, para as IDs genéricas.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale = | IDs de saída para pesquisar |
|--- |--- |
| de, de_ de, de_ at | Myimg_ D, myimg |
| fr | Myimg_ F, myimg |
| Todos os outros | Myimg_ E, myimg |

Você também pode ter um locsuffix dedicado, como U, apenas para localidades desconhecidas e forçar para a imagem padrão se não `_U` existir, como segue:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Ou você pode mapear diretamente para a ID genérica, como segue:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Localizar o localemap usando uma pesquisa em vários níveis*

Geralmente, é desejável agrupar localidades, como Europeu, Oriente Médio e Norte americano, para lidar com padrões regionais, como exposição de capa. Esse efeito pode ser obtido usando uma pesquisa em múltiplas camadas.

Neste exemplo, suponha que você queira oferecer suporte a coleções para uso do Oeste e do Oriente Médio. Ambas as coleções são baseadas na coleção de imagens genérica, e adicionam ou modificam algumas imagens. Ambas as coleções são refinadas para localidades específicas, como `m1, m2` para duas variantes do Oriente Médio, e `w1, w2,` para `w3` três localidades ocidentais, exceto para as imagens compartilhadas `w1` e `w3`. Localidades desconhecidas são mapeadas somente para a coleção genérica e não têm acesso a imagens específicas de localidades. A seguir, é a seguinte aparência do mapa:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale = | IDs de saída para pesquisar |
|--- |--- |
| w 1, w 3 | Myimg-W, myimg |
| w2 | Myimg-W 2, myimg-W, myimg |
| m1 | Myimg-M 1, myimg-M, myimg |
| m2 | Myimg-M 2, myimg-M, myimg |
| Todos os outros | mylmg |

*Localizar o localemap pesquisando IDs específicas*

Algumas convenções de nomenclatura de imagem podem não oferecer suporte a IDs de imagem genéricas. As IDs genéricas da solicitação devem ser mapeadas para uma ID específica no catálogo. No entanto, pode haver instâncias em que a ID exata exata não é conhecida.

Usando o primeiro exemplo como base, as imagens para todos os idiomas podem ter os sufixos `_1`, `_2`ou `_3`. Imagens específicas para localidades francesas podem ter os sufixos `_22` ou `_23` sufixo. E imagens específicas para localidades alemãs podem ter os sufixos `_470` ou `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale = | IDs de saída para pesquisar |
|--- |--- |
| fr | Myimg_ 22, myimg_ 23, myimg_ 1, myimg_ 2, myimg_ 3 |
| de, de_ at, de_ de | Myimg_ 470, myimg_ 480, myimg_ 1, myimg_ 2, myimg_ 3 |
| Todos os outros | Myimg_ 1, myimg_ 2, myimg_ 3 |

**Considerações importantes ao implementar o suporte à localização**

* A localização é limitada às chamadas de ativos com base em ID e não pode ser usada em chamadas de ativos com base em caminho. Portanto, ao chamar vídeos com localidade, ela deve ser chamada como empresa/ID; não há caminho completo para o vídeo. Isso significa que você não pode usar rtmp com localização porque esse método serve apenas com chamadas de vídeo baseadas em caminho.
* Não é possível usar um Conjunto de mídia mista que contenha um único vídeo quando o localemap estiver ativo, caso contrário, a chamada para o conteúdo do conjunto falhará. Para contornar esse problema, você pode adicionar um único vídeo a um Conjunto de vídeos adaptativo. Em seguida, adicione o Conjunto de vídeos adaptativo a um conjunto de mídia mista.
* Algumas solicitações não estão localizadas, como solicitações para o conteúdo de um Conjunto de vídeos adaptativo. Portanto, se você pretende usar Conjuntos de vídeos adaptativos com localização, coloque o conjunto de vídeos adaptativo em um conjunto de mídia mista. Em seguida, chame o conjunto em um visualizador de mídia mista com o `locale=` parâmetro.

## Renderizador de imagens {#image-renderer}

A tela do Renderizador de imagens estabelece configurações padrão para a entrega de Conjuntos de imagens a partir de servidores de renderização de imagens. As configurações estão disponíveis nessas cinco categorias (consulte a tela Servidor de imagens para obter descrições detalhadas das configurações):

**Gerenciamento de catálogo** Estas configurações determinam como o Sistema de publicação Scene 7 e o arquivo de catálogo interagem. As chamadas de URL do servidor de renderização do Dynamic Media Classic são feitas no catálogo, que, por sua vez, chama a entrega de imagens do servidor. Altere essas configurações somente com a assistência de uma pessoa de suporte do Dynamic Media Classic.

**Atributos de sessão** Estas configurações estabelecem parâmetros de erro, o URL para urls de imagem relativa e se a sobreposição do objeto é permitida.

**Atributos de material padrão** Estas configurações estabelecem a resolução padrão e as configurações de nitidez das imagens.

**Atributos de imagem de resposta** Estas configurações pertencem à aparência padrão das imagens.

**Atributos de gerenciamento de cores** Estas configurações pertencem às configurações de cores padrão das imagens.

## Vignette {#vignette}

A tela de Vinheta oferece configurações para estabelecer a aparência padrão de vinhetas (consulte a própria tela para obter descrições detalhadas das opções).
