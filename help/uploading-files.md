---
title: Upload de arquivos
seo-title: Upload de arquivos
description: nulo
seo-description: Saiba como carregar arquivos.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '3855'
ht-degree: 0%

---


# Upload de arquivos{#uploading-files}

Antes de fazer upload dos arquivos de ativos para o Dynamic Media Classic, verifique se os arquivos de ativos têm o nome correto e se a estrutura da pasta está configurada e organizada da maneira desejada. Você pode carregar arquivos de um site FTP fornecido pelo Dynamic Media Classic ou diretamente do computador ou da rede. Opções do Dynamic Media Classic oferta para otimização de arquivos à medida que você os carrega. Se você instalou o aplicativo Adobe Dynamic Media Classic para desktop, é possível fazer upload de arquivos e pastas arrastando-os diretamente da área de trabalho. (Consulte Configurações gerais [do aplicativo](application-setup.md#general_settings).)

## Preparação de ativos e pastas para upload {#preparing-your-assets-and-folders-for-uploading}

Antes de fazer upload dos ativos para o Dynamic Media Classic, verifique se eles estão no formato e tamanho corretos. Você também deve observar as regras do Dynamic Media Classic para nomear ativos. Ao configurar uma organização de pastas e uma estrutura para os arquivos, você pode localizar e trabalhar com arquivos facilmente.

### Formatos de arquivo de ativos suportados {#supported-asset-file-formats}

Esta tabela lista os formatos de arquivo de ativos compatíveis com o Dynamic Media Classic. Para obter informações sobre arquivos Camera Raw compatíveis, consulte [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formatos de arquivo de ativos | Descrição |
|--- |--- |
| Áudio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Folha de estilos em cascata | CSS |
| perfis coloridos | ICC, ICM |
| Fontes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imagens | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (somente Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Criação de imagens clássicas do Dynamic Media | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

O suporte para upload de TAR e ZIP inclui uma caixa de seleção para selecionar se deseja desempacotar os arquivos.

### Formatos de imagem não suportados no Dynamic Media {#unsupported-image-formats-dynamic-media}

A lista a seguir descreve os subtipos de formatos de arquivo de imagem rasterizada que *não* são suportados no Dynamic Media.

Consulte também [Detectar formatos de arquivo não suportados para Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Arquivos PNG com um tamanho de bloco IDAT maior que 100 MB.
* Arquivos PSB.
* Arquivos PSD com um espaço de cor diferente de CMYK, RGB, Escala de cinza ou Bitmap não são suportados. Espaços de cores Indexadas, Lab e DuoTone não são suportados.
* Arquivos PSD com uma profundidade de bits superior a 16.
* Arquivos TIFF com dados de ponto flutuante.
* Arquivos TIFF com espaço de cor Lab.

### Tipos de ativos {#asset-types}

Para obter os melhores resultados com a plataforma Dynamic Media Classic, use os formatos e tamanhos de arquivo recomendados. Esta tabela lista tipos de ativos, alguns com formatos recomendados e tamanhos de arquivos para ativos usados com frequência.

| Tipo de ativo | Descrição/Recomendações |
|--- |--- |
| Áudio | Os formatos de ativos de entrada de áudio incluem AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. É possível transcodificar o áudio para os seguintes formatos: MP3, AAC e HE-AAC. |
| Imagens (para Dimensionamento de imagem, Zoom, Conjuntos de imagens, Conjuntos de rotação) | As imagens devem ter pelo menos 2000 pixels na dimensão mais longa; os tamanhos de imagem típicos variam de 1500 a 2500 pixels na dimensão mais longa. São recomendados formatos de imagem sem perda, incluindo arquivos TIFF e PNG. Se você usar uma imagem JPEG, use as configurações de mais alta qualidade. Os arquivos GIF de animação são manipulados como outro conteúdo estático. |
| eCatalogs | Use arquivos PDF de alta resolução criados no Adobe® Acrobat® ou um aplicativo do Creative Suite salvo como &quot;pronto para impressão&quot;. Os PDFs incluem todas as fontes, imagens, máscaras e elementos gráficos referenciados necessários, como páginas únicas, páginas espelhadas de duplo ou em um formato de várias páginas. Ordene suas páginas nomeando os arquivos em ordem alfanumérica. Coloque todos os PDFs do seu eCatalog em uma única pasta para facilitar o upload. Você pode selecionar opções de recorte no upload para remover a área de aparagem de PDFs, incluindo marcas de recorte, públicos alvos de registro ou barras coloridas. A maioria dos arquivos PDF prontos para impressão está no espaço de cor CMYK, portanto, é importante obter o perfil de cor CMYK ICC usado com seus arquivos PDF. |
| Modelos | Imagem em camadas ou design de layout que pode incluir texto, imagens e camadas. Camadas de imagem, sequências de texto e atributos, como cor e tamanho, podem ser parametrizados para que os dados variáveis possam ser personalizados. Os requisitos de imagem para uso em modelos são os mesmos que outras imagens. Prepare seus gráficos no Photoshop ou em outro programa de edição de imagens. Salve cada gráfico como um arquivo transparente nivelado no formato TIFF ou PNG. Verifique se a resolução da imagem é apropriada para o uso esperado. As imagens para impressão devem ser de 300 ppi. |
| Vídeos | O Dynamic Media Classic é compatível com arquivos de vídeo salvos nos formatos OGV e MP4. Você pode transcodificar arquivos para o formato MP4 no upload.Consulte Formatos [de arquivo de ativo](#supported-static-file-formats)suportados. |
| Fontes | TrueType, Type1 (somente Windows), fontes OpenType e PhotoFonts carregados |
| Imagens | Imagens e arquivos de imagem em camadas. |
| Conjuntos de imagens e conjuntos de amostras | Um conjunto de imagens relacionadas que podem ser exibidas em um visualizador. |
| perfis ICC | Um perfil colorido que pode ser usado para converter uma imagem carregada de seu espaço de cor de origem em um espaço de cor diferente. |
| Vinhetas | Imagens criadas com o programa de criação de imagens, bem como arquivos relacionados. |
| Arquivos de conteúdo | Arquivos de conteúdo do Adobe InDesign, Illustrator ou Photoshop. |
| Arquivos FXG | Arquivos de formato gráfico independentes de resolução que você pode usar para criar modelos personalizáveis para saída para impressão, Web, email, desktop e dispositivos. |
| Arquivos SVG | Arquivos gráficos vetoriais escaláveis que os servidores de disponibilização de imagens podem renderizar. |
| Arquivos XML | Arquivos que definem regras de pré-processamento usadas para modificar as partes de caminho e query das solicitações. |
| Arquivos de folha de estilos em cascata. | Carregue capas CSS para personalização de visualizadores HTML5. |
| Arquivos JavaScript | Os arquivos Javascript são usados para instrumentação do visualizador para armazenar informações de conta. O Adobe Security recomenda isso somente para contas clientes que têm um domínio separado em uso para o delivery (para evitar scripts entre sites). |

>[!NOTE]
>
>Quando você carrega arquivos de imagem e PDFs no Dynamic Media Classic, o sistema converte esses arquivos de origem em arquivos P-TIFF (Pyramid TIFF). Esses P-TIFFs são os arquivos publicados posteriormente nos Dynamic Media Image Servers. O Dynamic Media Classic usa o formato de arquivo Pyramid Tiff porque contém várias proporções de zoom que permitem o aumento rápido do zoom quando visualizado com um Dynamic Media Classic Zoom Viewer.

### Formatos de arquivo estático suportados {#supported-static-file-formats}

O Dynamic Media Classic é compatível com vários formatos de arquivo estáticos. O conteúdo estático é qualquer ativo publicado &quot;no estado em que se encontra&quot;, como CSS, PDF, SVG, XML e assim por diante.

Os seguintes tipos de arquivos podem ser publicados:

* GIF animado
* Arquivos de áudio
* CSS
* JavaScript (quando a empresa é configurada com seu próprio domínio)
* Vídeo Principal
* PDF (quando o PDF estiver especificamente marcado para publicação após o upload, para evitar o delivery de todos os PDFs para o fluxo de trabalho existente do eCatalog/PDF)
* Vídeo PrX
* SVG
* XML
* ZIP

O Dynamic Media Classic não fornece a opção de gerar um URL de pré-visualização de conteúdo estático.

### Requisitos de nome de arquivo {#filename-requirements}

Como as extensões de nome de arquivo são removidas dos nomes de arquivo durante o processo de upload, o sistema não permite que os arquivos tenham o mesmo nome raiz. No sistema Dynamic Media Classic, o nome do arquivo do ativo menos a extensão do nome do arquivo se torna a ID do ativo. Por esse motivo, nenhum dos dois ativos pode ter o mesmo nome.

Certifique-se de que todos os usuários na empresa compreendam essas regras de nomenclatura de arquivos:

* IDs de ativos com o mesmo nome não são permitidas no sistema.
* Os nomes de ID de ativo fazem distinção entre maiúsculas e minúsculas.
* Como prática recomendada, certifique-se de que as IDs de ativo não contenham espaços em branco (por exemplo, o Black Jacket.tif e o blue Jacket.jpg). O Dynamic Media Classic ASCII codifica espaços em branco em nomes de ativos quando usa nomes de ativos para criar strings de URL. Esses códigos ASCII são difíceis de ler, o que pode dificultar a leitura de URLs.
* Caracteres específicos de idioma são permitidos em nomes de arquivo. No entanto, os seguintes caracteres não são permitidos nos nomes de arquivo:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se um nome de arquivo contiver um ou mais dos caracteres acima, os caracteres serão removidos do nome do arquivo no upload.

Na maioria dos casos, um nome de arquivo de ativo pode ser o mesmo que seu número de item, SKU de produto ou outro nome, como no seguinte:

| Item | Nome do arquivo | ID do ativo |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organização e estrutura da pasta {#folder-organization-and-structure}

Organize e estruture pastas e subpastas para seu conteúdo no Dynamic Media Classic antes de carregar seu conteúdo no sistema. O planejamento dessa forma tem duas grandes vantagens:

* Ao carregar seu conteúdo para o Dynamic Media Classic via FTP, você pode dizer ao sistema para replicar a estrutura da pasta durante o upload. Dessa forma, seu conteúdo é organizado nas mesmas pastas e subpastas do Dynamic Media Classic que no computador ou na rede. (Para replicar a estrutura de pastas no Dynamic Media Classic, selecione a opção Incluir subpastas ao fazer upload de ativos via FTP.)
* Reorganizar pastas dentro do sistema após o upload dos arquivos é muito mais difícil do que começar com uma estrutura de pastas cuidadosamente considerada.

A abordagem e estrutura de nomeação de pastas escolhidas para armazenar o conteúdo no Dynamic Media Classic depende das necessidades de sua organização. Estas são algumas estruturas de pastas de amostra:

**As Pastas baseadas** em SKU são nomeadas de acordo com SKUs ou números de item. Por exemplo, pastas separadas são criadas para todas as séries de 0, 20 e 30 números.

**Baseado** em marca Para fabricantes com várias linhas de marca e varejistas que comercializam outras marcas de outras empresas, separe os arquivos em pastas de produto designadas para marcas diferentes.

**As Pastas baseadas** em projetos são organizadas de acordo com a data de lançamento/desistência ou o nome do projeto. Os clientes que produzem principalmente eCatalogs favorecem essa abordagem.

**Espelho da hierarquia** de pastas do site Essa estrutura de pastas reflete a estrutura de pastas do site, com as pastas nomeadas, por exemplo, para categorias de produtos.

## Sobre o upload de arquivos {#uploading-your-files}

Você pode carregar arquivos individuais da área de trabalho ou fazer upload de pastas via FTP. Se você quiser carregar mais de 100 MB de arquivos ou fazer upload de pastas e subpastas inteiras, selecione a guia FTP **** VIA.

O Dynamic Media Classic envia uma mensagem de email para confirmar quando o trabalho de upload começa e termina, bem como para notificá-lo de qualquer problema.

Durante (ou imediatamente após) um grande trabalho de upload, alguns novos itens podem exibir a mensagem &quot;Imagem ainda não otimizada&quot;. Esta mensagem é exibida porque os arquivos ainda não foram totalmente processados e adicionados ao Dynamic Media Classic. Você pode otimizar esses arquivos posteriormente. (Consulte [Otimizar arquivos](application-setup.md#optimize_files).)

### Carregar arquivos usando a guia FROM DESKTOP (DESKTOP DE) {#upload-files-using-sps-desktop-application}

O aplicativo Dynamic Media Classic Desktop permite carregar arquivos e pastas arrastando.

1. No aplicativo Dynamic Media Classic Desktop, na barra Navegação global, clique em **Carregar**.
1. Na página Carregar, clique na guia **DE DESKTOP** .
1. No lado esquerdo da página Carregar, na área **Selecionar arquivos para upload** , clique em **Procurar** para selecionar os arquivos ou pastas que deseja carregar e clique em **Abrir**.
1. No lado direito da página Carregar, na área **Escolher destino** da pasta, navegue até uma pasta de destino onde deseja que os arquivos ou pastas carregados sejam adicionados.
1. (Opcional) Próximo à parte inferior da página Carregar, no campo Nome **da** tarefa, especifique o novo nome da tarefa de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Tarefas, onde você pode verificar o status dos trabalhos.
Consulte [Verificando arquivos](checking-job-files.md#checking_job_files)de trabalho.
1. (Opcional) Próximo à parte inferior da página Carregar, selecione **Publicar após carregar** se desejar publicar automaticamente os ativos que você carrega.
Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Carregar, selecione **Substituir em qualquer pasta, o mesmo nome do ativo básico, independentemente da extensão** , se desejar que os arquivos carregados substituam os arquivos existentes pelos mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em Configuração do **aplicativo > Configurações gerais > Carregar no aplicativo > Substituir imagens**.
1. Perto do canto inferior direito da página Carregar, clique em Opções **de** trabalho e especifique as opções desejadas.

   Consulte Opções [de](uploading-files.md#upload_options)upload.

1. Na caixa de diálogo Carregar opções de trabalho, clique em **Salvar**.
1. No canto inferior direito da página Carregar, clique em **Enviar upload**.
Para ver o progresso do upload, clique em **Tarefas** na barra de navegação global. Você pode continuar trabalhando no Dynamic Media Classic e retornar à página de Tarefas a qualquer momento para revisar um trabalho em andamento. Para cancelar um trabalho de upload em andamento, selecione **Cancelar** ao lado da Duração.

### Fazer upload de arquivos usando a guia FTP VIA {#upload-files-using-via-ftp}

1. Faça logon no site FTP do Dynamic Media Classic, que é específico para sua região específica. Use o nome de usuário e a senha FTP recebidos do administrador.
1. No Dynamic Media Classic, na barra Navegação global, clique em **Carregar**.
1. Na página Carregar, clique na guia FTP **** VIA.
1. No lado esquerdo da página Carregar, na área **Escolher pasta FTP para upload** , escolha uma pasta FTP da qual fazer upload de arquivos.
1. No lado direito da página Carregar, na área **Escolher destino** da pasta do Adobe Dynamic Media, escolha uma pasta de destino no Dynamic Media Classic.
1. (Opcional) Próximo à parte inferior da página Carregar, no campo Nome **da** tarefa, especifique o novo nome da tarefa de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Tarefas, onde você pode verificar o status dos trabalhos.
Consulte [Verificando arquivos](checking-job-files.md#checking_job_files)de trabalho.
1. (Opcional) Próximo à parte inferior da página Carregar, selecione **Publicar depois de carregar** se desejar publicar automaticamente os ativos que você carrega.
Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Carregar, selecione **Substituir em qualquer pasta, o mesmo nome do ativo básico, independentemente da extensão** , se desejar que os arquivos carregados substituam os arquivos existentes pelos mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em Configuração do **aplicativo > Configurações gerais > Carregar no aplicativo > Substituir imagens**.
1. (Opcional; disponível somente se você clicou na guia FTP **VIA) Próximo à parte inferior da página Carregar, selecione** Descompactar arquivos Zip ou Tar no upload **** se desejar extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. Perto do canto inferior direito da página Carregar, clique em Opções **de** trabalho e especifique as opções desejadas.

   Consulte Opções [de](uploading-files.md#upload_options)upload.

1. Na caixa de diálogo Carregar opções de trabalho, clique em **Salvar**.
1. No canto inferior direito da página Carregar, clique em **Enviar upload**.

   Para ver o progresso do upload, na barra de navegação global, clique em **Tarefas**. A página Tarefas mostra o progresso do upload. Você pode continuar trabalhando no Dynamic Media Classic e retornar à página de Tarefas a qualquer momento para revisar um trabalho em andamento.

Para cancelar um trabalho de upload em andamento, clique em **Cancelar** ao lado da Duração.

## Caixa de diálogo Carregar opções de trabalho {#upload-options}

Ao carregar arquivos, você pode escolher entre as seguintes opções na caixa de diálogo Carregar opções de trabalho:

* **TRABALHO** — Clique em **JOB** para escolher as opções que afetam todo o trabalho de upload.

   Observe que também é possível escolher opções *padrão* para fazer upload de trabalhos usando a caixa de diálogo Opções **de upload** padrão em Configurações gerais. Clique em **Configuração > Configuração do aplicativo > Configurações gerais > Opções** padrão de upload e, em seguida, defina as opções padrão desejadas.

   * **Quando** — A opção **Quando** está disponível somente se você selecionou a guia FTP **** VIA.
      * **Uma vez** — Especifique uma tarefa de carregamento que seja executada uma vez. As opções incluem:
         * **Agora** ... Executa o trabalho de upload imediatamente depois que você clica em **Salvar** na caixa de diálogo Carregar opções de trabalho e, em seguida, clique em **Enviar upload** na página Carregar.
         * **Agendar Para Mais Tarde** — Selecione o ano, o mês, o dia e a hora (em incrementos de 15 minutos) em que você deseja que o trabalho de upload seja executado.
      * **Recorrente** — Especifique um trabalho de upload que seja executado diariamente, semanalmente ou mensalmente. Ou personalize o trabalho de upload de acordo com suas próprias especificações.
         * **Diariamente** — Defina a hora em que deseja que o trabalho seja executado todos os dias. Se você quiser que o serviço seja executado somente de segunda a sexta-feira, selecione Somente **dias** semanais.
         * **Semanalmente** — Escolha um dia específico da semana e hora em que deseja que a tarefa seja executada.
         * **Mensalmente** — Escolha um dia específico do mês ou dia da semana, incluindo a hora do start, em que você deseja que a tarefa seja executada.
         * **Personalizado** — Personalize um intervalo de tempo de carregamento ou publicação de trabalho de acordo com suas próprias especificações. Consulte [Criação de um intervalo](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)de tempo de trabalho de upload ou publicação personalizado.
   * **Publicar após o upload** — Disponível se você selecionou a guia **DE DESKTOP** ou **VIA FTP** . Selecione essa opção para publicar automaticamente os ativos que você carrega. Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Essa opção também está disponível na página Carregar.

   * **Substituir em qualquer pasta, o mesmo nome do ativo base, independentemente da extensão** — Disponível se você selecionou a guia **DE DESKTOP** ou **VIA FTP** . Selecione essa opção se desejar que os arquivos carregados substituam os arquivos existentes pelos mesmos nomes. Essa opção também está disponível na página Carregar. O nome dessa opção pode ser diferente, dependendo das configurações em Configuração do **aplicativo > Configurações gerais > Carregar no aplicativo > Substituir imagens**.

   * **Descompactar arquivos Zip ou Tar no upload** — Disponível se você selecionou a guia **DE DESKTOP** ou **VIA FTP** .
Selecione essa opção se desejar extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.

   * **Incluir subpastas** — Disponível somente se você tiver selecionado a guia FTP **** VIA.
Selecione essa opção se desejar carregar subpastas da pasta que deseja carregar. Os nomes da pasta e suas subpastas carregadas são inseridos automaticamente no Dynamic Media Classic.

   * **Processar arquivos** de metadados — Disponível somente se você selecionou a guia FTP **** VIA. Selecione essa opção se desejar carregar um arquivo XML ou delimitado por tabulação para adicionar metadados a vários ativos.
Consulte [Importar metadados (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPÇÕES** DE CORTE — Para recortar automaticamente pixels de espaço em branco de uma imagem, abra o menu Recortar, escolha Manual e insira medidas de pixel nos campos Superior, Direita, Inferior e Esquerda para recortar das laterais. Você também pode escolher Aparar no menu Cortar e escolher estas opções:

   * **Aparar Com Base** Em — Escolha se deseja cortar com base na cor ou transparência:

      * **Cor** — Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto da imagem com a cor que melhor representa a cor do espaço em branco que você deseja cortar.

         Aparar com base na cor: Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Números próximos a 1 permitem mais diferenças de cor.

      * **Transparência** —  Escolha a opção Transparência.

         Aparar com base na transparência: Especifique 0 para cortar pixels somente se eles forem totalmente transparentes. números mais próximos de 1 permitem mais transparência.

      * **Tolerância** — Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

* **OPÇÕES** DE PERFIL DE COR — Escolha uma conversão de cores ao criar arquivos otimizados usados para o delivery dinâmico Dynamic Media Classic:

   * **Preservação** de cor padrão — Mantém as cores da imagem de origem sempre que as imagens contêm informações de espaço de cor; não há conversão de cores. Quase todas as imagens hoje têm o perfil de cor apropriado já incorporado. No entanto, se uma imagem de origem CMYK não contiver um perfil de cor incorporado, as cores serão convertidas em espaço de cor sRGB (azul verde padrão). O sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.

   * **Manter espaço** de cor original — Mantém as cores originais sem qualquer conversão de cores no ponto de ingestão no Dynamic Media Classic. Para imagens sem um perfil de cor incorporado, qualquer conversão de cor necessária para processar solicitações para a imagem é feita usando os perfis de cor padrão, conforme definido nas configurações de Publicação. Esses perfis coloridos podem não estar alinhados com a cor nos arquivos criados com essa opção. Portanto, é recomendável usar a opção Preservação de cor padrão.

   * **Personalizado De > Para** — Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Essa opção avançada substitui todas as informações de cores incorporadas no arquivo de origem. Você deve selecionar essa opção somente quando todas as imagens que está enviando contêm dados de perfil de cor incorretos ou ausentes.

* **OPÇÕES** DE EDIÇÃO DE IMAGENS — É possível preservar as máscaras &lt;> de recorte em imagens e escolher um perfil colorido.
Consulte Opções de edição de [imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPÇÕES** POSTSCRIPT — Você pode rasterizar arquivos PostScript®, cortar arquivos, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cor.
Consulte [Trabalhar com arquivos](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)PostScript e Illustrator.

* **OPÇÕES** DO PHOTOSHOP — Você pode criar modelos a partir de arquivos do Adobe® Photoshop®, manter camadas, especificar como as camadas são nomeadas, extrair texto e especificar como as imagens são ancoradas em modelos.
Consulte Opções [de upload de](psd-files.md#psd_upload_options)PSD.

* **OPÇÕES** DE PDF — Você pode rasterizar os arquivos, extrair palavras de pesquisa e links, gerar automaticamente um eCatalog, definir a resolução e escolher um espaço de cor.
Consulte Opções [de upload de](pdfs.md#pdf_upload_options)PDF.

* **OPÇÕES** DO ILLUSTRATOR — Você pode rasterizar arquivos do Adobe Illustrator®, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cor.
Consulte [Trabalhar com arquivos](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)PostScript e Illustrator.

* **OPÇÕES** DE EVIDEO — Você pode transcodificar um arquivo de vídeo escolhendo uma predefinição de vídeo.
Consulte [Trabalhar com predefinições](uploading-encoding-videos.md#working_with_video_encoding_presets)de codificação de vídeo.

* **METADADOS** ADICIONAIS — Digite as palavras-chave que descrevem os arquivos que você carregará. Separe palavras-chave por vírgula. As palavras-chave facilitam a pesquisa por ativos.
Consulte [Realização de uma pesquisa](searching-assets.md#conducting_an_advanced_search)avançada.

* **PREDEFINIÇÕES** DO CONJUNTO DE LOTES — Se quiser criar um Conjunto de imagens, um Conjunto de rotação de vários eixos ou um Conjunto de amostras a partir dos arquivos carregados, clique na coluna Ativo para a predefinição que deseja usar. É possível selecionar mais de uma predefinição. As predefinições são criadas na página Predefinições de Configuração de aplicativo/Conjunto de lotes.
Consulte Predefinições [de Conjunto de](application-setup.md#batch_set_presets)Lotes.

* **AVANÇADO** — Consulte [Siga um upload com outro trabalho](uploading-files.md#follow-an-upload-with-another-job).

## Siga um carregamento com outro trabalho {#follow-an-upload-with-another-job}

Ao fazer upload de itens usando FTP, você pode agendar um trabalho subsequente para começar assim que o upload for concluído. (Se outras tarefas estiverem programadas para começar nesse momento, a tarefa agendada aqui será colocada em fila depois delas.)

A nova ordem de produção envia uma notificação para o endereço especificado, para que o código nesse local possa ser acionado. Esse trabalho de publicação de continuação usa o mesmo nome do trabalho de upload, mas com o texto *Pub_* adicionado ao início.

**Para seguir um upload com outro trabalho**

1. Clique em **Carregar** e, em seguida, clique na guia FTP **** VIA.
1. No canto inferior direito da página Carregar, clique em Opções **** de trabalho.
1. Na caixa de diálogo Carregar opções de trabalho, expanda a seção **AVANÇADO** .
1. Escolha uma das seguintes opções na lista suspensa **Seguir upload com outra tarefa** :

   * Nenhum
   * Solicitação HTTP
   * Publicação de disponibilização de imagem
   * Publicação de renderização de imagem
   * Publicação de vídeo

1. Especifique o endereço HTTP.
1. Especifique se deseja executar somente se os arquivos tiverem sido carregados.
1. Indique se deseja executar essa solicitação sempre que este trabalho for concluído ou somente quando os arquivos forem publicados.

   >[!NOTE]
   >
   >Trabalhos programados regularmente podem não resultar na publicação de arquivos.

>[!MORELIKETHIS]
>
>* [Trabalhar com pastas de ativos](asset-folders.md#working_with_asset_folders)
>* [Manuseando trabalhos recorrentes de upload e publicação](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Usar um trabalho de upload ou publicação como disparador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

