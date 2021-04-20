---
title: Upload de arquivos
description: Saiba como fazer upload de arquivos.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '3859'
ht-degree: 0%

---


# Upload de arquivos{#uploading-files}

Antes de fazer upload dos arquivos de ativos para o Dynamic Media Classic, verifique se os arquivos de ativos estão nomeados corretamente e se a estrutura de pastas está configurada e organizada da maneira desejada. Você pode fazer upload de arquivos de um site FTP fornecido pelo Dynamic Media Classic ou diretamente de seu computador ou rede. O Dynamic Media Classic oferece opções para otimização de arquivos durante o upload. Se você instalou o aplicativo de desktop Adobe Dynamic Media Classic, é possível fazer upload de arquivos e pastas arrastando-os diretamente da área de trabalho. (Consulte [Configurações Gerais do Aplicativo](application-setup.md#general_settings).)

## Preparação de ativos e pastas para carregar {#preparing-your-assets-and-folders-for-uploading}

Antes de fazer upload dos ativos no Dynamic Media Classic, verifique se eles estão no formato e tamanho corretos. Também é necessário observar as regras do Dynamic Media Classic para nomear ativos. Ao configurar uma organização de pastas e uma estrutura para os arquivos, você pode localizar e trabalhar com arquivos facilmente.

### Formatos de arquivo de ativo compatíveis {#supported-asset-file-formats}

Esta tabela lista os formatos de arquivo de ativo compatíveis com o Dynamic Media Classic. Para obter informações sobre arquivos Camera Raw suportados, consulte [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formatos de arquivo de ativos | Descrição |
|--- |--- |
| Áudio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Folha de estilos em cascata | CSS |
| Perfis de cores | ICC, ICM |
| Fontes | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Imagens | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (somente Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG e Camera Raw |
| PostScript | EPS, PS |
| Criação de imagem do Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vídeo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

O suporte ao upload de TAR e ZIP inclui uma caixa de seleção para selecionar se deseja descompactar os arquivos.

### Formatos de imagem não aceitos no Dynamic Media {#unsupported-image-formats-dynamic-media}

A lista a seguir descreve os subtipos de formatos de arquivo de imagem rasterizada que são *not* suportados no Dynamic Media.

Consulte também [Detectar formatos de arquivo não suportados para Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Arquivos PNG com um tamanho de bloco IDAT superior a 100 MB.
* Arquivos PSB.
* Arquivos PSD com um espaço de cor diferente de CMYK, RGB, Escala de cinza ou Bitmap não são compatíveis. Não há suporte para espaços de cores DuoTone, Lab e Indexado.
* Arquivos PSD com uma profundidade de bits superior a 16.
* Arquivos TIFF com dados de ponto flutuante.
* Arquivos TIFF com espaço de cor Lab.

### Tipos de ativos {#asset-types}

Para obter os melhores resultados com a plataforma Dynamic Media Classic, use os formatos e tamanhos de arquivo recomendados. Esta tabela lista os tipos de ativos, alguns com formatos recomendados e tamanhos de arquivo para ativos usados com frequência.

| Tipo de ativo | Descrição/Recommendations |
|--- |--- |
| Áudio | Os formatos de ativos de áudio de entrada incluem AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Você pode transcodificar o áudio para os seguintes formatos: MP3, AAC e HE-AAC. |
| Imagens (para Dimensionamento de imagem, Zoom, Conjuntos de imagens, Conjuntos de rotação) | As imagens devem ter pelo menos 2000 pixels na dimensão mais longa; os tamanhos de imagem típicos variam de 1500 a 2500 pixels na dimensão mais longa. Recomendamos formatos de imagem sem perdas, incluindo arquivos TIFF e PNG. Se você usar uma imagem JPEG, use as configurações de mais alta qualidade. Os arquivos GIF de animação são manipulados como outro conteúdo estático. |
| Catálogos eletrônicos | Use arquivos PDF de alta resolução criados no Adobe® Acrobat® ou um aplicativo Creative Suite salvo como &quot;pronto para a imprensa&quot;. Os PDFs incluem todas as fontes, imagens, máscaras e elementos gráficos referenciados necessários, como páginas únicas, páginas espelhadas duplas ou em um formato de várias páginas. Ordene suas páginas nomeando os arquivos em ordem alfanumérica. Coloque todos os PDFs do seu eCatalog em uma única pasta para facilitar o upload. Você pode selecionar opções de recorte no upload para remover a área de corte dos PDFs, incluindo marcas de recorte, destinos de registro ou barras de cores. A maioria dos arquivos PDF prontos para impressão está no espaço de cores CMYK, portanto, é importante obter o perfil de cores CMYK ICC usado com seus arquivos PDF. |
| Modelos | Imagem em camadas ou design de layout que pode incluir texto, imagens e camadas. Camadas de imagem, sequências de texto e atributos, como cor e tamanho, podem ser parametrizados para que os dados variáveis possam ser personalizados. Os requisitos de imagem para usar em modelos são os mesmos que outras imagens. Prepare seus gráficos no Photoshop ou em outro programa de edição de imagens. Salve cada gráfico como um arquivo transparente nivelado no formato TIFF ou PNG. Certifique-se de que a resolução da imagem seja apropriada para o uso esperado. As imagens para impressão devem ser de 300 ppi. |
| Vídeos | O Dynamic Media Classic é compatível com arquivos de vídeo salvos no formato OGV e MP4. Você pode transcodificar arquivos para o formato MP4 no upload.Consulte [Formatos de arquivo de ativo compatíveis](#supported-static-file-formats). |
| Fontes | TrueType, Type1 (somente Windows), fontes de OpenType e FontesPhoto carregadas |
| Imagens | Imagens e arquivos de imagem em camadas. |
| Conjuntos de imagens e conjuntos de amostras | Um conjunto de imagens relacionadas que pode ser exibido em um visualizador. |
| Perfis ICC | Um perfil de cores que pode ser usado para converter uma imagem carregada de seu espaço de cores de origem em um espaço de cores diferente. |
| Vinhetas | Imagens criadas com o programa de criação de imagens, bem como arquivos relacionados. |
| Arquivos de conteúdo | Arquivos de conteúdo Adobe InDesign, Illustrator ou Photoshop. |
| Arquivos FXG | Arquivos de formato gráfico independentes de resolução que podem ser usados para criar modelos personalizáveis para saída para impressão, Web, email, desktop e dispositivos. |
| Arquivos SVG | Arquivos gráficos vetoriais dimensionáveis que os servidores de Exibição de imagens podem renderizar. |
| Arquivos XML | Arquivos que definem regras de pré-processamento que são usadas para modificar o caminho e as partes de consulta de solicitações. |
| Arquivos de folha de estilos em cascata. | Fazer upload de capas de CSS para personalização de visualizadores HTML5. |
| Arquivos JavaScript | Os arquivos Javascript são usados para instrumentação do visualizador para conter informações da conta. A Segurança do Adobe recomenda isso somente para contas de clientes que têm um domínio separado em uso para entrega (para evitar scripts entre sites). |

>[!NOTE]
>
>Ao fazer upload de arquivos de imagem e PDFs para o Dynamic Media Classic, o sistema converte esses arquivos de origem em arquivos P-TIFF (Pyramid TIFF). Esses P-TIFFs são os arquivos publicados posteriormente nos Servidores de Imagem da Dynamic Media. O Dynamic Media Classic usa o formato de arquivo Pyramid Tiff , pois contém várias taxas de zoom que permitem o zoom rápido quando visualizado com um Visualizador de Zoom do Dynamic Media Classic.

### Formatos de arquivo estático compatíveis {#supported-static-file-formats}

O Dynamic Media Classic é compatível com vários formatos de arquivo estáticos. O conteúdo estático é qualquer ativo publicado &quot;no estado em que se encontra&quot;, como CSS, PDF, SVG, XML e assim por diante.

Os seguintes tipos de arquivo podem ser publicados:

* GIF animado
* Arquivos de áudio
* CSS
* JavaScript (quando a empresa é configurada com seu próprio domínio)
* Vídeo principal
* PDF (quando o PDF é marcado especificamente para publicação após o upload, para evitar a entrega de todos os PDFs para o fluxo de trabalho eCatalog/PDF existente)
* Vídeo PrX
* SVG
* XML
* ZIP

O Dynamic Media Classic não fornece a opção para gerar um URL de visualização de conteúdo estático.

### Requisitos do nome de arquivo {#filename-requirements}

Como as extensões de nome de arquivo são removidas dos nomes de arquivo durante o processo de upload, o sistema não permite que os arquivos tenham o mesmo nome raiz. No sistema Dynamic Media Classic, o nome do arquivo de ativo menos a extensão do nome do arquivo se torna a ID do ativo para o ativo. Por esse motivo, dois ativos não podem ter o mesmo nome.

Certifique-se de que todos os usuários da empresa entendam essas regras de nomenclatura de arquivos:

* As IDs de ativo com o mesmo nome exato não são permitidas no sistema.
* Os nomes de ID de ativo fazem distinção entre maiúsculas e minúsculas.
* Como prática recomendada, verifique se as IDs de ativo não contêm espaços em branco (por exemplo, jacket.tif e blue jacket.jpg). O ASCII do Dynamic Media Classic codifica espaços em branco em nomes de ativos quando usa nomes de ativos para criar strings de URL. Esses códigos ASCII são difíceis de ler, o que pode dificultar a leitura de URLs.
* Caracteres específicos de idioma são permitidos em nomes de arquivo. No entanto, os seguintes caracteres não são permitidos em nomes de arquivo:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Se um nome de arquivo contiver um ou mais dos caracteres acima, os caracteres serão removidos do nome do arquivo no upload.

Na maioria dos casos, um nome de arquivo de ativo pode ser o mesmo número de item, SKU de produto ou outro nome que no seguinte:

| Item | Nome do arquivo | ID do ativo |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organização e estrutura de pastas {#folder-organization-and-structure}

Organize e estruture pastas e subpastas de seu conteúdo no Dynamic Media Classic antes de fazer upload do seu conteúdo no sistema. O planejamento dessa forma tem duas grandes vantagens:

* Ao carregar seu conteúdo para o Dynamic Media Classic via FTP, você pode dizer ao sistema para replicar sua estrutura de pastas durante o upload. Dessa forma, seu conteúdo é organizado nas mesmas pastas e subpastas do Dynamic Media Classic que está em seu computador ou rede. (Para replicar a estrutura de pastas no Dynamic Media Classic, selecione a opção Incluir subpastas ao fazer upload de ativos via FTP.)
* Reorganizar pastas dentro do sistema depois que os arquivos forem carregados é muito mais difícil do que começar com uma estrutura de pastas cuidadosamente considerada.

A abordagem de nomenclatura de pastas e a estrutura que você escolher para armazenar seu conteúdo no Dynamic Media Classic dependem das necessidades da sua organização. Estas são algumas estruturas de pastas de exemplo:

**As Pastas** baseadas em SKU são nomeadas de acordo com SKUs ou números de item. Por exemplo, pastas separadas são criadas para todas as séries de 0, 20 e 30 números.

**Baseado em marca** Para fabricantes com várias linhas de marca e varejistas que comercializam outras marcas de outras empresas, separe os arquivos em pastas de produto nomeadas para diferentes marcas.

**As Pastas** baseadas em projeto são organizadas de acordo com a data de implantação/soltar ou o nome do projeto. Os clientes que produzem principalmente eCatalogs favorecem essa abordagem.

**Espelhamento da** hierarquia de pastas do siteEssa estrutura de pastas reflete a estrutura de pastas do site, com as pastas nomeadas, por exemplo, para categorias de produtos.

## Sobre o upload de arquivos {#uploading-your-files}

Você pode fazer upload de arquivos individuais da área de trabalho ou fazer upload de pastas via FTP. Se desejar fazer upload de mais de 100 MB de arquivos ou fazer upload de pastas e subpastas inteiras, selecione a guia **VIA FTP**.

O Dynamic Media Classic envia uma mensagem de email para confirmar quando seu trabalho de upload começa e termina, e para notificá-lo de qualquer problema.

Durante (ou imediatamente após) um grande trabalho de upload, alguns novos itens podem exibir a mensagem &quot;Imagem ainda não otimizada&quot;. Essa mensagem é exibida porque os arquivos ainda não foram totalmente processados e adicionados ao Dynamic Media Classic. Você pode otimizar esses arquivos posteriormente. (Consulte [Otimizar arquivos](application-setup.md#optimize_files).)

### Upload de arquivos usando a guia FROM DESKTOP {#upload-files-using-sps-desktop-application}

O aplicativo Dynamic Media Classic Desktop permite fazer upload de arquivos e pastas arrastando.

1. No aplicativo Dynamic Media Classic Desktop, na barra Navegação global, clique em **Fazer upload**.
1. Na página Upload , clique na guia **FROM DESKTOP**.
1. No lado esquerdo da página Upload, na área **Selecionar arquivos para upload**, clique em **Procurar** para selecionar os arquivos ou pastas que deseja carregar e clique em **Abrir**.
1. No lado direito da página Upload, na área **Escolher destino da pasta**, navegue até uma pasta de destino onde deseja adicionar os arquivos ou pastas carregados.
1. (Opcional) Próximo à parte inferior da página Upload, no campo **Nome do trabalho**, especifique o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Trabalhos, onde você pode verificar o status dos trabalhos.
Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Fazer upload , selecione **Publicar após fazer upload** se desejar publicar automaticamente os ativos que você fez upload.
Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .
1. (Opcional) Próximo à parte inferior da página Upload , selecione **Substituir em qualquer pasta, o mesmo nome do ativo base, independentemente da extensão**, se desejar que os arquivos carregados substituam os arquivos existentes com os mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .
O nome dessa opção pode ser diferente, dependendo das configurações em **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. Próximo ao canto inferior direito da página Upload, clique em **Opções de trabalho** e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Opções de trabalho de upload , clique em **Salvar**.
1. No canto inferior direito da página Upload, clique em **Enviar upload**.
Para ver o progresso do upload, clique em **Jobs** na Barra de Navegação Global. Você pode continuar trabalhando no Dynamic Media Classic e retornar à página Trabalhos a qualquer momento para revisar um trabalho em andamento. Para cancelar um trabalho de upload em andamento, selecione **Cancelar** ao lado da Duração.

### Upload de arquivos usando a guia FTP VIA {#upload-files-using-via-ftp}

1. Faça logon no site FTP do Dynamic Media Classic, que é específico para sua região específica. Use o nome de usuário e a senha FTP recebidos do seu administrador.
1. No Dynamic Media Classic, na barra Navegação global, clique em **Fazer upload**.
1. Na página Upload , clique na guia **VIA FTP** .
1. No lado esquerdo da página Upload, na área **Escolher pasta FTP para upload** , escolha uma pasta FTP da qual deseja fazer upload de arquivos.
1. No lado direito da página Upload, na área **Choose Adobe Dynamic Media Folder Destination**, escolha uma pasta de destino no Dynamic Media Classic.
1. (Opcional) Próximo à parte inferior da página Upload, no campo **Nome do trabalho**, especifique o novo nome do trabalho de upload. Ou você pode simplesmente usar o nome padrão gerado pelo sistema fornecido pelo Dynamic Media Classic. O trabalho e outros trabalhos de upload e publicação são registrados na página Trabalhos, onde você pode verificar o status dos trabalhos.
Consulte [Verificando arquivos de trabalho](checking-job-files.md#checking_job_files).
1. (Opcional) Próximo à parte inferior da página Fazer upload , selecione **Publicar após o upload** se desejar publicar automaticamente os ativos que você fez upload.
Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .
1. (Opcional) Próximo à parte inferior da página Upload , selecione **Substituir em qualquer pasta, o mesmo nome do ativo base, independentemente da extensão**, se desejar que os arquivos carregados substituam os arquivos existentes com os mesmos nomes. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .
O nome dessa opção pode ser diferente, dependendo das configurações em **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. (Opcional; disponível somente se você clicou na guia **VIA FTP**) Próximo à parte inferior da página Upload, selecione **Descompactar arquivos Zip ou Tar no Upload** se desejar extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .
1. Próximo ao canto inferior direito da página Upload, clique em **Opções de trabalho** e especifique as opções desejadas.

   Consulte [Opções de upload](uploading-files.md#upload_options).

1. Na caixa de diálogo Opções de trabalho de upload , clique em **Salvar**.
1. No canto inferior direito da página Upload, clique em **Enviar upload**.

   Para ver o progresso do upload, na Barra de Navegação Global, clique em **Trabalhos**. A página Trabalhos mostra o progresso do upload. Você pode continuar trabalhando no Dynamic Media Classic e retornar à página Trabalhos a qualquer momento para revisar um trabalho em andamento.

Para cancelar um trabalho de upload em andamento, clique em **Cancelar** ao lado da Duração.

## Caixa de diálogo Fazer upload de opções de trabalho {#upload-options}

Ao carregar arquivos, você pode escolher entre as seguintes opções na caixa de diálogo Upload Job Options :

* **TRABALHO** — Clique em  **** TRABALHO para escolher opções que afetam todo o trabalho de upload.

   Observe que você também pode escolher as opções *padrão* para fazer upload de tarefas usando a caixa de diálogo **Opções de upload padrão** nas Configurações gerais. Clique em **Configurar > Configuração do aplicativo > Configurações gerais > Opções de upload padrão** e defina as opções padrão desejadas.

   * **Quando** — A  **** opção Quando está disponível somente se você selecionou a guia  **VIA** FTP.
      * **Ocasionalmente**  — especifique um trabalho de upload executado uma vez. As opções incluem:
         * **Agora** — Executa o trabalho de upload imediatamente após clicar em  **** Salvar na caixa de diálogo Opções de trabalho de upload e, em seguida, clique em  **Enviar** upload na página Upload.
         * **Agendar para mais tarde**  — Selecione o ano, mês, dia e hora (em incrementos de 15 minutos) em que deseja que o trabalho de upload seja executado.
      * **Recorrente**  — especifique um trabalho de upload que é executado diariamente, semanalmente ou mensalmente. Ou personalize o trabalho de upload de acordo com suas próprias especificações.
         * **Diariamente** — Defina a hora em que deseja que o trabalho seja executado todos os dias. Se desejar que o trabalho seja executado somente de segunda a sexta-feira, selecione **Somente dias da semana**.
         * **Semanalmente** — Escolha um dia específico da semana e hora em que deseja que a tarefa seja executada.
         * **Mensalmente** — Escolha um dia específico do mês ou dia da semana, incluindo a hora de início, em que deseja que a tarefa seja executada.
         * **Personalizado**  — Personalize um intervalo de tempo de trabalho de upload ou publicação de acordo com suas próprias especificações. Consulte [Criação de um intervalo de tempo de trabalho personalizado de upload ou publicação](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publicar após o upload**  — Disponível se você selecionou  **DA guia** DESKTOP ou  **VIA** FTP4. Selecione essa opção para publicar automaticamente os ativos que você fez upload. Ao publicar arquivos, os arquivos são enviados para servidores dinâmicos. As URLs desses arquivos podem ser usadas em sites e aplicativos externos. Essa opção também está disponível na página Upload .

   * **Substituir em qualquer pasta, o mesmo nome do ativo base independentemente da extensão**  — Disponível se você selecionou  **DA** DESKTOP ou a guia  **VIA** FTP. Selecione essa opção se desejar que os arquivos carregados substituam arquivos existentes com os mesmos nomes. Essa opção também está disponível na página Upload . O nome dessa opção pode ser diferente, dependendo das configurações em **Application Setup > General Settings > Upload to Application > Overwrite Images**.

   * **Descompactar arquivos Zip ou Tar no upload**  — Disponível se você selecionou  **DE** DESKTOP ou a guia  **VIA** FTP.
Selecione essa opção se quiser extrair automaticamente todos os arquivos do arquivo ZIP ou TAR carregado. Observe que essa mesma opção também está disponível na caixa de diálogo Opções de trabalho .

   * **Incluir subpastas**  — Disponível somente se você selecionou a guia  **VIA** FTP.
Selecione essa opção se desejar fazer upload de subpastas da pasta que deseja fazer upload. Os nomes da pasta e suas subpastas que você faz upload são inseridos automaticamente no Dynamic Media Classic.

   * **Processar arquivos de metadados**  — Disponível somente se você selecionou a guia  **VIA** FTP. Selecione essa opção se desejar fazer upload de um arquivo XML ou delimitado por tabulação para adicionar metadados a vários ativos.
Consulte [Importar metadados (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **RECORTAR OPTIONS**  — Para recortar automaticamente pixels de espaço em branco de uma imagem, abra o menu Recortar, escolha Manual e insira medidas de pixel nos campos Superior, Direita, Inferior e Esquerdo para recortar das laterais. Você também pode escolher Aparar no menu Cortar e escolher estas opções:

   * **Aparar com base em**  — Escolha se deseja recortar com base na cor ou na transparência:

      * **Cor** — Escolha a opção Cor. Em seguida, selecione o menu Canto e escolha o canto da imagem com a cor que melhor representa a cor do espaço em branco que deseja recortar.

         Aparar com base na cor: Especifique 0 para cortar pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Os números mais próximos de 1 permitem mais diferenças de cor.

      * **Transparência** — Escolha a opção Transparência.

         Aparar com base na transparência: Especifique 0 para cortar pixels somente se eles forem totalmente transparentes; números mais próximos de 1 permitem mais transparência.

      * **Tolerância**  — Arraste o controle deslizante para especificar uma tolerância de 0 a 1.

* **OPTIONS DE PERFIL DE COR** — Escolha uma conversão de cores ao criar arquivos otimizados usados para a entrega dinâmica do Dynamic Media Classic:

   * **Preservação de cor padrão**  — Mantém as cores da imagem de origem sempre que as imagens contêm informações sobre o espaço de cores; não há conversão de cores. Quase todas as imagens atuais têm o perfil de cores apropriado já incorporado. No entanto, se uma imagem de origem CMYK não contiver um perfil de cor incorporado, as cores serão convertidas em espaço de cor sRGB (azul verde padrão). sRGB é o espaço de cores recomendado para exibir imagens nas páginas da Web.

   * **Manter o espaço**  de cores original — Mantém as cores originais sem qualquer conversão de cores no ponto de assimilação no Dynamic Media Classic. Para imagens sem um perfil de cor incorporado, qualquer conversão de cor necessária para processar solicitações para a imagem é feita usando os perfis de cor padrão, conforme configurado nas configurações de Publicação. Esses perfis de cores podem não estar alinhados com a cor nos arquivos criados com essa opção. Portanto, é recomendável usar a opção Preservação de cor padrão.

   * **Personalizar de > Para**  — Abre menus para que você possa escolher um espaço de cores Converter de e Converter em. Essa opção avançada substitui qualquer informação de cor incorporada no arquivo de origem. Você deve selecionar essa opção somente quando todas as imagens enviadas contiverem dados de perfil de cor incorretos ou ausentes.

* **OPTIONS**  DE EDIÇÃO DE IMAGEM — Você pode preservar as  &lt;> máscaras de recorte em imagens e escolher um perfil de cor.
Consulte [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **POSTSCRIPT OPTIONS**  — Você pode rasterizar arquivos do PostScript®, recortar arquivos, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop OPTIONS**  — Você pode criar modelos a partir de arquivos Adobe® Photoshop®, manter camadas, especificar como as camadas são nomeadas, extrair texto e especificar como as imagens são ancoradas em modelos.
Consulte [Opções de carregamento de PSD](psd-files.md#psd_upload_options).

* **OPTIONS de PDF**  — Você pode rasterizar os arquivos, extrair palavras de pesquisa e links, gerar um eCatalog automaticamente, definir a resolução e escolher um espaço de cores.
Consulte [Opções de upload de PDF](pdfs.md#pdf_upload_options).

* **Illustrator OPTIONS**  — Você pode rasterizar arquivos Adobe Illustrator®, manter planos de fundo transparentes, escolher uma resolução e escolher um espaço de cores.
Consulte [Trabalhar com arquivos PostScript e Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **OPTIONS**  DE VÍDEO — Você pode transcodificar um arquivo de vídeo escolhendo uma Predefinição de vídeo.
Consulte [Trabalhar com predefinições de codificação de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **METADADOS ADICIONAIS** — Insira palavras-chave que descrevem os arquivos que você fará upload. Separe as palavras-chave por vírgula. As palavras-chave facilitam a pesquisa de ativos.
Consulte [Realização de uma pesquisa avançada](searching-assets.md#conducting_an_advanced_search).

* **PREDEFINIÇÕES DO CONJUNTO DE LOTES**  — Se você deseja criar um Conjunto de imagens, um Conjunto de rotação de vários eixos ou um Conjunto de amostras dos arquivos carregados, clique na coluna Ativo da predefinição que deseja usar. Você pode selecionar mais de uma predefinição. Você cria as predefinições na página Configuração do aplicativo/Predefinições do conjunto de lotes .
Consulte [Predefinições do conjunto de lotes](application-setup.md#batch_set_presets).

* **AVANÇADO** — Consulte  [Seguir um upload com outro trabalho](uploading-files.md#follow-an-upload-with-another-job).

## Siga um upload com outro trabalho {#follow-an-upload-with-another-job}

Ao fazer upload de itens usando FTP, você pode agendar um trabalho subsequente para começar assim que o upload for concluído. (Se outras tarefas estiverem programadas para começar nesse momento, a tarefa agendada aqui será colocada em fila depois delas.)

A nova tarefa envia uma notificação para o endereço especificado para que o código nesse local possa ser acionado. Esse trabalho de publicação de seguimento usa o mesmo nome do trabalho de upload, mas com o texto *Pub_* adicionado ao início.

**Seguir um upload com outro trabalho**

1. Clique em **Upload** e depois clique na guia **VIA FTP**.
1. No canto inferior direito da página Upload, clique em **Opções de trabalho**.
1. Na caixa de diálogo Upload Job Options , expanda a seção **ADVANCED**.
1. Escolha uma das opções a seguir na lista suspensa **Seguir upload com outro trabalho** :

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
   >Trabalhos agendados regularmente podem não resultar na publicação de arquivos.

>[!MORELIKETHIS]
>
>* [Trabalhar com pastas de ativos](asset-folders.md#working_with_asset_folders)
>* [Lidar com trabalhos recorrentes de upload e publicação](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Usar um trabalho de upload ou publicação como acionador](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

