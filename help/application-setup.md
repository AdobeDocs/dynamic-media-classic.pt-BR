---
title: Configuração do aplicativo
seo-title: Configuração do aplicativo
description: Saiba como configurar a área de aplicativos do Dynamic Media Classic.
seo-description: Saiba como configurar a área de aplicativos do Dynamic Media Classic.
uuid: 3 e 2 f 1 d 30-8 f 33-4 a 9 d-bbe 4-e 8 c 3 dbc 968 f 8
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/configuração
discoiquuid: ae 2 d 1895-a 437-4463-bfac -3960 c 8027551
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Configuração do aplicativo{#application-setup}

Você pode usar as páginas de Configuração de aplicativo para inserir configurações gerais, criar predefinições de imagens, predefinições de codificação de vídeo, predefinições do visualizador ou definir visualizadores padrão e metadados. Também é possível configurar predefinições de conjunto em lote para automatizar a geração de conjuntos de rotação 2 D (por exemplo), configurações de publicação e configurações de SEO de vídeo.

>[!NOTE]
>
>Somente os administradores do Scene 7 Publishing System podem alterar as configurações nas páginas de Configuração de aplicativo.

## Configurações gerais {#general-settings}

Para abrir a página Configurações gerais do aplicativo, na barra Navegação global, clique **[!UICONTROL Setup > Application Setup > General Settings]** em.

### Servidores

Na criação da conta, o Dynamic Media Classic fornece automaticamente os servidores atribuídos para sua empresa. Esses servidores são usados para criar strings de URL para seu site e aplicativos. Essas chamadas de URL são específicas para a sua conta.

Consulte [também Testar o serviço de teste seguro](testing-assets-making-them-public.md#testing_the_secure_testing_service).

**Nome do servidor publicado** Este servidor é o servidor CDN ativo usado em todas as chamadas de URL geradas pelo sistema específicas à sua conta. Não altere esse nome do servidor a menos que seja instruído a fazê-lo por um técnico de suporte do Dynamic Media Classic.

**Nome do servidor de origem** Esse servidor é usado apenas para testes de garantia de qualidade. Não altere esse nome do servidor, a menos que instruído a fazê-lo por um técnico de suporte do Dynamic Media Classic.

**Nome do servidor AGM** Este servidor é usado para modelos da Web para impressão. Esse servidor é definido em toda a empresa. Não altere esse nome do servidor, a menos que instruído a fazê-lo por um técnico de suporte do Dynamic Media Classic.

**O Test &amp; Target Server Name** your Test &amp; Target URL (Nome do Test &amp; Target), até o. com. Para obter instruções sobre como obter esse URL, consulte Integração do Dynamic Media Classic com o Target Classic.

**iOS Streaming Server Name** O URL para o servidor de streaming clássico do Dynamic Media Classic. Este servidor fornece vídeo de fluxo contínuo para dispositivos baseados em iOS usando protocolo HTTP.

**Nome do servidor de vídeo progressivo** O URL para o servidor de vídeo progressivo do Dynamic Media Classic. Este servidor fornece vídeo progressivo usando protocolo HTTP.

**Mostrar URL para ativos não publicados** Selecione essa opção se quiser que o Dynamic Media Classic exiba um URL ao visualizar qualquer ativo, seja ele publicado ou não. Se o ativo não for publicado, o URL não funcionará. No entanto, é possível usar o URL para fins de planejamento ou organização.

**Permitir instalação** do AIR Selecione esta opção para permitir que os usuários baixem a versão de desktop do Scene 7 Publishing System para seus discos rígidos locais. Os usuários instalam o aplicativo na área Versão da área de trabalho da tela Configuração pessoal.

Os usuários do AIR devem desinstalar manualmente o aplicativo existente e reinstalar a partir da versão da Web do Sistema de publicação Scene 7 (em Configurações pessoais). Após essa reinstalação única, você será solicitado a atualizar sempre que o servidor tiver uma versão mais nova do Sistema de publicação do Scene 7. O Scene 7 Publishing System é integrado com a Estrutura de atualização do aplicativo, que simplifica o processo de atualização.

**Modelo de invalidação de CDN** Especifica o modelo usado para invalidar o cache CDN (Content Delivery Network).

Por exemplo, suponha que você insira um URL da imagem (incluindo predefinições de imagens ou modificadores), `<ID>`em vez de uma ID de imagem específica como no exemplo a seguir:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

Se o modelo contiver `<ID>`apenas, então o SPS preencherá o `https://<server>/is/image`, onde `<server>` é o Nome do servidor de publicação definido em Configurações gerais.

Configurar o CDN Invalidate Template, selecionar uma imagem chamada Backpack_ B e clicar **em Arquivo** &gt; **Invalidar CDN** resulta no seguinte URL gerado na interface CDN Invalidate:

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

Na caixa de listagem URL, clique **em Continuar** para limpar o cache da chamada de URL da imagem específica. Observe que você também pode adicionar urls digitando ou colando-os na caixa de listagem do URL; não é necessário definir o modelo antecipadamente.

Depois que você selecionou seu Modelo de Invalidação CDN e fez uma solicitação Invalidar CDN, um indicador será exibido na interface do usuário que fornece uma estimativa do tempo que levará para limpar o cache.

Da mesma forma, se várias imagens forem selecionadas no SPS quando você clicar **em Arquivo** &gt; **Invalidar CDN**, cada imagem será mencionada no URL de modelo salvo. Portanto, você pode definir um CDN como referência a cada URL referenciado no site (como detalhes do produto, resultados da pesquisa etc.). Em seguida, quando você seleciona uma ou imagens para invalidação no cache, os urls preenchem automaticamente a interface.

Consulte [Armazenamento de conteúdo em cache](scene7-platform-overview.md#content_caching).

Consulte [Ativos republicados e atrasos](publishing-files.md#republished_assets_and_cdn_delays)de CDN.

**Procurar**

**Mostrar projetos** Determina se os Projetos estão disponíveis como um meio de organizar seus ativos do Dynamic Media Classic. Consulte Organização do trabalho com Projetos.

**Mostrar a amostra de Evideo Conteúdo** ativa ou desativa a exibição de um conteúdo de amostra evideo.

**Mostrar conteúdo gerado** em pastas, mostra o conteúdo gerado a partir de um ativo. Por exemplo, quando um arquivo PDF é rasterizado à medida que é carregado, o Dynamic Media Classic cria uma imagem para cada página no PDF original. Se a opção Mostrar conteúdo gerado estiver selecionada, cada imagem gerada quando o PDF original for carregado aparecerá juntamente com o PDF na pasta à qual o PDF foi carregado.

**Por padrão, Mostrar vídeos** codificados desmarcados (desligado).

Para pesquisar e procurar vídeos no Scene 7 Publishing System sem precisar navegar por diversos derivados codificados do mesmo vídeo, deixe essa opção desmarcada (padrão). Apenas a miniatura de vídeo mestre, que é o vídeo de origem que você carregou e usou para criar todos os derivados, e apenas a miniatura de vídeo adaptativa "pai", que contém todos os derivados «filho» do conjunto de vídeos codificados, são exibidos na interface do usuário.

No entanto, você ainda pode acessar vídeos codificados individuais do Vídeo mestre ou do Conjunto de vídeos adaptativo. Para fazer isso, clique duas vezes na imagem em miniatura do vídeo para abrir a Exibição de detalhes. Em seguida, clique **em Vídeos** codificados no painel direito para acessar todos os vídeos «filho».

Você também pode usar **Arquivo &gt; Reprocesso** para criar vídeos «filho» codificados diretamente de um Conjunto de vídeos adaptativo. O Scene 7 Publishing System encontra automaticamente o vídeo mestre "pai" do conjunto de vídeos adaptativo e usa esse vídeo como vídeo de origem para transcodificação. No entanto, ao salvar os novos vídeos codificados individuais, eles não são vistos quando você pesquisar ou navegar. No entanto, elas ainda podem ser acessadas na guia Vídeos codificados na Exibição de detalhes.

Consulte [Upload e transcodificação de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

Para continuar a ter acesso a todos os seus derivados de vídeo codificados ao pesquisar e navegar, selecione **Mostrar vídeos codificados**.

Há algumas ações no menu Build que funcionam somente, ou funcionam opcionalmente, com vídeos individuais. Essa funcionalidade torna necessário mostrar todos os derivados de vídeo codificados que podem ser selecionados, independentemente de como você configurar **Mostrar vídeos codificados**. As ações Build que sobrescreverem a configuração **Mostrar vídeos** codificados incluem **Conjuntos de vídeos adaptativos** e **ecatalogs**.

>[Observação]
>
>Se você não usou o Scene 7 Publishing System para fazer upload e codificar seus ativos de vídeo, o Dynamic Media Classic mostra todos os vídeos codificados individualmente, mesmo que essa opção esteja desmarcada.

**Mostrar o botão Atualizar subpastas** Ativa ou desativa a exibição das subpastas Atualizar o botão Atualizar.

**Conta FTP clássica do Dynamic Media**

**Servidor** lista seu servidor de conta FTP.

**Nome de usuário** Lista o nome de usuário da conta FTP.

**Carregar no aplicativo**

**Substituir imagens** do Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. Cada ID do sistema de publicação do Scene 7 de cada item (o nome da imagem menos a extensão de nome de arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Carregar tem uma opção Substituir. O efeito exato dessa opção depende da opção Substituir imagens especificadas. Essas opções especificam como as imagens de substituição são carregadas: se substituem as imagens originais ou se tornam imagens duplicadas. As imagens duplicadas são renomeadas com um «-1» (por exemplo, chair. tif é renomeado para cadeira -1. tif). Essas opções afetam as imagens carregadas em uma pasta diferente da original ou da imagens com uma extensão de nome de arquivo diferente da original (como JPG, TIF ou PNG). (Consulte Usando a opção Substituir imagens.)

**Substituir a pasta atual, mesmo nome/extensão da imagem base**

Essa opção é a regra mais estrita para substituição. Ele exige que você carregue a imagem de substituição para a mesma pasta que o original e que a imagem de substituição tenha a mesma extensão de nome de arquivo que o original. Se esses requisitos não forem cumpridos, uma duplicata será criada.

**Substituir a pasta atual, mesmo nome de ativo base, independentemente da extensão**

Exige que você carregue a imagem de substituição para a mesma pasta que o original, no entanto, a extensão de nome de arquivo pode ser diferente da original. Por exemplo, chair. tif substitui chair. jpg.

**Substituir qualquer pasta, mesmo nome de ativo base/extensão**

Requer que a imagem de substituição tenha a mesma extensão de nome de arquivo que a imagem original (por exemplo, chair.jpg deve substituir chair.jpg, não chair. tif). No entanto, é possível carregar a imagem de substituição para uma pasta diferente da original. A imagem atualizada reside na nova pasta; o arquivo não pode mais ser encontrado em seu local original

**Substituir qualquer pasta, mesmo nome de ativo base, independentemente da extensão**

Essa é a regra de substituição mais inclusiva. É possível carregar uma imagem de substituição para uma pasta diferente do original, carregar um arquivo com uma extensão de arquivo diferente e substituir o arquivo original. Se o arquivo original estiver em uma pasta diferente, a imagem substituta reside na nova pasta à qual foi carregada.

**Reter publicação** Especifica se uma imagem de substituição carregada no Dynamic Media Classic mantém a configuração Pronto para publicar da imagem substituída, ou a configuração é especificada no upload.

**Perfis de cor padrão** Especifica os perfis de cores aplicados como parte das Opções de perfil de cores padrão ao adicionar imagens CMYK.

**Opções de upload padrão** Abre a caixa de diálogo Carregar opções de trabalho, onde você pode especificar opções de upload padrão. Para obter informações sobre essas opções, consulte Opções de upload.

**Editor do mapa de imagens, ao aplicativo**

**O HREF mapeamento de imagem padrão** define o URL padrão usado na coluna href de mapeamento de imagem. Esse URL é o URL padrão que você vê quando cria novos Mapas de imagem.

**Modelo de mapeamento de imagem padrão** Define o Javascript padrão para o mapeamento da imagem no modelo href. Você pode definir um código personalizado aqui para ser executado sempre que clicar em um mapa de imagem.

**Outras configurações, ao aplicativo**

**Os Ativos de avisos** da Lixeira na Lixeira são removidos automaticamente dentro de sete dias. Selecione «Enviar e-mails antes dos itens de lixeira serem excluídos automaticamente» se você quiser que notificações enviadas aos administradores da empresa sejam usadas em quatro dias de exclusão permanente. Consulte Gerenciamento da pasta Lixeira.

## Uso da opção Substituir imagens {#using-the-overwrite-images-option}

O Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. Cada ID do sistema de publicação do Scene 7 de cada item (o nome da imagem menos a extensão de nome de arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Carregar inclui as opções Substituir imagens. O efeito exato dessa opção depende de uma configuração para as configurações internas do sistema de publicação do Scene 7 de cada empresa.

Se você carregou anteriormente imagens e depois alterava os arquivos originais (ou os substituiu), a opção Substituir o Dynamic Media especificará como o Dynamic Media Classic substitui as imagens. Nenhuma informação sobre a imagem muda, mas a nova imagem substitui a antiga. Se a pasta também contiver imagens que ainda não estão no Dynamic Media Classic, essas imagens serão adicionadas.

Use essa opção se as imagens que você carregou foram alteradas de alguma forma (a imagem foi alterada), mas a referência à imagem permanece a mesma. Substituir também é útil ao carregar e apagar os pdfs do Adobe®. Para ajustar como o Dynamic Media Classic *rila* a imagem, ajuste as opções de perfil de cores ICC na caixa de diálogo Fazer upload e faça upload novamente usando o recurso Substituir.

As IDs clássicas de mídia dinâmica usadas para acessar imagens dos servidores de produção são derivadas dos nomes de arquivo de imagem. O uso de caracteres maiúsculos e minúsculos no nome do arquivo é importante, tanto na substituição dos arquivos existentes quanto nas IDs clássicas de mídia dinâmica usadas para acessar a imagem. Certifique-se de que o uso de caracteres maiúsculos e minúsculos nos nomes de arquivo esteja correto antes de fazer upload no Dynamic Media Classic para evitar IDs de Dynamic Media que diferem somente no caso da mesma imagem.

Se você desmarcar essa opção, todas as imagens com os mesmos nomes de arquivo que as imagens existentes são tratadas como duplicatas e não são adicionadas.

## Predefinições de imagens {#image-presets}

A tela Predefinições de imagens é para criar e editar predefinições de imagens. As predefinições de imagens permitem que o Dynamic Media Classic forneça imagens dinamicamente em tamanhos diferentes da mesma imagem mestre. Cada predefinição de imagem representa uma coleção predefinida de comandos de tamanho e formatação para a exibição de imagens. Ao criar uma predefinição de imagem, você escolhe um tamanho para a entrega de imagens. Você também escolhe os comandos de formatação para que a aparência da imagem seja otimizada quando a imagem for entregue para exibição.

Os administradores podem criar predefinições para exportar ativos. Os usuários podem escolher uma predefinição quando exportam imagens, que também reformendem imagens às especificações especificadas pelo administrador.

Para abrir a tela Predefinição de imagem, na barra Navegação global, clique **em Configuração** &gt; **Predefinições de imagens**.

Consulte [Geração de imagens inteligentes](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

### Criação e edição de predefinições de imagens {#creating-and-editing-image-presets}

1. Clique **em Configuração** &gt; **Predefinições de imagens**.
1. Crie uma nova predefinição ou inicie de uma existente:
   * **Criando uma predefinição de imagem** - Clique **em Adicionar**.
   * **Criando uma predefinição de imagem a partir de uma predefinição** existente - Selecione a predefinição de imagem que você deseja criar e clique em Editar.

1. Na tela Adicionar (ou Editar) predefinida, insira um nome para a predefinição.
1. Defina as opções Predefinidas desejadas.

   Consulte [Opções de predefinição de imagens](application-setup.md#image_preset_options).

1. Clique **em Salvar**, ou se tiver iniciado de uma predefinição existente, clique **em Salvar como**.
1. Para visualizar a predefinição com sua própria imagem, clique **em Procurar** e selecione uma imagem. Para visualizar com a imagem padrão, clique **em Redefinir**.

É possível editar uma predefinição de imagem selecionando seu nome na tela Predefinições de imagens e clicando em Editar. Para excluir uma predefinição de imagem, selecione-a e clique em Excluir.

### Opções de predefinição de imagens {#image-preset-options}

As telas Adicionar predefinido e Editar predefinições oferecem as seguintes opções para criar e editar predefinições de imagens:

**Nome** da predefinçãoinsira um nome descritivo sem espaços em branco. Inclua a especificação de tamanho de imagem no nome para ajudar os usuários a identificar essa predefinição de imagem.

**Largura e Altura** Digita em pixels o tamanho em que a imagem é entregue.

**Formatar** escolha um formato no menu. A escolha do formato GIF, JPEG, PDF ou TIFF exibe opções adicionais:

* Opções de quantificação de cores GIF

   **Tipo**

   Escolha Adaptável (o padrão), Web ou Macintosh. Se você escolher GIF com alfa, a opção Macintosh® não estará disponível.

   **Pontilhamento**

   Escolha Difuso ou Desligado.

   **Número de Cores**

   Arraste o controle deslizante para digitar 2-255.

   **Lista de cores**

   Insira uma lista separada por vírgulas. Por exemplo, para branco, cinza e preto, digite 000000,888888, ffffff.

* Opções de JPEG

   **Qualidade**

   Controla o nível de compactação JPEG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade JPEG é de 1-100.

   **Ativar a redução de crominância JPG**

   Como o olho é menos sensível às informações de cores de alta frequência do que a luminância de alta frequência, as imagens JPEG dividem as informações da imagem em componentes de luminância e cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução total, enquanto os componentes de cor são reduzidos pela média de grupos de pixels. A redução da resolução reduz o volume de dados em metade ou um terço sem nenhum impacto sobre a qualidade percebida. A diminuição da resolução não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compressão útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

* Opções de PDF e TIFF

   **Compactação**

   Escolha um algoritmo de compactação.

**Colorspace** Escolha um espaço de cores.

**Nitidez** Selecione a opção Ativar nitidez simples para aplicar um filtro de nitidez básico à imagem depois que todo o dimensionamento ocorrer. A nitidez pode ajudar a compensar o desfoque que pode resultar na exibição de uma imagem em tamanho diferente.

Para obter mais informações sobre nitidez, modos de redefinição de metas e máscaras irregulares, consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

**Modo de reamostragem** Escolha uma opção de modo de Redefinição de metas. Essas opções tornam a imagem nítida quando ela é reduzida:

**B-Linear** O método de reamostragem mais rápido; alguns artefatos de alfinização são visíveis.

**O idioma bi-cubic** aumenta o uso da CPU no Servidor de imagens, mas produz imagens mais nítidas com artefatos de alias menos visíveis.

**Sharp 2** Pode produzir resultados ligeiramente mais nítidos do que a opção Bi-Cuic, mas com um custo de CPU ainda maior no Servidor de imagens.

**Tri-Linear** usa resoluções tanto maiores quanto mais baixas, se disponível; recomendado apenas quando a alçăo é um problema. Esse método reduz o tamanho do JPEG devido a dados reduzidos de alta frequência.

**Máscara de nitidez** escolha essas opções para ajustar o ajuste da nitidez:

**Amount** Controla a quantidade de contraste aplicada aos pixels da borda. O padrão é 1.0. Para imagens de alta resolução, é possível aumentá-la até 5.0. Pense em Amount como uma medida da intensidade do filtro.

**Raio** Determina o número de pixels em torno dos pixels da borda que afetam a nitidez. Para imagens de alta resolução, digite de 1 a 2. Um valor baixo aplica nitidez apenas aos pixels da borda; um valor alto compara uma banda maior de pixels. O valor correto depende do tamanho da imagem.

**Threshold** Determina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez é aplicado. Em outras palavras, essa opção determina como os pixels com nitidez devem ser provenientes da área circundante antes que sejam considerados pixels de borda e fiquem nítidos. Para evitar a apresentação de ruído, experimente com valores entre .02 e 0.2. O valor padrão de 6 compara todos os pixels na imagem.

**Cor** Determina Determina se a imagem usa o espaço em que a imagem foi criada, geralmente RGB (Original) ou um espaço de luminância (Intensidade).

**Cor** Escolha estas opções:

**Perfil de cor de saída** Selecione Usar padrão ou um dos perfis de cores ICC disponíveis no Sistema de publicação Scene 7.

Consulte também perfis [ICC](icc-profiles.md#icc_profiles).

**Propósito de renderização** Selecione uma opção se desejar substituir o propósito de renderização padrão do perfil de cores. Use essa opção quando um dos perfis ICC padrão for o espaço de cores de destino de uma conversão de cores, um dispositivo de saída (impressora ou monitor) será caracterizado por esse perfil, e o propósito de renderização especificado será válido para esse perfil.

**Perfil incorporado** Selecione esta opção para que, se você abrir essa imagem no Adobe® Photoshop®, ela usará esse perfil.

**Resolução de impressão** Escolha uma resolução para imprimir esta imagem; 72 pixels é o padrão.

**Modificadores** de URL Se preferir especificar os modificadores de URL que definem a Predefinição de imagem, em vez das configurações, insira os modificadores aqui.

**URL da imagem de amostra** Relaciona a cadeia de caracteres de URL «bruto» que o Servidor de imagem do Dynamic Media usa para fornecer imagens com a Predefinição de imagem que você está adicionando ou editando. Essa sequência de caracteres codifica todas as configurações de formato selecionadas na tela Adicionar predefinição ou Editar predefinição.

### Editar, remover ou desativar uma predefinição de imagem {#editing-removing-or-deactivating-an-image-preset}

1. Clique **em Configuração** &gt; **Predefinições de imagens**.
1. Na tela Predefinições de imagens, selecione uma predefinição na tabela e execute um dos procedimentos a seguir:

   * Clique **em Editar** e especifique novas opções na caixa de diálogo Editar predefinição.
   * Clique **em Excluir** para remover a predefinição da lista.
   * Desmarque a caixa de seleção Ativa ao lado de um nome predefinido para removê-la da interface de usuário do Scene 7 Publishing System para usuários mediaportal.

## Ativar ou desativar predefinições de vídeo adaptável {#activating-or-deactivating-adaptive-video-presets}

O Dynamic Media Classic oferece predefinições de codificação de vídeos adaptáveis. É uma lista mestre de predefinições que combina as predefinições de vídeo adaptável 16:9 e Vídeo adaptável 4:3 em um grupo. Essas predefinições predefinidas refletem as configurações de codificação mais comuns e são otimizadas para reprodução em dispositivos móveis de destino, tablets e desktops.

Somente as predefinições de codificação «Vídeo adaptativo» são ativadas (ativadas ou «ativadas») por padrão. Você pode desativá-la, se desejar. Predefinições de vídeo adaptável inativas não aparecem como uma opção selecionável na seção evideo da caixa de diálogo Opções de trabalho de upload.

Consulte [Upload e codificação de vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Para ativar ou desativar predefinições de vídeo adaptável**

1. Próximo ao canto superior direito do Sistema de publicação Scene 7, clique **em Configuração** &gt; Configuração **do aplicativo** &gt; **Predefinições de vídeo** &gt; **Predefinições de vídeo adaptável**.
1. Na página Predefinições de vídeo adaptativo, desmarque a caixa de seleção ao lado de um nome predefinido para remover a predefinição da lista Opções do evideo na caixa de diálogo Opções de carregamento de trabalho.
1. Clique **em Fechar**.

## Predefinições de vídeo para codificação de arquivos de vídeo {#video-presets-for-encoding-video-files}

Para escolher uma predefinição de codificação, no canto inferior direito da página Carregar, clique em Opções de trabalho. Na caixa de diálogo Carregar opções de trabalho, expanda Opções de evideo e escolha as predefinições de codificação de vídeo desejadas.

>[!NOTE]
>
>Com exceção de «Vídeo adaptativo», ativado por padrão, você pode não visualizar todas as outras predefinições de vídeo adaptativa ou de codificação de vídeo único na caixa de diálogo Opções de trabalho de upload. Os administradores do Dynamic Media Classic determinam quais predefinições de codificação de vídeo estão visíveis na caixa de diálogo Carregar opções de trabalho.

* Escolha uma das seguintes predefinições de codificação de vídeos adaptáveis ou de codificação simples:

   **Vídeo adaptável 16:9**

   Crie vídeos de proporção 16:9 para entrega em desktops, dispositivos móveis (iphone, ipad, Android) e tablets (ipad, Android), otimizados com a resolução e taxa de bits que melhor corresponde à velocidade de conexão do visualizador.

   **Vídeo adaptável 4:3**

   Crie vídeos de proporção 4:3 para entrega em desktops, dispositivos móveis (iphone, ipad, Android) e tablets (ipad, Android), otimizados com a resolução e taxa de bits que melhor corresponde à velocidade de conexão do visualizador.

   **Vídeo adaptável**

   Uma única predefinição de codificação que funciona com qualquer proporção para criar vídeos para distribuição em dispositivos móveis, tablet e desktop. Os vídeos de origem carregados que são codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo.

   Essa flexibilidade de ter uma «escala automática» também fica disponível por padrão quando você cria sua própria predefinição de codificação de vídeo personalizada.

   Consulte [Adicionar ou editar uma predefinição de codificação de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   **Codificação de vídeo adaptável (16:9 ou 4:3)**

   Crie vídeos de proporção 16:9 e 4:3 para entrega em desktops, dispositivos móveis (iphone, ipad, Android) e tablets (ipad, Android), otimizados com a resolução e taxa de bits que melhor corresponde à velocidade de conexão do visualizador.

   Consulte [Predefinições de vídeo adaptável de codificação de vídeo adaptável (16:9 ou 4:3](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)).

   **Predefinições de codificação única**

   >[OBSERVAÇÃO]
   >
   >Para fornecer vídeo a ipads, é possível escolher uma predefinição de codificação móvel ou uma predefinição de codificação de tablet. As predefinições de tablets são projetadas especialmente para o ipad, geralmente com maior resolução e qualidade para aproveitar o tamanho de tela maior e a conexão de largura de banda. A entrega de arquivos de vídeo codificados com uma predefinição de Tablet exige que você inclua código de detecção de dispositivo no seu site ou aplicativo móvel. Esse código muda entre uma experiência de vídeo do iphone ou do ipad, dependendo do dispositivo de reprodução. Escolher uma predefinição móvel para entregar arquivos de vídeo para o ipad é um fluxo de trabalho mais simplificado. O motivo é que você pode usar o mesmo arquivo de vídeo para iphones e ipads. No entanto, a qualidade é padronizada para a experiência de menor resolução do iphone.

   * No grupo Predefinições de codificação, na lista suspensa Classificar predefinições de codificação, selecione Nome ou Tamanho para classificar predefinições por nome ou tamanho de resolução.
   * Escolha uma predefinição de codificação com base no tamanho da resolução e largura de banda com a qual você planeja reproduzir o vídeo.
   * Você pode selecionar Codificação de vídeo adaptável e uma ou mais predefinições de codificação por vídeo. Por exemplo, você pode codificar um arquivo para desktop e dispositivos móveis em um trabalho de upload.

Após clicar **em Iniciar upload**, o arquivo mestre original será carregado e os arquivos codificados serão gerados a partir do arquivo mestre.

### Sobre as opções predefinidas de codificação {#about-encoding-preset-options}

Os parâmetros das opções predefinidas de codificação são:

**Velocidade de conexão do Target Velocidade** de conexão da Internet do usuário final direcionado.

**Sufixo do arquivo** codificado O sufixo que é anexado ao arquivo de vídeo codificado para fins de identificação.

**Taxa de bits de vídeo (taxa de dados)** A quantidade de dados codificada para formar um único segundo da reprodução do vídeo (em quilobits por segundo).

**Largura/altura de pixels** A dimensão de largura da imagem da tela, em pixels; a dimensão de altura da imagem da tela (em pixels).

**Quadro por segundo (fps)** O número de quadros, ou imagens ainda, para cada segundo do vídeo. Nos Estados Unidos e no Japão, a maioria dos vídeos é capturada em 29.97 fps; na Europa e na Ásia (exceto Japão), a maioria dos vídeos é capturada em 25 fps. Filme é capturado em 24 fps.

**Taxa de bits de áudio** A quantidade de dados codificada para formar um único segundo da reprodução de áudio, em quilobits por segundo.

As tabelas a seguir mostram as práticas recomendadas para selecionar predefinições de vídeo e as convenções de nomenclatura usadas para designar arquivos codificados.

### Vídeo adaptável (padrão) {#adaptive-video-default}

Uma predefinição de codificação que funciona com qualquer proporção para permitir a criação de vídeos para distribuição em dispositivos móveis, tablet e desktop. Os vídeos de origem carregados que são codificados usando essa predefinição (o padrão e a prática recomendada) são definidos com uma altura fixa, enquanto a largura é dimensionada automaticamente para preservar a proporção do vídeo.

**Vídeo adaptável (padrão)**

|  | Texto da predefinição de codificação/dica de ferramenta | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recomendações |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x 360, 800 Kbps | _ Mobile_ Autox 360 p_ 800 K | 800 | Autox360 | Igual à fonte | 64 | Para dispositivos móveis (iphone, ipad, Android) |
| 2 | Auto x 480, 1400 Kbps | _ Tablet_ Autox 480 p_ 1400 K | 1400 | Autox480 | Igual à fonte | 96 | Para tablet (ipad, Android) |
| 3 | Auto x 720, 2600 Kbps | _ Desktop_ Autox 720 p_ 2600 K | 2600 | Autox720 | Igual à fonte | 128 | Para desktop |

### Predefinições de vídeo adaptável de codificação de vídeo (16:9 ou 4:3) {#adaptive-video-encoding-or-video-presets}

Essas predefinições de codificação de vídeo adaptativa combinam uma série de predefinições de codificação individuais que são automaticamente selecionadas para você com base na proporção do vídeo que você carregou. Por exemplo, se você carregar um vídeo de 4:3, ele será codificado automaticamente usando as cinco predefinições:::3 encontradas na lista de predefinições mestre na opção Codificação de vídeo **adaptável (16:9 ou 4:3)** .

Para obter informações sobre os parâmetros de opções de codificação, consulte [Sobre opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Predefinições de codificação de vídeo adaptável (16:9 ou 4:3)**

|  | Texto da predefinição de codificação/dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recomendações |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobile (iphone, ipad, Android), (400 Kbps) | 500 | _ Mobile_ 512 x 288_ 400 K | 400 | 512x288 | Igual à fonte | 64 | Baixa resolução, 3 G |
| 2 | 4:3, 384 x 288 px, Mobile (iphone, ipad, Android), (400 Kbps) | 500 | _ Mobile_ 384 x 288_ 400 K | 400 | 384x288 | Igual à fonte | 64 | Baixa resolução, 3 G |
| 3 | 16:9, 512 x 288, Mobile (iphone, ipad, Android), (600 Kbps) | 700 | _ Mobile_ 512 x 288_ 600 K | 600 | 512x288 | Igual à fonte | 64 | Resolução média, 3 G |
| 4 | 4:3, 384 x 288, Mobile (iphone, ipad, Android), (600 Kbps) | 700 | _ Mobile_ 384 x 288_ 600 | 600 | 384x288 | Igual à fonte | 64 | Resolução média, 3 G |
| 5 | 16:9, 640 x 360, tablet (ipad, Android), (800 Kbps) | 900 | _ Ipad_ 640 x 360_ 800 K | 800 | 640x360 | Igual à fonte | 80 | Resolução média, wifi |
| 6 | 4:3, 640 x 480, tablet (ipad, Android), (800 Kbps) | 900 | _ Ipad_ 640 x 480_ 800 K | 800 | 640x480 | Igual à fonte | 80 | Resolução média, wifi |
| 7 | 16:9, 768 x 432, tablet (ipad, Android), (1200 Kbps) | 1.5 Mbps | _ Ipad_ 768 x 432_ 1200 K | 1200 | 768x432 | Igual à fonte | 96 | Alta resolução, wifi |
| 8 | 4:3, 768 x 576, tablet (ipad, Android), (1200 Kbps) | 1.5 Mbps | _ Ipad_ 768 x 576_ 1200 K | 1200 | 768x576 | Igual à fonte | 96 | Alta resolução, wifi |
| 9 | 16:9, 1280 x 720, Desktop, (2000 Kbps) | 3.0 Mbps | _ 1280 x 720_ 2000 K | 2000 | 1280x720 | Igual à fonte | 128 | Alta definição, widescreen |
| 10 | 4:3, 1280 x 960, Desktop, (2000 Kbps) | 3.0 Mbps | _ 1280 x 960_ 2000 K | 2000 Kbps | 1280x960 | Igual à fonte | 128 | Alta definição |

### Predefinições de codificação de vídeo para desktop {#desktop-video-encoding-presets}

Predefinições de codificação de vídeo para MP 4 e OGV em computadores desktop.

Para obter informações sobre os parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**H 264 Main 3.2 - Audio AAC, Extension file file extension**

|  | Texto da predefinição de codificação/dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recomendações |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps) | 500 | _ 480 x 270_ 400 K | 400 | 480x270 | Igual à fonte | 64 | Resolução de widescreen baixa |
| 2 | 16:9, 640 x 360 (800 Kbps) | 900 | _ 640 x 360_ 800 K | 800 | 640x360 | Igual à fonte | 80 | Resolução média de widescreen |
| 3 | 16:9, 800 x 450 (1200 Kbps) | 1.5 Mbps | _ 800 x 450_ 1200 K | 1200 | 800x450 | Igual à fonte | 96 | Resolução média de alta resolução |
| 4 | 16:9, 1280 x 720 (2000 Kbps) | 3.0 Mbps | _ 1280 x 720_ 2000 K | 2000 | 1280x720 | Igual à fonte | 128 | Alta definição, widescreen |
| 5 | 4:3, 320 x 240 (400 Kbps) | 500 | _ 320 X 240_ 400 K | 400 | 320x240 | Igual à fonte | 64 | Baixa resolução |
| 6 | 4:3, 480 x 360 (800 Kbps) | 900 | _ 480 x 360_ 800 K | 800 | 480x360 | Igual à fonte | 80 | Resolução média |
| 7 | 4:3, 640 x 480 (1200 Kbps) | 1.5 Mbps | _ 640 x 480_ 1200 K | 1200 | 640x480 | Igual à fonte | 96 | Resolução média de alta resolução |
| 8 | 4:3, 1280 x 960 (2000 Kbps) | 3.0 Mbps | _ 1280 x 960_ 2000 K | 2000 | 1280x960 | Igual à fonte | 128 | Alta definição |

**OGG Theora Vorbis - Extensão de arquivo OGV**

|  | Texto da predefinição de codificação/dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recomendações |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbps), OGG | 500 | _ OGG_ 480 x 270_ 400 K | 400 | 480x270 | Igual à fonte | 64 | Resolução de widescreen baixa |
| 2 | 16:9, 640 x 360 (800 Kbps), OGG | 900 | _ OGG_ 640 x 360_ 800 K | 800 | 640x360 | Igual à fonte | 80 | Resolução média de widescreen |
| 3 | 16:9, 800 x 450 (1200 Kbps), OGG | 1.5 Mbps | _ OGG_ 800 x 450_ 1200 K | 1200 | 800x450 | Igual à fonte | 96 | Resolução média de alta resolução |
| 4 | 16:9, 1280 x 720 (2000 Kbps), OGG | 3.0 Mbps | _ OGG_ 1280 x 720_ 2000 K | 2000 | 1280x720 | Igual à fonte | 128 | Alta definição, widescreen |
| 5 | 4:3, 320 x 240 (400 Kbps), OGG | 500 | _ OGG_ 320 X 240_ 400 K | 400 | 320x240 | Igual à fonte | 64 | Baixa resolução |
| 6 | 4:3, 480 x 360 (800 Kbps), OGG | 900 | _ OGG_ 480 x 360_ 800 K | 800 | 480x360 | Igual à fonte | 80 | Resolução média |
| 7 | 4:3, 640 x 480 (1200 Kbps), OGG | 1.5 Mbps | _ OGG_ 640 x 480_ 1200 K | 1200 | 640x480 | Igual à fonte | 96 | Resolução média de alta resolução |
| 8 | 4:3, 1280 x 960 (2000 Kbps), OGG | 3.0 Mbps | _ OGG_ 1280 x 960_ 2000 K | 2000 | 1280x960 | Igual à fonte | 128 | Alta definição |

### Predefinições de codificação de vídeos móveis {#mobile-video-encoding-presets}

Igual ao fps de origem. Predefinições de codificação de vídeo para dispositivos móveis iphone, ipad e Android.

Para obter informações sobre os parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Linha de base H 264 - Extensão de arquivo AAC, MP 4 de áudio**

|  | Texto da predefinição de codificação/dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de bits de vídeo (Kbps) | Largura/altura de pixels | Fps | Taxa de bits de áudio (Kbps) | Recomendações |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobile (400 Kbps) | 500 | _ Mobile_ 512 x 288_ 400 K | 400 | 512x288 | Igual à fonte | 64 | Baixa resolução, 3 G |
| 2 | 16:9, 512 x 288, Mobile (600 Kbps) | 700 | _ Mobile_ 512 x 288_ 600 K | 600 | 512x288 | Igual à fonte | 64 | Resolução média, 3 G |
| 3 | 16:9, 512 x 288, Mobile (800 Kbps) | 900 | _ Mobile_ 512 x 288_ 800 K | 800 | 512x288 | Igual à fonte | 80 | Resolução média, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobile (1000 Kbps) | 1.2 Mbps | _ Mobile_ 512 x 288_ 1000 K | 1000 | 512x288 | Igual à fonte | 80 | Alta resolução, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobile (1200 Kbps) | 1.5 Mbps | _ Mobile_ 512 x 288_ 1200 K | 1200 | 512x288 | Igual à fonte | 96 | Alta resolução, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobile (400 Kbps) | 500 | _ Mobile_ 384 x 288_ 400 K | 400 | 384x288 | Igual à fonte | 64 | Baixa resolução, 3 G |
| 7 | 4:3, 384 x 288, Mobile (600 Kbps) | 700 | _ Mobile_ 384 x 288_ 600 K | 600 | 384x288 | Igual à fonte | 64 | Resolução média, 3 G |
| 8 | 4:3, 448 x 336, Mobile (800 Kbps) | 900 | _ Mobile_ 448 x 336_ 800 K | 800 | 448x336 | Igual à fonte | 80 | Resolução média, Wi-Fi |
| 9 | 4:3, 448 x 336, Mobile (1000 Kbps) | 1.2 Mbps | _ Mobile_ 448 x 336_ 1000 K | 1000 | 448x336 | Igual à fonte | 80 | Alta resolução, Wi-Fi |
| 10 | 4:3, 448 x 336, Mobile (1200 Kbps) | 1.5 Mbps | _ Mobile_ 448 x 336_ 1200 K | 1200 | 448x336 | Igual à fonte | 96 | Alta resolução, Wi-Fi |

## Predefinições do visualizador {#viewer-presets}

>[!NOTE]
>
>**Aviso de fim da vida útil do Flash Viewers** - A partir de January 1 de janeiro de 21 17, o Sistema de publicação do Adobe Scene 7 terminou oficialmente o suporte à plataforma do visualizador Flash. Para obter mais informações sobre essa importante alteração, consulte o seguinte site de Perguntas frequentes: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Uma *predefinição* do visualizador é uma coleção de configurações que determinam como os usuários visualizam ativos de mídia avançada em telas de computador e dispositivos móveis. Como administrador, você pode criar Predefinições do visualizador. As configurações estão disponíveis para uma matriz de opções de configuração do visualizador. Por exemplo, você pode alterar o tamanho de exibição do visualizador, o comportamento de zoom, os esquemas de cores, as bordas e as fontes.

Como prática recomendada, use visualizadores de vídeo HTML 5 de Dynamic Media clássica. As predefinições usadas nos visualizadores de vídeo HTML 5 são players de vídeo robustos. Ao combinar em um único player a capacidade de projetar os componentes de reprodução usando HTML 5 e CSS, ter reprodução incorporada e usar streaming adaptável e progressivo, dependendo do recurso do navegador, você estende o alcance do conteúdo de mídia avançada para os usuários de desktop, tablet e móvel e garante uma experiência de vídeo simplificada.

Consulte [Sobre visualizadores HTML 5](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) no Guia de referência de visualizadores da Adobe.

Consulte [Matriz de compatibilidade do Visualizador de mídia do Dynamic Media clássica](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consulte [a prática recomendada: Uso do visualizador de vídeo HTML 5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependendo do visualizador, você pode adicionar recursos da comunidade. Os recursos da Comunidade incluem um botão Incorporar, botão de email, botão Link e o botão Site de visita. Esses botões permitem que as pessoas que usam os visualizadores compartilham o visualizador com outras pessoas ou abram o site da Web do Dynamic Media.

Consulte também [Exemplos de biblioteca de referência de visualizadores da Adobe](https://marketing.adobe.com/resources/help/en_US/s7/vlist/vlist.html).

### Suporte do visualizador para páginas da Web projetadas responsivas {#viewer-support-for-responsive-designed-web-pages}

Diferentes páginas da Web têm necessidades diferentes. Às vezes, você desejará uma página da Web que forneça um link que abre o visualizador HTML 5 em uma janela separada do navegador. Em outros casos, pode ser necessário incorporar o Visualizador HTML 5 diretamente na página de hospedagem. No último caso, a página da Web pode ter um layout estático. Ou pode ser "responsivo" e exibido de forma diferente em diferentes dispositivos ou em diferentes tamanhos de janela do navegador. Para acomodar essas necessidades, os visualizadores HTML 5 que vêm com o Dynamic Media Classic oferecem suporte para páginas da Web estáticas e páginas da Web projetadas responsivas.

Consulte [Biblioteca](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)de imagem estática responsiva na Ajuda da API de disponibilização de imagens *da Adobe* para obter mais informações sobre como incorporar visualizadores responsivos em suas páginas da Web.

### Tipos predefinidos do visualizador {#viewer-preset-types}

Os administradores podem criar e personalizar os seguintes tipos de Predefinições do visualizador:

**O Visualizador** do ecatalog Simula a experiência de ler um catálogo impresso. É possível mover de uma página para a outra, aumentar ou diminuir o zoom dos itens em uma página, usar mapas de imagem para ver mais informações sobre os itens na página ou pesquisar o catálogo. Você também pode incluir um Painel Informações para exibir informações detalhadas e um item mapeado de imagem se a área do mapa tiver um atributo de rollover_ key válido. Para incluir um Painel Informações, especifique um URL do servidor de informações no painel Configurações do painel Informações da janela Predefinição do visualizador do ecatalog.

**Visualizador de conjunto** de amostras Exibe uma imagem em uma cor, material, textura, conclusão ou tecido diferente. Os usuários clicam em uma miniatura para ver as variações na imagem.

**Visualizador de conjunto de mídias mistas** Exibe tipos diferentes de mídia em um visualizador. É possível incluir Conjuntos de amostras, Conjuntos de rotação, imagens e vídeos. É possível configurar guias para conter tipos diferentes de conteúdo, como uma guia para conjuntos de imagens e uma guia para vídeos. Vídeos reproduzidos de um conjunto de mídia mista usam um visualizador de vídeo padrão com controles de linha do tempo e vídeo, como Parar, Pausar, Rewind e Reproduzir. Ao configurar uma predefinição do Conjunto de mídia mista, você especifica quais visualizadores deseja usar para os diferentes tipos de ativos no Conjunto de mídia mista. Você também pode usar o Visualizador de grade ou o Carrossel do carrossel para exibir um Conjunto de mídia misto.

**Visualizador** de conjunto de rotação Fornece várias exibições de uma imagem para que os usuários possam girar o objeto para examinar os diferentes lados e ângulos.

**O visualizador** de vídeo exibe vídeos usando as dimensões de resolução do arquivo de origem ou um tamanho personalizado. O Dynamic Media Classic vem com muitas predefinições pré-definidas do visualizador para reprodução de vídeo e, se for um administrador, você pode criar predefinições personalizadas do Video Viewer. Há mais de uma dezena de configurações diferentes para configurar o Visualizador de vídeo. Você pode configurar seu tamanho, a cor em primeiro e segundo plano, os controles de vídeo e áudio, a barra de progresso, a capa da interface do usuário, os recursos sociais e a Ajuda.

**Os visualizadores** de zoom oferecem uma escolha de três tipos de visualizador de zoom:

**O Zoom do visualizador** permite que os usuários aumentem a zoom na área clicando nela. Eles podem clicar em controles para aumentar o zoom, reduzir o zoom e redefinir a imagem para o tamanho padrão.

**Visualizador de zoom: Fly-out** Exibe uma segunda imagem da área ampliada ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção sobre a área que desejam visualizar.

Ao determinar o uso de largura de banda completo para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem principal (largura e altura do palco) e o fator de zoom determinam o tamanho da imagem em flyout. Para impedir que o tamanho do arquivo flyout fique muito grande, equilibre estes dois valores: se você tiver um tamanho de imagem principal grande, reduza o valor do fator de zoom. (A Largura Flyout e a Altura do Flyout determinam o tamanho da janela flyout, mas não o tamanho da imagem flyout que é servida no visualizador.)

Por exemplo, se o tamanho da imagem principal for de 350 em 350 pixels, com um fator de zoom igual a 3, a imagem resultante será de 1050 em 1050 pixels. Se o tamanho da imagem principal for de 300 em 300 pixels, com um fator de zoom de 4, a imagem flyout será de 1200 em 1200 pixels. Dependendo da configuração de qualidade JPEG (configurações recomendadas estão entre 80-90), é possível diminuir significativamente o tamanho do arquivo. Os fatores de zoom recomendados são de 2.5 a 4, dependendo do tamanho da imagem principal.

### Matriz de compatibilidade do visualizador do Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Aviso de fim de vida do visualizador Flash**: A partir de January 1 de janeiro de 21 17, o Sistema de publicação do Adobe Scene 7 terminou oficialmente o suporte à plataforma do visualizador Flash.

Para obter mais informações sobre essa importante alteração, consulte o seguinte site de Perguntas frequentes: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

A tabela a seguir identifica as Predefinições do visualizador do Dynamic Media clássica disponíveis no momento. A tabela também especifica a compatibilidade do visualizador com dispositivos móveis e dispositivos móveis, e a tecnologia usada para cada visualizador.

Consulte também [Exemplos de biblioteca de referência de visualizadores da Adobe](https://marketing.adobe.com/resources/help/en_US/s7/vlist/vlist.html).

Para obter informações sobre o navegador da Web suportado e versões do sistema operacional para Visualizadores, você pode revisar as Notas de versão dos visualizadores.

Consulte [Notas de versão de referência dos visualizadores da Adobe](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Zoom de visualizadores |  |  |  |  |  |  |
| Universal_ HTML 5_ Flyout | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ Zoom_ inline | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ Zoom_ escuro | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ Zoom_ light | HTML5 | X | X | X | X | X |


|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de conjunto de imagens |  |  |  |  |  |  |
| Universal_ HTML 5_ Flyout | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ imageset_ dark | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ imageset_ light | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de conjunto de amostras |  |  |  |  |  |  |
| Universal_ HTML 5_ Flyout | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ swatchset_ dark | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ swatchset_ light | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do ecatalog |  |  |  |  |  |  |
| Universal_ HTML 5_ ecatalog_ Adv (inclui suporte para a pesquisa social e a pesquisa de catálogo.) | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ ecatalog (inclui suporte para a pesquisa em redes sociais e pesquisa de catálogo.) | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de rotação |  |  |  |  |  |  |
| Universal_ HTML 5_ spinset_ dark | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ spinset_ light | HTML5 | X | X | X | X | X |

**Visualizadores evideo**

O Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP 4 H .264.

* É possível encontrar dispositivos Blackberry compatíveis com este formato de vídeo: [Formatos de vídeo suportados no Blackberry](https://docs.blackberry.com/en/smartphone_users/deliverables/18349/711-01774-123_Supported_Media_Types_on_BlackBerry_Smartphones.pdf)
* Também é possível encontrar dispositivos Windows compatíveis com este formato de vídeo:[Formatos de vídeo suportados no Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx)

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android | Blackberry Smartphone | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_ HTML 5_ Video (inclui suporte para legendas ocultas.) Consulte [a prática recomendada: Usar o visualizador de vídeo HTML 5 universal.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_ HTML 5_ Video_ social (inclui suporte para legendagem e mídia social ocultas.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de conjunto de mídia mista |  |  |  |  |  |  |
| Universal_ HTML 5_ mixedmedia_ dark | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ mixedmedia_ light | HTML5 | X | X | X | X | X |

### Matriz de gestos de visualizadores móveis compatíveis {#supported-mobile-viewers-gestures-matrix}

A tabela a seguir identifica os gestos do visualizador móvel compatíveis com dispositivos iOS, Android 2. x e Android 3. x.

|  | Tecnologia do visualizador | Área de trabalho | Apple iphone | Apple ipad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de conjunto de imagens |  |  |  |  |  |  |
| Universal_ HTML 5_ Flyout | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ imageset_ dark | HTML5 | X | X | X | X | X |
| Universal_ HTML 5_ imageset_ light | HTML5 | X | X | X | X | X |

### Sobre a tela Predefinição do visualizador {#about-the-viewer-preset-screen}

Crie e gerencie Predefinições do visualizador na tela Predefinições do visualizador. Para abrir esta tela, clique **em Configuração** &gt; **Predefinições do visualizador**.

A tela Predefinições do visualizador oferece ferramentas para executar essas tarefas:

**Adicionar uma predefinição** Clique em Adicionar e faça escolhas na caixa de diálogo Adicionar predefinição do visualizador.

Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

**Editar uma predefinição** Selecione uma predefinição e clique **em Editar**.

Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

**Excluir uma predefinição** Selecione uma predefinição e clique **em Excluir**.

**Exportar uma predefinição** Selecione uma predefinição do visualizador HTML 5 e clique em Exportar para fazer download da capa do visualizador para que você possa usá-la como a base para criar e adicionar uma nova predefinição do visualizador.

Consulte [Exportar uma predefinição do visualizador HTML 5](application-setup.md#exporting_an_html5_viewer_preset).

**Filtrando a lista Predefinição do visualizador** Use estas ferramentas para filtrar a lista:

* Abra a lista suspensa **Ativo/Inativa** e escolha uma opção para mostrar predefinições ativas, predefinições inativas ou todas as predefinições.
* Abra a **lista** suspensa Visualizador e escolha uma opção para visualizar somente os visualizadores de determinado tipo. Escolha **Todos os visualizadores** para visualizar todos os visualizadores.

**Classificação de predefinições** Clique em um cabeçalho de coluna (Ativa, Tipo, Predefinição ou Plataforma) para classificar a lista em uma coluna. Clique no cabeçalho da coluna uma segunda vez para classificar a lista em ordem decrescente (ou crescente).

**Ativar e desativar predefinições** Selecione uma predefinição e clique na opção Ativa para ativá-la ou desativá-la.

Consulte [Ativação ou desativação das predefinições do visualizador](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Clique em Visualizar no lado direito da tela Predefinições do visualizador para ver como será um ativo na Predefinição do visualizador selecionada. Para ver um ativo diferente, clique em Procurar na tela Predefinições do visualizador e selecione um ativo diferente na caixa de diálogo Selecionar visualização do ativo.

### Adicionar e editar predefinições do visualizador {#adding-and-editing-viewer-presets}

Além de adicionar predefinições do visualizador usando Adicionar na interface do usuário, você também pode usar Exportar para adicionar uma predefinição do visualizador. Basta exportar uma predefinição do visualizador HTML 5 existente e usá-la como a base para a nova predefinição.

Consulte [Exportar uma predefinição do visualizador HTML 5](application-setup.md#exporting_an_html5_viewer_preset).

**Para adicionar e editar predefinições do visualizador**

1. Próximo ao canto superior direito do Sistema de publicação Scene 7, clique **em Configuração** &gt; Predefinições **do visualizador**.

   Você pode filtrar pela lista de predefinições. Por exemplo, para ver apenas predefinições para Visualizadores de vídeo, selecione Visualizador de vídeo no menu suspenso Visualizadores na barra de ferramentas diretamente acima da tabela.

1. Na tela Predefinições do visualizador, adicione ou edite a Predefinição do visualizador na tela Predefinições do visualizador.

   **Adicionar** clique em Adicionar na barra de ferramentas. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma e escolha um tipo de ativo de mídia avançada.

   Clique **em Salvar como** quando terminar de criar a Predefinição do visualizador.

   **Adicionar ao iniciar com uma Predefinição do visualizador** existente na tabela, selecione uma Predefinição do visualizador de vídeo e clique em Editar na barra de ferramentas.

   Depois de reconfigurar o Visualizador de vídeo, clique **em Salvar como** para salvar a predefinição usando um nome diferente no campo de texto Nome predefinido.

   **Edição** Selecione uma Predefinição do visualizador existente e clique **em Editar**.

1. Na tela Configurar visualizador, no campo Nome predefinido, insira ou edite o nome predefinido.
1. Defina as opções restantes desejadas.

   >[OBSERVAÇÃO]
   >
   >Escolha o mesmo que a fonte para dimensionar automaticamente o visualizador de vídeo para o tamanho de resolução do próprio vídeo codificado. Se escolher essa opção, não será possível inserir a Largura do palco e a Altura do palco. Em vez disso, essas opções vêm do próprio vídeo. Se escolher Igual como Fonte, defina a opção Tamanho da margem para refletir as dimensões de capa fora da área de reprodução do vídeo. Esse tamanho de margem é a altura e a largura de pixels dos controles de vídeo. Você pode usar a ilustração a seguir para ajudar a determinar os tamanhos de margem que deseja usar.*

   ![](assets/vs_video_viewer_configure_margin.png)

1. Execute um dos procedimentos a seguir:

   * Clique **em Salvar como** se você tiver adicionado uma predefinição do visualizador, começando por uma predefinição existente.
   * Clique **em Salvar** se tiver adicionado ou editado uma predefinição do Visualizador.

### Exportar uma predefinição do visualizador HTML 5 {#exporting-an-html-viewer-preset}

Você pode exportar uma Predefinição do visualizador HTML 5 existente para usar como a base para criar uma nova Predefinição do visualizador HTML 5. Essa opção de exportação é útil porque não é necessário criar o visualizador do zero. Em vez disso, você exporta uma predefinição que se comporta e se comporta perto do que você deseja, em seguida, pode usá-la como um ponto de partida para fazer ajustes de design.

Observe que todos os arquivos CSS predefinidos do visualizador de pré-lançamento no SPS usam caminhos de fornecimento de imagem relativos que apontam para ativos localizados `Scene7SharedAssets`. Por exemplo, este é um caminho relativo para um ativo de imagem em um arquivo CSS predefinido do visualizador, localizado em `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`No entanto, se estiver hospedando arquivos CSS do visualizador em seu próprio site, você deve resolver esse caminho de imagem relativo usando um caminho explícito para o Servidor de imagens em seu próprio ambiente. Para fins de ilustração, se você atualizasse o caminho relativo acima para um caminho explícito, ele seria semelhante ao seguinte, onde `https://s7d1.scene7.com` é o caminho direto para o servidor de imagem: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar uma predefinição do visualizador HTML 5**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Clique **em Configuração** &gt; **Predefinições do visualizador**.
1. Na barra de ferramentas Predefinições do visualizador, na segunda lista suspensa à esquerda, selecione **HTML 5**.
1. Na terceira lista suspensa à esquerda, selecione **Todos os visualizadores**.
1. Selecione a predefinição do visualizador que deseja usar como a base para uma nova Predefinição do visualizador HTML 5.
1. Na barra de ferramentas, clique **em Exportar**.
1. Na caixa de diálogo Exportar ativos selecionados, clique **em Enviar exportação**.

   A seguir, você receberá um arquivo CSS. Baixe e descompacte o arquivo.

1. Abra o arquivo CSS em um editor de CSS, faça as alterações e salve o arquivo.
1. Carregue o arquivo CSS no Sistema de publicação Scene 7.

   Consulte [Carregamento de arquivos](uploading-files.md#uploading_files).

1. Publique o arquivo CSS no Servidor de imagem do Dynamic Media.

   Consulte [Publicação de arquivos](publishing-files.md#publishing_files).

1. Adicione a nova predefinição do visualizador como de costume. Selecione o arquivo CSS do visualizador que você carregou.

   Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

### Ativar ou desativar predefinições do visualizador {#activating-or-deactivating-viewer-presets}

Para criar um URL para mostrar ativos, os usuários abrem a lista suspensa Predefinições na caixa de diálogo Visualizar, selecionam uma Predefinição do visualizador e clicam em Copiar URL (consulte [Copiar o URL de uma Predefinição do visualizador](application-setup.md#copying_the_url_of_a_viewer_preset)). Essa lista de Predefinições oferece predefinições do visualizador que os administradores adicionam e são gerenciados na tela Predefinições do visualizador. Por exemplo, todas as predefinições ativas do ecatalog Viewer aparecem na lista suspensa Predefinições na caixa de diálogo Visualizar quando um usuário visualiza um ecatalog.

A menos que você desative Predefinições do visualizador na tela Predefinições do visualizador, a lista suspensa Predefinições na caixa de diálogo Visualizar pode ser exibida.

**Para ativar ou desativar Predefinições do visualizador**

1. Escolha **Configuração** &gt; **Predefinições do visualizador** para abrir a tela Predefinições do visualizador.
1. Selecione ou desmarque opções Ativas para ativar ou desativar as Predefinições do visualizador.

### Copiando o URL de uma predefinição do visualizador {#copying-the-url-of-a-viewer-preset}

Depois de publicar um ativo, você pode copiar um URL para exibir o ativo com as configurações de uma Predefinição do visualizador.

O URL é copiado para a Área de transferência. Você pode usá-lo conforme necessário no código HTML da sua página da Web, dispositivo móvel ou aplicativo.

**Para copiar o URL de uma predefinição do visualizador**

1. Selecione o ativo no Painel Procurar.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade**. No painel Navegador de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. Nos urls e no painel Incorporar código à direita, clique **em Copiar URL** à direita do visualizador desejado.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Copiar URL**.

### Copiando o código incorporado de uma predefinição do visualizador {#copying-the-embed-code-of-a-viewer-preset}

Usar o recurso Incorporar código permite analisar o código do visualizador da Predefinição do visualizador selecionado. Também é possível copiar o código para a área de transferência para que você possa colá-lo em suas páginas da Web para implantação do visualizador.

A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de uma predefinição do visualizador**

1. Selecione o ativo no Painel Procurar ativo.
1. Acima do painel Navegador de ativos, no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Clique **em Exibição de grade**. No painel Navegador de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel urls à direita, clique em **Incorporar código**.
   * Clique **em Exibição de grade**. No painel Procurar ativo, selecione um único ativo e depois abaixo da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

   * Clique **em Exibição de lista**. No painel Procurar ativo, selecione um único ativo e, à direita da imagem em miniatura, clique **em Visualizar** &gt; Lista **do visualizador**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

   * Clique **em Exibição de grade**, **Exibição de lista** ou Exibição **de detalhes**. Na mesma barra de ferramentas, clique **em Visualizar** &gt; Lista **de visualizadores**.
   Na página Lista do visualizador, na coluna Ações da tabela, clique **em Incorporar código**.

1. Na caixa de diálogo Incorporar código, clique **em Copiar para a área de transferência**.
1. Clique **em Fechar**.

## Configuração de Visualizadores Padrão {#configuring-default-viewers}

Você pode usar os Visualizadores padrão para configurar o visualizador padrão associado a um ativo ao usar a opção Visualizar no sistema de publicação do Scene 7. Você pode configurar a experiência de visualização padrão para os seguintes tipos de ativos:

* Imagem
* Vídeo
* Spinset
* Catálogo
* Imageset
* Swatchset
* Mediaset

**Para configurar visualizadores padrão**

1. Na lista suspensa Configuração, clique **em Configuração do aplicativo**.
1. Na janela Configuração, no painel esquerdo, expanda Configuração **de aplicativo** &gt; **Visualizadores**
1. Clique **em Visualizadores padrão**.
1. Na janela Visualizadores padrão, na lista suspensa para cada tipo de ativo, selecione o visualizador que deseja associar à visualização do ativo.
1. No canto inferior direito da janela Visualizadores padrão, clique **em Salvar configurações**.
1. No canto inferior direito da janela Configuração, clique **em Fechar** para retornar à janela Ativo.

## Exibições de metadados {#metadata-views}

*Os metadados* são informações padronizadas sobre um ativo. Você pode usar metadados para simplificar seu fluxo de trabalho, organizar seus ativos e melhorar a pesquisa. O Dynamic Media Classic é compatível com o padrão IPTC (International Press Telecommunications Council) e o padrão XMP (extensible metadata platform). Antes dos usuários visualizarem ou inserirem metadados sobre um ativo na exibição Detalhe, poderão abrir o menu Exibições de metadados e escolher o conjunto de campos de metadados que deseja visualizar ou usar para descrever o ativo.

O Dynamic Media Classic vem com Exibições de metadados pré-definidas, e os administradores podem criar suas próprias Exibições de metadados para que os usuários escolham quando inserem metadados.

### Criação de uma exibição de metadados {#creating-a-metadata-view}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Exibições** de metadados.
1. Clique **em Adicionar**.
1. No campo de texto Nome predefinido, insira um nome para a exibição.
1. (Opcional) Marque **Tornar padrão** para tornar essa exibição aquela que os usuários veem quando abrirem o painel Metadados na Visualização de detalhes.
1. (Opcional) Selecione **Incluir UDF** para incluir campos definidos pelo usuário na visualização. Os campos definidos pelo usuário aparecem na parte superior do painel Metadados na Exibição de detalhes.
1. Selecione os campos que deseja exibir (clique **em Selecionar tudo** para selecionar todos os campos).
1. Clique **em Salvar**.

   As categorias e os campos selecionados para a exibição aparecem no painel Visualização.

### Gerenciamento de exibições de metadados {#managing-metadata-views}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Exibições** de metadados.
1. Execute um dos procedimentos a seguir:

   * Para visualizar uma exibição, selecione-a. Os campos na exibição aparecem no painel Visualização.
   * Para editar uma exibição, selecione-a e clique **em Editar**. Em seguida, marque ou desmarque os nomes de campo no painel Visualização e selecione ou desmarque **a** opção Incluir UDF.
   * Para excluir uma exibição, selecione-a e clique **em Excluir**.
   * Para exibir o padrão, selecione-o e clique **em Tornar padrão**. A exibição padrão é aquela que os usuários veem quando abrem um ativo na exibição Detalhe e vão para o painel Metadados.

## Predefinições de metadados {#metadata-presets}

As predefinições de metadados fornecem aos administradores uma maneira de controlar e inspecionar os metadados atribuídos aos ativos. Na exibição de Detalhes, um usuário pode inserir metadados sobre um ativo nos campos fornecidos para esse propósito. Por exemplo, um usuário pode inserir um nome de proprietário, descrição de copyright e endereço. Para garantir que os usuários insiram essas informações com precisão e total, você pode criar Predefinições de metadados. Escolher uma predefinição de metadados na exibição Detalhe preenche campos de metadados com valores pré-definidos. Por exemplo, um nome de proprietário, descrição de copyright e endereço são inseridos automaticamente.

Crie uma Predefinição de metadados para cada conjunto de valores de metadados que deseja que os usuários possam digitar automaticamente na exibição Detalhe para descrever um ativo.

### Criação ou edição de uma predefinição de metadados {#creating-or-editing-a-metadata-preset}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Predefinições** de metadados.
1. Na tela Predefinições de metadados, execute um dos seguintes procedimentos:

   * Para criar uma predefinição, clique **em Adicionar**. No campo de texto Nome do modelo de metadados, digite um nome para a predefinição e clique em Exibições **de metadados** e escolha uma exibição na lista suspensa (consulte Exibições [de metadados](application-setup.md#metadata_views)).
   * Para editar uma predefinição existente, selecione a predefinição na lista Predefinições de metadados e clique **em Editar**.

1. Expanda os cabeçalhos que deseja incluir na predefinição e digite os valores nos diferentes campos que deseja incluir na predefinição.
1. Clique **em Salvar**.

   As categorias e os campos selecionados para a predefinição aparecem no painel Visualização.

### Gerenciamento de Predefinições de Metadados {#managing-metadata-presets}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Predefinições de metadados**.
1. Execute um dos procedimentos a seguir:

   * Para visualizar uma predefinição, selecione a predefinição que deseja visualizar. As informações predefinidas (categorias e campos) aparecem na tela Visualizar.
   * Para excluir uma predefinição, selecione a predefinição e clique **em Excluir**.

## Campos definidos pelo usuário {#user-defined-fields}

Um administrador do portal de mídia ou um administrador de empresa pode criar campos de metadados definidos pelo usuário personalizado. Os campos personalizados podem ajudar a organizar ativos no Sistema de publicação Scene 7. Você pode marcar os campos como Ativo, conforme necessário. Quando ativados, os nomes desses campos de metadados personalizados aparecem no painel Metadados na exibição Detalhe. Os usuários podem inserir informações em campos de metadados definidos pelo usuário para descrever ativos. Os usuários também podem tornar um campo de metadados definido pelo usuário um critério em pesquisas.

Um uso eficaz dos campos de metadados definidos pelo usuário é atrasar o tempo de ativação de um ativo para uma inicialização ou venda específica. Você define um campo de «ativação», com base no tipo *Data*. Em seguida, usando o painel **Metadados** na **exibição de Detalhes** ou **Arquivo** &gt; **Editar informações**, você pode especificar quando o ativo é ativado. O Scene 7 Publishing System verifica o status de publicação de um ativo e o histórico de publicação. Se não estiver dentro do tempo de ativação, o status de publicação será exibido como «Não publicado».

>[!NOTE]
>
>Para tornar os campos definidos pelo usuário no painel Metadados na exibição Detalhe, inclua campos definidos pelo usuário nas Exibições de metadados. Na tela Exibições de metadados, selecione a opção Incluir UDF (campos definidos pelo usuário). Para obter mais informações, consulte [Exibições](application-setup.md#metadata_views)de metadados.

>[!NOTE]
>
>Para pesquisar ativos usando campos personalizados e definidos pelo usuário, clique **em Configuração** &gt; **Configuração** pessoal e selecione **Incluir udfs na Pesquisa**. Consulte [Configuração pessoal](personal-setup.md#personal_setup).

### Criação de um campo de metadados definido pelo usuário {#creating-a-user-defined-metadata-field}

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Campos definidos pelo usuário**.
1. Clique **em Adicionar**
1. Na caixa de diálogo Campo personalizado, defina as opções desejadas.

   **Nome** Digite um nome para o campo de metadados.

   **Digite** uma opção que define o tipo de informação que os usuários podem digitar no campo de metadados:

   **String** Uma string de texto.

   **Int** um número inteiro.

   **Flutuar** um número de ponto flutuante flutuante.

   **Sim/Não** um valor booliano sim/não.

   **Data** Uma data. O formato MM/DD/AAAA é aceito.

   **Nome do arquivo** O nome de um arquivo.

   **Cor** O nome de uma cor.

   **Dimensão** A largura e a altura do ativo.

   **Sem título** para compatibilidade retroativa. Não selecione essa opção.

   **Valor padrão** opcionalmente, digite o valor que os usuários têm maior probabilidade de digitar no campo. O valor inserido se torna o valor padrão do campo criado.

   **Se aplica a** opção Opcionalmente, escolha um tipo de ativo se desejar que o campo de metadados seja aplicado somente a um tipo específico de ativo.

   ***Observação**: Escolha uma **opção Aplicar a** cuidadosamente, pois não é possível alterar a **opção Aplicar a** depois de criar um campo definido pelo usuário. O Dynamic Media Classic permite editar o nome, tipo e valor padrão de um campo definido pelo usuário, mas não a **configuração Aplicar a** . *

1. Clique **em Salvar** quando terminar de criar o campo de metadados.

### Gerenciar campos definidos pelo usuário {#manage-user-defined-fields}

A tela Campos definidos pelo usuário oferece comandos para gerenciar campos de metadados personalizados e definidos pelo usuário.

Somente um administrador do portal de mídia ou um administrador de empresa podem gerenciar campos definidos pelo usuário.

Para abrir esta tela, clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Metadados** &gt; **Campos definidos pelo usuário**.

**Editar um campo** Selecione o campo e clique **em Editar**.

**Excluir um campo** Selecione o campo e clique **em Excluir**.

**Ativar campo** Clique para selecionar ou desmarcar a opção Ativa ao lado do nome de um campo. Se você estiver na função de administração da empresa, esta opção talvez não seja exibida. Como essa opção está relacionada ao mediaportal, é necessário selecionar (ativar) Recursos mediaportal em Configuração pessoal para ver os campos ativados.

## Otimizar arquivos {#optimize-files}

À medida que você carrega arquivos para o Sistema de publicação Scene 7, o sistema os otimiza para armazenamento e publicação. No entanto, se o processo de upload for interrompido, algumas imagens não poderão ser otimizadas. Nesse caso, você verá a mensagem «Imagem ainda não otimizada». No entanto, você pode otimizar esses arquivos se for um administrador.

O Scene 7 Publishing System pesquisa os arquivos e otimiza apenas aquelas que não foram totalmente otimizadas antes.

1. Escolha **Configuração** &gt; **Configuração** do aplicativo e selecione Otimizar **arquivos**.
1. Insira informações para o trabalho de otimização e clique **em Enviar**.

   Se estiver trabalhando com mais de uma empresa, otimize arquivos pertencentes a empresas diferentes separadamente.

## Predefinições de conjunto em lote {#batch-set-presets}

Use as predefinições de conjunto de lote para criar automaticamente conjuntos de imagens ou conjuntos de rotação enquanto uma tarefa está em execução para carregar ativos para o Sistema de publicação Scene 7.

Os administradores da empresa primeiro definem as convenções de nomenclatura para os ativos que desejam agrupar em conjunto em um conjunto. Em seguida, você pode criar uma predefinição definida para fazer referência a essas imagens. Cada predefinição é um conjunto exclusivo de instruções autodefinidas, que define como construir o conjunto usando imagens que correspondem às convenções de nomenclatura definidas na fórmula predefinida.

Todas as predefinições de conjunto de lote ativas de uma empresa estão listadas na caixa de diálogo Carregar opção de trabalho, para que você possa especificar qual predefinido você deseja aplicar durante cada sessão de upload. Os administradores da empresa veem todas as predefinições de conjunto de lote ativas e inativas. Quando você carrega arquivos, o Dynamic Media Classic cria automaticamente um conjunto com todos os arquivos que correspondem à convenção de nomenclatura definida nas predefinições ativas.

### Nomeação padrão {#default-naming}

O administrador da empresa cria uma convenção de nomenclatura padrão usada em qualquer fórmula predefinida de conjunto de lote. A convenção de nomenclatura padrão selecionada na definição predefinida do conjunto de lote pode ser necessária para que a sua empresa gere conjuntos de conjuntos para todos os sites. Uma predefinição de conjunto de lote é criada para usar a convenção de nomenclatura padrão definida. Você pode criar quantas predefinições de Conjunto de lote com convenções de nomenclatura alternativas e alternativas necessárias para um conjunto específico de conteúdo nos casos em que há uma exceção à nomeação padrão definida pela empresa.

Embora a configuração de uma convenção de nomenclatura padrão não seja necessária para usar a funcionalidade predefinida de conjunto de lote, a prática recomendada recomenda que você use a convenção de nomenclatura padrão para definir quantos elementos da convenção de nomenclatura você deseja agrupar em um conjunto para simplificar a criação do conjunto de lote.

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de conjunto em lote** &gt; **Nomeação padrão**.
1. Selecione **Exibir formulário** ou **Exibir código** para especificar como você deseja visualizar e inserir informações sobre cada elemento.

   É possível marcar a caixa de seleção Código de exibição para exibir o valor da expressão regular ao lado das seleções de formulário. Você poderá inserir ou alterar esses valores para ajudar a definir os elementos da convenção de nomenclatura, se a exibição do formulário limitar você por qualquer motivo. Se os valores não puderem ser analisados na exibição do formulário, os campos do formulário se tornarão inativos.

   >[!NOTE]
   Campos de formulário desativados não indicam uma expressão regular inválida. Não há validação de que suas expressões regulares estão corretas. Você verá os resultados da expressão regular que está criando para cada elemento depois da linha Resultado. A expressão regular completa está visível na parte inferior da página.

1. Expanda cada elemento conforme necessário e insira as convenções de nomenclatura que deseja usar.
1. Conforme necessário, clique **em Adicionar** para adicionar outra convenção de nomenclatura para um elemento. Ou clique **em Remover** para excluir uma convenção de nomeação de um elemento.
1. Clique **em Salvar como** e digite um nome para a predefinição. Ou clique **em Salvar** se estiver editando uma predefinição existente.

Como alternativa, você pode usar o Código de exibição sem campos de formulário disponíveis. Nesta exibição, você cria as definições de convenção de nomenclatura totalmente usando expressões regulares.

Dois elementos estão disponíveis para definição, Correspondência e Nome da Base. Esses campos permitem definir todos os elementos de uma convenção de nomenclatura e identificar a parte da convenção usada para nomear o conjunto em que estão contidos. A convenção de nomenclatura individual de uma empresa pode usar uma ou mais linhas de definição para cada um desses elementos. Você pode usar tantas linhas para sua definição exclusiva e agrupá-las em elementos distintos, como para Imagem principal, elemento Colorido, Elemento de Exibição alternativo e Elemento de amostra.

### Criação de uma predefinição de conjunto de lote {#creating-a-batch-set-preset}

O Dynamic Media Classic usa predefinições de conjunto de lote para organizar ativos que compartilham algumas informações ou conteúdos comuns em conjuntos de imagens para exibição nos visualizadores. As fórmulas predefinidas definidas por lote são executadas automaticamente juntamente com as tarefas de importação de ativos programadas no Dynamic Media Classic.

Use a Predefinição de lote em lote para criar, editar e gerenciar as predefinições de conjunto de lote. Você pode criar quantas predefinições de lote forem necessárias para cobrir todas as tarefas de ingestão de ativos necessárias. Há duas formas de definições predefinidas de conjunto de lote: uma para obter uma convenção de nomeação padrão que pode ter sido configurada e outra para convenções de nomeação personalizadas criadas dinamicamente.

É possível usar o método de campo de formulário para definir uma predefinição de conjunto de lote ou o método de código, que permite que você use expressões regulares. Como na Nomeação padrão, você pode escolher a Exibição de código ao mesmo tempo que está definindo na Exibição de formulário e no uso de expressões regulares para criar suas definições. Como alternativa, você pode desmarcar a exibição para usar um ou o outro exclusivamente.

Consulte também [Criar uma predefinição de lote para a geração automática de um Conjunto de rotação 2 D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Para criar uma predefinição de conjunto de lote**

1. Clique **em Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de conjunto em lote** &gt; **Predefinição de conjunto em lote**. **Exibir formulário**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista predefinida, clique **em Adicionar** para ativar os campos de definição no painel Detalhes no lado direito da tela.
1. No painel Detalhes, no campo Nome predefinido, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione um tipo predefinido.

   Para gerar automaticamente um Conjunto de rotação 2 D, selecione **Conjunto** de rotação de vários eixos na lista suspensa Tipo de conjunto de lote.

1. Execute um dos procedimentos a seguir:

   * Se você estiver usando uma convenção de nomenclatura padrão configurada anteriormente em Configuração do aplicativo &gt; Predefinições de conjunto em lote &gt; Nomeação padrão, expanda **Convenções** de nomeação de ativo e, na lista suspensa Nomenclatura de arquivo, clique **em Padrão**.
   * Para definir uma convenção de nomenclatura à medida que configurar a predefinição, expanda **Convenções de nomeação de ativos** e, na lista suspensa Nomenclatura de arquivo, clique **em Personalizado**.

1. Para Ordem de sequência, defina a ordem das imagens depois que o conjunto é agrupado no Dynamic Media Classic. Por padrão, os ativos são ordenados em ordem alfabética. No entanto, você pode usar uma lista separada por vírgulas de expressões regulares para definir a ordem.
1. Para Definir convenção de nomenclatura e criação, especifique o sufixo ou o prefixo ao nome básico definido na Convenção de nomenclatura de ativo. Também define onde o conjunto de imagens será criado na estrutura de pastas do Dynamic Media Classic.

   Se você definir um número grande de conjuntos de imagens, talvez prefira mantê-los separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados em lote aqui.

1. Clique **em Salvar** no painel Detalhes.

### Criação de uma predefinição de lote para a geração automática de um Conjunto de rotação 2 D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Você pode usar o Conjunto de rotação **de vários eixos em lote definido** para criar uma «receita» que automatiza a geração de conjuntos de rotação 2 D. O agrupamento de imagens usa expressões regulares de Linha e Coluna para que os itens de imagem sejam alinhados corretamente no local correspondente na matriz multidimensional.

Consulte [também Criação de uma predefinição de conjunto de lote](application-setup.md#creating_a_batch_set_preset).

Não há um número mínimo ou máximo de linhas ou colunas que você deve ter em um conjunto de rotação de vários eixos.

Como exemplo, suponha que você queira criar um conjunto de rotação de vários eixos chamado *spin -2 dspin*. Você tem um conjunto de imagens de rotação de rotação que contêm três linhas, com 12 imagens por linha. As imagens são nomeadas da seguinte maneira:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Com essas informações, a fórmula do Tipo de conjunto em lote pode ser criada da seguinte maneira:

![](assets/se_batch_set_recipe.png)

O agrupamento da parte do nome de ativo compartilhado do spinset é adicionado ao campo **Correspondência** (como destacado). A parte variável do nome do ativo contendo a linha e a coluna é adicionada aos campos **Linha** e **Coluna** , respectivamente.

Quando o Conjunto de rotação é carregado e publicado, você ativa o nome da fórmula Conjunto de rotação 2 D listada em Predefinições de conjuntos **de lote** na caixa de diálogo **Opções** de trabalho de upload.

**Para criar uma predefinição de lote para a geração automática de um Conjunto de rotação 2 D**

1. Escolha **Configuração** &gt; **Configuração do aplicativo** &gt; **Predefinições de conjunto em lote** &gt; **Predefinição de conjunto em lote**. **Exibir formulário**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista predefinida, clique **em Adicionar** para ativar os campos de definição no painel Detalhes no lado direito da tela.
1. No painel Detalhes, no campo Nome predefinido, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione Conjunto **de ativos**.
1. Na lista suspensa Subtipo, selecione Conjunto de rotação **de vários eixos**.
1. Expanda **Convenções de nomeação de ativos** e, na lista suspensa Nomenclatura de arquivo, clique **em Personalizado**.
1. Use **a Correspondência** e, opcionalmente, **os atributos Nome** básico para definir uma expressão regular para o nome de ativos de imagem que compõem o agrupamento.

   Por exemplo, a expressão regular Corresponder literal pode ser semelhante ao seguinte:

   `(\w+)-\w+-\w+`

1. Expanda **a Posição da coluna da linha** e defina o formato de nome para a posição do ativo de imagem na matriz de Conjunto de rotação 2 D.

   Use o parêntese para utilizar a posição da linha ou da coluna no nome do arquivo.

   Por exemplo, para a expressão regular da linha, pode ser semelhante ao seguinte:

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   Para a expressão regular da coluna, pode ser semelhante ao seguinte:

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   Lembre-se que estes são apenas exemplos. Você pode criar sua expressão regular no entanto, se quiser atender às suas necessidades.

   >[!NOTE]
   Se a combinação de expressões regulares de linha e coluna não conseguir determinar a posição do ativo na matriz de spinset multidimensional, esse ativo não será adicionado ao conjunto e um erro será registrado.

1. Para Definir convenção de nomenclatura e criação, especifique o sufixo ou o prefixo ao nome básico definido na Convenção de nomenclatura de ativo. Também define onde o conjunto de imagens será criado na estrutura de pastas do Dynamic Media Classic.

   Se você definir um número grande de conjuntos de imagens, talvez prefira mantê-los separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados em lote aqui.

1. Clique **em Salvar** no painel Detalhes.
1. Faça upload e publique seu Conjunto de rotação como de costume, certifique-se de ativar o nome de seu Conjunto de rotação 2 D na caixa de diálogo Opções de carregamento de trabalho, em Predefinições de conjuntos de lote.

>[!MORELIKETHIS]
* [Visualizar um ativo](previewing-asset.md#previewing_an_asset)
* [Configuração de predefinições de imagens](setting-image-presets.md#setting_up_image_presets)
* [Exibição, adição e exportação de metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Verificação de arquivos de trabalho](checking-job-files.md#checking_job_files)

