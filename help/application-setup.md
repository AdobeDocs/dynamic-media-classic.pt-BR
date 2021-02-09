---
title: Configuração do aplicativo
description: Saiba como configurar a área Aplicativo do Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '10904'
ht-degree: 4%

---


# Configuração do aplicativo{#application-setup}

Você pode usar as páginas de Configuração do aplicativo para inserir configurações gerais, criar predefinições de imagens, predefinições de codificação de vídeo, predefinições do visualizador ou para definir visualizadores padrão e metadados. Você também pode configurar predefinições de definição de lote para automatizar a geração de conjuntos de rotação 2D (por exemplo), configurações de publicação e configurações de SEO de vídeo.

>[!NOTE]
>
>Somente administradores do Dynamic Media Classic podem alterar as configurações nas páginas de Configuração do aplicativo.

## Configurações Gerais {#general-settings}

Para abrir a página Configurações gerais do aplicativo, na barra Navegação global, clique em **[!UICONTROL Setup > Application Setup > General Settings]**.

### Servidores

Na criação da conta, o Dynamic Media Classic fornece automaticamente os servidores atribuídos para a sua empresa. Esses servidores são usados para construir strings de URL para seu site e aplicativos. Essas chamadas de URL são específicas para sua conta.

Consulte também [Testando o serviço de Teste Seguro](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **Nome**  do servidor publicado - Este servidor é o servidor CDN ativo usado em todas as chamadas de URL geradas pelo sistema específicas para sua conta. Não altere esse nome de servidor a menos que seja instruído a fazê-lo por um técnico de suporte do Dynamic Media Classic.

* **Nome**  do servidor de origem - Este servidor é usado apenas para testes de garantia de qualidade. Não altere esse nome de servidor a menos que um técnico de suporte do Dynamic Media Classic o instrua a fazê-lo.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **Nome**  do servidor do Test&amp;Público alvo - URL do seu Test&amp;Público alvo, até .com, inclusive. Para obter instruções sobre como obter esse URL, consulte Integração [!DNL Dynamic Media Classic] com [!DNL Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **Nome**  do servidor de streaming do iOS - o URL do servidor de streaming do  [!DNL Dynamic Media Classic] iOS. Este servidor fornece vídeo de fluxo contínuo para dispositivos baseados no iOS usando o protocolo HTTP.

* **Nome**  do servidor de vídeo progressivo - o URL do servidor de vídeo  [!DNL Dynamic Media Classic] progressivo. Este servidor fornece vídeo progressivo usando o protocolo HTTP.

* **Mostrar URL para ativos**  não publicados - Selecione esta opção se desejar  [!DNL Dynamic Media Classic] exibir um URL ao visualizar qualquer ativo, seja publicado ou não. Se o ativo não for publicado, o URL não funcionará. No entanto, você pode usar o URL para fins de planejamento ou organização.

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **Modelo**  de Invalidação CDN - Especifica o modelo usado para invalidar o cache CDN (Rede de Delivery de Conteúdo).

   Por exemplo, suponha que você insira um URL de imagem (incluindo predefinições ou modificadores de imagem) referenciando `<ID>`, em vez de uma ID de imagem específica, como no exemplo a seguir:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Se o Modelo contiver apenas `<ID>`, o Dynamic Media Classic será preenchido em `https://<server>/is/image`, onde `<server>` é o Nome do servidor de publicação definido em Configurações gerais.

   Definir o Modelo de Invalidação CDN, selecionar uma imagem chamada Backpack_B e clicar em **Arquivo** > **Invalidar CDN** resulta no seguinte URL gerado na interface de Invalidação CDN:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Na caixa lista do URL, clique em **Continuar** para limpar o cache da chamada de URL de imagem específica. Observe que também é possível adicionar URLs digitando ou colando-os na caixa lista do URL; não é necessário definir o Modelo antecipadamente.

   Depois de selecionar seu Modelo de Invalidação CDN e fazer uma solicitação Invalidar CDN, aparecerá um indicador na interface do usuário que fornece uma estimativa do tempo necessário para limpar o cache.

   Da mesma forma, se várias imagens forem selecionadas no Dynamic Media Classic ao clicar em **Arquivo** > **Invalidar CDN**, cada imagem será referenciada no URL do modelo salvo. Portanto, você pode definir um Modelo de Invalidação CDN referenciando cada URL referenciado em seu site (como detalhes do produto, resultados de pesquisa e assim por diante). Em seguida, ao selecionar uma ou mais imagens para invalidação do cache, os URLs preenchem automaticamente a interface.

   Consulte [Armazenamento de conteúdo em cache](dmc-platform-overview.md#content_caching).

   Consulte [Ativos republicados e atrasos CDN](publishing-files.md#republished_assets_and_cdn_delays).

### Procurar

* **Mostrar projetos**  - determina se os projetos estão disponíveis como forma de organizar seus ativos do Dynamic Media Classic. Consulte Organização do trabalho com projetos.

* **Mostrar amostra de conteúdo**  de eVideo - Ativa ou desativa a exibição de conteúdo de amostra de eVideo.

* **Mostrar conteúdo**  gerado - nas pastas, mostra o conteúdo gerado de um ativo. Por exemplo, quando um arquivo PDF é rasterizado à medida que é carregado, o Dynamic Media Classic cria uma imagem para cada página no PDF original. Se a opção Mostrar conteúdo gerado estiver selecionada, cada imagem gerada quando o PDF original foi carregado aparecerá junto com o PDF na pasta para a qual o PDF foi carregado.

* **Mostrar vídeos**  codificados - Desmarcado (desmarcado) por padrão.

   Para pesquisar e procurar vídeos rapidamente no Dynamic Media Classic sem precisar navegar por vários derivados codificados do mesmo vídeo, deixe essa opção desmarcada (padrão). Somente a miniatura do Vídeo principal, que é o vídeo de origem carregado e usado para criar todos os derivados, e somente a miniatura do Conjunto de vídeos adaptáveis &quot;pai&quot;, que contém todos os derivados &quot;filho&quot; do conjunto de vídeos codificados, são exibidos na interface do usuário.

   No entanto, você ainda pode acessar vídeos codificados individuais a partir do vídeo Principal ou do Conjunto de vídeos adaptáveis. Para fazer isso, clique com o duplo na imagem em miniatura do vídeo para abrir a Visualização Detalhe. Em seguida, clique em **Vídeos codificados** no painel direito para acessar todos os vídeos &quot;filhos&quot;.

   Você também pode usar **Arquivo > Reprocessar** para criar vídeos &quot;filhos&quot; mais codificados diretamente de um Conjunto de vídeos adaptáveis. O Dynamic Media Classic encontra automaticamente o vídeo Principal &quot;pai&quot; do Conjunto de vídeos adaptáveis e o usa como vídeo de origem para transcodificação. No entanto, quando você salva os novos vídeos codificados individuais, eles não são vistos quando você pesquisa ou navega. No entanto, eles ainda estão acessíveis na guia Vídeos codificados na Visualização Detalhe.

   Consulte [Carregar e transcodificar vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Para continuar a capacidade de acessar todos os seus derivados de vídeo codificados ao pesquisar e navegar, selecione **Mostrar vídeos codificados**.

   Há determinadas ações no menu Criar que funcionam somente com vídeos individuais ou que funcionam como opção. Essa funcionalidade torna necessário mostrar todos os derivados de vídeo codificados dos quais você pode selecionar, independentemente de como você define **Mostrar vídeos codificados**. As ações de criação que substituem a configuração **Mostrar vídeos codificados** incluem **Conjuntos de vídeos adaptáveis** e **eCatalogs**.

   >[!NOTE]
   >
   >Se você não tiver usado o Dynamic Media Classic para fazer upload e codificar seus ativos de vídeo, o Dynamic Media Classic exibirá todos os vídeos codificados individuais, mesmo se essa opção estiver desmarcada.

* **Mostrar botão**  Atualizar subpastas - Ativa ou desativa a exibição do botão Atualizar subpastas.

### Conta FTP do Dynamic Media Classic

* **Servidor**  - Lista seu servidor de contas FTP.

* **Nome**  do usuário - Lista o nome de usuário da sua conta FTP.

### Carregar no aplicativo

* **Substituir imagens**  - o Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A ID do Dynamic Media Classic de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Devido a essa regra, a caixa de diálogo Carregar tem uma opção Substituir. O efeito exato dessa opção depende da opção Sobrescrever imagens especificada. Essas opções especificam como as imagens de substituição são carregadas: se elas substituem as imagens originais ou se tornam imagens de duplicado. As imagens de duplicado são renomeadas com um &quot;-1&quot; (por exemplo, o nome de President.tif é renomeado como sit-1.tif). Essas opções afetam as imagens carregadas em uma pasta diferente da original ou as imagens com uma extensão de nome de arquivo diferente da original (como JPG, TIF ou PNG). (Consulte Uso da opção Substituir imagens.)

   * **Substituir na pasta atual, mesmo nome/extensão**  da imagem base - Essa opção é a regra mais estrita para substituição. Ele requer que você carregue a imagem de substituição na mesma pasta que a original e que a imagem de substituição tenha a mesma extensão de nome de arquivo que a original. Se esses requisitos não forem atendidos, um duplicado será criado.

   * **Substituir na pasta atual, o mesmo nome do ativo básico independentemente da extensão**  - Requer que você carregue a imagem de substituição na mesma pasta do original, no entanto, a extensão do nome do arquivo pode ser diferente do original. Por exemplo, o arquivo visit.tif substitui o arquivo

   * **Substituir em qualquer pasta, o mesmo nome/extensão**  do ativo básico - Requer que a imagem de substituição tenha a mesma extensão de nome de arquivo que a imagem original (por exemplo, o arquivo visit.jpg deve substituir o arquivo .jpg, não o domínio .tif). No entanto, é possível carregar a imagem de substituição para uma pasta diferente da original. A imagem atualizada reside na nova pasta; o arquivo não pode mais ser encontrado em seu local original

   * **Substituir em qualquer pasta, o mesmo nome do ativo básico independentemente da extensão**  - Essa opção é a regra de substituição mais inclusiva. Você pode carregar uma imagem de substituição para uma pasta diferente da original, carregar um arquivo com uma extensão de nome de arquivo diferente e substituir o arquivo original. Se o arquivo original estiver em uma pasta diferente, a imagem de substituição residirá na nova pasta para a qual foi carregada.

* **Manter publicação**  - especifica se uma imagem de substituição carregada no Dynamic Media Classic retém a configuração Pronto para publicar da imagem que está substituindo ou se a configuração é especificada no upload.

* **Perfis**  de cor padrão - especifica os perfis de cor aplicados como parte das Opções de Perfil de cor padrão ao adicionar imagens CMYK.

* **Opções**  padrão de upload - abre a caixa de diálogo Opções de upload de trabalho, onde você pode especificar as opções padrão de upload. Para obter informações sobre essas opções, consulte Opções de upload.

### Editor de mapa de imagem, para Aplicativo

* **HREF**  de mapeamento de imagem padrão - Define o URL padrão usado para a coluna href de mapeamento de imagem. Esse URL é o URL padrão que você vê ao criar novos Mapas de imagem.

* **Modelo**  de mapeamento de imagem padrão - Define o Javascript padrão para o modelo href de mapeamento de imagem. Você pode definir o código personalizado aqui para ser executado sempre que clicar em um mapa de imagem.

### Outras configurações, para o aplicativo

* **Avisos**  de lixeira podem ser limpos - os ativos no lixo são removidos automaticamente dentro de sete dias. Selecione &quot;Enviar emails antes que itens de lixo sejam excluídos automaticamente&quot; se desejar que notificações sejam enviadas para administradores de empresas quando os ativos que estão no Lixeira estiverem a quatro dias de serem excluídos permanentemente. Consulte Gerenciamento da pasta Lixeira.

## Uso da opção de Substituição de imagens {#using-the-overwrite-images-option}

O Dynamic Media Classic não permite que dois arquivos tenham o mesmo nome. A ID do Dynamic Media Classic de cada item (o nome da imagem menos a extensão do nome do arquivo) deve ser exclusiva. Por causa dessa regra, a caixa de diálogo Carregar inclui as opções Substituir imagens. O efeito exato dessa opção depende de uma configuração para cada configuração interna do empresa Dynamic Media Classic.

Se você carregou imagens anteriormente e alterou os arquivos originais (ou os substituiu), a opção Substituir escolhida especifica como o Dynamic Media Classic substitui as imagens. Nenhuma informação sobre a imagem muda, mas a nova imagem substitui a antiga. Se a pasta também contiver imagens que ainda não estão no Dynamic Media Classic, essas imagens serão adicionadas.

Use essa opção se as imagens carregadas tiverem sido alteradas de alguma forma (a imagem foi alterada), mas a referência à imagem continuar a mesma. A substituição também é útil ao carregar e extrair PDFs Adobe®. Para ajustar como o Dynamic Media Classic *rips* a imagem, ajuste as opções de perfil de cor ICC na caixa de diálogo Carregar e faça upload novamente usando o recurso Substituir.

As Dynamic Media Classic IDs usadas para acessar imagens dos servidores de produção são derivadas dos nomes de arquivo de imagem. O uso de caracteres em maiúsculas e minúsculas no nome do arquivo é importante, tanto na substituição de arquivos existentes quanto para as IDs do Dynamic Media Classic usadas para acessar a imagem. Certifique-se de que o uso de caracteres em maiúsculas e minúsculas em nomes de arquivo esteja correto antes de fazer upload no Dynamic Media Classic para evitar IDs do Dynamic Media Classic que sejam diferentes apenas em maiúsculas para a mesma imagem.

Se você desmarcar essa opção, todas as imagens com os mesmos nomes de arquivo das imagens existentes serão tratadas como duplicados e não serão adicionadas.

## Predefinições de imagem {#image-presets}

A tela Predefinições de imagem é destinada à criação e edição de Predefinições de imagem. As predefinições de imagens permitem que o Dynamic Media Classic forneça imagens dinamicamente de tamanhos diferentes da mesma imagem principal. Cada predefinição de imagem representa uma coleção predefinida de comandos de dimensionamento e formatação para a exibição de imagens. Ao criar uma predefinição de imagem, escolha um tamanho para o delivery de imagem. Você também escolhe comandos de formatação para que a aparência da imagem seja otimizada quando a imagem for entregue para exibição.

Os administradores podem criar predefinições para exportar ativos. Os usuários podem escolher uma predefinição ao exportar imagens, o que também reformata as imagens de acordo com as especificações especificadas pelo administrador.

Para abrir a tela Predefinição de imagem, na barra Navegação global, clique em **Configuração** > **Predefinições de imagem**.

Consulte [Imagens inteligentes](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Criação e edição de predefinições de imagens {#creating-and-editing-image-presets}

1. Clique em **Configuração** > **Predefinições de imagem**.
1. Crie uma nova predefinição ou start a partir de uma existente:
   * **Criação de uma predefinição**  de imagem - Clique em  **Adicionar**.
   * **Criação de uma predefinição de imagem a partir de uma predefinição**  existente - Selecione a predefinição de imagem mais parecida com a que deseja criar e clique em Editar.

1. Na tela Adicionar (ou Editar) predefinição, digite um nome para a predefinição.
1. Defina as opções de Predefinição desejadas.

   Consulte [Opções de predefinição de imagem](application-setup.md#image_preset_options).

1. Clique em **Salvar** ou, se você começou a partir de uma predefinição existente, clique em **Salvar como**.
1. Para pré-visualização da predefinição com sua própria imagem, clique em **Procurar** e selecione uma imagem. Para pré-visualização com a imagem padrão, clique em **Redefinir**.

É possível editar uma predefinição de imagem selecionando seu nome na tela Predefinições de imagem e clicando em Editar. Para excluir uma predefinição de imagem, selecione-a e clique em Excluir.

### Opções de predefinição de imagem {#image-preset-options}

As telas Adicionar predefinição e Editar predefinição ofertas estas opções para criar e editar predefinições de imagens:

**Nome** predefinidoDigite um nome descritivo sem espaços em branco. Inclua a especificação do tamanho da imagem no nome para ajudar os usuários a identificar essa predefinição de imagem.

**Largura e** alturaInsira em pixels o tamanho no qual a imagem é entregue.

**** FormatoEscolha um formato no menu. A escolha do formato GIF, JPEG, PDF ou TIFF traz opções adicionais:

* Opções de quantificação de cores GIF

   **Tipo**

   Escolha Adaptável (padrão), Web ou Macintosh. Se você escolher GIF com alfa, a opção Macintosh® não estará disponível.

   **Ponta**

   Escolha Difuso ou Desativado.

   **Número de Cores**

   Arraste o controle deslizante para entrar em 2-255.

   **Lista de cores**

   Insira uma lista separada por vírgulas. Por exemplo, para branco, cinza e preto, digite 000000,888888,ffff.

* Opções JPEG

   **Qualidade**

   Controla o nível de compactação JPEG. Essa configuração afeta o tamanho do arquivo e a qualidade da imagem. A escala de qualidade JPEG é 1-100.

   **Ativar redução da resolução do Java Chrominance**

   Como o olho é menos sensível à informação de cores de alta frequência do que à luminância de alta frequência, as imagens JPEG dividem a informação da imagem em luminância e componentes de cor. Quando uma imagem JPEG é compactada, o componente de luminância é deixado em resolução completa, enquanto os componentes de cor têm resolução reduzida, fazendo a média em grupos de pixels. A diminuição da resolução reduz o volume de dados em metade ou um terço, com quase nenhum impacto na qualidade percebida. A redução da resolução não se aplica a imagens em tons de cinza. Essa técnica reduz a quantidade de compactação útil para imagens com alto contraste (por exemplo, imagens com texto sobreposto).

* Opções de PDF e TIFF

   **Compactação**

   Escolha um algoritmo de compactação.

**Espaço de** coresEscolha um espaço de cores.

**** NitidezSelecione a opção Ativar Nitidez Simples para aplicar um filtro básico de nitidez à imagem depois que toda a escala ocorrer. A nitidez pode ajudar a compensar o desfoque que pode resultar na exibição de uma imagem em um tamanho diferente.

Para obter mais informações sobre nitidez, modos de reamostragem e máscara de nitidez, consulte [Nitidez de uma imagem](sharpening-image.md#sharpening_an_image).

**Modo** de nova amostraEscolha uma opção de modo de nova amostra. Essas opções tornam a imagem nítida quando tem resolução reduzida:

**B-** LinearO método de reamostragem mais rápido; alguns artefatos de aliasing são perceptíveis.

**Bi-** CubicAumenta o uso da CPU no Servidor de imagens, mas produz imagens mais nítidas com artefatos de aliasing menos visíveis.

**Sharp2** Pode produzir resultados ligeiramente mais nítidos do que a opção Bi-Cubic, mas a um custo de CPU ainda maior no Image Server.

**Três** linearesUsa resoluções mais altas e mais baixas, se disponíveis; recomendado somente quando a suavização de borda for um problema. Este método reduz o tamanho do JPEG devido à redução dos dados de alta frequência.

**Mascaramento** de nitidezEscolha estas opções para ajustar a nitidez:

**** QuantiaControla a quantidade de contraste aplicada aos pixels da borda. O padrão é 1.0. Para imagens de alta resolução, é possível aumentá-las para até 5.0. Pense em Amount como uma medida da intensidade do filtro.

**** RaioDetermina o número de pixels em torno dos pixels da borda que afetam a nitidez. Para imagens de alta resolução, digite de 1 a 2. Um valor baixo torna nítido apenas os pixels da borda; um valor alto aumenta a nitidez de uma faixa maior de pixels. O valor correto depende do tamanho da imagem.

**** LimiteDetermina o intervalo de contraste a ser ignorado quando o filtro de máscara de nitidez é aplicado. Em outras palavras, essa opção determina o quão diferentes os pixels com nitidez devem ser da área ao redor antes que sejam considerados pixels de borda e sejam apontados. Para evitar a introdução de ruído, experimente valores entre 0,02 e 0,2. O valor padrão de 6 aumenta a nitidez de todos os pixels na imagem.

**Espaço** de corDetermina se a imagem usa o espaço no qual a imagem foi criada, geralmente RGB (Original) ou um espaço de luminância (Intensidade).

**** CorEscolha estas opções:

**Perfil de cor de saídaSelecione Usar padrão ou um dos perfis de cor ICC disponíveis no Dynamic Media Classic.** 

Consulte também [perfis ICC](icc-profiles.md#icc_profiles).

**Propósito de renderizaçãoSelecione uma opção se desejar substituir o propósito de renderização padrão do perfil de cores.** Use essa opção quando um dos perfis ICC padrão for o espaço de cor do público alvo de uma conversão de cor, um dispositivo de saída (impressora ou monitor) for caracterizado por esse perfil e o propósito de renderização especificado for válido para esse perfil.

**Incorporar** perfilSelecione esta opção para que, se você abrir esta imagem no Adobe® Photoshop®, ela use este perfil.

**Resolução** de impressãoEscolha uma resolução para imprimir esta imagem; 72 pixels é o padrão.

**Modificadores** de URLsSe você preferir especificar os modificadores de URL que definem sua Predefinição de imagem, em vez das configurações, insira os modificadores aqui.

**URL de imagem de amostra** lista a string de URL &quot;bruta&quot; que o Dynamic Media Image Server usa para fornecer imagens com a Predefinição de imagem que você está adicionando ou editando. Essa string de URL codifica todas as configurações de formato selecionadas na tela Adicionar predefinição ou Editar predefinição.

### Editar, remover ou desativar uma predefinição de imagem {#editing-removing-or-deactivating-an-image-preset}

1. Clique em **Configuração** > **Predefinições de imagem**.
1. Na tela Predefinições de imagem, selecione uma predefinição na tabela e execute um dos procedimentos a seguir:

   * Clique em **Editar** e especifique novas opções na caixa de diálogo Editar predefinição.
   * Clique em **Excluir** para remover a predefinição da lista.
   * Desmarque a caixa de seleção Ativo ao lado de um nome predefinido para removê-lo de toda a interface do usuário do Dynamic Media Classic para usuários do MediaPortal.

## Ativar ou desativar predefinições de vídeo adaptáveis {#activating-or-deactivating-adaptive-video-presets}

Predefinições de codificação de vídeo adaptável do Dynamic Media Classic oferta. É uma lista principal de predefinições que combina predefinições de vídeo adaptável 16:9 e predefinições de vídeo adaptativo 4:3 em um único grupo. Essas predefinições predefinidas refletem as configurações de codificação mais comuns e são otimizadas para reprodução em dispositivos móveis, tablets e desktops públicos alvos.

Somente as predefinições de codificação &quot;Vídeo adaptativo&quot; são ativadas (ativadas ou &quot;ativadas&quot;) por padrão. Você pode desativá-la, se desejar. As predefinições de Vídeo adaptativo inativo não aparecem como uma opção selecionável na seção eVideo da caixa de diálogo Opções de carregamento de trabalho.

Consulte [Carregar e codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Para ativar ou desativar predefinições de vídeo adaptáveis**

1. Perto do canto superior direito do Dynamic Media Classic, clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Vídeo** > **Predefinições de Vídeo Adaptáveis**.
1. Na página Predefinições de vídeo adaptáveis, desmarque a caixa de seleção ao lado de um nome predefinido para remover a predefinição da lista Opções de eVideo na caixa de diálogo Carregar opções de trabalho.
1. Clique em **Fechar**.

## Predefinições de vídeo para codificação de arquivos de vídeo {#video-presets-for-encoding-video-files}

Para escolher uma predefinição de codificação, no canto inferior direito da página Carregar, clique em Opções de trabalho. Na caixa de diálogo Carregar opções de trabalho, expanda Opções de eVideo e escolha as predefinições de codificação de vídeo desejadas.

>[!NOTE]
>
>Com exceção do &quot;Vídeo adaptativo&quot;, que está ativado por padrão, talvez você não veja todas as outras predefinições de codificação de vídeo adaptável ou de vídeo único na caixa de diálogo Opções de trabalho de upload. Os administradores do Dynamic Media Classic determinam quais predefinições de codificação de vídeo estão visíveis na caixa de diálogo Carregar opções de trabalho.

* Escolha entre as seguintes predefinições de codificação de vídeo adaptável ou de codificação única:

   **Vídeo adaptativo 16:9**

   Crie vídeos com proporção de 16:9 para delivery para desktops, dispositivos móveis (iPhone, iPad, Android) e tablets (iPad, Android), otimizados com resolução e taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   **Vídeo adaptável 4:3**

   Crie vídeos com proporção de 4:3 para desktops, dispositivos móveis (iPhone, iPad, Android) e tablets (iPad, Android), otimizados com resolução e taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   **Vídeo adaptável**

   Uma única predefinição de codificação que funciona com qualquer proporção para criar vídeos para delivery, tablet e desktop. Os vídeos de origem carregados que são codificados com essa predefinição são definidos com uma altura fixa. Entretanto, a largura é dimensionada automaticamente para preservar a proporção do vídeo.

   Essa flexibilidade de ter uma &quot;Escala automática&quot; também está disponível por padrão quando você cria sua própria predefinição de codificação de vídeo personalizada.

   Consulte [Adicionar ou editar uma predefinição de codificação de vídeo](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   **Codificação de vídeo adaptável (16:9 ou 4:3)**

   Crie vídeos com proporção de tela de 16:9 e 4:3 para desktops, dispositivos móveis (iPhone, iPad, Android) e tablets (iPad, Android), otimizados com resolução e taxa de bits que melhor correspondem à velocidade de conexão do visualizador.

   Consulte [Codificação de vídeo adaptável (16:9 ou 4:3) predefinições de vídeo](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   **Predefinições de codificação única**

   >[!NOTE]
   >
   >Para fornecer vídeo para iPads, você pode escolher uma predefinição de codificação móvel ou uma predefinição de codificação de tablet. As predefinições de tablet são projetadas especialmente para o iPad, geralmente com maior resolução e qualidade para aproveitar o tamanho de tela e a conexão de largura de banda maiores. Fornecer arquivos de vídeo codificados com uma predefinição de Tablet requer que você inclua o código de detecção de dispositivo no seu site ou aplicativo móvel. Esse código alterna entre uma experiência de vídeo em iPhone ou iPad, dependendo do dispositivo de reprodução. Escolher uma predefinição de Dispositivo móvel para fornecer arquivos de vídeo ao iPad é um fluxo de trabalho mais simplificado. O motivo é que você pode usar o mesmo arquivo de vídeo para iPhones e iPads. Entretanto, a qualidade é padronizada para a experiência de iPhone com resolução mais baixa.

   * No grupo Predefinições de codificação, na lista suspensa Classificar predefinições de codificação, selecione Nome ou Tamanho para classificar predefinições por nome ou tamanho de resolução.
   * Escolha uma predefinição de codificação com base no tamanho e largura de banda da resolução com os quais você planeja reproduzir o vídeo.
   * É possível selecionar a Codificação de vídeo adaptável e uma ou mais predefinições de codificação por vídeo. Por exemplo, você pode codificar um arquivo para desktop e dispositivo móvel em um único trabalho de upload.

Depois de clicar em **Upload de Start**, o arquivo de vídeo principal original é carregado e os arquivos codificados são gerados a partir do arquivo principal.

### Sobre a codificação de opções predefinidas {#about-encoding-preset-options}

Os parâmetros das opções predefinidas de codificação são os seguintes:

**Velocidade da conexão do público alvoA velocidade da conexão com a Internet do usuário final alvo.** 

**Sufixo** de arquivo codificadoO sufixo anexado ao arquivo de vídeo codificado para fins de identificação.

**Taxa de bits do vídeo (taxa de dados)** A quantidade de dados que é codificada para compor um único segundo de reprodução do vídeo (em kilobits por segundo).

**Largura/** altura do pixelA dimensão da largura da imagem do ecrã, em pixels; a dimensão de altura da imagem da tela (em pixels).

**Quadro por segundo (fps)** O número de quadros, ou imagens estáticas, para cada segundo do vídeo. Nos Estados Unidos e no Japão, a maioria dos vídeos são gravados a 29,97 fps; na Europa e na Ásia (excluindo o Japão), a maioria dos vídeos são gravados a 25 qps. O filme é filmado a 24 fps.

**** Taxa de bits de áudioA quantidade de dados que é codificada para formar um único segundo de reprodução de áudio, em kilobits por segundo.

As tabelas a seguir mostram as práticas recomendadas para selecionar predefinições de vídeo e as convenções de nomenclatura usadas para designar arquivos codificados.

### Vídeo adaptável (padrão) {#adaptive-video-default}

Uma predefinição de codificação que funciona com qualquer proporção para permitir que você crie vídeos para delivery para dispositivos móveis, tablets e desktops. Os vídeos de origem carregados que são codificados usando essa predefinição (padrão e prática recomendada) são definidos para uma altura fixa, enquanto a largura é dimensionada automaticamente para preservar a proporção do vídeo.

**Vídeo adaptativo (padrão)**

|  | Codificação do texto do nome da predefinição/dica de ferramenta | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/Altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | Auto x 360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | Igual à fonte | 64 | Para dispositivos móveis (iPhone, iPad, Android) |
| 2 | Auto x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | Igual à fonte | 96 | Para tablet (iPad, Android) |
| 1 | Auto x 720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | Igual à fonte | 128 | Para desktop |

### Predefinições de vídeo da Codificação de vídeo adaptativa (16:9 ou 4:3) {#adaptive-video-encoding-or-video-presets}

Essas predefinições de codificação de vídeo adaptáveis combinam uma série de predefinições de codificação individuais que são automaticamente selecionadas para você com base na proporção do vídeo que você carregou. Por exemplo, se você carregar um vídeo 4:3, ele será automaticamente codificado usando todas as cinco predefinições 4:3 encontradas na lista predefinida principal na opção **Adaptive Video Encoding (16:9 ou 4:3)**.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Predefinições de codificação de vídeo adaptável (16:9 ou 4:3)**

|  | Codificação do texto do nome da predefinição/dica de ferramenta | Velocidade de conexão do público alvo (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/Altura (pixels) | Fps | Taxa de bits de áudio (kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 512 x 288, Móvel (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual à fonte | 64 | Baixa resolução, 3G |
| 2 | 4:3, 384x288px, móvel (iPhone, iPad, Android), (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual à fonte | 64 | Baixa resolução, 3G |
| 3 | 16:9, 512 x 288, Móvel (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512 x 288 | Igual à fonte | 64 | Resolução média, 3G |
| 4 | 4:3, 384 x 288, Móvel (iPhone, iPad, Android), (600 Kbps) | 700 | _Mobile_384x288_600 | 800 | 384 x 288 | Igual à fonte | 64 | Resolução média, 3G |
| 5 | 16:9, 640 x 360, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Igual à fonte | 80 | Resolução média, WiFi |
| 6 | 4:3, 640x480, Tablet (iPad, Android), (800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Igual à fonte | 80 | Resolução média, WiFi |
| 7 | 16:9, 768 x 432, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | Igual à fonte | 96 | Alta resolução, WiFi |
| 8 | 4:3, 768 x 576, Tablet (iPad, Android), (1200 Kbps) | 1,5 Mbps | _iPad_768x576_1200K | 1200 | 768 x 576 | Igual à fonte | 96 | Alta resolução, WiFi |
| 9 | 16:9, 1280x720, Desktop, (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual à fonte | 128 | Alta definição, widescreen |
| 10 | 4:3, 1280x960, Desktop, (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 Kbps | 1280 x 960 | Igual à fonte | 128 | Alta definição |

### Predefinições de codificação de vídeo para desktop {#desktop-video-encoding-presets}

Predefinições de codificação de vídeo para MP4 e OGV em computadores desktop.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - AAC de áudio, extensão de arquivo MP4**

|  | Codificação do texto do nome da predefinição/dica de ferramenta | Velocidade de conexão do público alvo (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/Altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480 x 270 | Igual à fonte | 64 | Baixa resolução widescreen |
| 2 | 16:9, 640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640 x 360 | Igual à fonte | 80 | Resolução widescreen média |
| 1 | 16:9, 800x450 (1200 Kbps) | 1,5 Mbps | _800x450_1200K | 1200 | 800 x 450 | Igual à fonte | 96 | Resolução média-alta |
| 4 | 16:9, 1280x720 (2000 Kbps) | 3,0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | Igual à fonte | 128 | Alta definição, widescreen |
| 5 | 4:3, 320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320 x 240 | Igual à fonte | 64 | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480 x 360 | Igual à fonte | 80 | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps) | 1,5 Mbps | _640x480_1200K | 1200 | 640 x 480 | Igual à fonte | 96 | Resolução média-alta |
| 8 | 4:3, 1280x960 (2000 Kbps) | 3,0 Mbps | _1280x960_2000K | 2000 | 1280 x 960 | Igual à fonte | 128 | Alta definição |

**OGG Theora Vorbis - Extensão do arquivo OGV**

|  | Codificação do texto do nome da predefinição/dica de ferramenta | Velocidade de conexão do público alvo (Kbps) | Sufixo de arquivo codificado | Taxa de dados de vídeo (Kbps) | Largura/Altura (pixels) | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 480x270 (400 Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Igual à fonte | 64 | Baixa resolução widescreen |
| 2 | 16:9, 640x360 (800 Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Igual à fonte | 80 | Resolução widescreen média |
| 3 | 16:9, 800x450 (1200 Kbps), OGG | 1,5 Mbps | _OGG_800x450_1200K | 1200 | 800 x 450 | Igual à fonte | 96 | Resolução média-alta |
| 4 | 16:9, 1280x720 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x720_2000K | 2000 | 1280 x 720 | Igual à fonte | 128 | Alta definição, widescreen |
| 5 | 4:3, 320x240 (400 Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Igual à fonte | 64 | Baixa resolução |
| 6 | 4:3, 480x360 (800 Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Igual à fonte | 80 | Resolução média |
| 7 | 4:3, 640x480 (1200 Kbps), OGG | 1,5 Mbps | _OGG_640x480_1200K | 1200 | 640 x 480 | Igual à fonte | 96 | Resolução média-alta |
| 8 | 4:3, 1280x960 (2000 Kbps), OGG | 3,0 Mbps | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Igual à fonte | 128 | Alta definição |

### Predefinições de codificação de vídeo móvel {#mobile-video-encoding-presets}

Igual ao fps de origem. Predefinições de codificação de vídeo para dispositivos móveis iPhone, iPad e Android.

Para obter informações sobre parâmetros de opções de codificação, consulte [Sobre as opções predefinidas de codificação](application-setup.md#about_encoding_preset_options).

**Linha de base H264 2.1 - AAC de áudio, extensão de arquivo MP4**

|  | Codificação do texto do nome da predefinição/dica de ferramenta | Velocidade de conexão do público alvo (Kbps) | Sufixo de arquivo codificado | Taxa de bits do vídeo (Kbps) | Largura/altura do pixel | Fps | Taxa de bits de áudio (Kbps) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9, 512 x 288, Móvel (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Igual à fonte | 64 | Baixa resolução, 3G |
| 2 | 16:9, 512 x 288, Móvel (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512 x 288 | Igual à fonte | 64 | Resolução média, 3G |
| 3 | 16:9, 512 x 288, Móvel (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Igual à fonte | 80 | Resolução média, Wi-Fi |
| 4 | 16:9, 512 x 288, Móvel (1000 Kbps) | 1,2 Mbps | _Mobile_512x288_1000K | 1000 | 512 x 288 | Igual à fonte | 80 | Alta resolução, Wi-Fi |
| 5 | 16:9, 512 x 288, Móvel (1200 Kbps) | 1,5 Mbps | _Mobile_512x288_1200K | 1200 | 512 x 288 | Igual à fonte | 96 | Alta resolução, Wi-Fi |
| 6 | 4:3, 384 x 288, Móvel (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Igual à fonte | 64 | Baixa resolução, 3G |
| 7 | 4:3, 384 x 288, Móvel (600 Kbps) | 700 | _Mobile_384x288_600K | 800 | 384 x 288 | Igual à fonte | 64 | Resolução média, 3G |
| 8 | 4:3, 448x336, Móvel (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Igual à fonte | 80 | Resolução média, Wi-Fi |
| 9 | 4:3, 448x336, Móvel (1000 Kbps) | 1,2 Mbps | _Mobile_448x336_1000K | 1000 | 448 x 336 | Igual à fonte | 80 | Alta resolução, Wi-Fi |
| 10 | 4:3, 448x336, Móvel (1200 Kbps) | 1,5 Mbps | _Mobile_448x336_1200K | 1200 | 448 x 336 | Igual à fonte | 96 | Alta resolução, Wi-Fi |

## Predefinições do visualizador {#viewer-presets}

>[!NOTE]
>
>**Aviso**  de Fim da Vida Útil dos Visualizadores de Flashes - A partir de 31 de janeiro de 2017, o suporte do Adobe Dynamic Media Classic oficialmente terminou para a plataforma do visualizador de Flashes.

Uma *Predefinição do visualizador* é uma coleção de configurações que determinam como os usuários visualizações ativos de mídia avançada em suas telas de computadores e dispositivos móveis. Como administrador, você pode criar Predefinições do visualizador. As configurações estão disponíveis para uma matriz de opções de configuração do visualizador. Por exemplo, é possível alterar o tamanho de exibição do visualizador, o comportamento de zoom, os esquemas de cores, as bordas e as fontes.

Como prática recomendada, use visualizadores de vídeo HTML5 do Dynamic Media Classic. As predefinições usadas em visualizadores de vídeo HTML5 são players de vídeo robustos. Ao combinar em um único player a capacidade de projetar os componentes de reprodução usando HTML5 e CSS, ter reprodução integrada e usar streaming adaptável e progressivo dependendo da capacidade do navegador, você estende o alcance do conteúdo de mídia avançada para usuários de desktop, tablet e dispositivos móveis, além de garantir uma experiência de vídeo otimizada.

Consulte [Sobre Visualizadores HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) no Guia de Referência de Visualizadores de Adobe.

Consulte [Matriz de compatibilidade predefinida do Dynamic Media Classic Viewer](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Consulte [Prática recomendada: Usar o visualizador de vídeo HTML5](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Dependendo do visualizador, você pode adicionar recursos da comunidade. Os recursos da comunidade incluem um botão Incorporar, um botão de email, um botão Link e um botão Visitar site. Esses botões permitem que as pessoas que usam os visualizadores compartilhem o visualizador com outras pessoas ou abram o site do Dynamic Media Classic.

Consulte também [Exemplos de biblioteca de referência de visualizadores de Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Suporte do visualizador para páginas da Web responsivas {#viewer-support-for-responsive-designed-web-pages}

Páginas da Web diferentes têm necessidades diferentes. Às vezes, você desejará uma página da Web que forneça um link que abra o Visualizador HTML5 em uma janela separada do navegador. Em outros casos, pode ser necessário incorporar o Visualizador HTML5 diretamente na página de hospedagem. No último caso, a página da Web pode ter um layout estático. Ou pode ser &quot;responsivo&quot; e exibido de forma diferente em dispositivos diferentes ou para tamanhos diferentes de janelas do navegador. Para acomodar essas necessidades, os Visualizadores HTML5 fornecidos com o Dynamic Media Classic suportam páginas da Web estáticas e páginas da Web responsivas projetadas.

Consulte [Biblioteca de imagens estáticas responsivas](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)na *Ajuda da API de disponibilização de imagens do Adobe* para obter mais informações sobre como incorporar visualizadores responsivos às suas páginas da Web.

### Tipos de predefinição do visualizador {#viewer-preset-types}

Os administradores podem criar e personalizar os seguintes tipos de predefinições do visualizador:

**eCatalog** ViewerSimula a experiência de leitura de um catálogo impresso. Você pode mover de página em página, aumentar e diminuir o zoom dos itens em uma página, usar mapas de imagem para ver mais informações sobre os itens na página ou pesquisar no catálogo. Você também pode incluir um Painel de informações para exibir informações detalhadas e um item mapeado por imagem se a área do mapa tiver um atributo rollover_key válido. Para incluir um painel Informações, especifique um URL do Servidor de Informações no painel Configurações do painel Informações da janela Predefinição do visualizador do eCatalog.

**Visualizador do conjunto de** amostrasExibe uma imagem em uma cor, material, textura, acabamento ou malha diferente. Os usuários clicam em uma miniatura para ver as variações na imagem.

**Visualizador de conjunto de** mídia mistaExibe diferentes tipos de mídia em um visualizador. Você pode incluir Conjuntos de amostras, Conjuntos de rotação, imagens e vídeos. É possível configurar guias para conter tipos diferentes de conteúdo, como uma guia para conjuntos de imagens e uma guia para vídeos. Os vídeos reproduzidos de um Conjunto de mídia mista usam um visualizador de vídeo padrão com controles de linha do tempo e vídeo, como Parar, Pausar, Retroceder e Reproduzir. Quando você configura uma predefinição do visualizador de conjunto de mídia mista, especifica quais visualizadores deseja usar para os diferentes tipos de ativos no Conjunto de mídias mistas. Você também pode usar o Visualizador de grade ou o Visualizador de carrossel para visualização de um conjunto de mídia mista.

**** Visualizador de conjunto de rotaçãoFornece várias visualizações de uma imagem para que os usuários possam girar o objeto para examinar os diferentes lados e ângulos.

**Visualizador** de vídeoExibe vídeos usando as dimensões de resolução do arquivo de origem ou um tamanho personalizado. O Dynamic Media Classic vem com muitas predefinições de visualizador predefinidas para reprodução de vídeo e, se você for um administrador, poderá criar predefinições personalizadas do Visualizador de vídeo. Há mais de uma dúzia de configurações diferentes para configurar o Visualizador de vídeo. Você pode configurar seu tamanho, a cor do primeiro plano e do plano de fundo, os controles de áudio e vídeo, a barra de progresso, a interface do usuário com a pele, os recursos sociais e a Ajuda.

**Zoom** ViewersOferece uma opção de três tipos de visualizador de zoom:

**Zoom no** visualizadorPermite que os usuários aumentem o zoom na área clicando nela. Eles podem clicar em controles para aumentar o zoom, diminuir o zoom e redefinir a imagem para seu tamanho padrão.

**Visualizador de zoom: Reverter** Exibe uma segunda imagem da área com zoom ao lado da imagem original. Não há controles para usar, os usuários simplesmente movem a seleção para a área que desejam visualização.

Ao determinar o uso total da largura de banda para esse visualizador, considere que a imagem principal e a imagem flyout são servidas no visualizador. O tamanho da imagem principal (Largura e Altura do palco) e o Fator de zoom determinam o tamanho da imagem de flyout. Para impedir que o tamanho do arquivo de menu suspenso se torne muito grande, equilibre estes dois valores: se você tiver um tamanho de imagem principal grande, abaixe o valor do Fator de zoom. (A Largura do Flyout e a Altura do Flyout determinam o tamanho da janela do flyout, mas não o tamanho da imagem do flyout fornecida para o visualizador.)

Por exemplo, se o tamanho da sua imagem principal for 350 por 350 pixels, com um Fator de zoom de 3, a imagem de flyout resultante será de 1050 por 1050 pixels. Se o tamanho da imagem principal for 300 por 300 pixels, com um Fator de zoom de 4, a imagem de flyout será de 1200 por 1200 pixels. Dependendo da configuração de qualidade JPEG (as configurações recomendadas estão entre 80 e 90), é possível diminuir o tamanho do arquivo significativamente. Os fatores de zoom recomendados são de 2,5 a 4, dependendo do tamanho da imagem principal.

### Matriz de compatibilidade do Dynamic Media Classic Viewer Preset {#scene-viewer-preset-compatibility-matrix}

**Aviso** de Fim da Vida Útil para Visualizadores de Flashes: A partir de 31 de janeiro de 2017, o Adobe Dynamic Media Classic encerrou oficialmente o suporte para a plataforma do visualizador de Flashes.

A tabela a seguir identifica as predefinições do Dynamic Media Classic Viewer atualmente disponíveis. A tabela também especifica a compatibilidade do visualizador com dispositivos desktop e móveis e a tecnologia usada para cada visualizador.

Consulte também [Exemplos de biblioteca de referência de visualizadores de Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Para obter informações sobre o navegador da Web e as versões do sistema operacional compatíveis para visualizadores, consulte as Notas de versão dos visualizadores.

Consulte [Notas de versão de referência dos visualizadores do Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/home.html).

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de zoom |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_escuro | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_black | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de amostras |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_black | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do eCatalog |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Inclui suporte para mídia social e pesquisa de catálogo.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Inclui suporte para mídia social e pesquisa de catálogo.) | HTML5 | X | X | X | X | X |

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de rotação |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_black | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**Visualizadores de eVideo**

O Dynamic Media Classic oferece suporte à reprodução de vídeo móvel para vídeo MP4 H.264.

* Você pode encontrar dispositivos Blackberry compatíveis com este formato de vídeo no seguinte endereço: [Formatos de vídeo suportados no Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Você também pode encontrar dispositivos Windows compatíveis com este formato de vídeo no seguinte endereço:[Formatos de vídeo suportados no Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android | Blackberry Smartphone | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Inclui suporte para legendagem fechada). Consulte [Prática recomendada: Usando o Visualizador de vídeo Universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Inclui suporte para legendagem e mídia social.) | HTML5 | X | X | X | X | X | X | X |

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores de conjunto de mídia mista |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_black | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matriz de Gestos de Visualizadores Móveis Suportados {#supported-mobile-viewers-gestures-matrix}

A tabela a seguir identifica os gestos do visualizador móvel compatíveis com dispositivos iOS, Android 2.x e Android 3.x.

|  | Tecnologia do visualizador | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Tablet Android |
|--- |--- |--- |--- |--- |--- |--- |
| Visualizadores do conjunto de imagens |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_black | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Sobre a tela Predefinição do visualizador {#about-the-viewer-preset-screen}

Crie e gerencie as predefinições do visualizador na tela Predefinições do visualizador. Para abrir essa tela, clique em **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

A tela Predefinições do visualizador oferta as ferramentas para fazer estas tarefas:

**Adicionar uma predefiniçãoClique em Adicionar e faça opções na caixa de diálogo Adicionar predefinição do visualizador.** 

Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

**Edição de uma** predefiniçãoSelecione uma predefinição e clique em  **Editar**.

Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

**Excluindo uma** predefiniçãoSelecione uma predefinição e clique em  **Excluir**.

**Exportar uma** predefiniçãoSelecione uma predefinição do visualizador HTML5 e clique em Exportar para baixar a capa do visualizador para que você possa usá-la como a base para criar e adicionar uma nova predefinição do visualizador.

Consulte [Exportar uma predefinição do Visualizador HTML5](application-setup.md#exporting_an_html5_viewer_preset).

**Filtrando a** lista de predefinições do visualizadorUse estas ferramentas para filtrar a lista:

* Abra a lista suspensa **Ativa/Inativa** e escolha uma opção para mostrar predefinições ativas, predefinições inativas ou todas as predefinições.
* Abra a lista suspensa **Visualizador** e escolha uma opção para ver somente visualizadores de um determinado tipo. Escolha **[!UICONTROL All Viewers]** para ver todos os visualizadores.

**Classificação de** predefiniçõesClique no cabeçalho de uma coluna (Ativo, Tipo, Predefinido ou Plataforma) para classificar a lista em uma coluna. Clique no cabeçalho de uma coluna pela segunda vez para classificar a lista em ordem decrescente (ou crescente).

**Ativando e desativando** predefiniçõesSelecione uma predefinição e clique na opção Ativa para ativá-la ou desativá-la.

Consulte [Ativar ou desativar predefinições do Visualizador](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Clique em Pré-visualização no lado direito da tela Predefinições do visualizador para ver a aparência de um ativo na predefinição do visualizador selecionada. Para ver um ativo diferente, clique em Procurar na tela Predefinições do visualizador e selecione um ativo diferente na caixa de diálogo Selecionar Pré-visualização do ativo.

### Adicionar e editar predefinições do visualizador {#adding-and-editing-viewer-presets}

Além de adicionar predefinições do visualizador usando Adicionar na interface do usuário, você também pode usar Exportar para adicionar uma predefinição do visualizador. Basta exportar uma predefinição do visualizador HTML5 existente e usá-la como a base para a nova predefinição.

Consulte [Exportar uma predefinição do Visualizador HTML5](application-setup.md#exporting_an_html5_viewer_preset).

**Para adicionar e editar predefinições do visualizador**

1. Perto do canto superior direito do Dynamic Media Classic, clique em **Configuração** > **Predefinições do visualizador**.

   Você pode filtrar a lista de predefinições. Por exemplo, para ver somente predefinições para Visualizadores de vídeo, selecione Visualizador de vídeo no menu suspenso Visualizadores na barra de ferramentas logo acima da tabela.

1. Na tela Predefinições do visualizador, adicione ou edite a predefinição do visualizador na tela Predefinições do visualizador.

   **** AdicionarClique em Adicionar na barra de ferramentas. Na caixa de diálogo Adicionar predefinição do visualizador, escolha uma plataforma e um tipo de ativo de mídia avançada.

   Clique em **Salvar como** quando terminar de criar a predefinição do visualizador.

   **Adicionando a partir de uma** predefinição de visualizador existenteNa tabela, selecione uma predefinição de visualizador de vídeo e clique em Editar na barra de ferramentas.

   Depois de reconfigurar o Visualizador de vídeo, clique em **Salvar como** para salvar a predefinição usando um nome diferente no campo de texto Nome da predefinição.

   **** EdiçãoSelecione uma predefinição de visualizador existente e clique em  **Editar**.

1. Na tela Configurar visualizador, no campo Nome da predefinição, digite ou edite o nome da predefinição.
1. Defina as opções restantes desejadas.

   >[!NOTE]
   >
   >Escolha Igual à fonte para dimensionar automaticamente o Visualizador de vídeo para o tamanho de resolução do próprio vídeo codificado. Se você escolher essa opção, não será possível inserir a Largura do palco e a Altura do palco. Em vez disso, essas opções vêm do próprio vídeo. Se você escolher Igual à origem, defina a opção Tamanho da margem para refletir as dimensões da capa fora da área de reprodução do vídeo. Esse tamanho de margem é a altura e a largura do pixel dos controles de vídeo. Você pode usar a ilustração a seguir para ajudar a determinar os tamanhos de margens que deseja usar.*

   ![Configuração da margem do visualizador de vídeo](assets/vs_video_viewer_configure_margin.png)

1. Execute um dos procedimentos a seguir:

   * Clique em **Salvar como** se tiver adicionado uma predefinição do visualizador iniciando em uma predefinição existente.
   * Clique em **Salvar** se tiver adicionado ou editado uma predefinição do visualizador.

### Exportar uma predefinição do visualizador HTML5 {#exporting-an-html-viewer-preset}

Você pode exportar uma predefinição do visualizador HTML5 existente para usar como a base para a criação de uma nova predefinição do visualizador HTML5. Essa opção de exportação é útil porque você não precisa criar o visualizador do zero. Em vez disso, você exporta uma predefinição que parece e se comporta perto do que você quer, então você pode usá-la como um ponto de partida para fazer ajustes de design.

Observe que todos os arquivos CSS predefinidos padrão e predefinidos do visualizador no Dynamic Media Classic usam caminhos de serviço de imagem relativos que apontam para ativos localizados em `Scene7SharedAssets`. Por exemplo, o caminho a seguir é relativo para um ativo de imagem em um arquivo CSS predefinido do visualizador, localizado em `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`No entanto, se você estiver hospedando arquivos CSS do visualizador em seu próprio site, será necessário resolver esse caminho de imagem relativo usando um caminho explícito para o Servidor de imagens em seu próprio ambiente. Para fins ilustrativos, se você atualizar o caminho relativo acima para um caminho explícito, ele pode parecer com o seguinte, onde `https://s7d1.scene7.com` é o caminho direto para o servidor de imagem: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Para exportar uma predefinição do visualizador HTML5**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Clique em **Configuração** > **Predefinições do visualizador**.
1. Na barra de ferramentas Predefinições do visualizador, na segunda lista suspensa à esquerda, selecione **HTML5**.
1. Na terceira lista suspensa à esquerda, selecione **Todos os visualizadores**.
1. Selecione a predefinição do visualizador que você deseja usar como a base para uma nova predefinição do visualizador HTML5.
1. Na barra de ferramentas, clique em **Exportar**.
1. Na caixa de diálogo Exportar ativos selecionados, clique em **Enviar exportação**.

   Após a exportação, você obtém um arquivo CSS. Baixe e descompacte o arquivo.

1. Abra o arquivo CSS em um editor de CSS, faça as alterações e salve o arquivo.
1. Carregue o arquivo CSS no Dynamic Media Classic.

   Consulte [Carregando arquivos](uploading-files.md#uploading_files).

1. Publique o arquivo CSS no Dynamic Media Image Server.

   Consulte [Publicar arquivos](publishing-files.md#publishing_files).

1. Adicione a nova predefinição do visualizador, como de costume. Selecione o arquivo CSS do visualizador que você carregou.

   Consulte [Adicionar e editar predefinições do visualizador](application-setup.md#adding_and_editing_viewer_presets).

### Ativar ou desativar as predefinições do visualizador {#activating-or-deactivating-viewer-presets}

Para criar um URL para mostrar ativos, os usuários abrem a lista suspensa Predefinições na caixa de diálogo Pré-visualização, selecionam uma predefinição do visualizador e clicam em Copiar URL (consulte [Copiando o URL de uma predefinição do visualizador](application-setup.md#copying_the_url_of_a_viewer_preset)). Isso predefine as predefinições do visualizador do lista oferta que os administradores adicionam e gerenciam na tela Predefinições do visualizador. Por exemplo, todas as predefinições ativas do eCatalog Viewer aparecem na lista suspensa Predefinições na caixa de diálogo Pré-visualização quando um usuário pré-visualização um eCatalog.

A menos que você desative Predefinições do visualizador na tela Predefinições do visualizador, a lista suspensa Predefinições na caixa de diálogo Pré-visualização pode ficar lotada.

**Para ativar ou desativar as predefinições do visualizador**

1. Escolha **Configuração** > **Predefinições do visualizador** para abrir a tela Predefinições do visualizador.
1. Selecione ou desmarque Opções ativas para ativar ou desativar as predefinições do visualizador.

### Copiando o URL de uma predefinição do visualizador {#copying-the-url-of-a-viewer-preset}

Depois de publicar um ativo, você pode copiar um URL para exibir o ativo com as configurações de uma predefinição do visualizador.

O URL é copiado para a Área de transferência. Você pode usá-lo conforme necessário no código HTML da sua página da Web, dispositivo móvel ou aplicativo.

**Para copiar o URL de uma predefinição do visualizador**

1. Selecione o ativo no Painel de navegação.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade**. No painel Navegação de ativos, clique com o duplo em um único ativo para abri-lo na Visualização Detalhe. No painel URLs e Código incorporado à direita, clique em **Copiar URL** à direita do visualizador desejado.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Copiar URL**.

### Copiando o código incorporado de uma predefinição do visualizador {#copying-the-embed-code-of-a-viewer-preset}

Usar o recurso Incorporar código permite que você revise o código do visualizador para a predefinição do visualizador selecionada. Você também pode copiar o código para a área de transferência para colá-lo em suas páginas da Web para a implantação do visualizador.

A edição do código não é permitida na caixa de diálogo Incorporar código.

**Para copiar o código incorporado de uma predefinição do visualizador**

1. Selecione o ativo no Painel de navegação de ativos.
1. Acima do painel Navegação de ativos, no lado direito da barra de ferramentas, execute um dos procedimentos a seguir:

   * Clique em **Visualização de grade**. No painel Navegação de ativos, clique com o duplo em um único ativo para abri-lo na Visualização Detalhe. No painel URLs à direita, clique em **Código incorporado**.
   * Clique em **Visualização de grade**. No painel Navegação de ativos, selecione um único ativo e, abaixo da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

   * Clique em **Visualização de Lista**. No painel Navegação de ativos, selecione um único ativo e, à direita da imagem em miniatura, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

   * Clique em **Visualização de grade**, **Visualização de Lista** ou **Visualização de detalhes**. Na mesma barra de ferramentas, clique em **Pré-visualização** > **Lista do visualizador**.

   Na página Lista do visualizador, na coluna Ações da tabela, clique em **Código incorporado**.

1. Na caixa de diálogo Incorporar código, clique em **Copiar para a área de transferência**.
1. Clique em **Fechar**.

## Configuração de visualizadores padrão {#configuring-default-viewers}

Você pode usar Visualizadores padrão para configurar o visualizador padrão que está associado a um ativo ao usar a Pré-visualização no Dynamic Media Classic. Você pode configurar a experiência de pré-visualização padrão para os seguintes tipos de ativos:

* Imagem
* Vídeo
* SpinSet
* Catálogo
* ImageSet
* SwatchSet
* MediaSet

**Para configurar visualizadores padrão**

1. Na lista suspensa Configuração, clique em **Configuração do aplicativo**.
1. Na janela Configuração, no painel esquerdo, expanda **Configuração de Aplicativo** > **Visualizadores**
1. Clique em **Visualizadores Padrão**.
1. Na janela Visualizadores padrão, na lista suspensa para cada tipo de ativo, selecione o visualizador que você deseja associar à pré-visualização do ativo.
1. No canto inferior direito da janela Visualizadores padrão, clique em **Salvar configurações**.
1. No canto inferior direito da janela Configuração, clique em **Fechar** para voltar à janela Ativo.

## Visualizações de metadados {#metadata-views}

*Os* Metadatais padronizaram as informações sobre um ativo. Você pode usar metadados para simplificar o fluxo de trabalho, organizar os ativos e aprimorar a pesquisa. O Dynamic Media Classic suporta o padrão IPTC (International Press Telecommunications Council) e o padrão XMP (extensible metadata platform). Antes de os usuários visualizações ou inserirem metadados sobre um ativo em visualização Detalhada, eles podem abrir o menu Visualizações de metadados e escolher o conjunto de campos de metadados que desejam visualização ou usar para descrever o ativo.

O Dynamic Media Classic vem com Visualizações de Metadados predefinidas, e os administradores podem criar suas próprias Visualizações de Metadados para que os usuários escolham quando inserem metadados.

### Criação de uma Visualização de metadados {#creating-a-metadata-view}

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Visualizações de Metadados**.
1. Clique em **Adicionar**.
1. No campo de texto Nome da predefinição, digite um nome para a visualização.
1. (Opcional) Marque **Tornar padrão** para tornar essa visualização a  que os usuários veem quando abrem o painel Metadados na Visualização Detalhes.
1. (Opcional) Selecione **Incluir UDF** para incluir campos definidos pelo usuário na visualização. Os campos definidos pelo usuário aparecem na parte superior do painel Metadados na Visualização Detalhe.
1. Selecione os campos que deseja para a visualização (clique em **Selecionar tudo** para selecionar todos os campos).
1. Clique em **Salvar**.

   As categorias e os campos selecionados para a visualização são exibidos no painel Pré-visualização.

### Gerenciando Visualizações de metadados {#managing-metadata-views}

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Visualizações de Metadados**.
1. Execute um dos procedimentos a seguir:

   * Para pré-visualização de uma visualização, selecione-a. Os campos na visualização aparecem no painel Pré-visualização.
   * Para editar uma visualização, selecione-a e clique em **Editar**. Em seguida, selecione ou cancele a seleção dos nomes dos campos no painel Pré-visualização e marque ou desmarque a opção **Incluir UDF**.
   * Para excluir uma visualização, selecione-a e clique em **Excluir**.
   * Para tornar uma visualização o padrão, selecione-a e clique em **Tornar padrão**. A visualização padrão é aquela que os usuários veem quando abrem um ativo em visualização Detalhada e vão para o painel Metadados.

## Predefinições de metadados {#metadata-presets}

As predefinições de metadados fornecem aos administradores uma maneira de controlar e regular os metadados atribuídos aos ativos. Na visualização Detalhe, um usuário pode inserir metadados sobre um ativo em campos fornecidos para essa finalidade. Por exemplo, um usuário pode digitar um nome de proprietário, uma descrição de direitos autorais e um endereço. Para garantir que os usuários insiram essas informações de forma precisa e completa, é possível criar Predefinições de metadados. A escolha de uma predefinição de metadados na visualização Detalhe preenche os campos de metadados com valores predefinidos. Por exemplo, um nome de proprietário, uma descrição de direitos autorais e um endereço são inseridos automaticamente.

Crie uma predefinição de metadados para cada conjunto de valores de metadados que você deseja que os usuários possam inserir automaticamente na visualização Detalhe para descrever um ativo.

### Criação ou edição de uma predefinição de metadados {#creating-or-editing-a-metadata-preset}

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Predefinições de Metadados** .
1. Na tela Predefinições de metadados, execute um dos procedimentos a seguir:

   * Para criar uma predefinição, clique em **Adicionar**. No campo de texto Nome do modelo de metadados, digite um nome para a predefinição e clique em **Visualizações de metadados** e escolha uma visualização na lista suspensa (consulte [Visualizações de metadados](application-setup.md#metadata_views)).
   * Para editar uma predefinição existente, selecione a predefinição na lista de predefinições de metadados e clique em **Editar**.

1. Expanda os cabeçalhos que deseja incluir na predefinição e insira valores nos diferentes campos que deseja incluir na predefinição.
1. Clique em **Salvar**.

   As categorias e os campos selecionados para a predefinição aparecem no painel Pré-visualização.

### Gerenciando predefinições de metadados {#managing-metadata-presets}

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Predefinições de Metadados**.
1. Execute um dos procedimentos a seguir:

   * Para pré-visualização de uma predefinição, selecione a predefinição que deseja pré-visualização. As informações predefinidas (categorias e campos) são exibidas na tela de Pré-visualização.
   * Para excluir uma predefinição, selecione-a e clique em **Excluir**.

## Campos Definidos pelo Usuário {#user-defined-fields}

Um Administrador do Media Portal ou um Administrador de Empresas pode criar campos de metadados personalizados e definidos pelo usuário. Campos personalizados podem ajudá-lo a organizar ativos no Dynamic Media Classic. Você pode marcar os campos como ativos, conforme necessário. Quando ativados, os nomes desses campos de metadados personalizados são exibidos no painel Metadados na visualização Detalhe. Os usuários podem inserir informações nos campos de metadados definidos pelo usuário para descrever ativos. Os usuários também podem tornar um campo de metadados definido pelo usuário um critério em pesquisas.

Um uso eficaz dos campos de metadados definidos pelo usuário é atrasar o tempo de ativação de um ativo para uma inicialização ou venda específica. Você define um campo &quot;ativação&quot;, com base no tipo *Date*. Em seguida, usando o painel **Metadados** na visualização **Detail** ou **File** > **Editar informações**, você pode especificar quando o ativo é ativado. O Dynamic Media Classic verifica o status de publicação de um ativo e o histórico de publicação. Se não estiver dentro do tempo de ativação, o status de publicação será exibido como &quot;Não publicado&quot;.

>[!NOTE]
>
>Para que os campos definidos pelo usuário sejam exibidos no painel Metadados em visualização de detalhes, inclua campos definidos pelo usuário nas Visualizações de metadados. Na tela Visualizações de metadados, selecione a opção Incluir UDF (campos definidos pelo usuário). Para obter mais informações, consulte [Visualizações de metadados](application-setup.md#metadata_views).

>[!NOTE]
>
>Para pesquisar ativos usando campos personalizados e definidos pelo usuário, clique em **Configuração** > **Configuração Pessoal** e selecione **Incluir UDFs no Search**. Consulte [Configuração Pessoal](personal-setup.md#personal_setup).

### Criação de um campo de metadados definido pelo usuário {#creating-a-user-defined-metadata-field}

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Campos Definidos pelo Utilizador**.
1. Clique em **Adicionar**
1. Na caixa de diálogo Campo personalizado, defina as opções desejadas.

   **** NomeDigite um nome para o campo de metadados.

   **** TipoEscolha uma opção que defina o tipo de informação que os usuários podem digitar no campo de metadados:

   **** StringUma string de texto.

   **Número inteiro** IntAn.

   **** FlutuanteUm número de ponto flutuante.

   **Sim/** NãoUm valor booliano sim/não.

   **Data** Uma data. O formato MM/DD/AAAA é aceito.

   **Nome do** arquivoO nome de um arquivo.

   **** CorO nome de uma cor.

   **** DimensãoA largura e a altura do ativo.

   **** UntypedPara compatibilidade com versões anteriores. Não selecione essa opção.

   **Valor padrãoOpcionalmente,** informe o valor que os usuários provavelmente inserirão no campo. O valor inserido se torna o valor padrão para o campo criado.

   **Aplica** ToOpcionalmente, escolha um tipo de ativo se desejar que o campo de metadados seja aplicado somente a um tipo específico de ativo.

   ***Nota**: Escolha uma opção **Aplica-se a** cuidadosamente porque não é possível alterar a opção **Aplica-se a** depois de criar um campo definido pelo usuário. O Dynamic Media Classic permite que você edite o nome, o tipo e o valor padrão de um campo definido pelo usuário, mas não a configuração **Aplica-se a**. *

1. Clique em **Salvar** ao terminar de criar o campo de metadados.

### Gerenciar campos definidos pelo usuário {#manage-user-defined-fields}

A tela Campos definidos pelo usuário oferta comandos para gerenciar campos de metadados personalizados e definidos pelo usuário.

Somente um Administrador do Media Portal ou um Administrador de Empresas pode gerenciar campos definidos pelo usuário.

Para abrir esta tela, clique em **Configuração** > **Configuração de Aplicativo** > **Metadados** > **Campos Definidos pelo Utilizador**.

**Edição de um** campoSelecione o campo e clique em  **Editar**.

**Excluindo um** campoSelecione o campo e clique em  **Excluir**.

**Ativar** campoClique para selecionar ou desmarcar a opção Ativa ao lado do nome de um campo. Se você tiver uma função de administração de empresa, essa opção pode não ser exibida. Como essa opção está relacionada ao MediaPortal, você deve selecionar (ativar) Mostrar recursos do MediaPortal na Configuração pessoal para ver os campos de ativação.

## Otimizar arquivos {#optimize-files}

À medida que você carrega arquivos no Dynamic Media Classic, o sistema os otimiza para armazenamento e publicação. No entanto, se o processo de upload for interrompido, algumas imagens não poderão ser otimizadas. Nesse caso, você verá a mensagem &quot;Imagem ainda não otimizada&quot;. No entanto, você pode otimizar esses arquivos se for um administrador.

O Dynamic Media Classic pesquisa seus arquivos e otimiza somente as imagens que não foram totalmente otimizadas antes.

1. Escolha **Configuração** > **Configuração de Aplicação** e selecione O **otimizar Ficheiros**.
1. Digite as informações para o trabalho de otimização e clique em **Enviar**.

   Se você estiver trabalhando com mais de uma empresa, otimize os arquivos pertencentes a empresas diferentes separadamente.

## Predefinições do Conjunto de Lotes {#batch-set-presets}

Use as predefinições de conjuntos de lotes para criar automaticamente conjuntos de imagens ou conjuntos de rotação enquanto uma tarefa estiver sendo executada para fazer upload de ativos para o Dynamic Media Classic.

Os administradores de empresa definem primeiro as convenções de nomenclatura para os ativos que desejam agrupar em um conjunto. Em seguida, é possível criar uma predefinição de conjunto de abits para fazer referência a essas imagens. Cada predefinição é um conjunto exclusivo de instruções autocontidas e nomeadas que define como construir o conjunto usando imagens que correspondem às convenções de nomenclatura definidas na fórmula predefinida.

Todas as predefinições de conjuntos de lotes ativos para uma empresa são listadas na caixa de diálogo Carregar opção de trabalho, para que você possa especificar qual predefinição deseja aplicar durante cada sessão de upload. Os administradores de empresas veem todas as predefinições de conjunto de lotes ativas e inativas. Quando você carrega arquivos, o Dynamic Media Classic cria automaticamente um conjunto com todos os arquivos que correspondem à convenção de nomenclatura definida nas predefinições ativas.

### Nomeação padrão {#default-naming}

O administrador da empresa cria uma convenção de nomenclatura padrão que é usada em qualquer fórmula predefinida de conjunto de lotes. A convenção de nomenclatura padrão selecionada na definição predefinida do conjunto de lotes pode ser tudo o que sua empresa precisa para gerar conjuntos em lote para todos os sites. Uma predefinição de conjunto de lotes é criada para usar a convenção de nomenclatura padrão definida. Você pode criar quantas predefinições de Conjunto de Lotes tiver convenções de nomenclatura alternativas e personalizadas, necessárias para um determinado conjunto de conteúdo, em casos em que haja uma exceção para a nomeação padrão definida pela empresa.

Embora a configuração de uma convenção de nomenclatura padrão não seja necessária para usar a funcionalidade predefinida de conjunto de lotes, as práticas recomendadas recomendam que você use a convenção de nomenclatura padrão para definir quantos elementos da convenção de nomenclatura você deseja agrupar em um conjunto para simplificar a criação de conjuntos de lotes.

1. Clique em **Configuração** > **Configuração de Aplicativo** > **Predefinições de Conjunto de Lote** > **Nomeação Predefinida**.
1. Selecione **Exibir formulário** ou **Exibir código** para especificar como deseja exibir e inserir informações sobre cada elemento.

   Você pode marcar a caixa de seleção Código de Visualização para visualização da criação de valor de expressão normal ao lado das seleções de formulário. Você pode inserir ou alterar esses valores para ajudar a definir os elementos da convenção de nomenclatura, se a visualização de formulário limitar você por algum motivo. Se os valores não puderem ser analisados na visualização de formulário, os campos de formulário ficarão inativos.

   >[!NOTE]
   >
   >Campos de formulário desativados não indicam expressão regular inválida. Não há validação de que suas expressões normais estejam corretas. Você verá os resultados da expressão regular que está criando para cada elemento após a linha de resultados. A expressão regular completa fica visível na parte inferior da página.

1. Expanda cada elemento conforme necessário e informe as convenções de nomenclatura que deseja usar.
1. Conforme necessário, clique em **Adicionar** para adicionar outra convenção de nomenclatura para um elemento. Ou clique em **Remover** para excluir uma convenção de nomenclatura para um elemento.
1. Clique em **Salvar como** e digite um nome para a predefinição. Ou clique em **Salvar** se estiver editando uma predefinição existente.

Como alternativa, é possível usar o Código de Visualização sem campos de formulário disponíveis. Nessa visualização, você cria suas definições de convenção de nomenclatura totalmente usando expressões regulares.

Dois elementos estão disponíveis para definição, Correspondência e Nome básico. Esses campos permitem que você defina todos os elementos de uma convenção de nomenclatura e identifique a parte da convenção usada para nomear o conjunto no qual eles estão contidos. A convenção de nomenclatura individual de uma empresa pode utilizar uma ou mais linhas de definição para cada um desses elementos. Você pode usar quantas linhas desejar para sua definição exclusiva e agrupá-las em elementos distintos, como para a Imagem principal, o elemento Cor, o elemento Visualização alternativa e o elemento Amostra.

### Criando uma predefinição de conjunto de lotes {#creating-a-batch-set-preset}

O Dynamic Media Classic usa predefinições de conjuntos de lotes para organizar ativos que compartilham informações ou conteúdo comuns em conjuntos de imagens para exibição em visualizadores. As fórmulas predefinidas do conjunto de lotes são executadas automaticamente junto com os trabalhos de importação de ativos agendados no Dynamic Media Classic.

Use a predefinição de conjunto de lotes para criar, editar e gerenciar as predefinições de conjunto de lotes. Você pode criar quantas predefinições de conjuntos de lotes forem necessárias para cobrir todas as tarefas de assimilação de ativos forem necessárias. Existem duas formas de definições predefinidas de conjuntos de lotes: uma para uma convenção de nomenclatura padrão que você pode ter configurado e outra para convenções de nomenclatura personalizadas que você cria dinamicamente.

Você pode usar o método de campo de formulário para definir uma predefinição de conjunto de lotes ou o método de código, que permite usar expressões regulares. Como em Nomenclatura padrão, você pode escolher Visualização de código ao mesmo tempo que está definindo na Visualização de formulário e usar expressões comuns para criar suas definições. Como alternativa, você pode desmarcar qualquer visualização para usar uma ou a outra exclusivamente.

Consulte também [Criar um conjunto de lotes predefinido para a geração automática de um Conjunto de rotação 2D](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Para criar uma predefinição de conjunto de lotes**

1. Clique em **Configuração** > **Configuração de Aplicação** > **Predefinições de Conjunto de Lotes** > **Predefinição de Conjunto de Lotes**. **Formulário** de visualização, conforme definido no canto superior direito da página Detalhes, é a visualização padrão.
1. No painel Lista predefinida, clique em **Adicionar** para ativar os campos de definição no painel Detalhes no lado direito da tela.
1. No painel Detalhes, no campo Nome da predefinição, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lotes, selecione um tipo predefinido.

   Para gerar automaticamente um Conjunto de rotação 2D, selecione **Conjunto de rotação de vários eixos** na lista suspensa Tipo de conjunto de lotes.

1. Execute um dos procedimentos a seguir:

   * Se você estiver usando uma convenção de nomenclatura padrão configurada anteriormente em Configuração do aplicativo > Predefinições do conjunto de lotes > Nomeação padrão, expanda **Convenções de nomenclatura de ativos** e, na lista suspensa Nomeação de arquivos, clique em **Padrão**.
   * Para definir uma convenção de nomenclatura conforme você configura a predefinição, expanda **Convenções de nomenclatura de ativos** e, na lista suspensa Nomenclatura de arquivos, clique em **Personalizado**.

1. Para ordem de sequência, defina a ordem das imagens depois que o conjunto for agrupado no Dynamic Media Classic. Por padrão, seus ativos são ordenados alfanuméricos. Entretanto, é possível usar uma lista separada por vírgulas de expressões regulares para definir a ordem.
1. Para Definir a Convenção de Nomeação e Criação, especifique o sufixo ou o prefixo para o nome básico definido na Convenção de Nomeação de Ativos. Defina também onde o conjunto de imagens será criado na estrutura de pastas do Dynamic Media Classic.

   Se você definir grandes números de conjuntos de imagens, talvez prefira mantê-los separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados pelo conjunto de lotes aqui.

1. Clique em **Salvar** no Painel de detalhes.

### Criação de um conjunto de lotes predefinido para a geração automática de um conjunto de rotação 2D {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Você pode usar o Tipo de Conjunto de Lotes **Conjunto de rotação de vários eixos** para criar uma &quot;fórmula&quot; que automatiza a geração de Conjuntos de rotação 2D. O agrupamento de imagens usa expressões regulares de Linha e Coluna para que os ativos de imagem sejam alinhados corretamente no local correspondente na matriz multidimensional.

Consulte também [Criar um conjunto de lotes predefinido](application-setup.md#creating_a_batch_set_preset).

Não há um número mínimo ou máximo de linhas ou colunas que você deve ter em um conjunto de rotação de vários eixos.

Por exemplo, suponha que você queira criar um conjunto de rotação de vários eixos chamado *spin-2dspin*. Você tem um conjunto de imagens de conjunto de rotação que contém três linhas, com 12 imagens por linha. As imagens são nomeadas da seguinte forma:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Com essas informações, sua receita de Tipo de Conjunto de Lotes pode ser criada da seguinte maneira:

![](assets/se_batch_set_recipe.png)

O agrupamento para a parte do nome do ativo compartilhado do conjunto de rotação é adicionado ao campo **Correspondência** (como destacado). A parte variável do nome do ativo que contém a linha e a coluna é adicionada aos campos **Linha** e **Coluna**, respectivamente.

Quando o Conjunto de rotação é carregado e publicado, você ativaria o nome da fórmula do Conjunto de rotação 2D que está listada em **Predefinições de conjunto de lote** na caixa de diálogo **Opções de trabalho de upload**.

**Para criar um conjunto de lotes predefinido para a geração automática de um conjunto de rotação 2D**

1. Escolha **Configuração** > **Configuração de Aplicação** > **Predefinições de Conjunto de Lotes** > **Predefinição de Conjunto de Lotes**. **Formulário** de visualização, conforme definido no canto superior direito da página Detalhes, é a visualização padrão.
1. No painel Lista predefinida, clique em **Adicionar** para ativar os campos de definição no painel Detalhes no lado direito da tela.
1. No painel Detalhes, no campo Nome da predefinição, digite um nome para a predefinição.
1. No menu suspenso Tipo de conjunto de lote, selecione **Conjunto de ativos**.
1. Na lista suspensa Subtipo, selecione **Conjunto de rotação de vários eixos**.
1. Expanda **Convenções de nomenclatura de ativos** e, em seguida, na lista suspensa Nomenclatura de arquivos, clique em **Personalizado**.
1. Use os atributos **Correspondência** e, opcionalmente, **Nome de base** para definir uma expressão regular para nomear ativos de imagem que compõem o agrupamento.

   Por exemplo, sua expressão regular de Correspondência literal pode parecer com o seguinte:

   `(\w+)-\w+-\w+`

1. Expanda **Posição da coluna da linha** e, em seguida, defina o formato do nome para a posição do ativo de imagem na matriz 2D do Conjunto de rotação.

   Use os parênteses para adotar a posição de linha ou coluna no nome do arquivo.

   Por exemplo, para a sua expressão regular de linha, ela pode parecer com o seguinte:

   `\w+-R([0-9]+)-\w+`

   ou

   `\w+-(\d+)-\w+`

   Para sua expressão regular de coluna, pode ser semelhante ao seguinte:

   `\w+-\w+-C([0-9]+)`

   ou

   `\w+-\w+-C(\d+)`

   Lembre-se de que esses são apenas exemplos. Você pode criar sua expressão normal da maneira que quiser, de acordo com suas necessidades.

   >[!NOTE]
   >
   >Se a combinação de expressões regulares de linha e coluna não puder determinar a posição do ativo dentro da matriz de fiação multidimensional, esse ativo não será adicionado ao conjunto e um erro será registrado.

1. Para Definir a Convenção de Nomeação e Criação, especifique o sufixo ou o prefixo para o nome básico definido na Convenção de Nomeação de Ativos. Defina também onde o conjunto de imagens será criado na estrutura de pastas do Dynamic Media Classic.

   Se você definir grandes números de conjuntos de imagens, talvez prefira mantê-los separados das pastas que contêm os próprios ativos. Muitos clientes criam uma pasta Conjuntos de imagens e redirecionam o aplicativo para colocar conjuntos gerados pelo conjunto de lotes aqui.

1. Clique em **Salvar** no Painel de detalhes.
1. Carregue e publique seu Conjunto de rotação como de costume, certificando-se de ativar o nome do Conjunto de rotação 2D na caixa de diálogo Opções de carga de trabalho, em Predefinições de conjunto de lotes.

>[!MORELIKETHIS]
>
>* [Visualização de um ativo](previewing-asset.md#previewing_an_asset)
>* [Configuração de predefinições de imagens](setting-image-presets.md#setting_up_image_presets)
>* [Exibição, adição e exportação de metadados](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files)

