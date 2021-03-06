---
title: Upload de arquivos
description: Saiba como fazer upload de arquivos no Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: ec1a981dd5cfa92ce4ae8e2676dd131d1509216f
workflow-type: tm+mt
source-wordcount: '3714'
ht-degree: 0%

---

# Upload de arquivos{#uploading-files}

Antes de fazer upload dos arquivos de ativos para o Adobe Dynamic Media Classic, verifique se os arquivos de ativos estão nomeados corretamente e se a estrutura de pastas está configurada e organizada da maneira que desejar. Você pode fazer upload de arquivos de um site FTP fornecido pela Adobe Dynamic Media Classic ou diretamente de seu computador ou rede. O Adobe Dynamic Media Classic oferece opções para otimizar arquivos durante o upload. Se você instalou o aplicativo de desktop do Adobe Dynamic Media Classic, é possível fazer upload de arquivos e pastas arrastando-os diretamente da área de trabalho. Consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

## Preparar ativos e pastas para fazer upload {#preparing-your-assets-and-folders-for-uploading}

Antes de fazer upload dos ativos no Adobe Dynamic Media Classic, verifique se eles estão no formato e no tamanho corretos. Também é necessário observar as regras do Adobe Dynamic Media Classic para nomear ativos. Ao configurar uma organização de pastas e uma estrutura para os arquivos, você pode localizar e trabalhar com arquivos facilmente.

### Formatos de arquivo de ativo compatíveis {#supported-asset-file-formats}

