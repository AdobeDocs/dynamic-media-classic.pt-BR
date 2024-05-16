---
title: Configuração do aplicativo
description: Saiba como instalar e configurar a área Aplicativo do Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10351'
ht-degree: 1%

---

# Configuração do aplicativo{#application-setup}

Você pode usar as páginas Configuração do aplicativo para inserir Configurações gerais, criar Predefinições de imagem, Predefinições de codificação de vídeo, Predefinições do visualizador ou definir Visualizadores padrão e metadados. Você pode configurar Predefinições de conjunto de lotes para que elas automatizem a geração de Conjuntos de rotação 2D (por exemplo), configurações de publicação e configurações de SEO de vídeo.

>[!NOTE]
>
>Somente administradores do Adobe Dynamic Media Classic podem alterar configurações na Configuração do aplicativo.

## Configurações gerais {#general-settings}

Para abrir a página Configurações gerais do aplicativo, na barra Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.

### Servidores

Na criação da conta, a Adobe Dynamic Media Classic fornece automaticamente os servidores atribuídos à sua empresa. Esses servidores são usados para criar sequências de caracteres de URL para seu site e aplicativos. Essas chamadas de URL são específicas da sua conta.

Consulte também [Testar o serviço de teste seguro](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Published Server Name]**: este é o servidor CDN (Content Deliver Network) ativo usado em todas as chamadas de URL geradas pelo sistema específicas para sua conta. Altere esse nome de servidor somente se for instruído a fazê-lo por um técnico de suporte da Adobe Dynamic Media Classic.

* **[!UICONTROL Origin Server Name]**: este servidor é usado somente para testes de controle de qualidade. Altere esse nome de servidor somente se for instruído a fazê-lo por um técnico de suporte da Adobe Dynamic Media Classic.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&Target Server Name]**: o URL do Test&amp;Target, incluindo `.com`. Para obter instruções sobre como obter esse URL, consulte Integração [!DNL Adobe Dynamic Media Classic] com [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server Name]**: O URL para o seu [!DNL Adobe Dynamic Media Classic] servidor de transmissão iOS. Este servidor fornece streaming de vídeo para dispositivos baseados em iOS usando o protocolo HTTP.

* **[!UICONTROL Progressive Video Server Name]**: O URL para o seu [!DNL Adobe Dynamic Media Classic] servidor de vídeo progressivo. Esse servidor fornece vídeo progressivo usando o protocolo HTTP.

