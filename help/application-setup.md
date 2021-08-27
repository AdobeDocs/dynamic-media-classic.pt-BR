---
title: Configuração do aplicativo
description: Saiba como configurar a área Aplicativo do Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '10365'
ht-degree: 2%

---

# Configuração do aplicativo{#application-setup}

Você pode usar as páginas de Configuração do aplicativo para inserir configurações gerais, criar predefinições de imagens, predefinições de codificação de vídeo, predefinições do visualizador ou definir visualizadores padrão e metadados. Você pode configurar predefinições de conjuntos em lotes para também automatizar a geração de conjuntos de rotação 2D (por exemplo), configurações de publicação e configurações de SEO de vídeo.

>[!NOTE]
>
>Somente administradores do Adobe Dynamic Media Classic podem alterar as configurações nas páginas de Configuração do aplicativo.

## Configurações gerais {#general-settings}

Para abrir a página Configurações gerais do aplicativo , na barra Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.

### Servidores

Na criação da conta, o Adobe Dynamic Media Classic fornece automaticamente os servidores atribuídos à sua empresa. Esses servidores são usados para criar strings de URL para seu site e aplicativos. Essas chamadas de URL são específicas da sua conta do .

Consulte também [Testar o serviço de Teste Seguro](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Published Server Name]** - Este servidor é o servidor CDN (Content Deliver Network) em tempo real usado em todas as chamadas de URL geradas pelo sistema específicas da sua conta. Não altere o nome deste servidor a menos que seja instruído a fazê-lo por um técnico de suporte Adobe Dynamic Media Classic.

* **[!UICONTROL Origin Server Name]** - Este servidor é utilizado apenas para testes de garantia de qualidade. Não altere o nome deste servidor a menos que seja instruído por um técnico de suporte Adobe Dynamic Media Classic.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&Target Server Name]** - Seu URL do Test&amp;Target, até .com. Para obter instruções sobre como obter esse URL, consulte Integração [!DNL Adobe Dynamic Media Classic] com [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server Name]** - O URL do seu servidor de transmissão  [!DNL Adobe Dynamic Media Classic] iOS. Este servidor fornece vídeo de transmissão para dispositivos baseados em iOS usando protocolo HTTP.

* **[!UICONTROL Progressive Video Server Name]** - O URL do seu servidor de vídeo  [!DNL Adobe Dynamic Media Classic] progressivo. Este servidor fornece vídeo progressivo usando protocolo HTTP.

