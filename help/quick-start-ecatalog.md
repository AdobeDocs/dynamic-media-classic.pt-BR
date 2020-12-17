---
title: '"Start rápido: eCatalogs"'
seo-title: '"Start rápido: eCatalogs"'
description: nulo
seo-description: Uma introdução e um Start rápido para o eCatalog para ajudá-lo a começar a usar rapidamente as técnicas do eCatalog.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: 83b88623b898fdadd1b334b1c12901830c831c5c
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---


# Start rápido: eCatalogs{#quick-start-ecatalogs}

Um eCatalog é uma versão digital da Web de material impresso — catálogo, folheto, folheto, manual do produto ou circular de publicidade, por exemplo. Um eCatalog é exibido em um eCatalog Viewer em um site. Este visualizador simula a experiência de leitura de material impresso. Dependendo das configurações escolhidas para seu eCatalog, o visualizador pode permitir o seguinte:

* Procure no catálogo uma palavra-chave ou palavras-chave. Os resultados da pesquisa são exibidos como uma lista de miniaturas em um painel de pesquisa no lado esquerdo do catálogo. Cada miniatura clicável representa uma propagação de catálogo em que o termo de pesquisa destacado foi encontrado.

* Compartilhar o catálogo por meio de redes sociais; fazer download do catálogo para a visualização offline; habilite os Favoritos para marcar os itens para os quais deseja retornar rapidamente ou imprima o catálogo.
* Navegue pelo catálogo usando o sumário ou a visualização de grade da página; para frente ou para trás, clicando na borda média de uma página.
* Aumenta o zoom, diminui o zoom e desloca para examinar itens em uma página.
* Mova o ponteiro sobre uma região da página (chamada de Mapa de imagem) para ver uma janela pop-up com informações sobre um item.
* Clique em uma região de página para abrir uma nova página da Web com mais informações sobre um item.
* Escreva uma nota adesiva e anexe-a a uma página do eCatalog.
* Toque nos ícones do mapa de imagens para iniciar páginas da Web relacionadas ou painéis de informações no contexto.
* Use interações de gesto, incluindo apertar para aplicar zoom e deslizar para girar as páginas.
* Pesquise por palavra-chave por itens.

![O eCatalog, como ele parece para os usuários. A) Página de abertura do eCatalog. B)Catálogo virado para a página 2.](/help/assets/ec_cat_viewer_popup.png)

Para criar um eCatalog, você geralmente usa arquivos PDF de alta resolução criados no Adobe® Acrobat® ou em outro programa de impressão, mas também pode criar um eCatalog a partir de arquivos de imagem.

Como parte da criação do seu eCatalog, você pode organizar páginas ou páginas espelhadas na ordem escolhida. Você também pode declarar se deseja páginas únicas, páginas espelhadas de duplo ou páginas espelhadas múltiplas. Você pode criar Mapas de imagem para regiões de página para que os visualizadores possam, por exemplo, clicar em uma área na página e abrir uma nova página em seu site. Você pode gerenciar o texto de sobreposição que aparece usando as configurações do InfoPanel na tela eCatalog. Você também pode configurar o eCatalog Viewer escolhendo entre mais de 100 opções de configuração diferentes. Você pode adaptar os recursos e a aparência do seu visualizador para sua audiência específica.

