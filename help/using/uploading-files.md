---
title: Fazer upload de arquivos
description: Saiba como carregar arquivos no Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '3717'
ht-degree: 0%

---

# Fazer upload de arquivos{#uploading-files}

Antes de fazer upload de arquivos de ativos para o Adobe Dynamic Media Classic, verifique se os arquivos de ativos estão nomeados corretamente e se a estrutura de pastas está configurada e organizada da maneira desejada. Você pode fazer upload de arquivos de um site FTP fornecido pela Adobe Dynamic Media Classic ou diretamente do computador ou da rede. O Adobe Dynamic Media Classic oferece opções para otimizar os arquivos à medida que você os carrega. Se você instalou o aplicativo de desktop do Adobe Dynamic Media Classic, é possível fazer upload de arquivos e pastas arrastando-os diretamente da sua área de trabalho. Consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).

## Preparar seus ativos e pastas para upload {#preparing-your-assets-and-folders-for-uploading}

Antes de fazer upload dos ativos para o Adobe Dynamic Media Classic, verifique se eles estão no formato e no tamanho corretos. Também é necessário observar as regras do Adobe Dynamic Media Classic para nomear ativos. Ao configurar uma organização e estrutura de pastas para os arquivos, você garante que pode localizar e trabalhar com arquivos facilmente.

### Formatos de arquivo de ativo compatíveis {#supported-asset-file-formats}