* **[!UICONTROL Show URL for unpublished assets]**: selecione esta opção se desejar [!DNL Adobe Dynamic Media Classic] para exibir um URL ao visualizar qualquer ativo, publicado ou não. Se o ativo não for publicado, o URL não funcionará. No entanto, você pode usar o URL para fins de planejamento ou organização.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN Invalidation Template]**: especifica o modelo usado para invalidar o cache CDN (Content Delivery Network).

  Por exemplo, suponha que você insira um URL de imagem (incluindo Predefinições de imagem ou modificadores) referenciando `<ID>`, em vez de uma ID de imagem específica, como no exemplo a seguir:

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Se o modelo contiver apenas `<ID>`, em seguida, o Adobe Dynamic Media Classic preenche o `https://<server>/is/image`, onde `<server>` é o Nome do Servidor de Publicação definido em Configurações Gerais.

  Definindo o Modelo Invalidar da CDN, selecione uma imagem chamada Backpack_B e vá para **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** O resulta no seguinte URL gerado na interface CDN Invalidate:

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  Na caixa da lista URL, selecione **[!UICONTROL Continue]** para limpar o cache da chamada de URL da imagem específica. Você também pode adicionar URLs digitando ou colando-os na caixa de listagem URL; não é necessário definir o modelo antecipadamente.

  Depois de selecionar o Modelo de invalidação da CDN e fazer uma solicitação para Invalidar a CDN, um indicador aparecerá na interface do usuário. Ele fornece uma estimativa de quanto tempo leva para limpar o cache.

  Ao clicar em **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**, cada imagem é referenciada no URL de modelo salvo se várias imagens forem selecionadas no Dynamic Media Classic. Portanto, você pode definir um Modelo de invalidação CDN referenciando cada URL referenciado em seu site (como detalhes do produto e resultados de pesquisa). Em seguida, ao selecionar uma ou mais imagens para invalidação do cache, os URLs preenchem automaticamente a interface.

  Consulte [Armazenamento em cache de conteúdo](dmc-platform-overview.md#content_caching).

  Consulte [Ativos republicados e atrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Procurar

* **[!UICONTROL Show Projects]**: determina se os Projetos estão disponíveis como um meio de organizar os ativos do Adobe Dynamic Media Classic. Consulte [Organize seu trabalho com Projetos](/help/using/organizing-projects.md).

* **[!UICONTROL Show Sample eVideo Content]**: ativar ou desativar a exibição do conteúdo de amostra do eVideo.

* **[!UICONTROL Show Generated Content]**: nas pastas, ele mostra o conteúdo gerado de um ativo. Por exemplo, quando um arquivo PDF é rasterizado à medida que é carregado, o Adobe Dynamic Media Classic cria uma imagem para cada página no PDF original. Se Mostrar conteúdo gerado estiver selecionado, cada imagem gerada quando o PDF original for carregado será exibida. Ele aparece junto com o PDF na pasta para a qual o PDF foi carregado.

* **[!UICONTROL Show Encoded Videos]**: desmarcado (desativado) por padrão.

  Você pode pesquisar e procurar vídeos rapidamente no Adobe Dynamic Media Classic sem precisar navegar por vários derivados codificados do mesmo vídeo. Deixe essa opção desmarcada (padrão). Somente a miniatura do Vídeo principal (o vídeo de origem carregado e usado para criar os derivados) e a miniatura do Conjunto de vídeos adaptados &quot;pai&quot; (que contém os derivados &quot;filho&quot; do Conjunto de vídeos codificado) são exibidas.

  No entanto, você ainda pode acessar vídeos codificados individuais do Vídeo principal ou do Conjunto de vídeos adaptados. Para fazer isso, clique duas vezes na imagem em miniatura do vídeo para abrir a Exibição de detalhes. Em seguida, selecione **[!UICONTROL Encoded Videos]** no painel direito, para que você possa acessar todos os vídeos &quot;secundários&quot;.

  Você também pode ir para **[!UICONTROL File]** > **[!UICONTROL Reprocess]** para criar mais vídeos &quot;secundários&quot; codificados diretamente de um Conjunto de vídeos adaptados. O Adobe Dynamic Media Classic encontra automaticamente o vídeo principal do Conjunto de vídeos adaptados e o usa como o vídeo de origem para transcodificação. No entanto, quando você salva os novos vídeos codificados individuais, eles não são vistos ao pesquisar ou navegar. No entanto, eles ainda podem ser acessados na guia Vídeos codificados na Exibição de detalhes.

  Consulte [Fazer upload e transcodificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Para continuar a acessar todos os seus derivados de vídeo codificado ao pesquisar e navegar, selecione **[!UICONTROL Show Encoded Videos]**.

  Há certas ações no menu Criar que funcionam somente, ou opcionalmente, funcionam, com vídeos individuais. Essa funcionalidade torna necessário mostrar todos os derivados de vídeo codificados que você pode selecionar, independentemente de como você define **[!UICONTROL Show Encoded Videos]**. As ações do Build que substituem o **[!UICONTROL Show Encoded Videos]** configuração include **[!UICONTROL Adaptive Video Sets]**, e **[!UICONTROL eCatalogs]**.

  >[!NOTE]
  >
  >Se você não usou o Adobe Dynamic Media Classic para carregar e codificar seus ativos de vídeo, o Adobe Dynamic Media Classic mostrará todos os seus vídeos codificados individualmente, mesmo que essa opção não esteja selecionada.

* **[!UICONTROL Show Refresh Subfolders Button]**: ativar ou desativar a exibição do botão Atualizar das subpastas.

### Conta FTP da Adobe Dynamic Media Classic

* **[!UICONTROL Server]**: lista o servidor de conta FTP.

* **[!UICONTROL User Name]**: lista o nome de usuário da sua conta FTP.

### Carregar no aplicativo

Consulte também [Opções para trabalhos de upload](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) vídeo de treinamento.

* **[!UICONTROL Overwrite Images]**: o Adobe Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A Adobe Dynamic Media Classic ID de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Fazer upload tem uma opção Substituir. O efeito exato dessa opção depende da opção Substituir imagens especificada. Essas opções especificam como as imagens de substituição são carregadas: se elas substituem as imagens originais ou se tornam imagens duplicadas. Imagens duplicadas são renomeadas com um &quot;-1&quot; (por exemplo, chair.tif é renomeado chair-1.tif). Essas opções afetam as imagens carregadas em uma pasta diferente da original ou as imagens com uma extensão de nome de arquivo diferente da original (como JPG, TIF ou PNG). Consulte [Usar a opção Substituir imagens](#using-the-overwrite-images-option).

   * **[!UICONTROL Overwrite in current folder, same base image name or extension]**: essa opção é a regra mais rígida para substituição. Ela requer que você faça upload da imagem de substituição para a mesma pasta da original e que a imagem de substituição tenha a mesma extensão de nome de arquivo da original. Se esses requisitos não forem atendidos, uma duplicata será criada.

   * **[!UICONTROL Overwrite in current folder, same base asset name regardless of extension]**: Requer que você faça upload da imagem de substituição na mesma pasta da original, no entanto, a extensão do nome do arquivo pode ser diferente da original. Por exemplo, chair.tif substitui chair.jpg.

   * **[!UICONTROL Overwrite in any folder, same base asset name or extension]**: requer que a imagem de substituição tenha a mesma extensão de nome de arquivo que a imagem original. Por exemplo, chair.jpg deve substituir chair.jpg, não chair.tif). Entretanto, é possível fazer upload da imagem de substituição em uma pasta diferente da original. A imagem atualizada está na nova pasta; o arquivo não pode mais ser encontrado em seu local original

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]**: essa é a regra de substituição mais inclusiva. É possível fazer upload de uma imagem de substituição para uma pasta diferente da original, fazer upload de um arquivo com uma extensão de nome de arquivo diferente e substituir o arquivo original. Se o arquivo original estiver em uma pasta diferente, a imagem de substituição ficará localizada na nova pasta para a qual foi carregada.

* **[!UICONTROL Retain Publish]**: especifica se uma imagem de substituição carregada no Adobe Dynamic Media Classic retém a configuração Pronto para publicar da imagem que está substituindo. Ou a configuração é especificada no upload.

* **[!UICONTROL Default Color Profiles]**: Especifica os perfis de cores aplicados como parte das Opções de Perfil de Cores Padrão ao adicionar imagens CMYK.

* **[!UICONTROL Default Upload Options]**: abre a caixa de diálogo Fazer Upload das Opções de Job, onde você pode especificar opções de upload padrão. Para obter informações sobre essas opções, consulte [Opções de upload](/help/using/uploading-files.md#upload_options).

### Editor de mapa de imagem (para aplicativo)

* **[!UICONTROL Default Image Mapping HREF]**: define o URL padrão usado para a coluna HREF no mapeamento de imagem. Esse é o URL padrão que você vê ao criar Mapas de imagem.

* **[!UICONTROL Default Image Mapping Template]**: define o JavaScript padrão para o modelo HREF no mapeamento de imagem. É possível definir um código personalizado aqui para ser executado sempre que você selecionar um Mapa de imagem.

### Outras Configurações (para Aplicativo)

* **[!UICONTROL Trash Can Clean Up Warnings]**: os ativos na Lixeira são removidos automaticamente em sete dias. Selecione &quot;Enviar emails antes que os itens da lixeira sejam excluídos automaticamente&quot; para que as notificações sejam enviadas aos administradores da empresa quando os ativos que estão na lixeira estiverem a quatro dias de serem excluídos permanentemente. Consulte [Gerenciar a pasta Lixeira](/help/using/trash-folder.md).

## Usar a opção Substituir imagens {#using-the-overwrite-images-option}

O Adobe Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A Adobe Dynamic Media Classic ID de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Devido a essa regra, a caixa de diálogo Fazer upload inclui as opções Substituir imagens. O efeito exato dessa opção depende de uma configuração das Configurações internas do Adobe Dynamic Media Classic de cada empresa.

Se você carregou imagens anteriormente e alterou os arquivos originais (ou os substituiu), a opção de Substituição escolhida especifica como o Adobe Dynamic Media Classic substitui as imagens. Nenhuma informação sobre a imagem é alterada, mas a nova imagem substitui a antiga. Se a pasta também contiver imagens que ainda não estão no Adobe Dynamic Media Classic, essas imagens serão adicionadas.

Use essa opção se as imagens carregadas tiverem sido alteradas de alguma forma (a imagem foi alterada), mas a referência à imagem permanecer a mesma. A substituição também é útil ao carregar e ripar PDF Adobe®. É possível ajustar como o Adobe Dynamic Media Classic *rips* a imagem. Você também pode ajustar as opções de perfil de cores ICC na caixa de diálogo Fazer upload e fazer upload novamente usando o recurso de substituição.

As Adobe Dynamic Media Classic IDs usadas para acessar imagens dos servidores de produção são derivadas dos nomes de arquivo de imagem. O uso de caracteres em maiúsculas e minúsculas no nome do arquivo é importante, tanto para a substituição de arquivos existentes quanto para as Adobe Dynamic Media Classic IDs usadas para acessar a imagem. O uso de nomes de arquivo com caracteres em maiúsculas e minúsculas está correto antes de ser carregado no Adobe Dynamic Media Classic para evitar que as IDs do Adobe Dynamic Media Classic sejam diferentes apenas em maiúsculas e minúsculas para a mesma imagem.

Se você desmarcar essa opção, todas as imagens com os mesmos nomes de arquivo que as imagens existentes serão tratadas como duplicatas e não serão adicionadas.

## Predefinições da imagem {#image-presets}

A tela Predefinições de imagem é usada para criar e editar Predefinições de imagem. As Predefinições de imagem permitem que o Adobe Dynamic Media Classic forneça imagens dinamicamente em tamanhos diferentes da mesma imagem principal. Cada predefinição de imagem representa uma coleção predefinida de comandos de dimensionamento e formatação para a exibição de imagens. Ao criar uma Predefinição de imagem, você seleciona um tamanho para a entrega da imagem. Você também pode selecionar comandos de formatação para que a aparência da imagem seja otimizada quando ela for entregue para visualização.

Os administradores podem criar predefinições para exportar ativos. Os usuários podem escolher uma predefinição ao exportar imagens, o que também reformata imagens para as especificações especificadas pelo administrador.

Para abrir a tela Predefinição de imagem, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

Consulte [Imagem inteligente](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Criar e editar predefinições de imagem {#creating-and-editing-image-presets}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Criar uma predefinição ou iniciar com uma existente:

   * **Criar uma predefinição de imagem**: Selecionar **[!UICONTROL Add]**.
   * **Criar uma predefinição de imagem a partir de uma predefinição existente**: selecione a Predefinição de imagem mais parecida com a que deseja criar e selecione **[!UICONTROL Edit]**.

1. Na página Adicionar (ou Editar) predefinição, digite um nome para a predefinição.
1. Defina as opções de Predefinição desejadas.

   Consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

1. Selecionar **[!UICONTROL Save]** ou se tiver iniciado a partir de uma predefinição existente, selecione **[!UICONTROL Save As]**.
1. Para visualizar a predefinição com sua própria imagem, selecione **[!UICONTROL Browse]** e selecione uma imagem. Para visualizar com a imagem padrão, selecione **[!UICONTROL Reset]**.

É possível editar uma Predefinição de imagem selecionando o nome na tela Predefinições de imagem e, em seguida, selecionando **[!UICONTROL Edit]**. Para excluir uma predefinição de imagem, selecione-a e, em seguida, **[!UICONTROL Delete]**.

### Opções de predefinição de imagem {#image-preset-options}

As telas Adicionar predefinição e Editar predefinição oferecem estas opções para criar e editar Predefinições de imagem:

* **[!UICONTROL Preset Name]**: digite um nome descritivo sem espaços em branco. Para ajudar os usuários a identificarem essa predefinição de imagem, inclua a especificação do tamanho da imagem no nome.

* **[!UICONTROL Width and Height]**: insira, em pixels, o tamanho da imagem.

* **[!UICONTROL Format]**: selecione um formato no menu. A escolha do formato GIF, JPEG, PDF ou TIFF oferece mais opções:

   * Opções de quantização de cores do GIF

      * **[!UICONTROL Type]**: selecione Adaptável (o padrão), Web ou Mac. Se você selecionar **[!UICONTROL GIF With Alpha]**, a opção Mac não está disponível.

      * **[!UICONTROL Dither]**: Selecione Difuso ou Desativado.

      * **[!UICONTROL Number Of Colors]**: arraste o controle deslizante para inserir 2-255.

      * **[!UICONTROL Color List]**: Insira uma lista separada por vírgulas. Por exemplo, para branco, cinza e preto, insira `000000,888888,ffffff`.

   * Opções de JPEG

      * **[!UICONTROL Quality]**: controla o nível de compactação JPEG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade do JPEG é de 1 a 100.

      * **[!UICONTROL Enable JPG Chrominance Downsampling]**: como o olho é menos sensível a informações de cores de alta frequência do que a luminosidade de alta frequência, as imagens de JPEG dividem as informações da imagem em componentes de luminosidade e cor. Quando uma imagem de JPEG é compactada, o componente de luminosidade fica com a resolução total, enquanto os componentes de cor ficam com uma resolução mais baixa para calcular a média de grupos de pixels. A redução da resolução reduz o volume de dados pela metade ou em um terço com quase nenhum impacto na qualidade aparente. A redução da resolução não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

   * Opções de PDF e TIFF

      * **[!UICONTROL Compression]**: selecione um algoritmo de compactação.

* **[!UICONTROL Colorspace]**: selecione um espaço de cores.

* **[!UICONTROL Sharpening]**: selecione a opção Ativar nitidez simples para aplicar um filtro de nitidez básico à imagem depois que todo o dimensionamento ocorrer. A nitidez pode ajudar a compensar o desfoque que pode ocorrer ao exibir uma imagem de tamanho diferente.

  Para obter mais informações sobre nitidez, modos de reamostragem e mascaramento sem nitidez, consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image). Consulte também [Nitidez](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) vídeo de treinamento.

* **[!UICONTROL Resample Mode]**: selecione uma opção de modo de reamostragem. Essas opções deixam a imagem mais nítida quando a resolução é reduzida:

* **[!UICONTROL B-Linear]**: o método de reamostragem mais rápido; alguns artefatos de suavização são visíveis.

* **[!UICONTROL Bi-Cubic]**: aumenta o uso da CPU no servidor de imagens, mas produz imagens mais nítidas com menos artefatos de suavização visíveis.

* **[!UICONTROL `Sharp 2`]**: pode produzir resultados ligeiramente mais nítidos do que a opção Bi-Cubic, mas com um custo de CPU ainda maior no servidor de imagem.

* **[!UICONTROL Tri-Linear]**: usa resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando o alias for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

* **[!UICONTROL Unsharp Masking]**: escolha estas opções para ajustar a nitidez:

* **[!UICONTROL Amount]**: controla a quantidade de contraste aplicada aos pixels de borda. O padrão é 1.0. Para imagens de alta resolução, é possível aumentá-las para até 5,0. Pense na Quantidade como uma medida da intensidade do filtro.

* **[!UICONTROL Radius]**: determina o número de pixels em torno dos pixels de borda que afetam a nitidez. Para imagens de alta resolução, insira de 1 a 2. Um valor baixo aplica nitidez apenas aos pixels da borda; um valor alto aplica nitidez a uma faixa mais ampla de pixels. O valor correto depende do tamanho da imagem.

* **[!UICONTROL Threshold]**: determina o intervalo de contraste que deve ser ignorado quando o filtro Tirar nitidez da máscara for aplicado. Ou seja, isso pode ajudar a resolver a diferença entre os pixels com nitidez e a área ao redor antes de serem considerados pixels de borda e nitidez. Para evitar a introdução de ruídos, experimente valores entre `.02` e `0.2`. O valor padrão de 6 aplica nitidez a todos os pixels da imagem.

* **[!UICONTROL Color Space]**: determina se a imagem usa o espaço em que foi criada, geralmente RGB (Original) ou um espaço de luminosidade (Intensidade).

* **[!UICONTROL Color]** Escolha estas opções:

* **[!UICONTROL Output Color Profile]**: Selecionar **[!UICONTROL Use Default]** ou um dos perfis de cores ICC disponíveis no Adobe Dynamic Media Classic.

  Consulte também [Perfis ICC](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]**: selecione uma opção se desejar substituir a tentativa de renderização padrão do perfil de cores. Use esta opção quando um dos perfis ICC padrão for o espaço de cores de destino de uma conversão de cores. Ou, esse perfil caracteriza o dispositivo de saída (impressora ou monitor) e a tentativa de renderização especificada é válida para esse perfil.

* **[!UICONTROL Embed Profile]**: selecione esta opção para que, se você abrir esta imagem no Adobe® Photoshop®, ela use este perfil.

* **[!UICONTROL Print Resolution]**: selecione uma resolução para imprimir essa imagem; o padrão é 72 pixels.

* **[!UICONTROL URL Modifiers]**: se preferir especificar os modificadores de URL que definem sua Predefinição de imagem, em vez das configurações, insira os modificadores aqui.

* **[!UICONTROL Sample Image URL]**: lista a cadeia de caracteres de URL &quot;bruta&quot; que o Dynamic Media Image Server usa para fornecer imagens com a Predefinição de imagem que você está adicionando ou editando. Essa cadeia de caracteres de URL codifica todas as configurações de formato selecionadas na tela Adicionar predefinição ou Editar predefinição.

### Editar, remover ou desativar uma predefinição de imagem {#editing-removing-or-deactivating-an-image-preset}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Na tela Predefinições de imagem, selecione uma predefinição na tabela e siga um destes procedimentos:

   * Selecionar **[!UICONTROL Edit]** e especifique novas opções na caixa de diálogo Editar predefinição.
   * Selecionar **[!UICONTROL Delete]** para remover a predefinição da lista.
   * Desmarque a opção **[!UICONTROL Active]** caixa de seleção ao lado de um nome predefinido se desejar removê-lo de toda a interface do Adobe Dynamic Media Classic para usuários do MediaPortal.

## Ativar ou desativar predefinições do vídeo adaptável {#activating-or-deactivating-adaptive-video-presets}

O Adobe Dynamic Media Classic oferece predefinições de codificação de vídeo adaptável. É uma lista primária de predefinições que combina Predefinições de vídeo adaptável 16:9 e Predefinições de vídeo adaptável 4:3 em um grupo. Essas predefinições predefinidas refletem as configurações de codificação mais comuns e são otimizadas para reprodução em dispositivos móveis, tablets e desktops de destino.

Somente as predefinições de codificação do &quot;Vídeo adaptável&quot; são ativadas (ativadas ou &quot;ativadas&quot;) por padrão. Você pode desativá-la, se desejar. As predefinições de vídeo adaptável inativo não aparecem como uma opção que pode ser selecionada na seção eVideo da caixa de diálogo Fazer upload das opções de trabalho.

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

Consulte também [Predefinições de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

**Para ativar ou desativar predefinições de vídeo adaptável:**

1. Próximo ao canto superior direito do Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**.
1. Na página Predefinições de vídeo adaptável, desmarque a caixa de seleção ao lado de um nome predefinido para remover a predefinição da lista Opções de eVideo, na caixa de diálogo Fazer upload das opções de trabalho.
1. Selecionar **[!UICONTROL Close]**.

## Predefinições de vídeo para codificar arquivos de vídeo {#video-presets-for-encoding-video-files}

Para selecionar uma predefinição de codificação, no canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]**. Na caixa de diálogo Fazer upload das opções de trabalho, expanda Opções de eVideo e selecione as Predefinições de codificação de vídeo desejadas.

>[!NOTE]
>
>Exceto pelo &quot;Vídeo adaptável&quot;, que é ativado por padrão, não é possível ver todos os outros Vídeos adaptáveis ou Predefinições de codificação de vídeo únicas na caixa de diálogo Fazer upload das opções de trabalho. Os administradores do Adobe Dynamic Media Classic determinam quais Predefinições de codificação de vídeo estão visíveis na caixa de diálogo Fazer upload das opções de trabalho.

* Selecione uma das seguintes predefinições de codificação de vídeo adaptável ou codificação única:

   * **[!UICONTROL 16:9 Adaptive Video]**: crie vídeos com taxa de proporção de 16:9 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™), otimizados com a resolução e a taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   * **[!UICONTROL 4:3 Adaptive Video]**: crie vídeos com taxa de proporção de 4:3 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™), otimizados com a resolução e a taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   * **[!UICONTROL Adaptive Video]**: uma predefinição de codificação única que funciona com qualquer taxa de proporção para criar vídeos, para exibição em dispositivos móveis, tablets e computadores de mesa. Os vídeos de origem carregados codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo.

     Essa flexibilidade de ter uma &quot;Escala automática&quot; também está disponível por padrão ao criar sua própria predefinição de codificação de vídeo personalizada.

     Consulte [Adicionar ou editar uma predefinição de codificação de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Video Encoding (16:9 or 4:3)]**: crie vídeos com taxa de proporção de 16:9 e 4:3 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™). Tudo otimizado com a resolução e a taxa de bits que melhor corresponde à velocidade de conexão do visualizador.

     Consulte [Predefinições de vídeo da Codificação de vídeo adaptável (16:9 ou 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Single Encoding Presets]**

     >[!NOTE]
     >
     >Para enviar vídeo para iPads, você pode selecionar uma predefinição de codificação para dispositivos móveis ou uma predefinição de codificação do Tablet. As predefinições de tablet são projetadas especialmente para o iPad, normalmente com maior resolução e qualidade para aproveitar o tamanho maior da tela e da conexão de largura de banda. Para fornecer arquivos de vídeo codificados com uma predefinição de tablet, é necessário incluir o código de detecção de dispositivo no site ou aplicativo móvel. Esse código alterna entre uma experiência de vídeo iPhone ou iPad, dependendo do dispositivo de reprodução. A escolha de uma predefinição para dispositivos móveis para fornecer arquivos de vídeo à iPad é um fluxo de trabalho mais simplificado. O motivo é que você pode usar o mesmo arquivo de vídeo para iPhones e iPads. No entanto, a qualidade é padronizada para a experiência de iPhone de resolução mais baixa.

      * No grupo Predefinições de Codificação, na lista suspensa Classificar Predefinições de Codificação, selecione Nome ou Tamanho para classificar as predefinições por nome ou tamanho de resolução.
      * Selecione uma predefinição de codificação com base no tamanho da resolução e na largura de banda com a qual você planeja reproduzir o vídeo.
      * É possível selecionar a Codificação de vídeo adaptável e uma ou mais predefinições de codificação por vídeo. Por exemplo, você pode codificar um arquivo para desktop e dispositivo móvel em um trabalho de upload.

Depois de selecionar **[!UICONTROL Start Upload]**, o arquivo de Vídeo primário original é carregado e os arquivos codificados são gerados a partir do arquivo primário.

### Sobre as opções de predefinição de codificação {#about-encoding-preset-options}

Os parâmetros das opções de predefinição de codificação são os seguintes:

* **[!UICONTROL Target connection speed]**: a velocidade da conexão de Internet do usuário final direcionado.

* **[!UICONTROL Encoded file suffix]**: o sufixo anexado ao arquivo de vídeo codificado para fins de identificação.

* **[!UICONTROL Video bit rate (data rate)]**: a quantidade de dados codificados para compor um segundo único de reprodução de vídeo (em quilobits por segundo).

* **[!UICONTROL Pixel Width/Height]**: a dimensão da largura da imagem da tela, em pixels; a dimensão da altura da imagem da tela (em pixels).

* **[!UICONTROL Frame per second (fps)]**: o número de quadros ou imagens estáticas para cada segundo do vídeo. Nos Estados Unidos e no Japão, a maioria dos vídeos é filmada em 29,97 fps; na Europa e na Ásia (excluindo o Japão), a maioria dos vídeos é filmada em 25 fps. O filme é filmado a 24 fps.

* **[!UICONTROL Audio bit rate]**: a quantidade de dados codificada para compor um segundo único de reprodução de áudio, em quilobits por segundo.

As tabelas a seguir mostram as práticas recomendadas para selecionar predefinições de vídeo e as convenções de nomenclatura usadas para designar arquivos codificados.

### Vídeo adaptável (padrão) {#adaptive-video-default}

Uma predefinição de codificação que funciona com qualquer taxa de proporção para permitir que você crie vídeos para levar a dispositivos móveis, tablets e computadores de mesa. Os vídeos de origem carregados codificados com essa predefinição (o padrão e uma prática recomendada) são definidos com uma altura fixa, enquanto a largura é dimensionada automaticamente para preservar a proporção do vídeo.

**Vídeo adaptável (padrão)**

|  | Codificação de nome de predefinição/texto de dica de ferramenta | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | FPS | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automático × 360, 800 Kbps | _Celular_Automático×360p_800K | 800 | Automático×360 | Igual à origem | 64 | Para dispositivos móveis (iPhone, iPad, Android™) |
| 2 | Automático × 480, 1400 Kbps | _Tablet_Auto×480p_1400K | 1400 | Automático×480 | Igual à origem | 96 | Para tablets (iPad, Android™) |
| 3 | Automático × 720, 2600 Kbps | _Desktop_Automático×720p_2600K | 2600 | Automático×720 | Igual à origem | 128 | Para desktop |

### Predefinições da codificação de vídeo adaptável (16:9 ou 4:3) {#adaptive-video-encoding-or-video-presets}

Essas predefinições de codificação do vídeo adaptado combinam uma série de predefinições individuais de codificação, selecionadas automaticamente para você com base na proporção do vídeo carregado. Por exemplo, se você carregar um vídeo 4:3, ele será automaticamente codificado usando todas as cinco predefinições 4:3 encontradas na lista de predefinições primária na **Codificação de vídeo adaptável (16:9 ou 4:3)** opção.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções de predefinição de codificação](application-setup.md#about_encoding_preset_options).

**Predefinições da codificação de vídeo adaptável (16:9 ou 4:3)**

|  | Codificação de nome de predefinição/texto de dica de ferramenta | Velocidade de conexão de destino (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | FPS | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Celular_512x288_400K | 400 | 512x288 | Igual à origem | 64 | Baixa resolução, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Celular_384x288_400K | 400 | 384x288 | Igual à origem | 64 | Baixa resolução, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Celular_512x288_600K | 600 | 512x288 | Igual à origem | 64 | Resolução média, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Celular_384x288_600 | 600 | 384x288 | Igual à origem | 64 | Resolução média, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Igual à origem | 80 | Resolução média, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | Igual à origem | 80 | Resolução média, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Igual à origem | 96 | Alta resolução, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Igual à origem | 96 | Alta resolução, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Tela widescreen de alta definição |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Igual à origem | 128 | Alta definição |

### Predefinições de codificação de vídeo da área de trabalho {#desktop-video-encoding-presets}

Predefinições de codificação de vídeo para MP4 e OGV em computadores desktop.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções de predefinição de codificação](application-setup.md#about_encoding_preset_options).

**H264 Principal 3.2: áudio AAC, extensão de arquivo MP4**

|  | Codificação de nome de predefinição/texto de dica de ferramenta | Velocidade de conexão de destino (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | FPS | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Igual à origem | 64 | Baixa resolução em widescreen |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Igual à origem | 80 | Resolução média em tela larga |
| 3 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Igual à origem | 96 | Média-alta resolução |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Tela widescreen de alta definição |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Igual à origem | 64 | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | Igual à origem | 80 | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Igual à origem | 96 | Média-alta resolução |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Igual à origem | 128 | Alta definição |

**OGG Theora Vorbis: Extensão de arquivo OGV**

|  | Codificação de nome de predefinição/texto de dica de ferramenta | Velocidade de conexão de destino (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | FPS | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Igual à origem | 64 | Baixa resolução em widescreen |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Igual à origem | 80 | Resolução média em tela larga |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Igual à origem | 96 | Média-alta resolução |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Tela widescreen de alta definição |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Igual à origem | 64 | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Igual à origem | 80 | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | Igual à origem | 96 | Média-alta resolução |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Igual à origem | 128 | Alta definição |

### Predefinições de codificação de vídeo para dispositivos móveis {#mobile-video-encoding-presets}

O mesmo que fps de origem. Predefinições de codificação de vídeo para dispositivos móveis iPhone, iPad e Android™.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções de predefinição de codificação](application-setup.md#about_encoding_preset_options).

**Linha de base 2.1 do H264: áudio AAC, extensão de arquivo MP4**

|  | Codificação de nome de predefinição/texto de dica de ferramenta | Velocidade de conexão de destino (Kbps) | Sufixo de arquivo codificado | Taxa de bits de vídeo (Kbps) | Largura/altura do pixel | FPS | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Móvel (400 Kbps) | 500 | _Celular_512x288_400K | 400 | 512x288 | Igual à origem | 64 | Baixa resolução, 3G |
| 2 | 16:9, 512x288, Móvel (600 Kbps) | 700 | _Celular_512x288_600K | 600 | 512x288 | Igual à origem | 64 | Resolução média, 3G |
| 3 | 16:9, 512x288, Móvel (800 Kbps) | 900 | _Celular_512x288_800K | 800 | 512x288 | Igual à origem | 80 | Resolução média, Wi-Fi |
| 4 | 16:9, 512x288, Móvel (1000 Kbps) | 1,2 Mbps | _Celular_512x288_1000K | 1000 | 512x288 | Igual à origem | 80 | Alta resolução, Wi-Fi |
| 5 | 16:9, 512x288, Móvel (1200 Kbps) | 1,5 Mbps | _Celular_512x288_1200K | 1200 | 512x288 | Igual à origem | 96 | Alta resolução, Wi-Fi |
| 6 | 4:3, 384x288, Móvel (400 Kbps) | 500 | _Celular_384x288_400K | 400 | 384x288 | Igual à origem | 64 | Baixa resolução, 3G |
| 7 | 4:3, 384x288, Móvel (600 Kbps) | 700 | _Celular_384x288_600K | 600 | 384x288 | Igual à origem | 64 | Resolução média, 3G |
| 8 | 4:3, 448x336, Móvel (800 Kbps) | 900 | _Celular_448x336_800K | 800 | 448x336 | Igual à origem | 80 | Resolução média, Wi-Fi |
| 9 | 4:3, 448x336, Móvel (1000 Kbps) | 1,2 Mbps | _Celular_448x336_1000K | 1000 | 448x336 | Igual à origem | 80 | Alta resolução, Wi-Fi |
| 10 | 4:3, 448x336, Móvel (1200 Kbps) | 1,5 Mbps | _Celular_448x336_1200K | 1200 | 448x336 | Igual à origem | 96 | Alta resolução, Wi-Fi |

## Predefinições do visualizador {#viewer-presets}

>[!NOTE]
>
>**Aviso de fim de vida útil de visualizadores do Flash**: A partir de 31 de janeiro de 2017, a Adobe Dynamic Media Classic encerrou oficialmente o suporte para a plataforma de visualizador do Flash.

A *Predefinição do visualizador* O é uma coleção de configurações que determinam como os usuários visualizam os ativos de mídia avançada nas telas dos computadores e nos dispositivos móveis. Como administrador, você pode criar Predefinições do visualizador. As configurações estão disponíveis para uma matriz de opções de configuração do visualizador. Por exemplo, é possível alterar o tamanho de exibição do visualizador, o comportamento de zoom, os esquemas de cores, as bordas e as fontes.

Como prática recomendada, use visualizadores de vídeo Adobe Dynamic Media Classic HTML5. As predefinições usadas nos visualizadores de HTML5 Video são players de vídeo robustos.

Ao combinar em um único player o seguinte:

* A capacidade de projetar os componentes de reprodução usando HTML5 e CSS.
* Têm reprodução integrada.
* Use o fluxo adaptável e progressivo, dependendo da capacidade do navegador.

Estenda o alcance do seu conteúdo de mídia avançada para desktops, tablets e usuários de dispositivos móveis e garanta uma experiência de vídeo otimizada.

Consulte [Sobre visualizadores do HTML5](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) no Guia de referência de visualizadores do Adobe.

Consulte [Matriz de compatibilidade da Predefinição do visualizador do Adobe Dynamic Media Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consulte [Prática recomendada: uso do visualizador de vídeo HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependendo do visualizador, você pode adicionar recursos da comunidade. Os recursos da comunidade incluem um botão Incorporar, botão Email, botão Link e botão Visitar site. Esses botões permitem que as pessoas que usam os visualizadores compartilhem o visualizador com outras pessoas ou abram o site do Adobe Dynamic Media Classic na Web.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Suporte de visualizador para páginas da Web com design responsivo {#viewer-support-for-responsive-designed-web-pages}

Páginas da Web diferentes têm necessidades diferentes. Às vezes, você quer ter uma página da Web que forneça um link que abra o Visualizador de HTML 5 em uma janela separada do navegador. Em outros casos, é necessário incorporar o Visualizador HTML5 diretamente na página de hospedagem. No último caso, a página da Web provavelmente tem um layout estático. Ou é &quot;responsivo&quot; e é exibido de forma diferente em diferentes dispositivos ou para diferentes tamanhos de janela de navegador. Para acomodar essas necessidades, os visualizadores HTML5 fornecidos com o Adobe Dynamic Media Classic suportam páginas da Web estáticas e páginas da Web com design responsivo.

Para obter mais informações sobre como incorporar visualizadores responsivos nas suas páginas da Web, consulte [Sobre a biblioteca de imagens responsiva](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Usar biblioteca de imagens responsiva](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api), e [Referência de comando: Command attributes](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Tipos de predefinição do visualizador {#viewer-preset-types}

Os administradores podem criar e personalizar os seguintes tipos de Predefinições do visualizador:

* **[!UICONTROL eCatalog Viewer]**: simula a experiência de leitura de um catálogo impresso. Você pode mover de página para página, ampliar e reduzir itens em uma página, usar Mapas de imagem para ver mais informações sobre itens na página ou pesquisar o catálogo. Você também pode incluir um painel Informações para exibir informações detalhadas e um item mapeado por imagem se a área do mapa tiver um atributo rollover_key válido. Para incluir um painel Informações, especifique um URL do servidor de informações no painel Informações painel Configurações da janela Predefinição do visualizador de eCatalog.

* **[!UICONTROL Swatch Set Viewer]**: exibe uma imagem em uma cor, material, textura, acabamento ou malha diferente. Os usuários selecionam uma miniatura para ver as variações na imagem.

* **[!UICONTROL Mixed Media Set Viewer]**: exibe diferentes tipos de mídia em um visualizador. É possível incluir Conjuntos de amostras, Conjuntos de rotação, imagens e vídeos. É possível configurar guias para que tenham diferentes tipos de conteúdo, como uma guia para Conjuntos de imagens e uma guia para vídeos. Os vídeos reproduzidos de um Conjunto de mídias mistas usam um Visualizador de vídeo padrão com uma linha do tempo e controles de vídeo, como Parar, Pausar, Retroceder e Reproduzir. Ao configurar uma Predefinição do visualizador de conjunto de mídia mista, você especifica quais visualizadores deseja usar para os diferentes tipos de ativos no seu Conjunto de mídias mistas. Você também pode usar o Visualizador de grade ou o Visualizador do carrossel para exibir um Conjunto de mídias mistas.

* **[!UICONTROL Spin Set Viewer]**: fornece várias exibições de uma imagem para que os usuários possam transformar o objeto para examinar os diferentes lados e ângulos.

* **Visualizador de vídeo**: exibe vídeos usando as dimensões de resolução do arquivo de origem ou um tamanho personalizado. O Adobe Dynamic Media Classic vem com muitas Predefinições do visualizador predefinidas para reproduzir vídeo e, se você for um administrador, poderá criar Predefinições do visualizador de vídeo personalizadas. Há mais de 12 configurações diferentes para configurar o Visualizador de vídeo. Você pode configurar:

   * tamanho
   * cor do primeiro plano e do plano de fundo
   * controles de vídeo e áudio
   * barra de progresso
   * capa da interface do usuário
   * recursos sociais
   * e Ajuda

* **[!UICONTROL Zoom Viewers]**: oferece três tipos de visualizadores de zoom:

* **[!UICONTROL Zoom Viewer]**: permite que os usuários ampliem a área ao selecioná-la. Eles podem selecionar controles para ampliar, reduzir e redefinir a imagem para seu tamanho padrão.

* **[!UICONTROL Zoom Viewer: Fly-out]**: exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção sobre a área que desejam visualizar.

Ao determinar o uso completo da largura de banda para esse visualizador, considere que tanto a imagem principal quanto a imagem suspensa são fornecidas no visualizador. O tamanho da imagem principal (Largura e Altura do Palco) e o Fator de Zoom determinam o tamanho da imagem suspensa. Para evitar que o tamanho do arquivo de imagem suspensa fique muito grande, equilibre esses dois valores: se você tiver um tamanho grande de imagem principal, diminua o valor do Fator de zoom. (A Largura da imagem suspensa e a Altura da imagem suspensa determinam o tamanho da janela da imagem suspensa, mas não o tamanho da imagem suspensa que é exibida no visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com um Fator de Zoom de 3, a imagem suspensa resultante será 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de Zoom de 4, a imagem suspensa será de 1200 por 1200 pixels. Dependendo da configuração de qualidade do JPEG (as configurações recomendadas estão entre 80 e 90), é possível diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

### Matriz de compatibilidade da Predefinição do visualizador do Adobe Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Aviso de fim de vida útil de visualizadores do Flash**: A partir de 31 de janeiro de 2017, a Adobe Dynamic Media Classic encerrou oficialmente o suporte para a plataforma de visualizador do Flash.

A tabela a seguir identifica as Predefinições do visualizador do Adobe Dynamic Media Classic disponíveis no momento. A tabela também especifica a compatibilidade do visualizador com dispositivos móveis e de desktop, e a tecnologia usada para cada visualizador específico.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Para obter informações sobre o navegador da Web e as versões do sistema operacional compatíveis para Visualizadores, consulte as Notas de versão dos Visualizadores.

Consulte [Notas de versão de referência de visualizadores do Adobe](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de amostras |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Inclui suporte para redes sociais e pesquisa no catálogo.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Inclui suporte para redes sociais e pesquisa no catálogo.) | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de rotação |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizadores de eVideo**

O Adobe Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP4 H.264.

* Você pode encontrar dispositivos BlackBerry® compatíveis com esse formato de vídeo no seguinte endereço: [Formatos de vídeo compatíveis com o BlackBerry®](https://developers.blackberry.com/us/en)
* Você também pode encontrar dispositivos Windows® compatíveis com esse formato de vídeo no link a seguir: [Formatos de vídeo compatíveis com o Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Inclui suporte para legendas ocultas.) Consulte [Prática recomendada: uso do visualizador de vídeo Universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclui suporte para legendas ocultas e mídia social.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de mix de mídia |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matriz de gestos de visualizadores móveis compatíveis {#supported-mobile-viewers-gestures-matrix}

A tabela a seguir identifica os gestos do visualizador móvel compatíveis com dispositivos iOS, Android™ 2.x e Android™ 3.x.

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Smartphone Android™ | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Sobre a tela Predefinição do visualizador {#about-the-viewer-preset-screen}

Criar e gerenciar predefinições do visualizador na tela Predefinições do visualizador. Para abrir esta tela, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

A tela Predefinições do visualizador oferece ferramentas para executar estas tarefas:

* **Adicionar uma predefinição**: Selecionar **[!UICONTROL Add]** e faça escolhas na caixa de diálogo Adicionar predefinição do visualizador.

      Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).
  
* **Editar uma predefinição**: selecione uma predefinição e, em seguida, **[!UICONTROL Edit]**.

      Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).
  
* **Excluir uma predefinição**: selecione uma predefinição e, em seguida, **[!UICONTROL Delete]**.

* **Exportar uma predefinição**: selecione uma predefinição do visualizador HTML5. Clique em **[!UICONTROL Export]** para baixar a capa do visualizador e usá-la como base para criar e adicionar outra predefinição do visualizador.

      Consulte [Exportar uma predefinição do visualizador do HTML5](application-setup.md#exports_an_html5_viewer_preset).
  
* **Filtrar a lista Predefinição do visualizador**: use essas ferramentas para filtrar a lista:

      * Abra a lista suspensa **Ativo/Inativo** e selecione uma opção para mostrar predefinições ativas, predefinições inativas ou todas as predefinições.
      * Abra a lista suspensa **Visualizador** e selecione uma opção para ver somente os visualizadores de determinado tipo. Selecionar **[!UICONTROL All Viewers]** para ver todos os visualizadores.
  
* **Classificar predefinições**: selecione um cabeçalho de coluna (**[!UICONTROL Active]**, **[!UICONTROL Type]**, **[!UICONTROL Preset]** ou **[!UICONTROL Platform]**) para classificar a lista em uma coluna. Selecione um cabeçalho de coluna uma segunda vez para classificar a lista em ordem decrescente (ou crescente).

* **Ativar e desativar predefinições**: selecione uma predefinição e escolha a opção Ativo para ativá-la ou desativá-la.

      Consulte [Ativar ou desativar predefinições do visualizador](application-setup.md#ativating_or_deactivating_viewer_presets).
  
>[!NOTE]
>
>Selecionar **[!UICONTROL Preview]** no lado direito da página Predefinições do visualizador, para que você possa visualizar a aparência de um ativo na Predefinição do visualizador selecionada. Para ver um ativo diferente, selecione **[!UICONTROL Browse]** na página Predefinições do visualizador e selecione um ativo diferente na caixa de diálogo Selecionar visualização do ativo.

### Adicionar e editar predefinições do visualizador {#adding-and-editing-viewer-presets}

Além de adicionar predefinições do visualizador usando o **[!UICONTROL Add]** na interface do usuário, também é possível usar **[!UICONTROL Export]** para adicionar uma predefinição do visualizador. Basta exportar uma Predefinição do visualizador de HTML5 existente e usá-la como base para a nova predefinição.

Consulte [Exportação de predefinição do visualizador do HTML5](application-setup.md#exporting_an_html5_viewer_preset).

Consulte também [Predefinições do visualizador](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vídeo de treinamento.

**Para adicionar e editar Predefinições do visualizador:**

1. Próximo ao canto superior direito do Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

   É possível filtrar na lista de predefinições. Por exemplo, para ver apenas as predefinições de Visualizadores de vídeo, selecione Visualizador de vídeo no menu suspenso Visualizadores na barra de ferramentas, logo acima da tabela.

1. Na página Predefinições do visualizador, adicione ou edite a Predefinição do visualizador na tela Predefinições do visualizador.

   * **Adicionar**: Na barra de ferramentas, selecione **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, selecione uma plataforma e um tipo de ativo de mídia avançada.

         Selecionar **[!UICONTROL Save As]** quando terminar de criar a Predefinição do visualizador.
     
   * **Adicionar ao iniciar com base em uma Predefinição do visualizador existente**: na tabela, selecione uma Predefinição do visualizador de vídeo e, em seguida, selecione **[!UICONTROL Edit]** na barra de ferramentas.

         Depois de reconfigurar o Visualizador de vídeo, selecione **[!UICONTROL Save As]** para salvar a predefinição usando um nome diferente no campo de texto Nome da predefinição.
     
   * **Editar**: selecione uma Predefinição do visualizador existente e, em seguida, selecione **[!UICONTROL Edit]**.

1. Na página Configurando o visualizador, no campo Nome da predefinição, digite ou edite o nome da predefinição.
1. Defina as opções restantes desejadas.

   >[!NOTE]
   >
   >Selecionar **[!UICONTROL Same As Source]** para que você possa dimensionar automaticamente o Visualizador de vídeo para o tamanho da resolução do próprio vídeo codificado. Se você selecionar essa opção, não poderá inserir a Largura e a Altura do Palco. Em vez disso, essas opções vêm do próprio vídeo. Se você selecionar **[!UICONTROL Same As Source]**, defina a opção Tamanho da margem para refletir as dimensões da capa fora da área de reprodução do vídeo. Esse tamanho de margem é a altura e a largura do pixel dos controles de vídeo. Você pode usar a imagem a seguir para determinar os tamanhos das margens que deseja usar.*

   ![Configuração de margem do visualizador de vídeo](assets/vs_video_viewer_configure_margin.png)

1. Siga um destes procedimentos:

   * Selecionar **[!UICONTROL Save As]** se você tiver adicionado uma Predefinição do visualizador, iniciando com uma predefinição existente.
   * Selecionar **[!UICONTROL Save]** se você tiver adicionado ou editado uma Predefinição do visualizador.

### Exportar uma predefinição do visualizador HTML5 {#exporting-an-html-viewer-preset}

É possível exportar uma Predefinição do visualizador de HTML5 existente para usar como base para a criação de uma Predefinição do visualizador de HTML5. Essa opção de exportação é útil porque não é necessário criar o visualizador do zero. Em vez disso, exporte uma predefinição que pareça e se comporte de acordo com o que deseja e, em seguida, use-a como ponto de partida para fazer ajustes de design.

Todos os arquivos CSS de predefinição do visualizador padrão no Adobe Dynamic Media Classic usam caminhos de veiculação de imagens relativos que apontam para ativos no `Scene7SharedAssets`. Por exemplo, este é um caminho relativo para um ativo de imagem em um arquivo CSS de Predefinição do visualizador em

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

No entanto, se você hospeda arquivos CSS do Visualizador no seu próprio site, é necessário resolver esses caminhos de imagem relativos usando um caminho explícito para o Servidor de imagens no seu próprio ambiente. Por exemplo, se você atualizou o caminho relativo acima para um caminho explícito, ele pode ser semelhante ao seguinte, onde `https://s7d1.scene7.com` é o caminho direto para o Servidor de imagens: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar uma predefinição do visualizador HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na barra de ferramentas Predefinições do visualizador, na segunda lista suspensa à esquerda, selecione **[!UICONTROL HTML5]**.
1. Na terceira lista suspensa à esquerda, selecione **[!UICONTROL All Viewers]**.
1. Selecione a Predefinição do visualizador que você deseja usar como base para uma nova Predefinição do visualizador HTML5.
1. Na barra de ferramentas, selecione **[!UICONTROL Export]**.
1. Na caixa de diálogo Exportar ativos selecionados, selecione **[!UICONTROL Submit Export]**.

   Após a exportação, você obtém um arquivo CSS. Baixe e descompacte o arquivo.

1. Abra o arquivo CSS em um editor de CSS, faça as alterações e salve o arquivo.
1. Faça upload do arquivo CSS para o Adobe Dynamic Media Classic.

   Consulte [Fazer upload de arquivos](uploading-files.md#uploading_files).

1. Publique o arquivo CSS no Dynamic Media Image Server.

   Consulte [Publicar arquivos](publishing-files.md#publishing_files).

1. Adicione a nova Predefinição do visualizador como de costume. Selecione o arquivo CSS do Visualizador que você carregou.

   Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

### Ativar ou desativar predefinições do visualizador {#activating-or-deactivating-viewer-presets}

Para criar um URL para mostrar ativos, os usuários abrem a lista suspensa Predefinições na caixa de diálogo Visualização, selecionam uma Predefinição do visualizador e, em seguida, selecionam **[!UICONTROL Copy URL]** (consulte [Copiar o URL de uma predefinição do visualizador](application-setup.md#copying_the_url_of_a_viewer_preset)). Essa lista de Predefinições oferece Predefinições do visualizador que os administradores adicionam e gerenciam na tela Predefinições do visualizador. Por exemplo, todas as Predefinições do visualizador de eCatalog ativas são exibidas na lista suspensa Predefinições na caixa de diálogo Visualizar quando um usuário pré-visualiza um eCatalog.

A menos que você desative Predefinições do visualizador na tela Predefinições do visualizador, a lista suspensa Predefinições na caixa de diálogo Visualizar pode ficar lotada.

**Para ativar ou desativar as Predefinições do visualizador:**

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na página Predefinições do visualizador, marque ou desmarque **[!UICONTROL Active]** opções para ativar ou desativar as Predefinições do visualizador.

### Copiar o URL de uma predefinição do visualizador {#copying-the-url-of-a-viewer-preset}

Depois de publicar um ativo, é possível copiar um URL para exibir o ativo com as configurações de uma Predefinição do visualizador.

O URL é copiado para a área de transferência. Você pode usá-lo conforme necessário no código HTML da página da Web, do dispositivo móvel ou do aplicativo.

**Para copiar o URL de uma predefinição do visualizador:**

1. Selecione o ativo no painel Procurar.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e código incorporado à direita, selecione **[!UICONTROL Copy URL]** à direita do visualizador desejado.
   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, acesse **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecionar **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecionar **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

### Copiar o código incorporado de uma predefinição do visualizador {#copying-the-embed-code-of-a-viewer-preset}

O uso do recurso Incorporar código permite revisar o código do visualizador para a Predefinição do visualizador selecionada. Você também pode copiar o código para a área de transferência para poder colá-lo em suas páginas da Web para implantação do visualizador.

A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o Código de incorporação de uma predefinição do visualizador:**

1. Selecione o ativo no painel Navegar por ativos.
1. Acima do painel Navegar por ativos, no lado direito da barra de ferramentas, siga um destes procedimentos:

   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs à direita, selecione **[!UICONTROL Embed Code]**.
   * Selecionar **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, acesse **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecionar **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecionar **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista do Visualizador, na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

1. Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.
1. Selecionar **[!UICONTROL Close]**.

## Configurar visualizadores padrão {#configure-default-viewers}

Você pode usar Visualizadores padrão para configurar o visualizador padrão associado a um ativo ao usar Visualização no Adobe Dynamic Media Classic. Você pode configurar a experiência de visualização padrão para os seguintes tipos de ativos:

* Imagem
* Vídeo
* SpinSet
* Catálogo
* ImageSet
* SwatchSet
* MediaSet

**Para configurar visualizadores padrão:**

1. Na lista suspensa Configurar, selecione **[!UICONTROL Application Setup]**.
1. Na janela Configuração, no painel esquerdo, vá para **[!UICONTROL Application Setup]** > **[!UICONTROL Viewers]**
1. Selecionar **[!UICONTROL Default Viewers]**.
1. Na janela Visualizadores padrão, na lista suspensa para cada tipo de ativo, selecione o visualizador que você deseja associar à visualização do ativo.
1. No canto inferior direito da janela Visualizadores padrão, selecione **[!UICONTROL Save Settings]**.
1. No canto inferior direito da janela Configuração, selecione **[!UICONTROL Close]** para retornar à janela Ativo.

## Visualizações de metadados {#metadata-views}

*Metadados* O é uma informação padronizada sobre um ativo. Você pode usar metadados para simplificar seu fluxo de trabalho, organizar seus ativos e melhorar a pesquisa. A Adobe Dynamic Media Classic oferece suporte ao padrão IPTC (International Press Telecommunications Council) e ao padrão XMP (extensible metadata platform). Antes de exibir ou inserir metadados sobre um ativo na Exibição de detalhes, os usuários podem abrir o menu Exibições de metadados. A partir daí, eles podem selecionar o conjunto de campos de metadados que desejam visualizar ou usar para descrever o ativo.

O Adobe Dynamic Media Classic vem com Exibições de metadados predefinidas, e os administradores podem criar suas próprias Exibições de metadados para que os usuários escolham quando inserem metadados.

### Criar uma visualização de metadados {#creating-a-metadata-view}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Selecionar **[!UICONTROL Add]**.
1. No campo de texto Nome da predefinição, digite um nome para a exibição.
1. (Opcional) Marque **[!UICONTROL Make Default]** para tornar essa exibição a que os usuários veem quando abrem o painel Metadados na Exibição de detalhes.
1. (Opcional) Selecione **[!UICONTROL Include UDF]** para incluir campos definidos pelo usuário na visualização. Os campos definidos pelo usuário são exibidos na parte superior do painel Metadados na Exibição de detalhes.
1. Selecione os campos que deseja para a exibição (selecione **[!UICONTROL Select All]** para selecionar todos os campos).
1. Selecionar **[!UICONTROL Save]**.

   As categorias e os campos selecionados para a exibição aparecem no painel Visualização.

### Gerenciar Visualizações de Metadados {#managing-metadata-views}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Siga um destes procedimentos:

   * Para visualizar uma exibição, selecione-a. Os campos na exibição aparecem no painel Visualização.
   * Para editar uma exibição, selecione-a e, em seguida, **[!UICONTROL Edit]**. Em seguida, selecione ou desmarque nomes de campo no painel Visualização e selecione ou desmarque a **[!UICONTROL Include UDF]** opção.
   * Para excluir uma exibição, selecione-a e, em seguida, selecione **[!UICONTROL Delete]**.
   * Para tornar uma exibição padrão, selecione-a e, em seguida, selecione **[!UICONTROL Make Default]**. A exibição padrão é aquela que os usuários veem quando abrem um ativo na Exibição de detalhes e acessam o painel Metadados.

## Predefinições de metadados {#metadata-presets}

As predefinições de metadados oferecem aos administradores uma maneira de controlar e regular os metadados atribuídos aos ativos. Na Exibição de detalhes, um usuário pode inserir metadados sobre um ativo nos campos fornecidos para essa finalidade. Por exemplo, um usuário pode inserir um nome de proprietário, descrição de copyright e endereço. Para garantir que os usuários insiram essas informações de forma precisa e completa, é possível criar Predefinições de metadados. Escolher uma Predefinição de Metadados na Exibição de Detalhes preenche campos de metadados com valores predefinidos. Por exemplo, um nome de proprietário, descrição de direitos autorais e endereço são inseridos automaticamente.

Crie uma Predefinição de metadados para cada conjunto de valores de metadados que você deseja que os usuários possam inserir automaticamente na Exibição de detalhes para descrever um ativo.

### Criar ou editar uma predefinição de metadados {#creating-or-editing-a-metadata-preset}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Na tela Predefinições de metadados, siga um destes procedimentos:

   * Para criar uma predefinição, selecione **[!UICONTROL Add]**. No campo de texto Nome do modelo de metadados, digite um nome para a predefinição. Selecionar **[!UICONTROL Metadata Views]** e selecione uma exibição na lista suspensa (consulte [Visualizações de metadados](application-setup.md#metadata_views)).
   * Para editar uma predefinição existente, selecione-a na lista Predefinições de metadados e selecione **[!UICONTROL Edit]**.

1. Expanda os cabeçalhos que deseja incluir na predefinição e insira valores nos diferentes campos que deseja incluir na predefinição.
1. Selecionar **[!UICONTROL Save]**.

   As categorias e os campos selecionados para a predefinição são exibidos no painel Visualizar.

### Gerenciar predefinições de metadados {#managing-metadata-presets}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Siga um destes procedimentos:

   * Para visualizar uma predefinição, selecione a predefinição que deseja visualizar. As informações predefinidas (categorias e campos) são exibidas na tela Visualizar.
   * Para excluir uma predefinição, selecione-a e, em seguida, **[!UICONTROL Delete]**.

## Campos definidos pelo usuário {#user-defined-fields}

Um Administrador do Media Portal ou um Administrador da empresa pode criar campos de metadados personalizados definidos pelo usuário. Campos personalizados podem ajudar a organizar ativos no Adobe Dynamic Media Classic. Você pode marcar os campos como Ativos, conforme necessário. Quando ativados, os nomes desses campos de metadados personalizados aparecem no painel Metadados na Exibição de detalhes. Os usuários podem inserir informações em campos de metadados definidos pelo usuário para descrever ativos. Os usuários também podem tornar um campo de metadados definido pelo usuário um critério nas pesquisas.

Um uso eficaz de campos de metadados definidos pelo usuário é atrasar o tempo de ativação de um ativo para uma inicialização ou venda específica. Você define um campo &quot;ativação&quot;, com base no tipo *Data*. Em seguida, usando o **[!UICONTROL Metadata]** painel na Exibição de detalhes ou **[!UICONTROL File]** > **[!UICONTROL Edit Info]**, é possível especificar quando o ativo será ativado. O Adobe Dynamic Media Classic verifica o status publicado de um ativo e o histórico de publicação. Se não estiver no tempo de ativação, o status de publicação será exibido como &quot;Não publicado&quot;.

>[!NOTE]
>
>Para fazer com que os campos definidos pelo usuário apareçam no painel Metadados na Exibição de Detalhes, inclua campos definidos pelo usuário nas Exibições de Metadados. Na tela Exibições de Metadados, selecione a opção Incluir UDF (campos definidos pelo usuário). Para obter mais informações, consulte [Visualizações de metadados](application-setup.md#metadata_views).

>[!NOTE]
>
>Para pesquisar ativos usando campos personalizados definidos pelo usuário, acesse **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** e selecione **[!UICONTROL Include UDFs in Search]**. Consulte [Configuração pessoal](personal-setup.md#personal_setup).

### Criar um campo de metadados definido pelo usuário {#creating-a-user-defined-metadata-field}

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.
1. Selecionar **[!UICONTROL Add]**
1. Na caixa de diálogo Campo personalizado, defina as opções desejadas.

   * **[!UICONTROL Name]**: insira um nome para o campo de metadados.

   * **[!UICONTROL Type]**: selecione uma opção que defina o tipo de informações que os usuários podem inserir no campo de metadados:

   * **[!UICONTROL String]**: uma cadeia de texto.

   * **[!UICONTROL Int]**: um número inteiro.

   * **[!UICONTROL Float]**: um número de ponto flutuante.

   * **[!UICONTROL Yes/No]**: um valor booliano sim/não.

   * **[!UICONTROL Date]**: uma data. O formato MM/DD/AAAA é aceito.

   * **[!UICONTROL Filename]**: o nome de um arquivo.

   * **[!UICONTROL Color]**: O nome de uma cor.

   * **[!UICONTROL Dimension]**: a largura e a altura do ativo.

   * **[!UICONTROL Untyped]**: para compatibilidade com versões anteriores. Não selecione essa opção.

   * **[!UICONTROL Default Value]**: Opcional. Insira o valor que os usuários provavelmente digitarão no campo. O valor inserido torna-se o valor padrão para o campo criado.

   * **[!UICONTROL Applies To]**: Opcional. Selecione um tipo de ativo se desejar que o campo de metadados seja aplicado somente a um tipo específico de ativo.

     >[!NOTE]
     >
     >Selecione um **[!UICONTROL Applies To]** cuidadosamente porque não é possível alterar a **[!UICONTROL Applies To]** depois de criar um campo definido pelo usuário. O Adobe Dynamic Media Classic permite editar o nome, o tipo e o valor padrão de um campo definido pelo usuário, mas não o **[!UICONTROL Applies To]** configuração. *

1. Selecionar **[!UICONTROL Save]** quando terminar de criar o campo de metadados.

### Gerenciar campos definidos pelo usuário {#manage-user-defined-fields}

A tela Campos definidos pelo usuário oferece comandos para gerenciar campos de metadados personalizados e definidos pelo usuário.

Somente um Administrador do Portal de mídia ou um Administrador da empresa pode gerenciar campos definidos pelo usuário.

Para abrir esta tela, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.

* **Editar um campo**: selecione o campo e selecione **[!UICONTROL Edit]**.

* **Excluir um campo**: selecione o campo e selecione **[!UICONTROL Delete]**.

* **Ativar campo**: marque ou desmarque a opção **[!UICONTROL Active]** ao lado do nome de um campo. Se você estiver em uma função de administração de empresa, essa opção não será exibida. Como essa opção está relacionada ao MediaPortal, você deve selecionar (ativar) Mostrar recursos do MediaPortal na configuração pessoal para ver os campos ativados.

## Otimizar arquivos {#optimize-files}

À medida que você faz upload de arquivos para o Adobe Dynamic Media Classic, o sistema os otimiza para armazenamento e publicação. No entanto, se o processo de upload for interrompido, algumas imagens não poderão ser otimizadas. Nesse caso, você verá a mensagem &quot;Imagem ainda não otimizada&quot;. No entanto, você pode otimizar esses arquivos se for um administrador.

O Adobe Dynamic Media Classic pesquisa seus arquivos e otimiza apenas as imagens que antes não eram totalmente otimizadas.

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** e selecione **[!UICONTROL Optimize Files]**.
1. Especifique as informações para o job de otimização e selecione **[!UICONTROL Submit]**.

   Se você estiver trabalhando com mais de uma empresa, otimize os arquivos pertencentes a diferentes empresas separadamente.

## Predefinições de conjunto de lotes {#batch-set-presets}

Use as Predefinições de conjunto de lotes para criar automaticamente Conjuntos de imagens ou Conjuntos de rotação enquanto um trabalho está em execução para fazer upload de ativos para o Adobe Dynamic Media Classic.

Os administradores da empresa definem primeiro as convenções de nomenclatura dos ativos que desejam agrupar em um conjunto. Em seguida, é possível criar uma Predefinição de conjunto de lotes para fazer referência a essas imagens. Cada predefinição é um conjunto de instruções com nome exclusivo e independente que define como construir o conjunto usando imagens que correspondem às convenções de nomenclatura definidas na fórmula predefinida.

Todas as predefinições de conjunto de lotes ativas de uma empresa são listadas na caixa de diálogo Fazer upload da opção de trabalho, para que você possa especificar qual predefinição deseja aplicar durante cada sessão de upload. Os administradores da empresa visualizam todas as Predefinições de conjunto de lotes ativas e inativas. Ao fazer upload de arquivos, o Adobe Dynamic Media Classic cria automaticamente um conjunto com todos os arquivos que correspondem à convenção de nomenclatura definida nas predefinições ativas.

### Nomeação padrão {#default-naming}

O Administrador da empresa cria uma convenção de nomenclatura padrão que é usada em qualquer fórmula de Predefinição de conjunto de lotes. A convenção de nomenclatura padrão selecionada na definição de Predefinição de conjunto de lotes pode ser tudo o que sua empresa precisa para gerar conjuntos em lote para todos os sites. Uma Predefinição de conjunto de lotes é criada para usar a convenção de nomenclatura padrão que você define. Você pode criar quantas Predefinições de conjunto de lotes forem necessárias com convenções de nomenclatura alternativas e personalizadas para um conjunto específico de conteúdo nos casos em que houver uma exceção à nomenclatura padrão definida pela empresa.

A configuração de uma convenção de nomenclatura padrão não é necessária para usar a funcionalidade Predefinição de conjunto de lotes. No entanto, a prática recomendada do Adobe recomenda usar uma convenção de nomenclatura padrão para definir quantos elementos de sua convenção de nomenclatura você deseja agrupar em um conjunto. Isso ajuda a simplificar a criação de conjuntos de lotes.

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**.
1. Selecionar **[!UICONTROL View Form]** ou **[!UICONTROL View Code]** para especificar como deseja exibir e inserir informações sobre cada elemento.

   É possível selecionar a variável **[!UICONTROL View Code]** marque a caixa para exibir a criação do valor de expressão regular ao lado das seleções do formulário. Você pode informar ou alterar esses valores para ajudar a definir os elementos da convenção de nomenclatura, se a Exibição de Formulário limitar você por qualquer motivo. Se os valores não puderem ser analisados na Exibição de formulário, os campos de formulário ficarão inativos.

   >[!NOTE]
   >
   >Campos de formulário desativados não indicam expressão regular inválida. Não há validação para suas expressões regulares corretas. Você verá os resultados da expressão regular que está criando para cada elemento após a linha Resultado. A expressão regular completa é visível na parte inferior da página.

1. Expanda cada elemento conforme necessário e insira as convenções de nomenclatura que deseja usar.
1. Conforme necessário, selecione **[!UICONTROL Add]** para adicionar outra convenção de nomenclatura para um elemento. Ou selecione **[!UICONTROL Remove]** para excluir uma convenção de nomenclatura de um elemento.
1. Selecionar **[!UICONTROL Save As]** e digite um nome para a predefinição. Ou selecione **[!UICONTROL Save]** se estiver editando uma predefinição existente.

Como alternativa, você pode usar Exibir código sem campos de formulário disponíveis. Nesta visualização, você cria suas definições de convenção de nomenclatura inteiramente usando expressões regulares.

Dois elementos estão disponíveis para definição: Correspondência e Nome de base. Esses campos são todos os elementos definidos para uma convenção de nomenclatura. Eles podem ajudar a identificar a parte da convenção usada para nomear o conjunto no qual estão contidos. Uma convenção de nomenclatura individual de uma empresa poderia usar uma ou mais linhas de definição para cada um desses elementos. É possível usar quantas linhas desejar para sua definição exclusiva e agrupá-las em elementos distintos, como para imagem principal, elemento de Cor, elemento de Exibição Alternativa e elemento de Amostra.

### Criar uma predefinição de conjunto de lotes {#creating-a-batch-set-preset}

O Adobe Dynamic Media Classic usa Predefinições de conjunto de lotes para organizar ativos que compartilham algumas informações ou conteúdo comuns em conjuntos de imagens para exibição em visualizadores. As receitas da Predefinição de conjunto de lotes são executadas automaticamente junto com as tarefas de importação de ativos programadas no Adobe Dynamic Media Classic.

Use Predefinição de conjunto de lotes para criar, editar e gerenciar suas Predefinições de conjunto de lotes. É possível criar quantas predefinições forem necessárias para abranger todos os trabalhos de assimilação de ativos que você exigir. Há duas formas de definições de Predefinição de conjunto de lotes: uma para uma convenção de nomenclatura padrão que você configurou e outra para convenções de nomenclatura personalizadas que você cria dinamicamente.

Você pode usar o método de campo de formulário para definir uma Predefinição de conjunto de lotes ou o método de código, que permite usar expressões regulares. Como em **[!UICONTROL Default Naming]**, você pode selecionar **[!UICONTROL Code View]** ao mesmo tempo que você está definindo no Modo de exibição de formulário e o uso de expressões regulares para criar suas definições. Como alternativa, você pode desmarcar qualquer exibição para usar uma ou a outra exclusivamente.

Consulte também [Criar uma predefinição de conjunto de lotes para a geração automática de um conjunto de rotação 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Consulte também [Grupo de rotação 2D](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) vídeo de treinamento.

**Para criar uma predefinição de conjunto de lotes:**

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista de predefinições, selecione **[!UICONTROL Add]** para ativar os campos de definição no painel Detalhes no lado direito da página.
1. No painel Detalhes, no campo Nome da predefinição, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione um tipo de predefinição.

   Para gerar automaticamente um conjunto de rotação 2D, selecione **[!UICONTROL Multi-Axis Spin Set]** na lista suspensa Tipo de conjunto de lote.

1. Siga um destes procedimentos:

   * Se você estiver usando uma convenção de nomenclatura padrão configurada anteriormente em **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**, expandir **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomeação de Arquivo, selecione **[!UICONTROL Default]**.
   * Para definir uma convenção de nomenclatura conforme configura a predefinição, expanda **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomeação de Arquivo, selecione **[!UICONTROL Custom]**.

1. Para Ordem de sequência, defina a ordem das imagens depois que o conjunto for agrupado no Adobe Dynamic Media Classic. Por padrão, seus ativos são ordenados alfanumericamente. No entanto, você pode usar uma lista separada por vírgulas de expressões regulares para definir a ordem.
1. Em Definir convenção de nomeação e criação, especifique o sufixo ou prefixo para o Nome de base definido na Convenção de nomeação de ativos. Defina também onde o conjunto de imagens é criado na estrutura de pastas do Adobe Dynamic Media Classic.

   Se você definir um grande número de Conjuntos de imagens, mantenha esses conjuntos separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados pelo Conjunto de lotes aqui.

1. Selecionar **[!UICONTROL Save]** no painel Detalhes.

### Criar uma predefinição de conjunto de lotes para a geração automática de um conjunto de rotação 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Você pode usar o Tipo de conjunto de lotes **Grupo de rotação de vários eixos** para criar uma &quot;fórmula&quot; que automatiza a geração de Conjuntos de rotação 2D. O agrupamento de imagens usa expressões regulares de Linha e Coluna para que os ativos de imagem sejam alinhados corretamente no local correspondente na matriz multidimensional.

Consulte também [Criar uma predefinição de conjunto de lotes](application-setup.md#creating_a_batch_set_preset).

Não há número mínimo ou máximo de linhas ou colunas que você deve ter em um Spin Set multieixo.

Por exemplo, suponha que você queira criar um Conjunto de rotação multieixo chamado *spin-2dspin*. Você tem um conjunto de imagens do Conjunto de rotação que contêm três linhas, com 12 imagens por linha. As imagens são nomeadas da seguinte maneira:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Com essas informações, a fórmula Tipo de conjunto de lotes pode ser criada da seguinte maneira:

![Imagem da fórmula do conjunto de lotes](assets/se_batch_set_recipe.png)

O agrupamento para a parte do nome do ativo compartilhado do Spin Set é adicionado ao campo Correspondência (como destacado). A parte variável do nome do ativo que contém a linha e a coluna é adicionada aos campos Linha e Coluna, respectivamente.

Quando o Conjunto de rotação é carregado e publicado, você ativaria o nome da fórmula do Conjunto de rotação 2D que está listada em **[!UICONTROL Batch Set Presets]** na caixa de diálogo Fazer Upload das Opções de Job.

**Para criar uma predefinição de conjunto de lotes para a geração automática de um conjunto de rotação 2D:**

1. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista de predefinições, selecione **[!UICONTROL Add]** para ativar os campos de definição no painel Detalhes no lado direito da página.
1. No painel Detalhes, no campo Nome da predefinição, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione **[!UICONTROL Asset Set]**.
1. Na lista suspensa Subtipo, selecione **[!UICONTROL Multi-Axis Spin Set]**.
1. Expandir **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomeação de Arquivo, selecione **[!UICONTROL Custom]**.
1. Use o **[!UICONTROL Match]** e, opcionalmente, **[!UICONTROL Base Name]** atributos para definir uma expressão regular para nomear ativos de imagem que compõem o agrupamento.

   Por exemplo, sua expressão regular de Correspondência literal pode ser semelhante ao seguinte:

   `(\w+)-\w+-\w+`

1. Expandir **[!UICONTROL Row Column Position]** e, em seguida, defina o formato do nome para a posição do ativo de imagem na matriz do Conjunto de rotação 2D.

   Use os parênteses para incorporar a posição da linha ou da coluna no nome do arquivo.

   Por exemplo, para a expressão regular da linha, ela pode ser semelhante ao seguinte:

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   Para sua expressão regular de coluna, ela pode ser semelhante ao seguinte:

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   Lembre-se de que essas expressões são apenas exemplos. Você pode criar sua expressão regular da maneira que quiser que atenda às suas necessidades.

   >[!NOTE]
   >
   >Se a combinação de expressões regulares em linhas e colunas não puder determinar a posição do ativo na matriz do grupo de rotação multidimensional, esse ativo não será adicionado ao conjunto. Um erro é registrado.

1. Em Definir convenção de nomeação e criação, especifique o sufixo ou prefixo para o Nome de base definido na Convenção de nomeação de ativos. Defina também onde o conjunto de imagens é criado na estrutura de pastas do Adobe Dynamic Media Classic.

   Se você definir um grande número de Conjuntos de imagens, mantenha esses conjuntos separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados pelo Conjunto de lotes aqui.

1. Selecionar **[!UICONTROL Save]** no painel Detalhes.
1. Carregue e publique seu Conjunto de rotação como de costume, certificando-se de ativar o nome do seu Conjunto de rotação 2D na caixa de diálogo Opções de carregamento de trabalho, em Predefinições de conjunto de lote.

>[!MORELIKETHIS]
>
>* [Visualizar um ativo](previewing-asset.md#previewing_an_asset)
>* [Configurar predefinições da imagem](setting-image-presets.md#setting_up_image_presets)
>* [Visualizar, adicionar e exportar metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Verificar arquivos de trabalho](checking-job-files.md#checking_job_files)