>[!NOTE]
>
>Se você for um usuário AEM Dynamic Media - no modo Scene7 e quiser usar o eCatalog, precisará editar o valor `pdfbrochure` no CRXDE Lite. Para fazer isso, em AEM, clique em **[!UICONTROL Tools > General > CRXDE Lite]**. Na árvore de navegação do painel esquerdo, navegue até `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>No painel inferior direito, na guia **[!UICONTROL Properties]**, selecione a linha `jobParam`. Defina o valor para `pdfbrochure` de `false` para `true`. Como em `pdfbrochure=true`
>
>No canto superior esquerdo da página CRXDE Lite, clique em **[!UICONTROL Save All]**.
>
>Agora você poderá criar eCatalogs no Dynamic Media Classic.

**Start rápido**

Este Start rápido do eCatalog foi projetado para ajudá-lo a começar a funcionar rapidamente com eCatalogs. Siga as etapas de 1 a 7. Depois de cada etapa é uma referência cruzada para um cabeçalho de tópico no qual você pode encontrar mais informações.

**1. Fazer upload dos arquivos PDF**

Os arquivos Adobe PDF geralmente são a fonte de um eCatalog. Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. O Dynamic Media Classic detecta essas imagens e as converte usando um perfil de cores CMYK padrão. No entanto, talvez seja necessário carregar e usar um perfil de cores personalizado.

Clique em Fazer upload na barra de navegação global para fazer upload de start de arquivos PDF ou imagens para seu eCatalog. Você pode fazer upload de arquivos do seu desktop ou via FTP; O FTP é recomendado se você estiver carregando vários arquivos ou arquivos com mais de 100 MB.

Em Opções de PDF, a tela Carregar fornece opções para carregar arquivos PDF na resolução correta e no espaço de cor correto. Recomenda-se uma resolução de 150 pixels por polegada. Você pode selecionar a opção Gerar eCatalog automaticamente para criar um eCatalog ao carregar um arquivo PDF.

Consulte [Carregar os arquivos PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Criação de um eCatalog**

Crie seu eCatalog selecionando arquivos PDF ou de imagem no painel Procurar e, em seguida, clicando no botão Criar e escolhendo eCatalogs. A tela eCatalog (Catálogo eletrônico) é aberta.

Na guia Páginas do pedido, selecione um botão Layout - 1 Para cima, 2 Para cima ou Personalizado - para escolher se deseja páginas espelhadas únicas, de duplo ou personalizadas. É possível reorganizar páginas ou páginas espelhadas arrastando-as ou, em um eCatalog grande, escolhendo um nome de página no menu Mover para.

Para adicionar páginas, selecione uma pasta na Biblioteca de ativos e arraste os arquivos PDF ou de imagem para a tela Páginas de pedidos. Em vez de números de página padrão, você pode fornecer nomes de página personalizados ou importar um grande número de nomes de página.

Clique em **[!UICONTROL Save]**, digite um nome para seu eCatalog, escolha uma pasta do Dynamic Media Classic para armazená-lo e clique em **[!UICONTROL Save]**. Sempre que alterar a ordem de página ou editar seu eCatalog, salve suas alterações clicando em **[!UICONTROL Save]**.

Consulte [Criação de um eCatalog](creating-ecatalog.md).

**3. Criação de mapas de imagem**

Os mapas de imagem adicionam outra dimensão às páginas do eCatalog. Um Mapa de imagem é uma região em uma página que fornece mais informações sobre um item. Quando os visualizadores posicionam o ponteiro sobre um Mapa de imagem, eles veem uma descrição do item. Clicar em um Mapa de imagem ativa uma referência externa que abre uma nova página da Web na qual você pode saber mais sobre um item.

Para criar um Mapa de imagem, abra a tela eCatalog. Em seguida, vá até a guia **[!UICONTROL Map Pages]** da tela eCatalog e desenhe o mapa com a ferramenta Retângulo Image Map ou Polygon Image Map. É possível ajustar a posição e o tamanho dos Mapas de imagem arrastando as bordas do mapa com a ferramenta Deslocamento.

Depois de desenhar o Mapa de imagem, insira o endereço de URL para o qual você deseja ir ao clicar no Mapa de imagem. Você também pode inserir o texto de sobreposição que aparece ao mover o ponteiro sobre o Mapa de imagem.

Consulte [Criação de mapas de imagem do eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Usar mapas de imagem para incorporar mídia avançada em um eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Você pode configurar e gerenciar o texto do mapa de imagem usando as configurações do Painel de informações na tela eCatalog.

Consulte [Gerenciamento do conteúdo do Painel de informações](info-panel-content.md#managing-info-panel-content).

**4. Configuração das predefinições do visualizador do eCatalog**

Os usuários finais veem seu eCatalog no eCatalog Viewer. Se você for um administrador, poderá configurar o eCatalog Viewer. Você pode alterar a cor do contorno e selecionar uma nova &quot;capa&quot; para marcar seu eCatalog. O Dynamic Media Classic vem com várias &quot;práticas recomendadas&quot; predefinições do visualizador de eCatalog. Você pode escolher uma dessas predefinições para exibir seus eCatalogs. Você também pode criar uma predefinição do visualizador do eCatalog se você for um administrador.

Para criar uma predefinição de visualizador de eCatalog, na barra Navegação global, clique em **[!UICONTROL Setup]** e escolha **[!UICONTROL Viewer Presets]**. Em seguida, clique em **[!UICONTROL Add]**, escolha uma plataforma e clique em **[!UICONTROL eCatalog > Viewer]**.

Consulte [Configuração das predefinições do visualizador do eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Visualização de eCatalogs no Visualizador de eCatalog**

As predefinições do visualizador do eCatalog determinam o estilo e o comportamento dos visualizadores do eCatalog.

Para descobrir como as predefinições do visualizador do eCatalog exibem seu eCatalog, selecione seu eCatalog no painel Procurar e clique em **[!UICONTROL Preview]**. A tela Pré-visualização é aberta no visualizador padrão.

Observe a orientação, o esquema de cores, a aparência dos controles para páginas alteradas e a aparência das páginas quando elas são giradas.

Consulte [Visualizar eCatalogs no Visualizador de eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publicar eCatalog e PDFs associados**

A publicação do seu eCatalog e do PDF associado coloca-o em servidores de imagem Dynamic Media para que possa ser entregue ao seu site e aplicativo. Como parte do processo de publicação, o Dynamic Media Classic ativa a string de URL para seu eCatalog. Use este URL para chamar o eCatalog dos Servidores de Imagens Dynamic Media para seu site ou aplicativo.

Depois de marcar seu eCatalog e PDF para publicação no Painel de navegação, selecione o botão Publicar na barra de navegação global para iniciar uma publicação. Na tela Publicar, clique em **[!UICONTROL Start Publish]**.

Consulte [Publicar eCatalogs e PDFs associados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Vincular um eCatalog a uma página da Web**

O Dynamic Media Classic ativa a string de chamada de URL necessária para exibir seu eCatalog quando você o publica em Dynamic Media Image Servers. É possível copiar essa string de URL da tela de Pré-visualização e do Painel de navegação (em visualização detalhada) selecionando URLs no painel. Depois de copiar a string do URL, ela fica disponível para seus sites e aplicativos.

Entre em contato com sua equipe de TI para colocar o link para o eCatalog no local apropriado em sua página da Web. Quando os usuários clicam no link, o eCatalog Viewer é exibido e os usuários podem navegar pelo seu eCatalog.

Consulte [Vincular um eCatalog a uma página da Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