Essa tabela lista os formatos de arquivo de ativos compatíveis com o Adobe Dynamic Media Classic. Para obter informações sobre arquivos Camera Raw compatíveis, consulte [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Formatos de arquivo do ativo | Descrição |
| --- | --- |
| Áudio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Folha de Estilos em Cascata | CSS |
| Perfis de cores | ICC, ICM |
| Fontes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imagens | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (somente para Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Criação de imagem do Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

O suporte para upload de TAR e ZIP inclui uma caixa de seleção para selecionar se você deseja descompactar os arquivos.

### Formatos de imagem não aceitos no Dynamic Media {#unsupported-image-formats-dynamic-media}

A lista a seguir descreve os subtipos de formatos de arquivo de imagem rasterizada que são *não* compatível com o Dynamic Media.

Consulte também [Detectar formatos de arquivo não compatíveis com o Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Arquivos PNG com tamanho de bloco IDAT maior que 100 MB.
* Arquivos PSB.
* Arquivos PSD com um espaço de cor diferente de CMYK, RGB, Tons de cinza ou Bitmap não são suportados. Espaços de cores DuoTone, Lab e Indexado não são compatíveis.
* Arquivos PSD com profundidade de bits superior a 16.
* Arquivos TIFF que possuem dados de ponto flutuante.
* Arquivos TIFF com espaço de cores Lab.

### Tipos de ativos {#asset-types}

Para obter os melhores resultados com o programa Adobe Dynamic Media Classic, certifique-se de usar os formatos e tamanhos de arquivo recomendados. Esta tabela lista os tipos de ativos, alguns com formatos e tamanhos de arquivo recomendados para ativos usados com frequência.

| Tipo de ativo | Descrição/Recommendations |
| --- | --- |
| Áudio | Os formatos de ativos de áudio de entrada incluem AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. É possível transcodificar áudio nos seguintes formatos: MP3, AAC e HE-AAC. |
| Imagens (para dimensionamento de imagem, zoom, conjuntos de imagem, conjuntos de rotação) | As imagens devem ter pelo menos 2000 pixels no tamanho mais longo; os tamanhos de imagem típicos variam de 1500 a 2500 pixels no tamanho mais longo. São recomendados formatos de imagem sem perda, incluindo arquivos TIFF e PNG. Se você usar uma imagem de JPEG, use as configurações de mais alta qualidade. Os arquivos de GIF animados são tratados como outros conteúdos estáticos. |
| eCatalogs | Use arquivos de PDF de alta resolução criados no Adobe Acrobat ou um aplicativo de Creative Suite de Adobe salvo como &quot;pronto para impressão&quot;. Os PDF incluem todas as fontes, imagens, máscaras e elementos gráficos referenciados necessários, como páginas únicas, páginas duplas ou em um formato de várias páginas. Ordene suas páginas nomeando os arquivos em ordem alfanumérica. Coloque todos os PDF do eCatalog em uma única pasta para facilitar o upload. Você pode selecionar opções de corte no upload para remover a área de corte dos PDF, incluindo marcas de corte, destinos de registro ou barras de cores. A maioria dos arquivos de PDF prontos para impressão está no espaço de cores CMYK, portanto, é importante obter o perfil de cores CMYK ICC usado com seus arquivos de PDF. |
| Modelos | Design de imagem ou layout em camadas que pode incluir texto, imagens e camadas. Camadas de imagem, cadeias de caracteres de texto e atributos, como cor e tamanho, podem ser parametrizados para que os dados variáveis possam ser personalizados. Os requisitos de imagem para uso em modelos são os mesmos de outras imagens. Prepare seus gráficos no Photoshop ou outro programa de edição de imagens. Salve cada gráfico como um arquivo plano transparente no formato TIFF ou PNG. Verifique se a resolução da imagem é adequada para o uso esperado. As imagens para impressão têm 300 ppi. |
| Vídeos | O Adobe Dynamic Media Classic é compatível com arquivos de vídeo salvos nos formatos OGV e MP4. Você pode transcodificar arquivos para o formato MP4 no upload. Consulte [Formatos de arquivo de ativo compatíveis](#supported-static-file-formats). |
| Fontes | Carregado TrueType, Type1 (somente Windows®), fontes OpenType® e PhotoFonts. |
| Imagens | Imagens e arquivos de imagem em camadas. |
| Conjuntos de imagens e conjuntos de amostras | Um conjunto de imagens relacionadas que podem ser exibidas em um visualizador. |
| Perfis ICC | Um perfil de cores que pode ser usado para converter uma imagem carregada de seu espaço de cores de origem em um espaço de cores diferente. |
| Vinhetas | Imagens criadas com o programa de Criação de imagens e arquivos relacionados. |
| Arquivos de conteúdo | Arquivos de conteúdo do Adobe InDesign, Illustrator ou Photoshop. |
| Arquivos FXG | Arquivos de formato gráfico independentes de resolução que você pode usar para criar modelos personalizáveis para saída em impressão, Web, email, desktop e dispositivos. |
| arquivos SVG | Arquivos gráficos de vetor dimensionáveis que podem ser renderizados pelos servidores do Servidor de imagens. |
| Arquivos XML | Arquivos que definem regras de pré-processamento usadas para modificar o caminho e consultar partes de solicitações. |
| Arquivos de folha de estilos em cascata. | Faça upload de capas CSS para personalizar visualizadores HTML5. |
| Arquivos JavaScript | Os arquivos JavaScript são usados para a instrumentação do visualizador para armazenar informações da conta. A Segurança de Adobe recomenda esse tipo de ativo somente para contas de clientes que tenham um domínio separado em uso para entrega (para evitar script entre sites). |

>[!NOTE]
>
>Quando você faz upload de arquivos de imagem e PDF para o Adobe Dynamic Media Classic, o sistema converte esses arquivos de origem em arquivos P-TIFF (Pyramid TIFF). Esses P-TIFF são os arquivos publicados posteriormente nos Servidores de imagem Dynamic Media. O Adobe Dynamic Media Classic usa o formato de arquivo Pyramid Tiff porque contém várias taxas de zoom que permitem zoom rápido quando visualizado com um Visualizador de zoom do Adobe Dynamic Media Classic.

### Formatos de Arquivo Estático Suportados {#supported-static-file-formats}

O Adobe Dynamic Media Classic é compatível com vários formatos de arquivo estáticos. O conteúdo estático é qualquer ativo publicado &quot;como está&quot;, como CSS, PDF, SVG e XML.

Os seguintes tipos de arquivos podem ser publicados:

* GIF animado
* Arquivos de áudio
* CSS
* JavaScript (quando a empresa está configurada com seu próprio domínio)
* Vídeo principal
* PDF (quando PDF estiver marcado para publicação após o upload, para evitar o delivery de todos os PDF para o fluxo de trabalho eCatalog/PDF existente)
* Vídeo PrX
* SVG
* XML
* ZIP

O Adobe Dynamic Media Classic não fornece a opção de gerar um URL de visualização de conteúdo estático.

### Requisitos de nome de arquivo {#filename-requirements}

Como as extensões de nome de arquivo são removidas dos nomes de arquivo durante o processo de upload, o sistema não permite que os arquivos tenham o mesmo nome raiz. No sistema Adobe Dynamic Media Classic, o nome do arquivo do ativo menos a extensão do nome do arquivo se torna a ID do ativo para o ativo. Por esse motivo, dois ativos não podem ter o mesmo nome.

Certifique-se de que todos os usuários em sua empresa entendam essas regras para nomear arquivos:

* IDs de ativos com o mesmo nome exato não são permitidas no sistema.
* Os nomes de ID de ativo fazem distinção entre maiúsculas e minúsculas.
* Como prática recomendada, verifique se as IDs de ativo não contêm espaços em branco (por exemplo, jaqueta preta.tif e jaqueta azul.jpg). O Adobe Dynamic Media Classic ASCII codifica espaços em branco em nomes de ativos quando usa nomes de ativos para criar sequências de caracteres de URL. Esses códigos ASCII são difíceis de ler, o que pode dificultar a leitura dos URLs.
* Caracteres específicos de idioma são permitidos em nomes de arquivo. No entanto, os seguintes caracteres não são permitidos em nomes de arquivo:

  \ ; / ? : @ &amp; = + $ , &#42; &quot; &lt; > | &#39; { } %

  Se um nome de arquivo contiver um ou mais dos caracteres acima, os caracteres serão removidos do nome do arquivo no upload.

Normalmente, um nome de arquivo de ativo pode ser igual ao número do item, SKU do produto ou outro nome como no seguinte:

| Item | Nome do arquivo | ID do ativo |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organização e estrutura da pasta {#folder-organization-and-structure}

Organize e estruture pastas e subpastas para o conteúdo no Adobe Dynamic Media Classic antes de fazer upload do conteúdo para o sistema. O planejamento antecipado dessa maneira tem duas vantagens principais:

* Ao fazer upload do conteúdo para a Adobe Dynamic Media Classic via FTP, você pode solicitar que o sistema replique a estrutura de pastas durante o upload. Dessa forma, o conteúdo é organizado nas mesmas pastas e subpastas do Adobe Dynamic Media Classic que está no computador ou na rede. (Para replicar a estrutura de pastas no Adobe Dynamic Media Classic, selecione a opção Incluir subpastas ao fazer upload de ativos via FTP.)
* Reorganizar as pastas dentro do sistema depois que os arquivos forem carregados é muito mais difícil do que começar com uma estrutura de pastas cuidadosamente considerada.

A abordagem de nomenclatura de pastas e a estrutura escolhidas para armazenar o conteúdo na Adobe Dynamic Media Classic dependem das necessidades da organização. Estes são alguns exemplos de estruturas de pastas:

**Baseado em SKU** - As pastas são nomeadas de acordo com SKUs ou números de item. Por exemplo, pastas separadas são criadas para todas as séries de 0, 20, 30 números.

**Baseado em marca** - Para fabricantes com várias linhas de marca e varejistas que comercializam outras marcas de outras empresas, separe os arquivos em pastas de produtos com nomes de marcas diferentes.

**Baseado em projeto** - As pastas são organizadas de acordo com a data de implantação/entrega ou o nome do projeto. Os clientes que produzem principalmente eCatalogs favorecem essa abordagem.

**Espelho da hierarquia de pastas do site** - Essa estrutura de pastas espelha a estrutura de pastas do site, com as pastas nomeadas, por exemplo, para categorias de produtos.

## Sobre o upload de arquivos {#uploading-your-files}

Você pode fazer upload de arquivos individuais da área de trabalho ou carregar pastas via FTP. Para carregar mais de 100 MB de arquivos ou carregar pastas e subpastas inteiras, selecione a **VIA FTP** guia.

O Adobe Dynamic Media Classic envia uma mensagem de email para confirmar quando o trabalho de upload começa e termina e para notificá-lo de quaisquer problemas.

Durante (ou imediatamente após) um trabalho de upload grande, alguns novos itens podem exibir a mensagem &quot;Imagem ainda não otimizada&quot;. Essa mensagem é exibida porque os arquivos ainda não foram totalmente processados e adicionados ao Adobe Dynamic Media Classic. Você pode otimizar esses arquivos posteriormente. Consulte [Otimizar arquivos](application-setup.md#optimize_files).

### Fazer upload de arquivos usando a guia Da área de trabalho {#upload-files-using-sps-desktop-application}

O aplicativo Adobe Dynamic Media Classic Desktop permite fazer upload de arquivos e pastas arrastando.

1. No aplicativo Adobe Dynamic Media Classic Desktop, na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload, selecione a variável **[!UICONTROL From Desktop]** guia.
1. No lado esquerdo da página Upload, na guia **[!UICONTROL Select Files for Upload]** , selecione **[!UICONTROL Browse]** para selecionar os arquivos ou pastas dos quais deseja fazer upload, selecione **[!UICONTROL Open]**.
1. No lado direito da página Upload, na guia **Escolher destino da pasta** navegue até uma pasta de destino na qual deseja adicionar os arquivos ou pastas carregados.
1. (Opcional) Próximo à parte inferior da página Upload, no campo de texto Nome da tarefa, digite o novo nome da tarefa de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema que a Adobe Dynamic Media Classic fornece. O job e outros jobs de upload e publicação são registrados na página Jobs, onde você pode verificar o status dos jobs. Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Fazer upload, selecione **[!UICONTROL Publish After Uploading]** se quiser publicar automaticamente os ativos dos quais fez upload.
Ao publicar arquivos, eles são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.
1. (Opcional) Próximo à parte inferior da página Fazer upload, selecione **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** se quiser que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.
O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Próximo ao canto inferior direito da página Fazer upload, selecione **[!UICONTROL Job Options]** e, em seguida, especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Save]**.
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Submit Upload]**.
Para ver o progresso do upload, selecione **[!UICONTROL Jobs]** na Barra de navegação global. Você pode continuar trabalhando no Adobe Dynamic Media Classic e retornar à página Jobs a qualquer momento para revisar um job em andamento. Para cancelar um trabalho de upload em andamento, selecione **[!UICONTROL Cancel]** ao lado de Duração.

### Fazer upload de arquivos usando a guia VIA FTP {#upload-files-using-via-ftp}

1. Faça logon no site FTP da Adobe Dynamic Media Classic que é específico para a sua região específica. Use o nome de usuário e a senha FTP recebidos do administrador.
1. No Adobe Dynamic Media Classic, na barra Navegação global, selecione **[!UICONTROL Upload]**.
1. Na página Upload, selecione a variável **[!UICONTROL VIA FTP]** guia.
1. No lado esquerdo da página Upload, na guia **[!UICONTROL Choose FTP Folder For Upload]** escolha uma pasta FTP da qual fazer upload de arquivos.
1. No lado direito da página Upload, na guia **[!UICONTROL Choose Adobe Dynamic Media Folder Destination]** selecione uma pasta de destino no Adobe Dynamic Media Classic.
1. (Opcional) Próximo à parte inferior da página Upload, no campo de texto Nome da tarefa, digite o novo nome da tarefa de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema que a Adobe Dynamic Media Classic fornece. O job e outros jobs de upload e publicação são registrados na página Jobs, onde você pode verificar o status dos jobs.
Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Fazer upload, selecione **[!UICONTROL Publish After Upload]** se quiser publicar automaticamente os ativos dos quais fez upload.
Ao publicar arquivos, eles são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.
1. (Opcional) Próximo à parte inferior da página Fazer upload, selecione **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** se quiser que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.
O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Opcional; disponível somente se você clicou na opção **[!UICONTROL VIA FTP]** guia. Próximo à parte inferior da página Upload, selecione **[!UICONTROL Uncompress Zip or Tar Files on Upload]** se você deseja extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.
1. Próximo ao canto inferior direito da página Fazer upload, selecione **[!UICONTROL Job Options]** e, em seguida, especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Save]**.
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Submit Upload]**.

   Para ver o progresso do upload, na Barra de navegação global, selecione **[!UICONTROL Jobs]**. A página Jobs mostra o progresso do upload. Você pode continuar trabalhando no Adobe Dynamic Media Classic e retornar à página Jobs a qualquer momento para revisar um job em andamento.

Para cancelar um trabalho de upload em andamento, selecione **[!UICONTROL Cancel]** ao lado de Duração.

## Caixa de diálogo Fazer upload das opções de trabalho {#upload-options}

Ao fazer upload de arquivos, você pode escolher entre as seguintes opções na caixa de diálogo Fazer Upload das Opções de Job:

* **TRABALHO** - Selecionar **[!UICONTROL JOB]** para escolher opções que afetam todo o job de upload.

  Você também pode escolher *padrão* opções para fazer upload de tarefas usando o **[!UICONTROL Default Upload Options]** caixa de diálogo em Configurações gerais. Ir para **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]** e defina as opções padrão desejadas.

   * **[!UICONTROL When]** - Essa opção só estará disponível se você tiver selecionado a opção **[!UICONTROL VIA FTP]** guia.
      * **[!UICONTROL One-Time]** - Especifique um trabalho de upload que é executado uma vez. As opções incluem o seguinte:
         * **[!UICONTROL Now]** - Executa o processo de upload imediatamente após a seleção **[!UICONTROL Save]** na caixa de diálogo Fazer Upload das Opções de Job, selecione **[!UICONTROL Submit Upload]** na página Upload.
         * **[!UICONTROL Schedule For Later]** - Selecione o ano, mês, dia e hora (em incrementos de 15 minutos) em que deseja que o trabalho de upload seja executado.
      * **[!UICONTROL Recurring]** - Especifique um trabalho de upload que seja executado diariamente, semanalmente ou mensalmente. Ou personalize o trabalho de upload de acordo com suas próprias especificações.
         * **[!UICONTROL Daily]** - Defina a hora em que deseja que o trabalho seja executado todos os dias. Para que o job seja executado somente de segunda a sexta-feira, selecione **[!UICONTROL Weekdays Only]**.
         * **[!UICONTROL Weekly]** - Escolha um dia da semana e hora específicos em que deseja que o job seja executado.
         * **[!UICONTROL Monthly]** - Escolha um dia específico do mês ou dia da semana, incluindo a hora de início, em que deseja que o job seja executado.
         * **[!UICONTROL Custom]** - Personalize um intervalo de tempo para fazer upload ou publicar de acordo com suas próprias especificações. Consulte [Criar um intervalo de tempo de trabalho personalizado de carregamento ou publicação](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publish After Uploading]** - Disponível se você selecionou a opção **[!UICONTROL FROM DESKTOP]** ou na guia **[!UICONTROL VIA FTP]** guia. Selecione essa opção para publicar automaticamente os ativos dos quais você fez upload. Ao publicar arquivos, eles são enviados para servidores ativos. Os URLs desses arquivos podem ser usados em sites e aplicativos externos. Essa opção também está disponível na página Fazer upload.

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** - Disponível se você selecionou a opção **[!UICONTROL FROM DESKTOP]** ou na guia **[!UICONTROL VIA FTP]** guia. Selecione essa opção se desejar que os arquivos dos quais você fez upload substituam arquivos existentes com os mesmos nomes. Essa opção também está disponível na página Fazer upload. O nome dessa opção pode ser diferente, dependendo das configurações em **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

   * **[!UICONTROL Uncompress Zip or Tar Files on Upload]** - Disponível se você selecionou a opção **[!UICONTROL FROM DESKTOP]** ou na guia **[!UICONTROL VIA FTP]** guia.
Selecione esta opção se você deseja extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Essa mesma opção também está disponível na caixa de diálogo Opções de tarefa.

   * **[!UICONTROL Include subfolders]** - Disponível somente se você tiver selecionado a variável **[!UICONTROL VIA FTP]** guia.
Selecione essa opção se desejar fazer upload de subpastas da pasta que deseja fazer upload. Os nomes da pasta e suas subpastas que você faz upload são inseridos automaticamente no Adobe Dynamic Media Classic.

   * **[!UICONTROL Process metadata files]** - Disponível somente se você selecionou a opção **[!UICONTROL VIA FTP]** guia. Selecione essa opção se desejar fazer upload de um arquivo XML delimitado por tabulação para adicionar metadados a vários ativos.
Consulte [Importar metadados (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Opções de corte** - Para cortar automaticamente os pixels de espaço em branco de uma imagem, abra o **[!UICONTROL Crop]** selecione **[!UICONTROL Manual]** e insira medidas de pixel nos campos de texto Superior, Direito, Inferior e Esquerdo para cortar das laterais. Também é possível selecionar **[!UICONTROL Trim]** no menu Cortar e escolha estas opções:

   * **[!UICONTROL Trim Away Based On]** - Escolha se deseja cortar com base na cor ou na transparência:
      * **[!UICONTROL Color]** - Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto da imagem com a cor que melhor representa a cor do espaço em branco que você deseja cortar.
Corte com base na cor: especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Números próximos a 1 permitem mais diferença de cor.
      * **[!UICONTROL Transparency]** - Escolha a **[!UICONTROL Transparency]** opção.
Corte baseado em transparência: especifique 0 para cortar pixels apenas se forem transparentes; números mais próximos a 1 permitem mais transparência.
      * **[!UICONTROL Tolerance]** - Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

* **Opções de perfil de cores** - Escolha uma conversão de cores ao criar arquivos otimizados usados para a entrega dinâmica do Adobe Dynamic Media Classic:

   * **[!UICONTROL Default Color Preservation]** - Mantém as cores da imagem de origem sempre que as imagens contêm informações de espaço de cores; não há conversão de cores. Quase todas as imagens atuais têm o perfil de cores apropriado já incorporado. No entanto, se uma imagem de origem CMYK não contiver um perfil de cores incorporado, as cores serão convertidas no espaço de cores sRGB (azul vermelho verde padrão). sRGB é o espaço de cores recomendado para exibir imagens em páginas da Web.
   * **[!UICONTROL Keep Original Color Space]** - Mantém as cores originais sem nenhuma conversão de cores no ponto de assimilação no Adobe Dynamic Media Classic. Para imagens sem um perfil de cores incorporado, qualquer conversão de cores necessária para processar solicitações da imagem é feita usando os perfis de cores padrão, conforme definido nas configurações de Publicação. Esses perfis de cores nem sempre estão alinhados com a cor nos arquivos criados com essa opção. Portanto, é recomendável usar a opção Preservação de cor padrão.
   * **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Abre menus para que você possa escolher um **[!UICONTROL Convert From]** e **[!UICONTROL Convert To]** espaço de cores. Essa opção avançada substitui qualquer informação de cor incorporada no arquivo de origem. Selecione essa opção somente quando todas as imagens que você está enviando contiverem dados de perfil de cores incorretos ou ausentes.

* **Opções de edição de imagem** - É possível preservar as máscaras de recorte &lt;> em imagens e escolher um perfil de cores.
Consulte [Opções de ajuste de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **opções do PostScript®** - Você pode rasterizar arquivos de PostScript®, cortar arquivos, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opções do Photoshop** - Você pode criar modelos a partir de arquivos Adobe® Photoshop®, manter camadas, especificar como as camadas são nomeadas, extrair texto e especificar como as imagens são ancoradas em modelos.
Consulte [opções de upload de PSD](psd-files.md#psd_upload_options).

* **opções de PDF** - Você pode rasterizar os arquivos, extrair palavras e links de pesquisa, gerar automaticamente um eCatalog, definir a resolução e escolher um espaço de cores.
Consulte [opções de upload de PDF](pdfs.md#pdf_upload_options).

* **Opções do Illustrator** - Você pode rasterizar arquivos Adobe Illustrator®, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Opções de VÍDEO** - É possível transcodificar um arquivo de vídeo escolhendo uma Predefinição de vídeo.
Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Metadados adicionais** - Insira palavras-chave que descrevam os arquivos que você pretende fazer upload. Separe as palavras-chave por vírgula. As palavras-chave facilitam a pesquisa de ativos.
Consulte [Realizar uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search). Consulte também [Fazer upload de palavras-chave](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) vídeo de treinamento.

* **Predefinições de conjunto de lotes** - Se quiser criar um Conjunto de imagens, um Conjunto de rotação ou um Conjunto de amostras a partir dos arquivos carregados, selecione a variável **[!UICONTROL Active]** para a predefinição que deseja usar. É possível selecionar mais de uma predefinição. Crie as predefinições na página Configuração do aplicativo/Predefinições de conjunto de lotes.
Consulte [Predefinições de conjunto de lotes](application-setup.md#batch_set_presets).

* **Avançado** - Consulte [Seguir um upload com outro trabalho](uploading-files.md#follow-an-upload-with-another-job).

## Seguir um upload com outro trabalho {#follow-an-upload-with-another-job}

Ao fazer upload de itens usando o FTP, você pode agendar um trabalho subsequente para começar quando o upload estiver concluído. Se outros trabalhos estiverem agendados para começar, o trabalho agendado aqui será enfileirado depois deles.

O novo trabalho envia uma notificação para o endereço especificado, para que o código nesse local possa ser acionado. Esse trabalho de publicação complementar usa o mesmo nome do trabalho de upload, mas com o texto *Pub_* adicionado ao início.

**Para seguir um upload com outro job:**

1. Selecionar **[!UICONTROL Upload]**, em seguida, selecione a **[!UICONTROL VIA FTP]** guia.
1. No canto inferior direito da página Upload, selecione **[!UICONTROL Job Options]**.
1. Na caixa de diálogo Fazer Upload das Opções de Job, expanda a **[!UICONTROL ADVANCED]** seção.
1. Escolha uma das seguintes opções no **[!UICONTROL Follow Upload with another job]** lista suspensa:

   * Nenhum
   * Solicitação HTTP
   * Publicação no Servidor de imagens
   * Publicação de renderização de imagem
   * Publicação de vídeo

1. Especifique o endereço HTTP.
1. Especifique se deseja executar somente se os arquivos foram carregados.
1. Indique se você deseja executar esta solicitação sempre que este trabalho for concluído ou somente quando os arquivos forem publicados.

   >[!NOTE]
   >
   >Trabalhos agendados regularmente podem, às vezes, resultar na não publicação de arquivos.

>[!MORELIKETHIS]
>
>* [Trabalhar com pastas de ativos](asset-folders.md#working_with_asset_folders)
>* [Lidar com trabalhos recorrentes de upload e publicação](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Usar um trabalho de upload ou publicação como acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