* **[!UICONTROL Show URL for unpublished assets]** - Selecione essa opção se desejar  [!DNL Adobe Dynamic Media Classic] exibir um URL ao visualizar qualquer ativo, seja publicado ou não. Se o ativo não for publicado, o URL não funcionará. No entanto, você pode usar o URL para fins de planejamento ou organização.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN Invalidation Template]** - Especifica o modelo que é usado para invalidar o cache CDN (Content Delivery Network).

   Por exemplo, suponha que você insira um URL de imagem (incluindo predefinições ou modificadores de imagem) que faça referência a `<ID>`, em vez de uma ID de imagem específica, como no exemplo a seguir:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Se o Modelo contiver apenas `<ID>`, o Adobe Dynamic Media Classic preencherá o `https://<server>/is/image`, onde `<server>` é o Nome do servidor de publicação definido nas Configurações gerais.

   Definir o modelo de invalidação CDN, selecionar uma imagem chamada Backpack_B e, em seguida, ir para **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** resulta no seguinte URL gerado na interface de invalidação CDN:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Na caixa de listagem URL, selecione **[!UICONTROL Continue]** para limpar o cache da chamada de URL da imagem específica. Também é possível adicionar URLs digitando ou colando na caixa de listagem URL; não é necessário definir o Modelo com antecedência.

   Após selecionar seu modelo de invalidação CDN e fazer uma solicitação de invalidação CDN, um indicador aparece na interface do usuário. Ele fornece uma estimativa de quanto tempo leva para limpar o cache.

   Da mesma forma, se várias imagens forem selecionadas no Adobe Dynamic Media Classic ao acessar **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**, cada imagem será referenciada no URL de modelo salvo. Portanto, você pode definir um Modelo de invalidação CDN referenciando cada URL referenciado em seu site (como detalhes do produto e resultados de pesquisa). Em seguida, ao selecionar uma ou mais imagens para invalidação do cache, os URLs preenchem automaticamente a interface.

   Consulte [Armazenamento de conteúdo em cache](dmc-platform-overview.md#content_caching).

   Consulte [Ativos republicados e atrasos de CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Procurar

* **[!UICONTROL Show Projects]** - Determina se os Projetos estão disponíveis como meio de organizar os ativos do Adobe Dynamic Media Classic. Consulte Organizar o trabalho com Projetos.

* **[!UICONTROL Show Sample eVideo Content]** - Ativa ou desativa a exibição do conteúdo de amostra do eVideo.

* **[!UICONTROL Show Generated Content]** - Em pastas, mostra o conteúdo gerado de um ativo. Por exemplo, quando um arquivo PDF é rasterizado à medida que é carregado, o Adobe Dynamic Media Classic cria uma imagem para cada página no PDF original. Se a opção Mostrar conteúdo gerado estiver selecionada, cada imagem gerada quando o PDF original foi carregado aparecerá junto com o PDF na pasta para a qual o PDF foi carregado.

* **[!UICONTROL Show Encoded Videos]** - Desmarcado (desativado) por padrão.

   Para pesquisar e procurar vídeos rapidamente no Adobe Dynamic Media Classic sem precisar navegar por vários derivados codificados do mesmo vídeo, deixe essa opção desmarcada (padrão). Somente a miniatura de Vídeo Principal (o vídeo de origem carregado e usado para criar os derivados) e a miniatura do Conjunto de Vídeo Adaptativo &quot;principal&quot; (que contém os derivados &quot;filho&quot; do conjunto de vídeo codificado) são exibidas.

   No entanto, você ainda pode acessar vídeos individuais codificados do Vídeo Principal ou do Conjunto de vídeos adaptáveis. Para fazer isso, clique duas vezes na imagem de miniatura do vídeo para abrir a Exibição de detalhes. Em seguida, selecione **[!UICONTROL Encoded Videos]** no painel direito para acessar todos os vídeos &quot;filho&quot;.

   Você também pode acessar **[!UICONTROL File]** > **[!UICONTROL Reprocess]** para criar vídeos &quot;secundários&quot; mais codificados diretamente de um Conjunto de vídeos adaptáveis. O Adobe Dynamic Media Classic encontra automaticamente o vídeo Principal &quot;principal&quot; do Conjunto de vídeos adaptáveis e o usa como vídeo de origem para transcodificação. No entanto, ao salvar os novos vídeos codificados individuais, eles não são vistos quando você pesquisa ou navega. No entanto, elas ainda podem ser acessadas na guia Vídeos codificados na Exibição detalhada.

   Consulte [Fazer upload e transcodificar o vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Para continuar a capacidade de acessar todos os derivados de vídeo codificados ao pesquisar e navegar, selecione **[!UICONTROL Show Encoded Videos]**.

   Há determinadas ações no menu Criar que funcionam apenas, ou opcionalmente, com vídeos individuais. Essa funcionalidade torna necessário mostrar todos os derivados de vídeo codificados que podem ser selecionados, independentemente de como você define **[!UICONTROL Show Encoded Videos]**. As ações de Build que substituem a configuração **[!UICONTROL Show Encoded Videos]** incluem **[!UICONTROL Adaptive Video Sets]** e **[!UICONTROL eCatalogs]**.

   >[!NOTE]
   >
   >Se você não tiver usado o Adobe Dynamic Media Classic para fazer upload e codificar seus ativos de vídeo, o Adobe Dynamic Media Classic exibirá todos os seus vídeos codificados individuais, mesmo que essa opção esteja desmarcada.

* **[!UICONTROL Show Refresh Subfolders Button]** - Ativa ou desativa a exibição do botão Atualizar das subpastas.

### Conta FTP do Adobe Dynamic Media Classic

* **[!UICONTROL Server]** - Lista seu servidor de contas FTP.

* **[!UICONTROL User Name]** - Lista o nome de usuário da conta FTP.

### Fazer upload para o aplicativo

* **[!UICONTROL Overwrite Images]** - O Adobe Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A Adobe Dynamic Media Classic ID de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Upload tem uma opção de Substituição. O efeito exato dessa opção depende da opção de Substituição de imagens especificada. Essas opções especificam como as imagens de substituição são carregadas: se eles substituem as imagens originais ou se tornam imagens duplicadas. Imagens duplicadas são renomeadas com um &quot;-1&quot; (por exemplo, chair.tif é renomeado chair-1.tif). Essas opções afetam as imagens enviadas para uma pasta diferente da original ou as imagens com uma extensão de nome de arquivo diferente da original (como JPG, TIF ou PNG). (Consulte Uso da opção Substituir imagens .)

   * **[!UICONTROL Overwrite in current folder, same base image name/extension]** - Essa opção é a regra mais estrita para substituição. Ela requer que você carregue a imagem de substituição na mesma pasta do original e que a imagem de substituição tenha a mesma extensão de nome de arquivo do original. Se esses requisitos não forem atendidos, uma duplicata será criada.

   * **[!UICONTROL Overwrite in current folder, same base asset name regardless of extension]** - Requer que você carregue a imagem de substituição na mesma pasta do original, no entanto, a extensão do nome do arquivo pode ser diferente do original. Por exemplo, chair.tif substitui chair.jpg.

   * **[!UICONTROL Overwrite in any folder, same base asset name/extension]** - Requer que a imagem de substituição tenha a mesma extensão de nome de arquivo que a imagem original (por exemplo, chair.jpg deve substituir chair.jpg, não chair.tif). No entanto, é possível fazer upload da imagem de substituição para uma pasta diferente da original. A imagem atualizada reside na nova pasta; o arquivo não pode mais ser encontrado em seu local original

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** - Essa é a regra de substituição mais inclusiva. Você pode fazer upload de uma imagem de substituição para uma pasta diferente do original, fazer upload de um arquivo com uma extensão de nome de arquivo diferente e substituir o arquivo original. Se o arquivo original estiver em uma pasta diferente, a imagem de substituição residirá na nova pasta para a qual foi carregada.

* **[!UICONTROL Retain Publish]** - Especifica se uma imagem de substituição carregada no Adobe Dynamic Media Classic retém a configuração Pronto para publicar da imagem que está substituindo ou se a configuração está especificada no upload.

* **[!UICONTROL Default Color Profiles]** - Especifica os perfis de cores aplicados como parte das Opções de perfil de cor padrão ao adicionar imagens CMYK.

* **[!UICONTROL Default Upload Options]** - Abre a caixa de diálogo Upload Job Options , onde é possível especificar as opções de upload padrão. Para obter informações sobre essas opções, consulte Opções de upload .

### Editor do Mapa de Imagens, para Aplicativo

* **[!UICONTROL Default Image Mapping HREF]** - Define o URL padrão usado para a coluna HREF no mapeamento de imagem. Esse URL é o URL padrão que você vê ao criar mapas de imagem.

* **[!UICONTROL Default Image Mapping Template]** - Define o JavaScript padrão para o modelo HREF no mapeamento de imagem. Você pode definir um código personalizado aqui para ser executado sempre que selecionar um mapa de imagem.

### Outras configurações, para Aplicativo

* **[!UICONTROL Trash Can Clean Up Warnings]** - Os ativos na lixeira são removidos automaticamente em sete dias. Selecione &quot;Enviar emails antes que os itens de lixo sejam excluídos automaticamente&quot; se desejar que as notificações sejam enviadas para administradores de empresas quando os ativos que estão na Lixeira estiverem a quatro dias de serem excluídos permanentemente. Consulte Gerenciamento da pasta Lixeira.

## Use a opção Substituir imagens {#using-the-overwrite-images-option}

O Adobe Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A Adobe Dynamic Media Classic ID de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Carregar inclui as opções de Substituir imagens. O efeito exato dessa opção depende de uma configuração das configurações internas do Adobe Dynamic Media Classic de cada empresa.

Se você carregou imagens anteriormente e alterou os arquivos originais (ou as substituiu), a opção Substituir escolhida especifica como o Adobe Dynamic Media Classic substitui as imagens. Nenhuma informação sobre a imagem muda, mas a nova imagem substitui a antiga. Se a pasta também contiver imagens que ainda não estão no Adobe Dynamic Media Classic, essas imagens serão adicionadas.

Use esta opção se as imagens que você carregou tiverem sido alteradas de alguma forma (a imagem foi alterada), mas a referência à imagem permanece a mesma. A substituição também é útil ao carregar e extrair PDFs Adobe®. Para ajustar como o Adobe Dynamic Media Classic *rips* da imagem, ajuste as opções de perfil de cor ICC na caixa de diálogo Carregar e faça novamente o upload usando o recurso Substituir .

As IDs do Adobe Dynamic Media Classic usadas para acessar imagens dos servidores de produção são derivadas dos nomes de arquivo da imagem. O uso de caracteres em maiúsculas e minúsculas no nome do arquivo é importante, tanto para a substituição de arquivos existentes quanto para as IDs clássicas do Adobe usadas para acessar a imagem. Certifique-se de que o uso de caracteres em letras maiúsculas e minúsculas em nomes de arquivo esteja correto antes de fazer upload no Adobe Dynamic Media Classic para evitar as IDs do Adobe Dynamic Media Classic que diferem somente em letras maiúsculas e minúsculas para a mesma imagem.

Se você desmarcar essa opção, todas as imagens com os mesmos nomes de arquivo das imagens existentes serão tratadas como duplicatas e não serão adicionadas.

## Predefinições de imagem {#image-presets}

A tela Predefinições de imagem é usada para criar e editar Predefinições de imagem. As predefinições de imagens permitem que o Adobe Dynamic Media Classic forneça imagens dinamicamente em tamanhos diferentes da mesma imagem principal. Cada predefinição de imagem representa uma coleção predefinida de comandos de dimensionamento e formatação para a exibição de imagens. Ao criar uma Predefinição de imagem, você seleciona um tamanho para a entrega da imagem. Você também seleciona comandos de formatação para que a aparência da imagem seja otimizada quando a imagem for entregue para exibição.

Os administradores podem criar predefinições para exportar ativos. Os usuários podem escolher uma predefinição quando exportam imagens, o que também reformata as imagens para as especificações especificadas pelo administrador.

Para abrir a tela Predefinição de imagem, na barra Navegação global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

Consulte [Imagem inteligente](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Criar e editar predefinições de imagens {#creating-and-editing-image-presets}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Crie uma predefinição ou comece com uma predefinição existente:

   * **Criar uma predefinição de imagem**  - Selecione  **[!UICONTROL Add]**.
   * **Criar uma predefinição de imagem a partir de uma predefinição existente**  - Selecione a predefinição de imagem mais parecida com a que deseja criar e selecione  **[!UICONTROL Edit]**.

1. Na página Adicionar (ou Editar) predefinição , digite um nome para a predefinição.
1. Defina as opções de Predefinição desejadas.

   Consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

1. Selecione **[!UICONTROL Save]** ou, se você começou com uma predefinição existente, selecione **[!UICONTROL Save As]**.
1. Para visualizar a predefinição com sua própria imagem, selecione **[!UICONTROL Browse]** e selecione uma imagem. Para visualizar com a imagem padrão, selecione **[!UICONTROL Reset]**.

Você pode editar uma predefinição de imagem selecionando seu nome na tela Predefinições de imagem e depois selecionando **[!UICONTROL Edit]**. Para excluir uma Predefinição de imagem, selecione-a e, em seguida, selecione **[!UICONTROL Delete]**.

### Opções de predefinição de imagem {#image-preset-options}

As telas Adicionar predefinição e Editar predefinição oferecem estas opções para criar e editar Predefinições de imagem:

* **[!UICONTROL Preset Name]** - Insira um nome descritivo sem espaços em branco. Para ajudar os usuários a identificar essa predefinição de imagem, inclua a especificação do tamanho da imagem no nome.

* **[!UICONTROL Width and Height]** - Insira em pixels o tamanho em que a imagem é entregue.

* **[!UICONTROL Format]** - Selecione um formato no menu . Escolher o formato GIF, JPEG, PDF ou TIFF traz mais opções:

   * Opções de quantificação de cores GIF

      * **[!UICONTROL Type]** - Selecione Adaptável (padrão), Web ou Macintosh. Se você selecionar **[!UICONTROL GIF With Alpha]**, a opção Macintosh não estará disponível.

      * **[!UICONTROL Dither]** - Selecione Difuso ou Desativado.

      * **[!UICONTROL Number Of Colors]** - Arraste o controle deslizante para entrar em 2-255.

      * **[!UICONTROL Color List]** - Insira uma lista separada por vírgulas. Por exemplo, para branco, cinza e preto, digite `000000,888888,ffffff`.
   * Opções JPEG

      * **[!UICONTROL Quality]** - Controla o nível de compactação JPEG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade JPEG é de 1 a 100.

      * **[!UICONTROL Enable JPG Chrominance Downsampling]** - Como o olho é menos sensível à informação de cores de alta frequência do que à luminância de alta frequência, as imagens JPEG dividem as informações da imagem em componentes de luminância e cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução completa, enquanto os componentes de cor são reduzidos pela média de grupos de pixels. A redução da amostragem reduz o volume de dados em um terço ou metade, quase sem impacto na qualidade percebida. A redução da amostragem não é aplicável a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).
   * Opções de PDF e TIFF

      * **[!UICONTROL Compression]** - Selecione um algoritmo de compactação.



* **[!UICONTROL Colorspace]** - Selecione um espaço de cores.

* **[!UICONTROL Sharpening]** - Selecione a opção Ativar nitidez simples para aplicar um filtro de nitidez básico à imagem depois que toda a escala ocorrer. A nitidez pode ajudar a compensar a indefinição que pode resultar na exibição de uma imagem em um tamanho diferente.

   Para obter mais informações sobre nitidez, modos de amostra e mascaramento com nitidez, consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

* **[!UICONTROL Resample Mode]** - Selecione uma opção Resampling mode . Essas opções aprimoram a imagem quando ela é reduzida:

* **[!UICONTROL B-Linear]** - o método de reamostragem mais rápido; alguns artefatos de aliasing são perceptíveis.

* **[!UICONTROL Bi-Cubic]** - Aumenta o uso da CPU no Servidor de imagem, mas gera imagens mais nítidas com artefatos de aliasing menos perceptíveis.

* **[!UICONTROL Sharp2]** - Pode produzir resultados ligeiramente mais nítidos do que a opção Bi-Cubic, mas com um custo de CPU ainda maior no servidor de imagem.

* **[!UICONTROL Tri-Linear]** - Utiliza resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando aliasing for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

* **[!UICONTROL Unsharp Masking]** - Escolha estas opções para ajustar a nitidez:

* **[!UICONTROL Amount]** - Controla a quantidade de contraste aplicado aos pixels da borda. O padrão é 1.0. Para imagens de alta resolução, você pode aumentá-lo até 5.0. Considere Quantia como uma medida de intensidade de filtro.

* **[!UICONTROL Radius]** - Determina o número de pixels em torno dos pixels da borda que afetam a nitidez. Para imagens de alta resolução, digite de 1 a 2. Um valor baixo ajuste a nitidez apenas dos pixels da borda; um valor alto ajuste a nitidez de uma faixa mais ampla de pixels. O valor correto depende do tamanho da imagem.

* **[!UICONTROL Threshold]** - Determina o intervalo de contraste a ser ignorado quando o filtro de máscara nítida for aplicado. Em outras palavras, essa opção determina o quão diferentes os pixels com nitidez devem ser da área ao redor antes de serem considerados pixels de borda e terem nitidez. Para evitar a introdução de ruído, experimente valores entre .02 e 0.2. O valor padrão de 6 ajuste a nitidez de todos os pixels na imagem.

* **[!UICONTROL Color Space]** - Determina se a imagem usa o espaço em que a imagem foi criada, geralmente RGB (Original) ou um espaço de luminância (Intensidade).

* **[!UICONTROL Color]** Escolha estas opções:

* **[!UICONTROL Output Color Profile]** - Selecione  **[!UICONTROL Use Default]** ou um dos perfis de cores ICC disponíveis no Adobe Dynamic Media Classic.

   Consulte também [Perfis ICC](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]** - Selecione uma opção se desejar substituir o propósito de renderização padrão do perfil de cores. Use essa opção quando um dos perfis ICC padrão for o espaço de cores de destino de uma conversão de cores. Ou, um dispositivo de saída (impressora ou monitor) é caracterizado por esse perfil e o propósito de renderização especificado é válido para esse perfil.

* **[!UICONTROL Embed Profile]** - Selecione esta opção para que, se você abrir esta imagem no Adobe® Photoshop®, ela use este perfil.

* **[!UICONTROL Print Resolution]** - Selecione uma resolução para imprimir esta imagem; 72 pixels é o padrão.

* **[!UICONTROL URL Modifiers]** - Se preferir especificar os modificadores de URL que definem sua predefinição de imagem, em vez das configurações, insira os modificadores aqui.

* **[!UICONTROL Sample Image URL]** - Lista a cadeia de caracteres de URL &quot;bruta&quot; que o Dynamic Media Image Server usa para fornecer imagens com a predefinição de imagem que você está adicionando ou editando. Essa cadeia de caracteres de URL codifica todas as configurações de formato selecionadas na tela Adicionar predefinição ou Editar predefinição .

### Editar, remover ou desativar uma predefinição de imagem {#editing-removing-or-deactivating-an-image-preset}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Na tela Predefinições de imagem, selecione uma predefinição na tabela e siga um destes procedimentos:

   * Selecione **[!UICONTROL Edit]** e especifique novas opções na caixa de diálogo Editar predefinição .
   * Selecione **[!UICONTROL Delete]** para remover a predefinição da lista.
   * Desmarque a caixa de seleção **[!UICONTROL Active]** ao lado de um nome predefinido se desejar removê-lo de toda a interface do usuário do Adobe Dynamic Media Classic para usuários do MediaPortal.

## Ativar ou desativar predefinições de vídeo adaptável {#activating-or-deactivating-adaptive-video-presets}

O Adobe Dynamic Media Classic oferece predefinições de codificação de vídeo adaptável. É uma lista principal de predefinições que combina predefinições de Vídeo adaptável 16:9 e predefinições de Vídeo adaptável 4:3 em um grupo. Essas predefinições predefinidas refletem as configurações de codificação mais comuns e são otimizadas para reprodução em dispositivos móveis, tablets e desktops de destino.

Somente as predefinições de codificação de &quot;Vídeo adaptável&quot; são ativadas (ativadas ou &quot;ativadas&quot;) por padrão. Você pode desativá-la, se desejar. As predefinições de Vídeo adaptativo inativo não aparecem como uma opção selecionável na seção eVideo da caixa de diálogo Opções de trabalho de upload .

Consulte [Fazer upload e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Para ativar ou desativar predefinições de vídeo adaptável:**

1. Próximo ao canto superior direito do Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**.
1. Na página Predefinições de vídeo adaptativo , desmarque a caixa de seleção ao lado de um nome predefinido para remover a predefinição da lista Opções de vídeo eletrônico na caixa de diálogo Opções de trabalho de upload .
1. Selecione **[!UICONTROL Close]**.

## Predefinições de vídeo para codificação de arquivos de vídeo {#video-presets-for-encoding-video-files}

Para selecionar uma predefinição de codificação, no canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]**. Na caixa de diálogo Upload Job Options , expanda eVideo Options e selecione as predefinições de codificação de vídeo desejadas.

>[!NOTE]
>
>Com exceção do &quot;Vídeo adaptável&quot;, que é ativado por padrão, não é possível ver todas as outras predefinições de codificação de vídeo adaptável ou único na caixa de diálogo Opções de trabalho de upload . Os administradores do Adobe Dynamic Media Classic determinam quais predefinições de codificação de vídeo estão visíveis na caixa de diálogo Upload Job Options .

* Selecione dentre as seguintes predefinições de codificação de vídeo adaptável ou de codificação única:

   * **[!UICONTROL 16:9 Adaptive Video]** - Crie vídeos com a taxa de proporção de 16:9 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™), otimizados com a resolução e a taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   * **[!UICONTROL 4:3 Adaptive Video]** - Crie vídeos com relação de aspecto de 4:3 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™), otimizados com a resolução e a taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   * **[!UICONTROL Adaptive Video]** - Uma única predefinição de codificação que funciona com qualquer proporção para criar vídeos para entrega em dispositivos móveis, tablets e desktops. Os vídeos de origem carregados codificados com essa predefinição são definidos com uma altura fixa. No entanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo.

      Essa flexibilidade de ter uma &quot;Escala automática&quot; também está disponível por padrão quando você cria sua própria predefinição de codificação de vídeo personalizada.

      Consulte [Adicionar ou editar uma predefinição de codificação de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Video Encoding (16:9 or 4:3)]** - Crie vídeos com proporção de aspecto de 16:9 e 4:3 para entrega em desktops, dispositivos móveis (iPhone, iPad, Android™) e tablets (iPad, Android™). Tudo otimizado com a resolução e a taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

      Consulte [Adaptive Video Encoding (16:9 ou 4:3) video presets](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Single Encoding Presets]**

      >[!NOTE]
      >
      >Para enviar vídeo para iPads, você pode selecionar uma predefinição de codificação Mobile ou uma predefinição de codificação Tablet. As predefinições de tablet são projetadas especialmente para o iPad, normalmente com maior resolução e qualidade para aproveitar o tamanho da tela e a conexão de largura de banda maiores. A entrega de arquivos de vídeo codificados com uma predefinição do Tablet requer que você inclua o código de detecção do dispositivo no site ou aplicativo móvel. Esse código alterna entre uma experiência de vídeo de iPhone ou iPad, dependendo do dispositivo de reprodução. Escolher uma predefinição para dispositivos móveis para fornecer arquivos de vídeo ao iPad é um fluxo de trabalho mais simplificado. Isso ocorre porque você pode usar o mesmo arquivo de vídeo para iPhones e iPads. No entanto, a qualidade é padronizada para a experiência de iPhone em resolução mais baixa.

      * No grupo Predefinições de codificação , na lista suspensa Classificar predefinições de codificação , selecione Nome ou Tamanho para classificar predefinições por nome ou tamanho de resolução.
      * Selecione uma predefinição de codificação com base no tamanho da resolução e na largura de banda com a qual planeja reproduzir o vídeo.
      * Você pode selecionar Codificação de vídeo adaptável e uma ou mais predefinições de codificação por vídeo. Por exemplo, você pode codificar um arquivo para desktop e dispositivo móvel em um trabalho de upload.

Após selecionar **[!UICONTROL Start Upload]**, o arquivo de vídeo principal original é carregado e os arquivos codificados são gerados a partir do arquivo principal.

### Sobre as opções predefinidas de codificação {#about-encoding-preset-options}

Os parâmetros das opções predefinidas de codificação são os seguintes:

* **[!UICONTROL Target connection speed]** - A velocidade de ligação à Internet do utilizador final visado.

* **[!UICONTROL Encoded file suffix]** - O sufixo anexado ao arquivo de vídeo codificado para fins de identificação.

* **[!UICONTROL Video bit rate (data rate)]** - A quantidade de dados que é codificada para formar um único segundo de reprodução de vídeo (em kilobits por segundo).

* **[!UICONTROL Pixel Width/Height]** - A dimensão da largura da imagem da tela, em pixels; a dimensão de altura da imagem da tela (em pixels).

* **[!UICONTROL Frame per second (fps)]** - O número de quadros, ou imagens estáticas, para cada segundo de vídeo. Nos Estados Unidos e Japão, a maioria dos vídeos é filmada a 29,97 fps; na Europa e na Ásia (excluindo o Japão), a maioria dos vídeos é filmada a 25 fps. O filme é filmado a 24 fps.

* **[!UICONTROL Audio bit rate]** - A quantidade de dados que é codificada para formar um único segundo de reprodução de áudio, em kilobits por segundo.

As tabelas a seguir mostram as práticas recomendadas para selecionar predefinições de vídeo e as convenções de nomenclatura usadas para designar arquivos codificados.

### Vídeo adaptável (padrão) {#adaptive-video-default}

Uma predefinição de codificação que funciona com qualquer proporção de aspecto para permitir que você crie vídeos para entrega em dispositivos móveis, tablets e desktops. Os vídeos de origem carregados que são codificados usando essa predefinição (o padrão e uma prática recomendada) são definidos com uma altura fixa, enquanto a largura é dimensionada automaticamente para preservar a proporção do vídeo.

**Vídeo adaptável (padrão)**

|  | Codificação do nome da predefinição/texto da dica de ferramenta | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x 360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | Igual à origem | 64º | Para dispositivos móveis (iPhone, iPad, Android™) |
| 2 | Auto x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | Igual à origem | 96 | Para tablet (iPad, Android™) |
| 1 | Auto x 720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | Igual à origem | 128 | Para desktop |

### Predefinições de vídeo da Codificação de vídeo adaptável (16:9 ou 4:3) {#adaptive-video-encoding-or-video-presets}

Essas predefinições de codificação de vídeo adaptável combinam uma série de predefinições de codificação individuais que são automaticamente selecionadas para você com base na proporção do vídeo que você enviou. Por exemplo, se você fizer upload de um vídeo 4:3, ele será automaticamente codificado usando todas as cinco predefinições 4:3 encontradas na lista predefinida principal na opção **Adaptive Video Encoding (16:9 ou 4:3)** .

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Predefinições de codificação de vídeo adaptável (16:9 ou 4:3)**

|  | Codificação do nome da predefinição/texto da dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Igual à origem | 64º | Baixa resolução, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Igual à origem | 64º | Baixa resolução, 3G |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 800 | 512x288 | Igual à origem | 64º | Resolução média, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 800 | 384x288 | Igual à origem | 64º | Resolução média, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 600 | 640x360 | Igual à origem | 80º | Resolução média, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 600 | 640x480 | Igual à origem | 80º | Resolução média, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | Igual à origem | 96 | Alta resolução, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | Igual à origem | 96 | Alta resolução, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Alta definição, widescreen |
| 10º | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | Igual à origem | 128 | Alta definição |

### Predefinições de codificação de vídeo de desktop {#desktop-video-encoding-presets}

Predefinições de codificação de vídeo para MP4 e OGV em computadores desktop.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - Audio AAC, extensão de arquivo MP4**

|  | Codificação do nome da predefinição/texto da dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | Igual à origem | 64º | Baixa resolução de ecrã panorâmico |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | Igual à origem | 80º | Resolução widescreen média |
| 1 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800x450 | Igual à origem | 96 | Resolução média-alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Alta definição, widescreen |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | Igual à origem | 64º | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 600 | 480x360 | Igual à origem | 80º | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640x480 | Igual à origem | 96 | Resolução média-alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280x960 | Igual à origem | 128 | Alta definição |

**OGG Theora Vorbis - Extensão do arquivo OGV**

|  | Codificação do nome da predefinição/texto da dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Igual à origem | 64º | Baixa resolução de ecrã panorâmico |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Igual à origem | 80º | Resolução widescreen média |
| 1 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | Igual à origem | 96 | Resolução média-alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | Igual à origem | 128 | Alta definição, widescreen |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Igual à origem | 64º | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Igual à origem | 80º | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | Igual à origem | 96 | Resolução média-alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | Igual à origem | 128 | Alta definição |

### Predefinições de codificação de vídeo móvel {#mobile-video-encoding-presets}

Igual a fps de origem. Predefinições de codificação de vídeo para dispositivos móveis iPhone, iPad e Android™.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Linha de base H264 2.1 - AAC de áudio, extensão de arquivo MP4**

|  | Codificação do nome da predefinição/texto da dica de ferramenta | Velocidade de conexão do Target (Kbps) | Sufixo de arquivo codificado | Taxa de bits do vídeo (Kbps) | Largura/altura dos pixels | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Móvel (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Igual à origem | 64º | Baixa resolução, 3G |
| 2 | 16:9, 512x288, Móvel (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512x288 | Igual à origem | 64º | Resolução média, 3G |
| 1 | 16:9, 512x288, Móvel (800 Kbps) | 900 | _Mobile_512x288_800K | 600 | 512x288 | Igual à origem | 80º | Resolução média, Wi-Fi |
| 4 | 16:9, 512x288, Móvel (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | Igual à origem | 80º | Alta resolução, Wi-Fi |
| 5 | 16:9, 512x288, Móvel (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | Igual à origem | 96 | Alta resolução, Wi-Fi |
| 6 | 4:3, 384x288, Móvel (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Igual à origem | 64º | Baixa resolução, 3G |
| 7 | 4:3, 384x288, Móvel (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Igual à origem | 64º | Resolução média, 3G |
| 8 | 4:3, 448x336, Móvel (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Igual à origem | 80º | Resolução média, Wi-Fi |
| 9 | 4:3, 448x336, Móvel (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | Igual à origem | 80º | Alta resolução, Wi-Fi |
| 10º | 4:3, 448x336, Móvel (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | Igual à origem | 96 | Alta resolução, Wi-Fi |

## Predefinições do visualizador {#viewer-presets}

>[!NOTE]
>
>**Aviso de fim de vida útil de visualizadores de Flash**  - a partir de 31 de janeiro de 2017, o Adobe Dynamic Media Classic oficialmente encerrou o suporte para a plataforma do visualizador de Flashes.

Uma *Predefinição do visualizador* é uma coleção de configurações que determinam como os usuários visualizam ativos de mídia avançada em suas telas de computadores e dispositivos móveis. Como administrador, você pode criar Predefinições do visualizador. As configurações estão disponíveis para uma matriz de opções de configuração do visualizador. Por exemplo, você pode alterar o tamanho de exibição do visualizador, o comportamento de zoom, esquemas de cores, bordas e fontes.

Como prática recomendada, use visualizadores de vídeo HTML5 do Adobe Dynamic Media Classic. As predefinições usadas em visualizadores de vídeo HTML5 são players de vídeo robustos.

Ao combinar em um único reprodutor o seguinte:

* A capacidade de projetar os componentes de reprodução usando HTML5 e CSS.
* Reprodução incorporada.
* Use streaming adaptável e progressivo, dependendo da capacidade do navegador.

Você estende o alcance do seu conteúdo de mídia avançada para usuários de desktop, tablet e dispositivos móveis e garante uma experiência de vídeo simplificada.

Consulte [Sobre visualizadores HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) no Guia de referência de visualizadores do Adobe.

Consulte [Matriz de compatibilidade de predefinições do visualizador do Adobe Classic](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consulte [Prática recomendada: Usando o visualizador de vídeo HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependendo do visualizador, você pode adicionar recursos da comunidade. Os recursos da comunidade incluem um botão Incorporar, um botão de Email, um botão Link e um botão Visitar site. Esses botões permitem que as pessoas que usam os visualizadores compartilhem o visualizador com outras pessoas ou abram o site do Adobe Dynamic Media Classic.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Suporte de visualizador para páginas da Web responsivas projetadas {#viewer-support-for-responsive-designed-web-pages}

Páginas da Web diferentes têm necessidades diferentes. Às vezes, você deseja uma página da Web que forneça um link que abra o Visualizador de HTML5 em uma janela separada do navegador. Em outros casos, é necessário incorporar o Visualizador HTML5 diretamente na página de hospedagem. No último caso, a página da Web provavelmente tem um layout estático. Ou é &quot;responsivo&quot; e exibido de forma diferente em diferentes dispositivos ou para tamanhos de janela de navegador diferentes. Para acomodar essas necessidades, os visualizadores HTML5 fornecidos com o Adobe Dynamic Media Classic suportam páginas da Web estáticas e páginas da Web responsivas projetadas.

Para obter mais informações sobre como incorporar visualizadores responsivos às suas páginas da Web, consulte [Sobre a biblioteca de imagens responsivas](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Usar biblioteca de imagens responsivas](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) e [Referência de comando - Atributos de comando](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Tipos de predefinição do visualizador {#viewer-preset-types}

Os administradores podem criar e personalizar os seguintes tipos de Predefinições do visualizador:

* **[!UICONTROL eCatalog Viewer]** - Simula a experiência de ler um catálogo impresso. Você pode mover de página em página, ampliar e reduzir itens em uma página, usar mapas de imagem para ver mais informações sobre itens na página ou pesquisar o catálogo. Você também pode incluir um Painel de informações para exibir informações detalhadas e um item mapeado por imagem se a área do mapa tiver um atributo rolover_key válido. Para incluir um painel Informações, especifique um URL do Servidor de Informações no painel Configurações do painel Informações da janela Predefinição do visualizador de catálogo eletrônico.

* **[!UICONTROL Swatch Set Viewer]** - Exibe uma imagem em uma cor, material, textura, acabamento ou tecido diferente. Os usuários selecionam uma miniatura para ver as variações na imagem.

* **[!UICONTROL Mixed Media Set Viewer]** - Exibe diferentes tipos de mídia em um visualizador. Você pode incluir Conjuntos de amostras, Conjuntos de rotação, imagens e vídeos. É possível configurar guias para conter diferentes tipos de conteúdo, como uma guia para conjuntos de imagens e uma guia para vídeos. Os vídeos reproduzidos de um Conjunto de mídias mistas usam um visualizador de vídeo padrão com uma linha do tempo e controles de vídeo, como Parar, Pausar, Voltar e Reproduzir. Ao configurar uma predefinição do Visualizador de conjunto de mídias mistas, você especifica quais visualizadores deseja usar para os diferentes tipos de ativos no seu Conjunto de mídias mistas. Você também pode usar o Visualizador de grade ou o Visualizador de carrossel para exibir um Conjunto de mídias mistas.

* **[!UICONTROL Spin Set Viewer]** - Fornece várias visualizações de uma imagem para que os usuários possam girar o objeto para examinar os diferentes lados e ângulos.

* **Visualizador de vídeo**  - Exibe vídeos usando as dimensões de resolução do arquivo de origem ou um tamanho personalizado. O Adobe Dynamic Media Classic vem com muitas predefinições predefinidas do visualizador para reprodução de vídeo e, se você for um administrador, poderá criar predefinições personalizadas do visualizador de vídeo. Há mais de uma dúzia de configurações diferentes para definir o Visualizador de vídeo. Você pode configurar o tamanho, a cor de primeiro e segundo plano, os controles de áudio e vídeo, a barra de progresso, a interface do usuário de pele, os recursos sociais e a Ajuda.

* **[!UICONTROL Zoom Viewers]** - Oferece uma escolha de três tipos de visualizador de zoom:

* **[!UICONTROL Zoom Viewer]** - Permite que os usuários ampliem a área selecionando-a. Eles podem selecionar controles para ampliar, reduzir e redefinir a imagem para seu tamanho padrão.

* **[!UICONTROL Zoom Viewer: Fly-out]** - Exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção para a área que desejam visualizar.

Ao determinar o uso total da largura de banda para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem principal (Largura e Altura do Palco) e o Fator de Zoom determinam o tamanho da imagem do flyout. Para impedir que o tamanho do arquivo flyout se torne muito grande, equilibre esses dois valores: se você tiver um tamanho de imagem principal grande, abaixe o valor de Fator de Zoom. (A Largura do Flyout e a Altura do Flyout determinam o tamanho da janela do flyout, mas não o tamanho da imagem do flyout que é servida no visualizador.)

Por exemplo, se o tamanho da imagem principal for 350 por 350 pixels, com um Fator de Zoom de 3, a imagem de flyout resultante será de 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de Zoom de 4, a imagem de flyout será de 1200 por 1200 pixels. Dependendo da configuração de qualidade JPEG (as configurações recomendadas estão entre 80 e 90), você pode diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

### Matriz de compatibilidade de predefinições do visualizador do Adobe Dynamic Media Classic {#scene-viewer-preset-compatibility-matrix}

**Aviso** de fim de vida útil de visualizadores de Flashes: A partir de 31 de janeiro de 2017, o Adobe Dynamic Media Classic encerrou oficialmente o suporte para a plataforma do visualizador de Flashes.

A tabela a seguir identifica as predefinições do visualizador clássico do Adobe atualmente disponíveis. A tabela também especifica a compatibilidade do visualizador com dispositivos móveis e de desktop e a tecnologia usada para cada visualizador específico.

Consulte também [Exemplos de biblioteca de referência de visualizadores do Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Para obter informações sobre versões compatíveis de navegadores da Web e sistemas operacionais para visualizadores, consulte as Notas de versão dos visualizadores.

Consulte [Notas de versão de referência de visualizadores do Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de amostras |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Inclui suporte para mídia social e pesquisa de catálogo.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Inclui suporte para mídia social e pesquisa de catálogo.) | HTML5 | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de rotação |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizadores de eVideo**

O Adobe Dynamic Media Classic é compatível com a reprodução de vídeo móvel para vídeo MP4 H.264.

* Você pode encontrar dispositivos BlackBerry® que suportam este formato de vídeo no seguinte endereço: [Formatos de vídeo suportados no BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Você também pode encontrar dispositivos Windows® que suportam este formato de vídeo no seguinte endereço: [Formatos de vídeo suportados no Windows® Phone](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ | Smartphone BlackBerry® | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Inclui suporte para legendas ocultas.) Consulte [Prática recomendada: Usando o visualizador de vídeo HTML5 universal.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclui suporte para legendas ocultas e redes sociais.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de mídias mistas |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matriz de gestos de visualizadores móveis compatíveis {#supported-mobile-viewers-gestures-matrix}

A tabela a seguir identifica os gestos do visualizador móvel que são suportados em dispositivos iOS, Android™ 2.x e Android™ 3.x.

|  | Tecnologia de visualizador | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Tablet Android™ |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Sobre a tela Predefinição do visualizador {#about-the-viewer-preset-screen}

Crie e gerencie as Predefinições do visualizador na tela Predefinições do visualizador . Para abrir esta tela, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

A tela Predefinições do visualizador oferece ferramentas para executar estas tarefas:

* **Adicionar uma predefinição**  - Selecione  **[!UICONTROL Add]** e faça escolhas na caixa de diálogo Adicionar predefinição do visualizador.

       Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).
   
* **Editar uma predefinição**  - Selecione uma predefinição e selecione  **[!UICONTROL Edit]**.

       Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).
   
* **Excluir uma predefinição**  - Selecione uma predefinição e selecione  **[!UICONTROL Delete]**.

* **Exportar uma predefinição**  - Selecione uma predefinição do visualizador HTML5 e selecione  **[!UICONTROL Export]** para baixar a capa do visualizador para usá-la como a base para criar e adicionar outra predefinição do visualizador.

       Consulte [Exportar uma predefinição do visualizador de HTML5](application-setup.md#export_an_html5_viewer_preset).
   
* **Filtrar a lista Predefinição do visualizador**  - Use estas ferramentas para filtrar a lista:

       * Abra a lista suspensa **Ativo/Inativo** e selecione uma opção para mostrar predefinições ativas, predefinições inativas ou todas as predefinições.
       * Abra a lista suspensa **Visualizador** e selecione uma opção para ver apenas visualizadores de um determinado tipo. Selecione **[!UICONTROL All Viewers]** para ver todos os visualizadores.
   
* **Classificar predefinições**  - Selecione um cabeçalho de coluna (**[!UICONTROL Active]**,  **[!UICONTROL Type]**,  **[!UICONTROL Preset]** ou  **[!UICONTROL Platform]**) para classificar a lista em uma coluna. Selecione um cabeçalho de coluna uma segunda vez para classificar a lista em ordem decrescente (ou crescente).

* **Ativar e desativar predefinições**  - Selecione uma predefinição e, em seguida, a opção Ativa para ativá-la ou desativá-la.

       Consulte [Ativar ou desativar predefinições do visualizador](application-setup.md#ativating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Selecione **[!UICONTROL Preview]** no lado direito da página Predefinições do visualizador para que você possa ver a aparência de um ativo na Predefinição do visualizador selecionada. Para ver um ativo diferente, selecione **[!UICONTROL Browse]** na página Predefinições do visualizador e selecione um ativo diferente na caixa de diálogo Selecionar visualização de ativo.

### Adicionar e editar predefinições do visualizador {#adding-and-editing-viewer-presets}

Além de adicionar predefinições do visualizador usando **[!UICONTROL Add]** na interface do usuário, você também pode usar **[!UICONTROL Export]** para adicionar uma predefinição do visualizador. Basta exportar uma predefinição existente do visualizador de HTML5 e usá-la como a base para a nova predefinição.

Consulte [Exportar uma predefinição do Visualizador HTML5](application-setup.md#exporting_an_html5_viewer_preset).

**Para adicionar e editar predefinições do Visualizador:**

1. Próximo ao canto superior direito do Adobe Dynamic Media Classic, vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

   Você pode filtrar na lista de predefinições. Por exemplo, para ver apenas predefinições para Visualizadores de vídeo, selecione Visualizador de vídeo no menu suspenso Visualizadores na barra de ferramentas logo acima da tabela.

1. Na página Predefinições do visualizador , adicione ou edite a Predefinição do visualizador na tela Predefinições do visualizador .

   * **Adicionar**  - Na barra de ferramentas, selecione  **[!UICONTROL Add]**. Na caixa de diálogo Adicionar predefinição do visualizador, selecione uma plataforma e um tipo de ativo de mídia avançada.

          Selecione **[!UICONTROL Save As]** quando terminar de criar a Predefinição do visualizador.
      
   * **Adicionar iniciando em uma predefinição existente do Visualizador**  - na tabela, selecione uma Predefinição do visualizador de vídeo e selecione  **[!UICONTROL Edit]** na barra de ferramentas.

          Após reconfigurar o Visualizador de vídeo, selecione **[!UICONTROL Save As]** para salvar a predefinição usando um nome diferente no campo de texto Nome da predefinição.
      
   * **Editar**  - Selecione uma Predefinição do visualizador existente e selecione  **[!UICONTROL Edit]**.

1. Na tela Configurar visualizador, no campo Nome da predefinição , digite ou edite o nome da predefinição.
1. Defina as opções restantes que deseja.

   >[!NOTE]
   >
   >Selecione **[!UICONTROL Same As Source]** para dimensionar automaticamente o Visualizador de vídeo para o tamanho de resolução do próprio vídeo codificado. Se você selecionar essa opção, não poderá inserir a Largura do palco e a Altura do palco. Em vez disso, essas opções vêm do próprio vídeo. Se você selecionar **[!UICONTROL Same As Source]**, defina a opção Tamanho da margem para refletir as dimensões de capa fora da área de reprodução do vídeo. Esse tamanho da margem é a altura e a largura do pixel dos controles de vídeo. Você pode usar a imagem a seguir para ajudá-lo a determinar os tamanhos de margem que deseja usar.*

   ![Configuração de margem do visualizador de vídeo](assets/vs_video_viewer_configure_margin.png)

1. Siga um destes procedimentos:

   * Selecione **[!UICONTROL Save As]** se tiver adicionado uma predefinição do Visualizador, começando com uma predefinição existente.
   * Selecione **[!UICONTROL Save]** se tiver adicionado ou editado uma predefinição do Visualizador.

### Exportar uma predefinição de visualizador HTML5 {#exporting-an-html-viewer-preset}

Você pode exportar uma Predefinição do visualizador HTML5 existente para usar como a base para criar uma Predefinição do visualizador HTML5. Essa opção de exportação é útil, pois não é necessário criar o visualizador do zero. Em vez disso, você exporta uma predefinição que se comporta e tem a aparência desejada, então pode usá-la como ponto de partida para fazer ajustes de design.

Todos os arquivos CSS predefinidos padrão e prontos para uso do Visualizador no Adobe Dynamic Media Classic usam caminhos de exibição de imagens relativas que apontam para ativos em `Scene7SharedAssets`. Por exemplo, o seguinte é um caminho relativo para um ativo de imagem em um arquivo CSS predefinido do visualizador em

`Scene7SharedAsset`:  `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

No entanto, se você hospeda arquivos CSS do Visualizador em seu próprio site, é necessário resolver esses caminhos de imagem relativos usando um caminho explícito para o Servidor de imagem em seu próprio ambiente. Por exemplo, se você atualizasse o caminho relativo acima para um caminho explícito, ele poderia parecer o seguinte, onde `https://s7d1.scene7.com` é o caminho direto para o seu servidor de imagem: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar uma predefinição do visualizador HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na barra de ferramentas Predefinições do visualizador, na segunda lista suspensa à esquerda, selecione **[!UICONTROL HTML5]**.
1. Na terceira lista suspensa à esquerda, selecione **[!UICONTROL All Viewers]**.
1. Selecione a predefinição do visualizador que você deseja usar como a base para uma nova Predefinição do visualizador HTML5.
1. Na barra de ferramentas, selecione **[!UICONTROL Export]**.
1. Na caixa de diálogo Exportar ativos selecionados , selecione **[!UICONTROL Submit Export]**.

   Após a exportação, você obtém um arquivo CSS. Baixe e descompacte o arquivo .

1. Abra o arquivo CSS em um editor de CSS, faça as alterações e salve o arquivo.
1. Faça upload do arquivo CSS para o Adobe Dynamic Media Classic.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. Publique o arquivo CSS no servidor de imagem do Dynamic Media.

   Consulte [Publicação de arquivos](publishing-files.md#publishing_files).

1. Adicione a nova predefinição do visualizador como de costume. Selecione o arquivo CSS do visualizador que você carregou.

   Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

### Ativar ou desativar predefinições do visualizador {#activating-or-deactivating-viewer-presets}

Para criar um URL para mostrar ativos, os usuários abrem a lista suspensa Predefinições na caixa de diálogo Visualizar , selecionam uma Predefinição do visualizador e selecionam **[!UICONTROL Copy URL]** (consulte [Copiar o URL de uma Predefinição do visualizador](application-setup.md#copying_the_url_of_a_viewer_preset)). Essa lista de Predefinições oferece Predefinições do visualizador que os administradores adicionam e gerenciam na tela Predefinições do visualizador. Por exemplo, todas as predefinições ativas do Visualizador do eCatalog são exibidas na lista suspensa Predefinições na caixa de diálogo Visualizar quando um usuário visualiza um eCatalog.

A menos que você desative as Predefinições do visualizador na tela Predefinições do visualizador, a lista suspensa Predefinições na caixa de diálogo Visualizar pode ser lotada.

**Para ativar ou desativar as Predefinições do visualizador:**

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Na página Predefinições do visualizador , selecione ou desmarque as opções **[!UICONTROL Active]** para ativar ou desativar as Predefinições do visualizador.

### Copiar o URL de uma predefinição do visualizador {#copying-the-url-of-a-viewer-preset}

Após publicar um ativo, é possível copiar um URL para exibir o ativo com as configurações de uma Predefinição do visualizador.

O URL é copiado para a Área de Transferência. Você pode usá-lo conforme necessário no código HTML de sua página da Web, dispositivo móvel ou aplicativo.

**Para copiar o URL de uma predefinição do visualizador:**

1. Selecione o ativo no painel Procurar.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs e Código incorporado à direita, selecione **[!UICONTROL Copy URL]** à direita do visualizador desejado.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, em seguida, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Copy URL]**.

### Copiar o código incorporado de uma predefinição do visualizador {#copying-the-embed-code-of-a-viewer-preset}

Usar o recurso Incorporar código permite que você revise o código do visualizador para a Predefinição do visualizador selecionada. Você também pode copiar o código para a área de transferência, de modo que possa colá-lo em suas páginas da Web para a implantação do visualizador.

A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de uma predefinição do visualizador:**

1. Selecione o ativo no painel Navegação de ativos.
1. Acima do painel Navegação de ativos , no lado direito da barra de ferramentas, execute um dos seguintes procedimentos:

   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, clique duas vezes em um único ativo para abri-lo na Exibição de detalhes. No painel URLs à direita, selecione **[!UICONTROL Embed Code]**.
   * Selecione **[!UICONTROL Grid View]**. No painel Navegação de ativos, selecione um único ativo e, em seguida, abaixo da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL List View]**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

   * Selecione **[!UICONTROL Grid View]**, **[!UICONTROL List View]** ou **[!UICONTROL Detail View]**. Na mesma barra de ferramentas, vá para **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   Na página Lista de visualizadores , na coluna Ações da tabela, selecione **[!UICONTROL Embed Code]**.

1. Na caixa de diálogo Incorporar código, selecione **[!UICONTROL Copy to Clipboard]**.
1. Selecione **[!UICONTROL Close]**.

## Configurar visualizadores padrão {#configuring-default-viewers}

Você pode usar Visualizadores padrão para configurar o visualizador padrão associado a um ativo quando você usa Visualização no Adobe Dynamic Media Classic. Você pode configurar a experiência de visualização padrão para os seguintes tipos de ativos:

* Imagem
* Vídeo
* SpinSet
* Catálogo
* ImageSet
* SwatchSet
* MediaSet

**Para configurar visualizadores padrão:**

1. Na lista suspensa Configurar , selecione **[!UICONTROL Application Setup]**.
1. Na janela Configuração, no painel esquerdo, vá para **[!UICONTROL Application Setup]** > **[!UICONTROL Viewers]**
1. Selecione **[!UICONTROL Default Viewers]**.
1. Na janela Visualizadores padrão, na lista suspensa de cada tipo de ativo, selecione o visualizador que deseja associar à visualização do ativo.
1. No canto inferior direito da janela Visualizadores padrão, selecione **[!UICONTROL Save Settings]**.
1. No canto inferior direito da janela Configurar, selecione **[!UICONTROL Close]** para retornar à janela Ativo.

## Visualizações de metadados {#metadata-views}

** Metadados padronizam informações sobre um ativo. Você pode usar metadados para simplificar seu fluxo de trabalho, organizar seus ativos e melhorar a pesquisa. O Adobe Dynamic Media Classic é compatível com o padrão IPTC (International Press Telecommunications Council) e o padrão XMP (extensible metadata platform). Antes de os usuários visualizarem ou inserirem metadados sobre um ativo na Exibição de detalhes, eles podem abrir o menu Visualizações de metadados . A partir daí, é possível selecionar o conjunto de campos de metadados que deseja exibir ou usar para descrever o ativo.

O Adobe Dynamic Media Classic vem com Exibições de metadados predefinidas, e os administradores podem criar suas próprias Exibições de metadados para que os usuários escolham quando inserem metadados.

### Criar uma visualização de metadados {#creating-a-metadata-view}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Selecione **[!UICONTROL Add]**.
1. No campo de texto Nome da predefinição , digite um nome para a exibição.
1. (Opcional) Marque **[!UICONTROL Make Default]** para tornar essa visualização aquela que os usuários veem quando abrem o painel Metadados na Exibição detalhada.
1. (Opcional) Selecione **[!UICONTROL Include UDF]** para incluir campos definidos pelo usuário na exibição. Os campos definidos pelo usuário são exibidos na parte superior do painel Metadados na Exibição de detalhes.
1. Selecione os campos que deseja para a exibição (selecione **[!UICONTROL Select All]** para selecionar todos os campos).
1. Selecione **[!UICONTROL Save]**.

   As categorias e campos selecionados para a exibição são exibidos no painel Visualização .

### Gerenciar visualizações de metadados {#managing-metadata-views}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Siga um destes procedimentos:

   * Para visualizar uma visualização, selecione-a. Os campos na exibição aparecem no painel Visualização.
   * Para editar uma exibição, selecione-a e depois selecione **[!UICONTROL Edit]**. Em seguida, selecione ou desmarque nomes de campos no painel Visualização e selecione ou desmarque a opção **[!UICONTROL Include UDF]**.
   * Para excluir uma exibição, selecione-a e, em seguida, selecione **[!UICONTROL Delete]**.
   * Para tornar uma exibição o padrão, selecione-a e, em seguida, selecione **[!UICONTROL Make Default]**. A exibição padrão é aquela que os usuários veem quando abrem um ativo na Exibição detalhada e vão para o painel Metadados.

## Predefinições de metadados {#metadata-presets}

As Predefinições de metadados fornecem aos administradores uma maneira de controlar e regular os metadados que são atribuídos a ativos. Na Exibição de detalhes, um usuário pode inserir metadados sobre um ativo em campos fornecidos para essa finalidade. Por exemplo, um usuário pode inserir um nome de proprietário, uma descrição de copyright e um endereço. Para garantir que os usuários insiram essas informações de maneira precisa e completa, é possível criar Predefinições de metadados. A escolha de uma Predefinição de metadados na Exibição de detalhes preenche os campos de metadados com valores predefinidos. Por exemplo, um nome de proprietário, uma descrição de copyright e um endereço são inseridos automaticamente.

Crie uma Predefinição de metadados para cada conjunto de valores de metadados que deseja que os usuários possam inserir automaticamente na Exibição de detalhes para descrever um ativo.

### Criar ou editar uma predefinição de metadados {#creating-or-editing-a-metadata-preset}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Na tela Predefinições de metadados, execute um dos seguintes procedimentos:

   * Para criar uma predefinição, selecione **[!UICONTROL Add]**. No campo de texto Nome do modelo de metadados , digite um nome para a predefinição. Selecione **[!UICONTROL Metadata Views]** e selecione uma exibição na lista suspensa (consulte [Visualizações de metadados](application-setup.md#metadata_views)).
   * Para editar uma predefinição existente, selecione a predefinição na lista Predefinições de metadados e selecione **[!UICONTROL Edit]**.

1. Expanda os cabeçalhos que deseja incluir na predefinição e insira valores nos diferentes campos que deseja incluir na predefinição.
1. Selecione **[!UICONTROL Save]**.

   As categorias e campos selecionados para a predefinição aparecem no painel Visualização .

### Gerenciar predefinições de metadados {#managing-metadata-presets}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Siga um destes procedimentos:

   * Para visualizar uma predefinição, selecione a predefinição que deseja visualizar. As informações predefinidas (categorias e campos) são exibidas na tela Preview .
   * Para excluir uma predefinição, selecione a predefinição e selecione **[!UICONTROL Delete]**.

## Campos definidos pelo usuário {#user-defined-fields}

Um Administrador do Media Portal ou um Administrador de empresa pode criar campos de metadados personalizados e definidos pelo usuário. Os campos personalizados podem ajudar a organizar ativos no Adobe Dynamic Media Classic. Você pode marcar os campos como Ativos, conforme necessário. Quando ativados, os nomes desses campos de metadados personalizados são exibidos no painel Metadados na Exibição de detalhes. Os usuários podem inserir informações em campos de metadados definidos pelo usuário para descrever ativos. Os usuários também podem tornar um campo de metadados definido pelo usuário um critério em pesquisas.

Um uso eficaz de campos de metadados definidos pelo usuário é atrasar o tempo de ativação de um ativo para uma inicialização ou venda específica. Você define um campo &quot;ativação&quot;, com base no tipo *Date*. Em seguida, usando o painel **[!UICONTROL Metadata]** na Exibição de detalhes ou **[!UICONTROL File]** > **[!UICONTROL Edit Info]**, é possível especificar quando o ativo é ativado. O Adobe Dynamic Media Classic verifica o status de publicação de um ativo e o histórico de publicação. Se não estiver dentro do tempo de ativação, o status de publicação será exibido como &quot;Não publicado&quot;.

>[!NOTE]
>
>Para fazer com que os campos definidos pelo usuário apareçam no painel Metadados na Exibição detalhada, inclua os campos definidos pelo usuário nas Exibições de metadados. Na tela Visualizações de metadados, selecione a opção Incluir UDF (campos definidos pelo usuário) . Para obter mais informações, consulte [Visualizações de metadados](application-setup.md#metadata_views).

>[!NOTE]
>
>Para pesquisar ativos usando campos personalizados e definidos pelo usuário, vá para **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** e selecione **[!UICONTROL Include UDFs in Search]**. Consulte [Configuração Pessoal](personal-setup.md#personal_setup).

### Criar um campo de metadados definido pelo usuário {#creating-a-user-defined-metadata-field}

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.
1. Selecione **[!UICONTROL Add]**
1. Na caixa de diálogo Campo personalizado, defina as opções desejadas.

   * **[!UICONTROL Name]** - Insira um nome para o campo de metadados.

   * **[!UICONTROL Type]** - Selecione uma opção que defina o tipo de informação que os usuários podem inserir no campo de metadados:

   * **[!UICONTROL String]** - Uma string de texto.

   * **[!UICONTROL Int]** - Um número inteiro.

   * **[!UICONTROL Float]** - Um número de ponto flutuante.

   * **[!UICONTROL Yes/No]** - Um valor booleano sim/não.

   * **[!UICONTROL Date]** - Uma data. O formato MM/DD/AAAA é aceito.

   * **[!UICONTROL Filename]** - O nome de um arquivo.

   * **[!UICONTROL Color]** - O nome de uma cor.

   * **[!UICONTROL Dimension]** - A largura e a altura do ativo.

   * **[!UICONTROL Untyped]** - Para compatibilidade com versões anteriores. Não selecione essa opção.

   * **[!UICONTROL Default Value]** - Opcionalmente, insira o valor que os usuários provavelmente inserirão no campo. O valor inserido se torna o valor padrão para o campo criado.

   * **[!UICONTROL Applies To]** - Opcionalmente, selecione um tipo de ativo se desejar que o campo de metadados seja aplicado somente a um tipo específico de ativo.

      >[!NOTE]
      >
      >Selecione uma opção **[!UICONTROL Applies To]** cuidadosamente porque não é possível alterar a opção **[!UICONTROL Applies To]** depois de criar um campo definido pelo usuário. O Adobe Dynamic Media Classic permite editar o nome, o tipo e o valor padrão de um campo definido pelo usuário, mas não a configuração **[!UICONTROL Applies To]**. *

1. Selecione **[!UICONTROL Save]** quando terminar de criar o campo de metadados.

### Gerenciar campos definidos pelo usuário {#manage-user-defined-fields}

A tela Campos definidos pelo usuário oferece comandos para gerenciar campos de metadados personalizados e definidos pelo usuário.

Somente um Administrador do Media Portal ou um Administrador de empresa pode gerenciar campos definidos pelo usuário.

Para abrir esta tela, vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.

* **Editar um campo**  - Selecione o campo e selecione  **[!UICONTROL Edit]**.

* **Excluir um campo**  - Selecione o campo e selecione  **[!UICONTROL Delete]**.

* **Ativate field**  - Selecione ou desmarque a  **[!UICONTROL Active]** opção ao lado do nome de um campo. Se você estiver em uma função de administração da empresa, essa opção não será exibida. Como essa opção está relacionada ao MediaPortal, você deve selecionar (ativar) Mostrar recursos do MediaPortal em Configuração Pessoal para ver os campos de ativação.

## Otimizar arquivos {#optimize-files}

À medida que você carrega arquivos no Adobe Dynamic Media Classic, o sistema os otimiza para armazenamento e publicação. No entanto, se o processo de upload for interrompido, algumas imagens não poderão ser otimizadas. Nesse caso, você verá a mensagem &quot;Imagem ainda não otimizada&quot;. No entanto, você pode otimizar esses arquivos se for um administrador.

O Adobe Dynamic Media Classic pesquisa seus arquivos e otimiza apenas as imagens que não estavam totalmente otimizadas antes.

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** e selecione **[!UICONTROL Optimize Files]**.
1. Insira as informações do trabalho de otimização e selecione **[!UICONTROL Submit]**.

   Se você estiver trabalhando com mais de uma empresa, otimize os arquivos pertencentes a empresas diferentes separadamente.

## Predefinições do conjunto de lotes {#batch-set-presets}

Use as predefinições do conjunto de lotes para criar automaticamente conjuntos de imagens ou conjuntos de rotação enquanto uma tarefa está em execução para carregar ativos no Adobe Dynamic Media Classic.

Os administradores de empresas definem primeiro as convenções de nomenclatura dos ativos que desejam agrupar em um conjunto. Em seguida, é possível criar uma predefinição de conjunto de lotes para fazer referência a essas imagens. Cada predefinição é um conjunto de instruções autocontidas e com nome exclusivo que define como construir o conjunto usando imagens que correspondem às convenções de nomenclatura definidas na receita predefinida.

Todas as predefinições do conjunto de lotes ativas de uma empresa são listadas na caixa de diálogo Upload Job Option , para que você possa especificar qual predefinição deseja aplicar durante cada sessão de upload. Os administradores da empresa veem todas as predefinições de conjunto de lotes ativas e inativas. Ao carregar arquivos, o Adobe Dynamic Media Classic cria automaticamente um conjunto com todos os arquivos que correspondem à convenção de nomenclatura definida nas predefinições ativas.

### Nomenclatura padrão {#default-naming}

O administrador da empresa cria uma convenção de nomenclatura padrão usada em qualquer receita predefinida de conjunto de lotes. A convenção de nomenclatura padrão selecionada na definição predefinida do conjunto de lotes pode ser tudo o que é necessário para que sua empresa gere conjuntos em lote para todos os sites. Uma predefinição de conjunto de lotes é criada para usar a convenção de nomenclatura padrão que você definir. Você pode criar quantas predefinições do Conjunto de Lotes tiverem as convenções de nomenclatura alternativas e personalizadas necessárias para um conjunto específico de conteúdo, em casos em que há uma exceção na nomenclatura padrão definida pela empresa.

A configuração de uma convenção de nomenclatura padrão não é necessária para usar a funcionalidade predefinida do conjunto de lotes. No entanto, a prática recomendada pelo Adobe é usar uma convenção de nomenclatura padrão para definir quantos elementos da convenção de nomenclatura você deseja agrupar em um conjunto. Isso ajuda a simplificar a criação de conjuntos em lotes.

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**.
1. Selecione **[!UICONTROL View Form]** ou **[!UICONTROL View Code]** para especificar como deseja visualizar e inserir informações sobre cada elemento.

   Você pode marcar a caixa de seleção **[!UICONTROL View Code]** para exibir a criação do valor da expressão regular ao lado das seleções de formulário. É possível inserir ou alterar esses valores para ajudar a definir os elementos da convenção de nomenclatura, se a exibição do formulário limitar você por qualquer motivo. Se os valores não puderem ser analisados na visualização do formulário, os campos do formulário ficarão inativos.

   >[!NOTE]
   >
   >Campos de formulário desativados não indicam expressões regulares inválidas. Não há validação de que suas expressões regulares estejam corretas. Você verá os resultados da expressão regular que está criando para cada elemento após a linha Resultado. A expressão regular completa é visível na parte inferior da página.

1. Expanda cada elemento conforme necessário e insira as convenções de nomenclatura que deseja usar.
1. Conforme necessário, selecione **[!UICONTROL Add]** para adicionar outra convenção de nomenclatura para um elemento. Ou selecione **[!UICONTROL Remove]** para excluir uma convenção de nomenclatura para um elemento.
1. Selecione **[!UICONTROL Save As]** e digite um nome para a predefinição. Ou selecione **[!UICONTROL Save]** se estiver editando uma predefinição existente.

Como alternativa, você pode usar Exibir código sem nenhum campo de formulário disponível. Nesta visualização, você cria suas definições de convenção de nomenclatura totalmente usando expressões regulares.

Dois elementos estão disponíveis para definição, Correspondência e Nome de base. Esses campos permitem definir todos os elementos de uma convenção de nomenclatura e identificar a parte da convenção usada para nomear o conjunto no qual eles estão contidos. A convenção de nomenclatura individual de uma empresa pode usar uma ou mais linhas de definição para cada um desses elementos. Você pode usar quantas linhas para sua definição exclusiva e agrupá-las em elementos distintos, como para Imagem principal, Elemento de cor, Elemento de exibição alternativo e Elemento de amostra.

### Criar uma predefinição de conjunto de lotes {#creating-a-batch-set-preset}

O Adobe Dynamic Media Classic usa predefinições de conjunto em lote para organizar ativos que compartilham algumas informações ou conteúdo comuns em conjuntos de imagens para exibição em visualizadores. As receitas predefinidas do conjunto de lotes são executadas automaticamente junto com os trabalhos de importação de ativos agendados no Adobe Dynamic Media Classic.

Use a predefinição do conjunto de lotes para criar, editar e gerenciar as predefinições do conjunto de lotes. É possível criar quantas predefinições forem necessárias para cobrir todas as tarefas de assimilação de ativos forem necessárias. Existem duas formas de definições predefinidas de conjunto de lotes: um para uma convenção de nomenclatura padrão que você configurou e um para convenções de nomenclatura personalizadas que você cria em tempo real.

Você pode usar o método de campo de formulário para definir uma predefinição de conjunto de lotes ou o método de código, que permite usar expressões regulares. Como em **[!UICONTROL Default Naming]**, você pode selecionar **[!UICONTROL Code View]** ao mesmo tempo em que está definindo na Exibição de formulário e usando expressões regulares para criar suas definições. Como alternativa, você pode desmarcar qualquer exibição para usar uma ou a outra exclusivamente.

Consulte também [Criar uma predefinição de conjunto de lotes para a geração automática de um Conjunto de rotação 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Para criar uma predefinição de conjunto de lotes:**

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista de predefinições , selecione **[!UICONTROL Add]** para ativar os campos de definição no painel Detalhes no lado direito da página.
1. No painel Detalhes, no campo Nome da predefinição , digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione um tipo predefinido.

   Para gerar automaticamente um Conjunto de rotação 2D, selecione **[!UICONTROL Multi-Axis Spin Set]** na lista suspensa Tipo de conjunto de lotes .

1. Siga um destes procedimentos:

   * Se estiver usando uma convenção de nomenclatura padrão configurada anteriormente em **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**, expanda **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomenclatura de Arquivo, selecione **[!UICONTROL Default]**.
   * Para definir uma convenção de nomenclatura conforme configura a predefinição, expanda **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomeação de arquivo , selecione **[!UICONTROL Custom]**.

1. Para Sequência, defina a ordem das imagens depois que o conjunto for agrupado no Adobe Dynamic Media Classic. Por padrão, os ativos são classificados alfanumérico. No entanto, é possível usar uma lista separada por vírgulas de expressões regulares para definir a ordem.
1. Para Definir a Convenção de Nomenclatura e Criação, especifique o sufixo ou prefixo do nome básico definido na Convenção de Nomenclatura de Ativos. Defina também onde o conjunto de imagens é criado na estrutura de pastas do Adobe Dynamic Media Classic.

   Se você definir grandes números de conjuntos de imagens, mantenha esses conjuntos separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados por conjuntos em lotes aqui.

1. Selecione **[!UICONTROL Save]** no Painel de Detalhes.

### Criar uma predefinição de conjunto de lotes para a geração automática de um Conjunto de rotação 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Você pode usar o Tipo de Conjunto de Lotes **Conjunto de Rotação de Vários Eixos** para criar uma &quot;receita&quot; que automatiza a geração de Conjuntos de Rotação 2D. O agrupamento de imagens usa expressões regulares de Linha e Coluna para que os ativos de imagem sejam alinhados corretamente no local correspondente na matriz multidimensional.

Consulte também [Criar uma predefinição de conjunto de lotes](application-setup.md#creating_a_batch_set_preset).

Não há um número mínimo ou máximo de linhas ou colunas que você deve ter em um conjunto de rotação de vários eixos.

Como exemplo, suponha que você queira criar um conjunto de rotação de vários eixos chamado *spin-2dspin*. Você tem um conjunto de imagens de conjunto de rotação que contém três linhas, com 12 imagens por linha. As imagens são nomeadas da seguinte maneira:

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

![](assets/se_batch_set_recipe.png)

O agrupamento para a parte do nome do ativo compartilhado do conjunto de rotação é adicionado ao campo Correspondência (como destacado). A parte variável do nome do ativo que contém a linha e a coluna é adicionada aos campos Linha e Coluna, respectivamente.

Quando o Conjunto de rotação é carregado e publicado, você ativaria o nome da fórmula do Conjunto de rotação 2D que está listada em **[!UICONTROL Batch Set Presets]** na caixa de diálogo Opções de trabalho de upload .

**Para criar uma predefinição de conjunto de lotes para a geração automática de um Conjunto de rotação 2D:**

1. Vá para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, conforme definido no canto superior direito da página Detalhes, é a exibição padrão.
1. No painel Lista de predefinições , selecione **[!UICONTROL Add]** para ativar os campos de definição no painel Detalhes no lado direito da página.
1. No painel Detalhes, no campo Nome da predefinição , digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione **[!UICONTROL Asset Set]**.
1. Na lista suspensa Subtipo , selecione **[!UICONTROL Multi-Axis Spin Set]**.
1. Expanda **[!UICONTROL Asset Naming Conventions]** e, na lista suspensa Nomeação de arquivo , selecione **[!UICONTROL Custom]**.
1. Use os atributos **[!UICONTROL Match]** e, opcionalmente, **[!UICONTROL Base Name]** para definir uma expressão regular para nomear ativos de imagem que compõem o agrupamento.

   Por exemplo, a expressão regular Correspondência literal pode ter a seguinte aparência:

   `(\w+)-\w+-\w+`

1. Expanda **[!UICONTROL Row Column Position]** e defina o formato do nome para a posição do ativo de imagem dentro da matriz de Conjunto de rotação 2D.

   Use os parênteses para abraçar a posição da linha ou da coluna no nome do arquivo.

   Por exemplo, para sua expressão regular de linha, ela pode ter a seguinte aparência:

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   Para a expressão regular da coluna, pode ser semelhante ao seguinte:

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   Lembre-se de que essas expressões são apenas exemplos. Você pode criar sua expressão regular da maneira que quiser, de acordo com suas necessidades.

   >[!NOTE]
   >
   >Se a combinação de expressões regulares de linha e coluna não puder determinar a posição do ativo na matriz do conjunto de rotação multidimensional, esse ativo não será adicionado ao conjunto e um erro será registrado.

1. Para Definir a Convenção de Nomenclatura e Criação, especifique o sufixo ou prefixo do nome básico definido na Convenção de Nomenclatura de Ativos. Defina também onde o conjunto de imagens é criado na estrutura de pastas do Adobe Dynamic Media Classic.

   Se você definir grandes números de conjuntos de imagens, mantenha esses conjuntos separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta de Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados por conjuntos em lotes aqui.

1. Selecione **[!UICONTROL Save]** no Painel de Detalhes.
1. Faça upload e publique seu Conjunto de rotação como de costume, certificando-se de ativar o nome do seu Conjunto de rotação 2D na caixa de diálogo Opções de carregamento da tarefa, em Predefinições de conjunto de lotes.

>[!MORELIKETHIS]
>
>* [Visualizar um ativo](previewing-asset.md#previewing_an_asset)
>* [Configurar predefinições da imagem](setting-image-presets.md#setting_up_image_presets)
>* [Exibir, adicionar e exportar metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Verificar arquivos de trabalho](checking-job-files.md#checking_job_files)

