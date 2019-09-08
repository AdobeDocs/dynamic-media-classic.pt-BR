---
title: Carregamento de arquivos
seo-title: Carregamento de arquivos
description: 'null'
seo-description: Saiba como carregar arquivos.
uuid: b 3025 f 84-4 f 28-4276-bc 9 c-f 0 c 0 c 2 a 26 e 12
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: b 2 bc 3 bf 9-e 313-481 a -8670-c 3 bedde 21 b 1 a
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# Carregamento de arquivos{#uploading-files}

Antes de fazer upload de arquivos de ativos para o Sistema de publicação Scene 7, certifique-se de que os arquivos de ativos sejam nomeados corretamente e que sua estrutura de pastas esteja configurada e organizada da maneira desejada. É possível carregar arquivos de um site FTP fornecido pelo Dynamic Media ou diretamente do computador ou rede. O Dynamic Media Classic oferece opções para otimizar arquivos à medida que você os carrega. Se você instalou o aplicativo de publicação do Adobe Scene 7 Publishing System, é possível carregar arquivos e pastas arrastando-os diretamente da área de trabalho. (Consulte [Configurações gerais do aplicativo](application-setup.md#general_settings).)

## Preparação de ativos e pastas para upload {#preparing-your-assets-and-folders-for-uploading}

Antes de carregar ativos no Sistema de publicação do Scene 7, verifique se eles estão no formato e no tamanho corretos. Você também deve observar as regras do Dynamic Media Classic para nomear ativos. Ao configurar uma organização de pastas e uma estrutura para os arquivos, você pode localizar e trabalhar com arquivos facilmente.

### Formatos de arquivo de ativos suportados {#supported-asset-file-formats}

Esta tabela lista os formatos de arquivo de ativos suportados pelo Sistema de publicação Scene 7. Para obter informações sobre arquivos Camera Raw compatíveis, consulte [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formatos de arquivo de ativos | Descrição |
|--- |--- |
| Áudio | AAC, HE-AAC, AC 3, WAV, WMA, AIFF, MP 3 |
| Folha de estilo em cascata | CSS |
| Perfis de cores | ICC, ICM |
| Fontes | AFM, OTF, PFB, PFM, photofont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imagens | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (somente Windows), TIF, TIFF |
| Indesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| Postscript | EPS, PS |
| Criação de imagem clássica do Dynamic Media | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3 GP, AVI, M 2 P, M 2 T, M 2 TS, M 2 V, M 2 V, MOV, MP 4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

O suporte ao upload do TAR e ZIP inclui uma caixa de seleção para selecionar se você deseja desempacotar os arquivos.

### Tipos de ativos {#asset-types}

Para obter resultados ideais com a plataforma do Dynamic Media Classic, certifique-se de usar os formatos e tamanhos de arquivo recomendados. Esta tabela lista tipos de ativos, alguns com formatos recomendados e tamanhos de arquivo para ativos comumente usados.

| Tipo de ativo | Descrição/Recommendations |
|--- |--- |
| Áudio | Os formatos de ativo de entrada de áudio incluem AAC, HE-AAC, AC 3, WAV, WMA, AIFF, MP 3. É possível transcodificar áudio para os seguintes formatos: MP 3, AAC e HE-AAC. |
| Imagens (para dimensionamento de imagem, zoom, conjuntos de imagens, conjuntos de rotação) | As imagens devem ter pelo menos 2000 pixels na dimensão mais longa; tamanhos de imagem típicos variam de 1500 a 2500 pixels na dimensão mais longa. São recomendados formatos de imagem sem perdas, incluindo arquivos TIFF e PNG. Se você usar uma imagem JPEG, use as configurações de mais alta qualidade. Os arquivos GIF animados são manipulados como outro conteúdo estático. |
| Ecatalogs | Use arquivos PDF de alta resolução criados no Adobe® Acrobat® ou em um aplicativo Creative Suite salvo como «pressionamento-pronto. » Os pdfs incluem todas as fontes, imagens, máscaras e elementos gráficos referenciados necessárias, como páginas únicas, propagandas duplas ou em formato de várias páginas. Ordene suas páginas nomeando os arquivos em ordem alfanumérica. Coloque todos os pdfs para o seu ecatalog em uma única pasta para facilitar o upload. É possível selecionar opções de corte no upload para remover a área de aparagem de pdfs, incluindo marcas de corte, metas de registro ou barras de cores. A maioria dos arquivos PDF prontos para pressionar estão no espaço de cores CMYK, portanto, é importante obter o perfil de cores ICC CMYK usado com seus arquivos PDF. |
| Modelos | Imagem em camadas ou design de layout que pode incluir texto, imagens e camadas. Camadas de imagem, sequências de texto e atributos, como cor e tamanho, podem ser instrumentados para que os dados variáveis possam ser personalizados. Os requisitos de imagem para uso em modelos são os mesmos que outras imagens. Prepare seus gráficos no Photoshop ou outro programa de edição de imagens. Salve cada gráfico como um arquivo transparente nivelado no formato TIFF ou PNG. Certifique-se de que a resolução da imagem seja apropriada para o uso esperado. Imagens para impressão devem ser de 300 ppi. |
| Vídeos | O Dynamic Media Classic é compatível com arquivos de vídeo salvos no formato OGV e MP 4. É possível transcodificar arquivos para o formato MP 4 no carregamento. Consulte [Formatos de arquivo de ativos suportados](#supported-static-file-formats). |
| Fontes | Carregado truetype, Type 1 (somente Windows), fontes opentype e photofonts |
| Imagens | Imagens e arquivos de imagem em camadas. |
| Conjuntos de imagens e conjuntos de amostras | Um conjunto de imagens relacionadas que podem ser exibidas em um visualizador. |
| perfis ICC | Um perfil de cor que pode ser usado para converter uma imagem carregada de seu espaço de cor de origem em um espaço de cores diferente. |
| Vinhetas | Imagens criadas com o programa de criação de imagens, bem como arquivos relacionados. |
| Arquivos de conteúdo | Arquivos de conteúdo do Adobe indesign, Illustrator ou Photoshop. |
| Arquivos FXG | Arquivos gráficos independentes de resolução que podem ser usados para criar modelos personalizáveis para a saída para impressão, Web, email, desktop e dispositivos. |
| Arquivos SVG | Arquivos gráficos de vetor dimensionáveis que os servidores de Disponibilização de imagens podem renderizar. |
| Arquivos XML | Arquivos que definem as regras de pré-processamento usadas para modificar o caminho e as partes de consulta das solicitações. |
| Arquivos em cascata em cascata. | Carregue capas de CSS para personalização de visualizadores HTML 5. |
| Arquivos javascript | Os arquivos Javascript são usados para a instrumentação do visualizador para manter as informações da conta. A Adobe Security recomenda isso apenas para contas de cliente que tenham um domínio separado em uso para entrega (para evitar scripts entre sites). |

>[!NOTE]
>
>Quando você carrega arquivos de imagem e pdfs para o SPS, o sistema converte esses arquivos de origem em arquivos P-TIFF (Pyramid TIFF). Esses P-tiffs são os arquivos publicados posteriormente nos servidores de imagem do Dynamic Media. O Dynamic Media Classic usa o formato de arquivo Tiff Pirâmide, pois contém várias taxas de zoom que permitem zoom rápido quando visualizados com um Visualizador de zoom clássico do Media Media.

### Formatos de arquivo estáticos suportados {#supported-static-file-formats}

O Dynamic Media Classic oferece suporte a vários formatos de arquivo estáticos. O conteúdo estático é qualquer ativo publicado como "como-é", como CSS, PDF, SVG, XML e assim por diante.

Os seguintes tipos de arquivo podem ser publicados:

* GIF animado
* Arquivos de áudio
* CSS
* Javascript (quando a empresa está configurada com seu próprio domínio)
* Vídeo mestre
* PDF (quando PDF é marcado especificamente para publicar após o upload, para evitar a entrega de todos os pdfs para o fluxo de trabalho do ecatalog/PDF existente)
* Vídeo prx
* SVG
* XML
* ZIP

O Dynamic Media Classic não fornece a opção de gerar um URL de visualização de conteúdo estático.

### Requisitos do nome do arquivo {#filename-requirements}

Como as extensões de nome de arquivo são removidas dos nomes de arquivo durante o processo de upload, o sistema não permite que os arquivos tenham o mesmo nome de raiz. No sistema do Dynamic Media Classic, o nome do arquivo de ativos menos a extensão de nome de arquivo torna-se a ID do ativo do ativo. Por esse motivo, nenhum ativo pode ter o mesmo nome.

Verifique se todos os usuários da empresa entendem essas regras de nomeação de arquivos:

* As IDs de ativos com o mesmo nome exato não são permitidas no sistema.
* Os nomes de ID de ativo diferenciam maiúsculas de minúsculas.
* Como prática recomendada, certifique-se de que as IDs de ativos não contenham espaços em branco (por exemplo, jaqueta preta. tif e azul jacket.jpg). O Dynamic Media Classic codifica espaços em branco em espaços em branco quando usa nomes de ativos para criar strings de URL. Esses códigos ASCII são difíceis de ler, o que pode tornar os urls de leitura mais difíceis.
* Caracteres específicos de idioma são permitidos em nomes de arquivo. No entanto, os seguintes caracteres não são permitidos nos nomes de arquivo:

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   Se um nome de arquivo contiver um ou mais dos caracteres acima, os caracteres serão removidos do nome do arquivo no upload.

Na maioria dos casos, um nome de arquivo de ativo pode ser o mesmo do número do item, SKU do produto ou outro nome da seguinte maneira:

| Item | Nome de arquivo | ID do ativo |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48 A 3_ 2 X | 48 A 3_ 2 X. tif | 48 A 3_ 2 X |

### Organização e estrutura da pasta {#folder-organization-and-structure}

Organize e estrutestrutestruture pastas e subpastas para seu conteúdo no Sistema de publicação Scene 7 antes de carregar seu conteúdo no sistema. O planejamento desse modo tem duas vantagens importantes:

* Ao carregar seu conteúdo para o SPS via FTP, você pode informar ao sistema para replicar a estrutura de pastas durante o upload. Dessa forma, o conteúdo é organizado nas mesmas pastas e subpastas no SPS que está no computador ou na rede. (Para replicar a estrutura de pastas no SPS, selecione a opção Incluir subpastas quando fizer upload de ativos via FTP.)
* A reorganização de pastas dentro do sistema depois que os arquivos são carregados é muito mais difícil do que começar com uma estrutura de pastas cuidadosamente considerada.

A abordagem e a estrutura de nomenclatura de pastas escolhidas para armazenar seu conteúdo no Sistema de publicação Scene 7 depende das necessidades de sua organização. Estas são algumas amostras de estruturas de pastas:

**As pastas baseadas em SKU** são nomeadas de acordo com skus ou números de item. Por exemplo, pastas separadas são criadas para todas as séries de 0, 20 e number 0 números.

**Baseado em marcas** para fabricantes com várias linhas de marca e varejistas que comercializam outras marcas de outras empresas, separam arquivos em pastas de produtos chamadas de marcas diferentes.

**As pastas** baseadas em projeto são organizadas de acordo com a data de lançamento/data ou o nome do projeto. Clientes que produzem principalmente o ecatalogs preferem essa abordagem.

**Espelho da hierarquia de pastas do site** da Web Essa estrutura de pastas espelha a estrutura de pastas do site, com as pastas denominadas, por exemplo, para categorias de produtos.

## Sobre o carregamento de arquivos {#uploading-your-files}

Você pode fazer upload de arquivos individuais da área de trabalho ou de pastas de upload via FTP. Se desejar carregar mais de 100 MB de arquivos ou carregar pastas e subpastas inteiras, selecione a **guia VIA FTP** .

Se você instalou o aplicativo de desktop do Scene 7 Publishing System, pode arrastar arquivos e pastas diretamente do seu desktop para a pasta de upload de destino.

O Sistema de publicação Scene 7 envia uma mensagem de email para confirmar quando o trabalho de upload começa e termina, e para notificar sobre quaisquer problemas.

Durante (ou imediatamente depois) uma tarefa de upload grande, alguns novos itens podem exibir a mensagem «Imagem ainda não otimizada». Esta mensagem é exibida porque os arquivos ainda não são totalmente processados e adicionados ao SPS. É possível otimizar esses arquivos posteriormente. (Consulte [Otimizar arquivos](application-setup.md#optimize_files).)

### Fazer upload de arquivos usando a guia FROM DESKTOP {#upload-files-using-sps-desktop-application}

O aplicativo Scene 7 Publishing System Desktop permite carregar arquivos e pastas arrastando.

1. No aplicativo de Publicação do sistema de publicação Scene 7, na barra de Navegação global, clique em **Carregar**.
1. Na página Upload, clique na **guia FROM DESKTOP** .
1. No lado esquerdo da página Upload, na área **Selecionar arquivos para fazer upload, clique** em **Procurar** para selecionar os arquivos ou pastas que deseja carregar e clique **em Abrir**.
1. No lado direito da página Upload, na área **Escolher destino** da pasta, navegue até uma pasta de destino onde deseja que os arquivos ou pastas carregados sejam adicionados.
1. (Opcional) Próximo à parte inferior da página Upload, no campo **Nome** do trabalho, especifique o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema que o SPS fornece. Os trabalhos e outras tarefas de upload e publicação são registrados na página Tarefas, onde você pode verificar o status das tarefas.
Consulte [Verificação de arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Upload, selecione **Publicar depois de fazer upload** se desejar publicar automaticamente os ativos que você carrega.
Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os urls para esses arquivos podem ser usados em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Upload, selecione **Substituir em qualquer pasta, mesmo nome de ativo base, independentemente da extensão** , se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em Configuração **do aplicativo &gt; Configurações gerais &gt; Carregar em aplicativo &gt; Substituir imagens**.
1. Próximo ao canto inferior direito da página Carregar, clique **em Opções** de trabalho e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Carregar opções de trabalho, clique **em Salvar**.
1. No canto inferior direito da página Upload, clique **em Enviar upload**.
Para ver o progresso do upload, clique **em Tarefas** na barra de navegação global. Você pode continuar a trabalhar no Sistema de publicação Scene 7 e retornar à página Tarefas a qualquer momento para revisar um trabalho em andamento. Para cancelar um trabalho de upload em andamento, selecione **Cancelar** ao lado do tempo de duração.

### Fazer upload de arquivos usando a guia VIA FTP {#upload-files-using-via-ftp}

1. Faça logon no site FTP clássica do Dynamic Media que é específico para sua região específica. Use o nome de usuário e a senha do FTP recebidos do administrador.
1. No Dynamic Media Classic, na barra Navegação global, clique em **Carregar**.
1. Na página Upload, clique na **guia VIA FTP** .
1. No lado esquerdo da página Upload, na **área Escolher pasta FTP para upload** , escolha uma pasta FTP na qual carregar arquivos.
1. No lado direito da página Upload, na área **Escolher destino** da pasta SPS, escolha uma pasta de destino no Sistema de publicação Scene 7.
1. (Opcional) Próximo à parte inferior da página Upload, no campo **Nome** do trabalho, especifique o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema que o SPS fornece. Os trabalhos e outras tarefas de upload e publicação são registrados na página Tarefas, onde você pode verificar o status das tarefas.
Consulte [Verificação de arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Upload, selecione **Publicar depois de fazer upload** se desejar publicar automaticamente os ativos carregados.
Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os urls para esses arquivos podem ser usados em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. (Opcional) Próximo à parte inferior da página Upload, selecione **Substituir em qualquer pasta, mesmo nome de ativo base, independentemente da extensão** , se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
O nome dessa opção pode ser diferente, dependendo das configurações em Configuração **do aplicativo &gt; Configurações gerais &gt; Carregar em aplicativo &gt; Substituir imagens**.
1. (Opcional; disponível somente se você clicou na **guia VIA FTP** ) Próximo à parte inferior da página Carregar, selecione **Descompactar zip ou arquivos tar em upload** se desejar extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.
1. Próximo ao canto inferior direito da página Carregar, clique **em Opções** de trabalho e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Carregar opções de trabalho, clique **em Salvar**.
1. No canto inferior direito da página Upload, clique **em Enviar upload**.

   Para ver o progresso do upload, na barra de navegação global, clique **em Tarefas**. A página de Tarefas mostra o progresso do upload. Você pode continuar a trabalhar no Sistema de publicação Scene 7 e retornar à página Tarefas a qualquer momento para revisar um trabalho em andamento.

Para cancelar um trabalho de upload em andamento, clique **em Cancelar** ao lado do tempo de duração.

## Caixa de diálogo Carregar opções de trabalho {#upload-options}

Ao carregar arquivos, você pode escolher entre as seguintes opções na caixa de diálogo Opções de upload de trabalho:

* **TRABALHO** — Clique **em JOB** para escolher opções que afetam todo o trabalho de upload.

   Observe que você também pode escolher *opções padrão* para fazer upload de tarefas usando a **caixa de diálogo Opções** de upload padrão em Configurações gerais. Clique **em Configuração &gt; Configuração do aplicativo &gt; Configurações gerais &gt; Opções** de upload padrão e defina as opções padrão desejadas.

   * **Quando** — A **opção Quando** está disponível somente se você selecionou a **guia VIA FTP** .
      * **Uma vez** — Especifique um trabalho de upload executado uma vez. As opções incluem:
         * **Agora** — Executa o trabalho de upload imediatamente depois de clicar **em Salvar** na caixa de diálogo Opções de trabalho de upload e, em seguida, clique **em Enviar upload** na página Carregar.
         * **Agendar para mais tarde** — Selecione o ano, mês, dia e hora (em incrementos de 15 minutos) que você deseja que o serviço de upload execute.
      * **Recorrente** — Especifique um trabalho de upload que execute diariamente, semanalmente ou mensalmente. Ou, personalize o trabalho de upload para suas próprias especificações.
         * **Diariamente** — Defina o tempo que deseja que o serviço execute todos os dias. Se você quiser que a tarefa seja executada somente de segunda a sexta, selecione **Somente dias da semana**.
         * **Semanalmente** — Escolha um dia específico da semana e hora que você deseja que o serviço execute.
         * **Mensalmente** — Escolha um dia específico do mês ou do dia da semana, incluindo a hora inicial, que você deseja que o serviço execute.
         * **Personalizado** — Personalize um intervalo de tempo de trabalho de upload ou publicação para suas próprias especificações. Consulte [Criar um intervalo de tempo de trabalho ou um intervalo de tempo de trabalho personalizado](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publicar após o upload** — Disponível se você selecionou a **guia FROM DESKTOP** ou **a** guia VIA FTP. Selecione essa opção para publicar automaticamente os ativos que você carrega. Quando você publica arquivos, os arquivos são enviados para servidores ativos. Os urls para esses arquivos podem ser usados em sites e aplicativos externos. Essa opção também está disponível na página Upload.

   * **Substituir qualquer pasta, mesmo nome de ativo base, independentemente da extensão** — Disponível se você selecionou a **guia FROM DESKTOP** ou **a** guia VIA FTP. Selecione essa opção se desejar que os arquivos carregados substituam arquivos existentes pelos mesmos nomes. Essa opção também está disponível na página Upload. O nome dessa opção pode ser diferente, dependendo das configurações em Configuração **do aplicativo &gt; Configurações gerais &gt; Carregar em aplicativo &gt; Substituir imagens**.

   * **Descompactar arquivos Zip ou Tar no upload** — Disponível se você selecionou a **guia FROM DESKTOP** ou **a** guia VIA FTP.
Selecione essa opção se desejar extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho.

   * **Incluir subpastas** — Disponível somente se você selecionou a **guia VIA FTP** .
Selecione essa opção se desejar carregar subpastas da pasta que deseja carregar. Os nomes da pasta e suas subpastas são inseridos automaticamente no SPS.

   * **Processar arquivos** de metadados— Disponível apenas se você selecionou a **guia VIA FTP** . Selecione essa opção se desejar carregar um arquivo delimitado por tabulação ou XML para adicionar metadados a vários ativos.
Consulte [Importar metadados (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPÇÕES** DE RECORTE— Para cortar automaticamente pixels de espaço em branco de uma imagem, abra o menu Cortar, escolha Manual e insira medições de pixel nos campos Superior, Direito, Inferior e Esquerda para cortar das laterais. Você também pode escolher Aparar no menu Cortar e escolher estas opções:

   * **Aparar com base em Escolha se deseja cortar com base em cor ou transparência:**

      * **Cor** — Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto da imagem com a cor que representa melhor a cor de espaço em branco que você deseja cortar.

         Aparar com base em cor: Especifique 0 para cortar pixels apenas se eles corresponderem exatamente à cor selecionada no canto da imagem. Números mais próximos a 1 permitem mais diferença de cor.

      * **Transparência** — Escolha a opção Transparência.

         Aparar com base na transparência: Especifique 0 para cortar pixels apenas se eles forem totalmente transparentes; os números mais próximos a 1 permitem mais transparência.

      * **Tolerância** — Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

* **OPÇÕES DE PERFIL DE COR** — Escolha uma conversão de cor ao criar arquivos otimizados que são usados para a entrega dinâmica do Dynamic Media Classic:

   * **Preservação** de cor padrão— Mantém as cores da imagem de origem sempre que as imagens contêm informações sobre espaço de cores; não há conversão de cores. Quase todas as imagens hoje têm o perfil de cor adequado já incorporado. Entretanto, se uma imagem de origem CMYK não contiver um perfil de cores incorporado, as cores serão convertidas em espaço de cores srgb (vermelho vermelho vermelho). O srgb é o espaço de cores recomendado para exibir imagens em páginas da Web.

   * **Manter espaço** de cor original— Mantém as cores originais sem nenhuma conversão de cor no ponto de ingestão no Sistema de publicação do Scene 7. Para imagens sem um perfil de cores incorporado, qualquer conversão de cor necessária para processar solicitações de imagem é feita usando os perfis de cores padrão conforme configurado nas configurações de Publicação. Esses perfis de cores podem não ficar alinhados com a cor dos arquivos criados com essa opção. Portanto, é recomendável usar a opção Preservação padrão de cor.

   * **Personalizado de &gt; Para** — Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Essa opção avançada substitui todas as informações de cores incorporadas ao arquivo de origem. Você deve selecionar essa opção somente quando todas as imagens que você está enviando contêm dados de perfil de cores incorretos ou ausentes.

* **OPÇÕES DE EDIÇÃO DE IMAGENS** — É possível preservar o recorte &lt; &gt; máscaras em imagens e escolher um perfil de cor.
Consulte [Opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **OPÇÕES** DE POSTSCRIPT— É possível rasterizar arquivos postscript®, recortar arquivos, manter fundos transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos postscript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPÇÕES** do PHOTOSHOP— É possível criar modelos a partir de arquivos do Adobe® Photoshop®, manter camadas, especificar como as camadas são nomeadas, extrair texto e especificar como as imagens são ancoradas em modelos.
Consulte [Opções de upload de PSD](psd-files.md#psd_upload_options).

* **OPÇÕES** DE PDF— É possível rasterizar os arquivos, extrair palavras de pesquisa e links, gerar automaticamente um ecatalog, definir a resolução e escolher um espaço de cores.
Consulte [Opções de upload de PDF](pdfs.md#pdf_upload_options).

* **OPÇÕES** do ILLUSTRATOR— É possível rasterizar arquivos do Adobe Illustrator®, manter fundos transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos postscript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPÇÕES** DE EVIDEO— É possível transcodificar um arquivo de vídeo escolhendo uma Predefinição de vídeo.
Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADADOS** ADICIONAIS— Insira palavras-chave que descrevam os arquivos que serão carregados. Separe palavras-chave por vírgula. Palavras-chave facilitam a pesquisa por ativos.
Consulte [Realizar uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

* **PREDEFINIÇÕES** DE CONJUNTO DE LOTE— Se quiser criar um Conjunto de imagens, Conjunto de rotação de vários eixos ou Conjunto de amostras dos arquivos carregados, clique na coluna Ativa da predefinição que deseja usar. Você pode selecionar mais de uma predefinição. Crie as predefinições na página Configurar aplicativo/Definir lote de predefinições.
Consulte [Predefinições de conjunto em lote](application-setup.md#batch_set_presets).

* **ADVANCED** — Consulte [Seguir um upload com outra tarefa](uploading-files.md#follow-an-upload-with-another-job).

## Siga um upload com outra tarefa {#follow-an-upload-with-another-job}

Quando você carrega itens usando FTP, é possível agendar uma tarefa subsequente para que o upload seja concluído. (Se outras tarefas estiverem programadas para começar nesse momento, o trabalho agendado aqui será colocado em fila após eles.)

O novo serviço envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse trabalho de publicação de acompanhamento usa o mesmo nome do trabalho de upload, mas com o texto *Pub_* adicionado ao início.

**Para seguir um upload com outra tarefa**

1. Clique **em Fazer upload** e clique na **guia VIA FTP** .
1. No canto inferior direito da página Carregar, clique em Opções **de trabalho**.
1. Na caixa de diálogo Carregar opções de trabalho, expanda a **seção AVANÇADO** .
1. Escolha um dos seguintes no **Acompanhamento de envio com outra lista** suspensa de tarefas:

   * Nenhum
   * Solicitação HTTP
   * Publicação de imagens
   * Publicação de renderização de imagens
   * Publicação de vídeo

1. Especifique o endereço HTTP.
1. Especifique se você deseja executar somente se os arquivos forem carregados.
1. Indique se deseja executar esta solicitação toda vez que essa tarefa for concluída ou somente quando os arquivos tiverem sido publicados.

   >[!NOTE]
   >
   >Trabalhos agendados regularmente podem não resultar em nenhum arquivo publicado.

>[!MORELIKETHIS]
>
>* [Trabalhar com pastas de ativos](asset-folders.md#working_with_asset_folders)
>* [Manipulação de trabalhos de upload e publicação recorrentes](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Uso de um serviço de upload ou publicação como disparador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