Esta tabela lista os formatos de arquivo de ativo compatíveis com o Adobe Dynamic Media Classic. Para obter informações sobre arquivos Camera Raw suportados, consulte [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Formatos de arquivo de ativos | Descrição |
| --- | --- |
| Áudio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Folha de estilos em cascata | CSS |
| Perfis de cores | ICC, ICM |
| Fontes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imagens | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (somente Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Criação de imagens no Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

O suporte ao upload de TAR e ZIP inclui uma caixa de seleção para selecionar se deseja descompactar os arquivos.

### Formatos de imagem não aceitos no Dynamic Media {#unsupported-image-formats-dynamic-media}

A lista a seguir descreve os subtipos de formatos de arquivo de imagem rasterizada que são *not* compatível com o Dynamic Media.

Consulte também [Detectar formatos de arquivo não suportados para o Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Arquivos PNG com um tamanho de bloco IDAT superior a 100 MB.
* Arquivos PSB.
* Arquivos PSD com um espaço de cores diferente de CMYK, RGB, Escala de cinza ou Bitmap não são compatíveis. Não há suporte para espaços de cores DuoTone, Lab e Indexado.
* Arquivos PSD com profundidade de bits superior a 16.
* Arquivos TIFF com dados de ponto flutuante.
* Arquivos TIFF com espaço de cores Lab.

### Tipos de ativos {#asset-types}

Para obter os melhores resultados com o programa Adobe Dynamic Media Classic, use os formatos e tamanhos de arquivo recomendados. Esta tabela lista os tipos de ativos, alguns com formatos recomendados e tamanhos de arquivo para ativos usados com frequência.

| Tipo de ativo | Descrição/Recommendations |
| --- | --- |
| Áudio | Os formatos de ativos de áudio de entrada incluem AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Você pode transcodificar o áudio para os seguintes formatos: MP3, AAC e HE-AAC. |
| Imagens (para Dimensionamento de imagem, Zoom, Conjuntos de imagens, Conjuntos de rotação) | As imagens devem ter pelo menos 2000 pixels no tamanho mais longo; os tamanhos de imagem típicos variam de 1500 a 2500 pixels no tamanho mais longo. Recomendamos formatos de imagem sem perdas, incluindo arquivos TIFF e PNG. Se você usar uma imagem JPEG, use as configurações de mais alta qualidade. Os arquivos GIF de animação são manipulados como outro conteúdo estático. |
| Catálogos eletrônicos | Use arquivos PDF de alta resolução criados no Adobe Acrobat ou um aplicativo Adobe Creative Suite salvo como &quot;pronto para a imprensa&quot;. As PDF incluem todas as fontes, imagens, máscaras e elementos gráficos referenciados necessários, como páginas únicas, páginas espelhadas duplas ou em um formato de várias páginas. Ordene suas páginas nomeando os arquivos em ordem alfanumérica. Coloque todas as PDF para seu eCatalog em uma única pasta para facilitar o upload. Você pode selecionar opções de recorte no upload para remover a área de corte dos PDF, incluindo marcas de recorte, destinos de registro ou barras de cores. A maioria dos arquivos PDF prontos para impressão está no espaço de cores CMYK, portanto, é importante obter o perfil de cores CMYK ICC usado com seus arquivos PDF. |
| Modelos | Imagem em camadas ou design de layout que pode incluir texto, imagens e camadas. Camadas de imagem, sequências de texto e atributos, como cor e tamanho, podem ser parametrizados para que os dados variáveis possam ser personalizados. Os requisitos de imagem para usar em modelos são os mesmos que outras imagens. Prepare seus gráficos no Photoshop ou em outro programa de edição de imagens. Salve cada gráfico como um arquivo transparente nivelado no formato TIFF ou PNG. Certifique-se de que a resolução da imagem seja apropriada para o uso esperado. As imagens para impressão são 300 ppi. |
| Vídeos | O Adobe Dynamic Media Classic oferece suporte a arquivos de vídeo salvos no formato OGV e MP4. Você pode transcodificar arquivos no formato MP4 no upload. Consulte [Formatos de arquivo de ativo compatíveis](#supported-static-file-formats). |
| Fontes | Foram carregadas as fontes TrueType, Type1 (somente Windows®), OpenType® e PhotoFonts. |
| Imagens | Imagens e arquivos de imagem em camadas. |
| Conjuntos de imagens e conjuntos de amostras | Um conjunto de imagens relacionadas que pode ser exibido em um visualizador. |
| Perfis ICC | Um perfil de cores que pode ser usado para converter uma imagem carregada de seu espaço de cores de origem em um espaço de cores diferente. |
| Vinhetas | Imagens criadas com o programa de criação de imagens e arquivos relacionados. |
| Arquivos de conteúdo | Arquivos de conteúdo Adobe InDesign, Illustrator ou Photoshop. |
| Arquivos FXG | Arquivos de formato gráfico independentes de resolução que podem ser usados para criar modelos personalizáveis para saída para impressão, Web, email, desktop e dispositivos. |
| Arquivos SVG | Arquivos gráficos vetoriais dimensionáveis que os servidores de Exibição de imagens podem renderizar. |
| Arquivos XML | Arquivos que definem regras de pré-processamento que são usadas para modificar o caminho e as partes de consulta de solicitações. |
| Arquivos de folha de estilos em cascata. | Fazer upload de capas de CSS para personalização de visualizadores do HTML5. |
| Arquivos JavaScript | Os arquivos JavaScript são usados para instrumentação do visualizador para conter informações da conta. A Segurança de Adobe recomenda esse tipo de ativo somente para contas de clientes que tenham um domínio separado em uso para entrega (para evitar scripts entre sites). |

>[!NOTE]
>
>Quando você carrega arquivos de imagem e PDF para o Adobe Dynamic Media Classic, o sistema converte esses arquivos de origem em arquivos P-TIFF (Pyramid TIFF). Esses P-TIFF são os arquivos publicados posteriormente nos Dynamic Media Image Servers. O Adobe Dynamic Media Classic usa o formato de arquivo Pyramid Tiff porque contém várias taxas de zoom que permitem o zoom rápido quando visualizado com um Visualizador de Zoom do Adobe Dynamic Media Classic.

### Formatos de arquivo estático compatíveis {#supported-static-file-formats}

O Adobe Dynamic Media Classic suporta vários formatos de arquivo estático. O conteúdo estático é qualquer ativo publicado &quot;no estado em que se encontra&quot;, como CSS, PDF, SVG e XML.

Os seguintes tipos de arquivo podem ser publicados:

* GIF animado
* Arquivos de áudio
* CSS
* JavaScript (quando a empresa é configurada com seu próprio domínio)
* Vídeo principal
* PDF (quando o PDF for marcado para publicação após o upload, para evitar a entrega de todos os PDF para o fluxo de trabalho eCatalog/PDF existente)
* Vídeo PrX
* SVG
* XML
* ZIP

O Adobe Dynamic Media Classic não fornece a opção para gerar um URL de visualização de conteúdo estático.

### Requisitos de nome de arquivo {#filename-requirements}

Como as extensões de nome de arquivo são removidas dos nomes de arquivo durante o processo de upload, o sistema não permite que os arquivos tenham o mesmo nome raiz. No sistema Adobe Dynamic Media Classic, o nome do arquivo de ativo menos a extensão do nome do arquivo se torna a ID do ativo do ativo. Por esse motivo, dois ativos não podem ter o mesmo nome.

Certifique-se de que todos os usuários da empresa entendam essas regras de nomenclatura de arquivos:

* As IDs de ativo com o mesmo nome exato não são permitidas no sistema.
* Os nomes de ID de ativo fazem distinção entre maiúsculas e minúsculas.
* Como prática recomendada, verifique se as IDs de ativo não contêm espaços em branco (por exemplo, jacket.tif e blue jacket.jpg). O Adobe Dynamic Media Classic ASCII codifica espaços em branco em nomes de ativos quando usa nomes de ativos para criar strings de URL. Esses códigos ASCII são difíceis de ler, o que pode dificultar a leitura de URLs.
* Caracteres específicos de idioma são permitidos em nomes de arquivo. No entanto, os seguintes caracteres não são permitidos em nomes de arquivo:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se um nome de arquivo contiver um ou mais dos caracteres acima, os caracteres serão removidos do nome do arquivo no upload.

Geralmente, um nome de arquivo de ativo pode ser o mesmo que o número do item, SKU do produto ou outro nome, como no seguinte:

| Item | Nome do arquivo | ID do ativo |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organização e estrutura de pastas {#folder-organization-and-structure}

Organize e estruture pastas e subpastas de seu conteúdo no Adobe Dynamic Media Classic antes de fazer upload do seu conteúdo no sistema. O planejamento dessa forma tem duas grandes vantagens:

* Ao fazer upload de seu conteúdo para a Adobe Dynamic Media Classic via FTP, você pode dizer ao sistema para replicar sua estrutura de pastas durante o upload. Dessa forma, seu conteúdo é organizado nas mesmas pastas e subpastas no Adobe Dynamic Media Classic que está em seu computador ou rede. (Para replicar a estrutura de pastas no Adobe Dynamic Media Classic, selecione a opção Incluir subpastas ao fazer upload de ativos via FTP.)
* Reorganizar pastas dentro do sistema depois que os arquivos forem carregados é muito mais difícil do que começar com uma estrutura de pastas cuidadosamente considerada.

A abordagem de nomeação de pastas e a estrutura escolhida para armazenar seu conteúdo na Adobe Dynamic Media Classic dependem das necessidades da sua organização. Estas são algumas estruturas de pastas de exemplo:

**Baseado em SKU** - As pastas são nomeadas de acordo com SKUs ou números de item. Por exemplo, pastas separadas são criadas para todas as séries de 0, 20 e 30 números.

**Baseado em marca** - Para fabricantes com várias linhas de marca e varejistas que comercializam outras marcas de outras empresas, separe os arquivos em pastas de produtos nomeadas para diferentes marcas.

**Baseado em projeto** - As pastas são organizadas de acordo com a data de lançamento/soltar ou o nome do projeto. Os clientes que produzem principalmente eCatalogs favorecem essa abordagem.

**Espelhamento da hierarquia de pastas do site** - Essa estrutura de pastas reflete a estrutura de pastas do site, com as pastas nomeadas, por exemplo, para categorias de produtos.

## Sobre o upload de arquivos {#uploading-your-files}

Você pode fazer upload de arquivos individuais da área de trabalho ou fazer upload de pastas via FTP. Para carregar mais de 100 MB de arquivos ou fazer upload de pastas e subpastas inteiras, selecione o **VIA FTP** guia .

O Adobe Dynamic Media Classic envia uma mensagem de email para confirmar o início e o término do trabalho de upload, bem como para notificá-lo de qualquer problema.

Durante (ou imediatamente após) um grande trabalho de upload, alguns novos itens poderiam exibir a mensagem &quot;Imagem ainda não otimizada&quot;. Essa mensagem é exibida porque os arquivos ainda não foram totalmente processados e adicionados ao Adobe Dynamic Media Classic. Você pode otimizar esses arquivos posteriormente. Consulte [Otimizar arquivos](application-setup.md#optimize_files).

### Fazer upload de arquivos usando a guia Da área de trabalho {#upload-files-using-sps-desktop-application}

O aplicativo Adobe Dynamic Media Classic Desktop permite fazer upload de arquivos e pastas arrastando.

1. No aplicativo Adobe Dynamic Media Classic Desktop, na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload , selecione o **[!UICONTROL From Desktop]** guia .
1. No lado esquerdo da página Upload , no **[!UICONTROL Select Files for Upload]** , selecione **[!UICONTROL Browse]** para selecionar os arquivos ou pastas que deseja fazer upload, selecione **[!UICONTROL Open]**.
1. No lado direito da página Upload , no **Escolher destino da pasta** navegue até uma pasta de destino onde deseja adicionar os arquivos ou pastas carregados.
1. (Opcional) Próximo à parte inferior da página Upload , no campo de texto Nome do trabalho , digite o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Adobe Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Trabalhos, onde você pode verificar o status dos trabalhos. Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Upload , selecione **[!UICONTROL Publish After Uploading]** se desejar publicar automaticamente os ativos que você fez upload.
Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Upload , selecione **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Próximo ao canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]** e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Fazer upload de opções de trabalho , selecione **[!UICONTROL Save]**.
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Submit Upload]**.
Para ver o progresso do upload, selecione **[!UICONTROL Jobs]** na Barra de Navegação Global. Você pode continuar trabalhando no Adobe Dynamic Media Classic e retornar à página Trabalhos a qualquer momento para revisar um trabalho em andamento. Para cancelar um trabalho de upload em andamento, selecione **[!UICONTROL Cancel]** ao lado de Duração.

### Upload de arquivos usando a guia FTP do VIA {#upload-files-using-via-ftp}

1. Faça logon no site FTP da Adobe Dynamic Media Classic específico da sua região. Use o nome de usuário e a senha FTP recebidos do seu administrador.
1. Na Adobe Dynamic Media Classic, na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload , selecione o **[!UICONTROL VIA FTP]** guia .
1. No lado esquerdo da página Upload , no **[!UICONTROL Choose FTP Folder For Upload]** escolha uma pasta FTP da qual deseja fazer upload de arquivos.
1. No lado direito da página Upload , no **[!UICONTROL Choose Adobe Dynamic Media Folder Destination]** escolha uma pasta de destino no Adobe Dynamic Media Classic.
1. (Opcional) Próximo à parte inferior da página Upload , no campo de texto Nome do trabalho , digite o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Adobe Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Trabalhos, onde você pode verificar o status dos trabalhos.
Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Upload , selecione **[!UICONTROL Publish After Upload]** se desejar publicar automaticamente os ativos que você fez upload.
Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Upload , selecione **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Facultativo; disponível somente se você tiver clicado no **[!UICONTROL VIA FTP]** guia . Próximo à parte inferior da página Upload , selecione **[!UICONTROL Uncompress Zip or Tar Files on Upload]** se quiser extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. Próximo ao canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]** e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Fazer upload de opções de trabalho , selecione **[!UICONTROL Save]**.
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Submit Upload]**.

   Para ver o progresso do upload, na Barra de navegação global, selecione **[!UICONTROL Jobs]**. A página Trabalhos mostra o progresso do upload. Você pode continuar trabalhando no Adobe Dynamic Media Classic e retornar à página Trabalhos a qualquer momento para revisar um trabalho em andamento.

Para cancelar um trabalho de upload em andamento, selecione **[!UICONTROL Cancel]** ao lado de Duração.

## Caixa de diálogo Fazer upload de opções de trabalho {#upload-options}

Ao carregar arquivos, você pode escolher entre as seguintes opções na caixa de diálogo Upload Job Options :

* **TRABALHO** - Selecionar **[!UICONTROL JOB]** para escolher opções que afetam todo o trabalho de upload.

   Você também pode escolher *default* opções para fazer upload de tarefas usando o **[!UICONTROL Default Upload Options]** em Configurações gerais. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]**, em seguida, defina as opções padrão desejadas.

   * **[!UICONTROL When]** - Essa opção só estará disponível se você tiver selecionado a variável **[!UICONTROL VIA FTP]** guia .
      * **[!UICONTROL One-Time]** - Especifique um trabalho de upload que seja executado uma vez. As opções incluem:
         * **[!UICONTROL Now]** - Executa o trabalho de upload imediatamente após a seleção **[!UICONTROL Save]** na caixa de diálogo Upload Job Options e, em seguida, selecione **[!UICONTROL Submit Upload]** na página Upload.
         * **[!UICONTROL Schedule For Later]** - Selecione o ano, mês, dia e hora (em incrementos de 15 minutos) em que você deseja que o trabalho de upload seja executado.
      * **[!UICONTROL Recurring]** - Especifique um trabalho de upload que seja executado diariamente, semanalmente ou mensalmente. Ou personalize o trabalho de upload de acordo com suas próprias especificações.
         * **[!UICONTROL Daily]** - Defina a hora em que deseja que o trabalho seja executado todos os dias. Se quiser que o trabalho seja executado somente de segunda a sexta-feira, selecione **[!UICONTROL Weekdays Only]**.
         * **[!UICONTROL Weekly]** - Escolha um dia específico da semana e hora em que deseja que o trabalho seja executado.
         * **[!UICONTROL Monthly]** - Escolha um dia específico do mês ou dia da semana, incluindo a hora de início, em que você deseja que a tarefa seja executada.
         * **[!UICONTROL Custom]** - Personalize um intervalo de tempo de trabalho de upload ou publicação de acordo com suas próprias especificações. Consulte [Criar um intervalo de tempo de trabalho de upload ou publicação personalizado](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **[!UICONTROL Publish After Uploading]** - Disponível se você selecionou a variável **[!UICONTROL FROM DESKTOP]** ou a guia **[!UICONTROL VIA FTP]** guia . Selecione essa opção para publicar automaticamente os ativos que você fez upload. Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Essa opção também está disponível na página Upload .

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** - Disponível se você selecionou a variável **[!UICONTROL FROM DESKTOP]** ou a guia **[!UICONTROL VIA FTP]** guia . Selecione essa opção se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa opção também está disponível na página Upload . O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

   * **[!UICONTROL Uncompress Zip or Tar Files on Upload]** - Disponível se você selecionou a variável **[!UICONTROL FROM DESKTOP]** ou a guia **[!UICONTROL VIA FTP]** guia .
Selecione essa opção se quiser extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.

   * **[!UICONTROL Include subfolders]** - Disponível somente se você selecionou a variável **[!UICONTROL VIA FTP]** guia .
Selecione essa opção se desejar fazer upload de subpastas da pasta que deseja fazer upload. Os nomes da pasta e suas subpastas que você faz upload são inseridos automaticamente no Adobe Dynamic Media Classic.

   * **[!UICONTROL Process metadata files]** - Disponível somente se você selecionou a variável **[!UICONTROL VIA FTP]** guia . Selecione essa opção se desejar fazer upload de um arquivo XML ou delimitado por tabulação para adicionar metadados a vários ativos.
Consulte [Importar metadados (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **Opções de corte** - Para cortar automaticamente pixels de espaço em branco de uma imagem, abra o **[!UICONTROL Crop]** selecione **[!UICONTROL Manual]** e insira medidas de pixel nos campos de texto Superior, Direita, Inferior e Esquerdo para cortar das laterais. Você também pode selecionar **[!UICONTROL Trim]** no menu Recortar e escolha estas opções:

   * **[!UICONTROL Trim Away Based On]** - Escolha se deseja cortar com base na cor ou na transparência:
      * **[!UICONTROL Color]** - Escolha a opção Color . Em seguida, selecione o menu Canto e escolha o canto da imagem com a cor que melhor representa a cor do espaço em branco que deseja recortar.
Aparar com base na cor: Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Os números mais próximos de 1 permitem mais diferenças de cor.
      * **[!UICONTROL Transparency]** - Escolha o **[!UICONTROL Transparency]** opção.
Aparar com base na transparência: Especifique 0 para cortar pixels somente se eles forem transparentes; números mais próximos de 1 permitem mais transparência.
      * **[!UICONTROL Tolerance]** - Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

* **Opções de perfil de cor** - Escolha uma conversão de cores ao criar arquivos otimizados usados para o delivery dinâmico do Adobe Dynamic Media Classic:

   * **[!UICONTROL Default Color Preservation]** - Mantém as cores das imagens de origem sempre que as imagens contêm informações sobre o espaço de cores; não há conversão de cores. Quase todas as imagens atuais têm o perfil de cores apropriado já incorporado. No entanto, se uma imagem de origem CMYK não contiver um perfil de cor incorporado, as cores serão convertidas em espaço de cor sRGB (azul verde padrão). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.
   * **[!UICONTROL Keep Original Color Space]** - Mantém as cores originais sem qualquer conversão de cores no ponto de ingestão no Adobe Dynamic Media Classic. Para imagens sem um perfil de cor incorporado, qualquer conversão de cor necessária para processar solicitações para a imagem é feita usando os perfis de cor padrão, conforme configurado nas configurações de Publicação. Esses perfis de cores nem sempre estão alinhados com a cor nos arquivos criados com essa opção. Portanto, é recomendável usar a opção Preservação de cor padrão.
   * **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Abre menus para que você possa escolher um **[!UICONTROL Convert From]** e **[!UICONTROL Convert To]** espaço de cores. Essa opção avançada substitui qualquer informação de cor incorporada no arquivo de origem. Selecione essa opção somente quando todas as imagens enviadas contiverem dados de perfil de cores incorretos ou ausentes.

* **Opções de edição de imagem** - Você pode preservar as máscaras de recorte &lt;> em imagens e escolher um perfil de cor.
Consulte [Opções de ajuste de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **Opções do PostScript®** - Você pode rasterizar arquivos do PostScript®, recortar arquivos, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opções do Photoshop** - Você pode criar modelos a partir de arquivos Adobe® Photoshop®, manter camadas, especificar como as camadas são nomeadas, extrair texto e especificar como as imagens são ancoradas em modelos.
Consulte [Opções de upload do PSD](psd-files.md#psd_upload_options).

* **Opções de PDF** - Você pode rasterizar os arquivos, extrair palavras de pesquisa e links, gerar automaticamente um eCatalog, definir a resolução e escolher um espaço de cores.
Consulte [Opções de upload do PDF](pdfs.md#pdf_upload_options).

* **Opções do Illustrator** - Você pode rasterizar arquivos Adobe Illustrator®, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opções de EVIDEO** - Você pode transcodificar um arquivo de vídeo escolhendo uma Predefinição de vídeo.
Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Metadados adicionais** - Insira palavras-chave que descrevem os arquivos que você pretende carregar. Separe as palavras-chave por vírgula. As palavras-chave facilitam a pesquisa de ativos.
Consulte [Realizar uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search). Consulte também [Fazer upload de palavras-chave](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) vídeo de treinamento.

* **Predefinições do conjunto de lotes** - Se quiser criar um Conjunto de imagens, Conjunto de rotação ou Conjunto de amostras a partir dos arquivos carregados, selecione o **[!UICONTROL Active]** para a predefinição que deseja usar. Você pode selecionar mais de uma predefinição. Você cria as predefinições na página Configuração do aplicativo/Predefinições do conjunto de lotes .
Consulte [Predefinições do conjunto de lotes](application-setup.md#batch_set_presets).

* **Avançado** - Consulte [Siga um upload com outro trabalho](uploading-files.md#follow-an-upload-with-another-job).

## Siga um upload com outro trabalho {#follow-an-upload-with-another-job}

Ao fazer upload de itens usando FTP, você pode agendar um trabalho subsequente para começar quando o upload for concluído. Se outras tarefas estiverem programadas para começar, a tarefa agendada aqui será colocada em fila depois delas.

A nova tarefa envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse trabalho de publicação de continuação usa o mesmo nome do trabalho de upload, mas com o texto *Pub_* adicionado ao início.

**Para seguir um upload com outro trabalho:**

1. Selecionar **[!UICONTROL Upload]**, em seguida, selecione o **[!UICONTROL VIA FTP]** guia .
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]**.
1. Na caixa de diálogo Fazer upload de opções de trabalho , expanda a **[!UICONTROL ADVANCED]** seção.
1. Escolha uma das opções a seguir no **[!UICONTROL Follow Upload with another job]** lista suspensa:

   * Nenhum
   * Solicitação HTTP
   * Publicação de fornecimento de imagem
   * Publicação da renderização da imagem
   * Publicação de vídeo

1. Especifique o endereço HTTP.
1. Especifique se deseja executar somente se os arquivos foram carregados.
1. Indique se deseja executar essa solicitação sempre que esse trabalho for concluído ou somente quando os arquivos forem publicados.

   >[!NOTE]
   >
   >Às vezes, os trabalhos agendados regularmente não resultam na publicação de arquivos.

>[!MORELIKETHIS]
>
>* [Trabalhar com pastas de ativos](asset-folders.md#working_with_asset_folders)
>* [Gerenciar trabalhos recorrentes de upload e publicação](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Usar um trabalho de upload ou publicação como acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

