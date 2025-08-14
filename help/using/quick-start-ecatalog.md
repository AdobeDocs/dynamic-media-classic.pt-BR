---
title: 'Início rápido: eCatalogs'
description: Uma introdução e o Início rápido dos eCatalogs para ajudar você a começar a usar rapidamente as técnicas de eCatalog no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Início rápido: eCatalogs{#quick-start-ecatalogs}

Um eCatalog é uma versão digital da Web de material impresso — um catálogo, folheto, panfleto, manual de produto ou circular de publicidade, por exemplo. Um eCatalog é exibido em um eCatalog Viewer em um site da Web. Este visualizador simula a experiência de leitura de material impresso.

Consulte também os seguintes vídeos de treinamento:

* [Início rápido 1: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Início rápido 2: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Dependendo das configurações escolhidas para o seu eCatalog, o visualizador pode permitir que você faça o seguinte:

* Pesquise no catálogo por uma ou mais palavras-chave. Os resultados da pesquisa são exibidos como uma lista de miniaturas em um painel de pesquisa no lado esquerdo do catálogo. Cada miniatura clicável representa uma página espelhada no catálogo em que o termo de pesquisa destacado foi encontrado.

* Compartilhe o catálogo por meio de redes sociais; baixe o catálogo para exibi-lo offline; habilite os Favoritos para marcar os itens que deseja retornar rapidamente ou imprima o catálogo.
* Navegue pelo catálogo usando o índice ou a exibição de grade da página; avançar ou retroceder página selecionando a borda intermediária de uma página.
* Amplie, reduza e desloque para examinar os itens em uma página.
* Mova o ponteiro sobre uma região da página (chamada de Mapa de imagem) para que você possa ver uma janela pop-up com informações sobre um item.
* Selecione uma região de página para que ela abra uma nova página da Web com mais informações sobre um item.
* Escreva uma nota adesiva e anexe-a a uma página de eCatalog.
* Toque nos ícones do Mapa de imagem se desejar iniciar páginas da Web relacionadas ou painéis de informações no contexto.
* Use interações de gestos, incluindo pinçar para aplicar zoom e deslizar o dedo para virar as páginas.
* Procurar itens por palavra-chave.

![O eCatalog como ele aparece para os usuários. A) Página de abertura do eCatalog. B)eCatalog ativado para página 2.](/help/using/assets/ec_cat_viewer_popup.png)

Para criar um eCatalog, você geralmente usa arquivos PDF de alta resolução criados no Adobe Acrobat ou outro programa de impressão, mas também pode criar um eCatalog a partir de arquivos de imagem.

Como parte da criação do eCatalog, você pode organizar as páginas ou páginas espelhadas na ordem escolhida. Você também pode declarar se deseja páginas únicas, páginas duplas ou páginas múltiplas. Você pode criar Mapas de imagem para regiões da página para que os visualizadores possam, por exemplo, selecionar uma área na página e abrir uma nova página no seu site. Você pode gerenciar o texto de sobreposição exibido usando as configurações do InfoPanel na tela do eCatalog. Você também pode configurar o eCatalog Viewer escolhendo entre mais de 100 opções de configuração diferentes. Você pode adaptar os recursos e a aparência do seu Visualizador para o seu público em particular.

>[!NOTE]
>
>Se você for um usuário do modo Dynamic Media: Scene7 e quiser usar eCatalogs, edite o valor `pdfbrochure` no CRXDE Lite. Para fazer isso, no Adobe Experience Manager, vá para **[!UICONTROL Tools]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. Na árvore de navegação do painel esquerdo, navegue até `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>No painel inferior direito, na guia **[!UICONTROL Properties]**, selecione a linha `jobParam`. Defina o valor de `pdfbrochure` de `false` para `true`. Como em `pdfbrochure=true`
>
>No canto superior esquerdo da página do CRXDE Lite, selecione **[!UICONTROL Save All]**.
>
>Agora é possível criar eCatalogs no Adobe Dynamic Media Classic.

Este Início rápido do eCatalog foi projetado para ajudá-lo a começar a trabalhar rapidamente com eCatalogs. Siga as etapas de 1 a 7. Após cada etapa, há uma referência cruzada a um cabeçalho de tópico onde você pode encontrar mais informações.

## &#x200B;1. Faça upload dos arquivos do PDF

Os arquivos do Adobe PDF geralmente são a origem de um eCatalog. Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. O Adobe Dynamic Media Classic detecta essas imagens e as converte usando um perfil de cores CMYK padrão. No entanto, você deve carregar e usar um perfil de cores personalizado.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para começar a carregar arquivos ou imagens do PDF para seu eCatalog. Você pode fazer upload de arquivos do seu desktop ou por meio do FTP. O FTP é recomendado se você estiver fazendo upload de muitos arquivos ou de arquivos com mais de 100 MB.

Em Opções do PDF, a tela Fazer upload fornece opções para fazer upload de arquivos PDF com a resolução e o espaço de cores corretos. Recomenda-se uma resolução de 150 pixels por polegada. Você pode selecionar a opção **[!UICONTROL Auto-Generate eCatalog]** para criar um eCatalog ao carregar um arquivo do PDF.

Consulte [Carregar os arquivos do PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## &#x200B;2. Criar um eCatalog

Crie seu eCatalog selecionando PDF ou arquivos de imagem no painel Procurar. Selecione **[!UICONTROL Build]** e escolha **[!UICONTROL eCatalogs]**.

Na página de eCatalog, na guia **[!UICONTROL Order Pages]**, selecione uma opção de Layout: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]**, ou **[!UICONTROL Custom]**. É possível reorganizar páginas ou páginas espelhadas arrastando-as ou, em um eCatalog grande, escolhendo um nome de página no menu Mover para.

Para adicionar páginas, selecione uma pasta na Biblioteca de ativos e arraste arquivos PDF ou de imagem da tela Ordenar páginas. Em vez de números de página padrão, você pode fornecer nomes de página personalizados ou importar muitos nomes de página.

Selecione **[!UICONTROL Save]**, insira um nome para o seu eCatalog, escolha uma pasta do Adobe Dynamic Media Classic para armazená-lo e selecione **[!UICONTROL Save]**. Sempre que você alterar a ordem de paginação ou editar seu eCatalog, salve suas alterações selecionando **[!UICONTROL Save]**.

Consulte [Criar um eCatalog](creating-ecatalog.md).

## &#x200B;3. Criar mapas de imagem

Os mapas de imagem adicionam outro aspecto às páginas do eCatalog. Um Mapa de imagem é uma região de uma página que fornece mais informações sobre um item. Quando os visualizadores rolam o ponteiro sobre um Mapa de imagem, eles veem uma descrição do item. Clicar em um Mapa de imagem ativa uma referência externa que abre uma nova página da Web onde você pode saber mais sobre um item.

Para criar um Mapa de imagem, abra a tela eCatalog. Em seguida, vá para a guia **[!UICONTROL Map Pages]** da tela eCatalog e enquadre o mapa com a ferramenta Mapa de imagem retangular ou Mapa de imagem de polígono. É possível ajustar a posição e o tamanho dos Mapas de imagem arrastando as bordas do mapa com a ferramenta Deslocar.

Depois de enquadrar o Mapa de imagem, insira o endereço do URL para o qual deseja ir ao selecionar o Mapa de imagem. Também é possível inserir o texto de sobreposição exibido ao mover o ponteiro sobre o Mapa de imagem.

Consulte [Criar Mapas de Imagens de eCatalog](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Usar Mapas de Imagens para inserir mídia avançada em um eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Você pode configurar e gerenciar o texto do Mapa de imagem usando as configurações do Painel de informações na tela eCatalog.

Consulte [Gerenciar conteúdo do Painel de Informações em eCatalogs](/help/using/info-panel-content-ecatalog.md).

## &#x200B;4. Configurar Predefinições do Visualizador de eCatalog

Os usuários finais veem seu eCatalog no eCatalog Viewer. Se você for um administrador, poderá configurar o eCatalog Viewer. É possível alterar a cor do contorno e selecionar uma nova &quot;capa&quot; para marcar seu eCatalog. O Adobe Dynamic Media Classic vem com várias predefinições de visualizador do eCatalog de &quot;práticas recomendadas&quot;. Você pode escolher uma dessas predefinições para exibir seus eCatalogs. Você também pode criar sua própria Predefinição do visualizador do eCatalog se for um administrador.

Para criar uma Predefinição do Visualizador de eCatalog, na barra de Navegação Global, selecione **[!UICONTROL Setup]** e escolha **[!UICONTROL Viewer Presets]**. Selecione **[!UICONTROL Add]**, escolha uma plataforma e selecione **[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]**.

Consulte [Configurar Predefinições do Visualizador de eCatalog](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## &#x200B;5. Visualizar eCatalogs no Visualizador de eCatalog

As Predefinições do visualizador de eCatalog determinam o estilo e o comportamento dos visualizadores de eCatalog.

Para descobrir como as Predefinições do Visualizador de eCatalog exibem seu eCatalog, selecione seu eCatalog no painel Procurar e, em seguida, selecione **[!UICONTROL Preview]**. A tela Preview é aberta no visualizador padrão.

Observe a orientação, o esquema de cores, a aparência dos controles para alterar as páginas e a aparência das páginas quando elas são viradas.

Consulte [Visualizar eCatalogs no eCatalog Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## &#x200B;6. Publicar eCatalog e PDFs associados

A publicação do eCatalog e do PDF associado o coloca nos servidores de imagem do Dynamic Media para que ele possa ser entregue ao seu site e aplicativo. Como parte do processo de publicação, o Adobe Dynamic Media Classic ativa a cadeia de caracteres de URL do seu eCatalog. Use esse URL para chamar o eCatalog dos servidores de imagem do Dynamic Media para o seu site ou aplicativo.

Depois de marcar seu eCatalog e o PDF para publicação no painel Procurar, selecione o botão Publicar na barra Navegação global para iniciar uma publicação. Na página Publicação, selecione **[!UICONTROL Submit Publish]**.

Consulte [Publicar eCatalogs e PDFs associados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## &#x200B;7. Vincular um eCatalog a uma página da Web

O Adobe Dynamic Media Classic ativa a string de chamada de URL necessária para exibir seu eCatalog quando você o publica em Servidores de imagem do Dynamic Media. Você pode copiar essa cadeia de caracteres de URL na tela Visualização e no painel Procurar (na Exibição de detalhes) selecionando URLs no painel. Depois de copiar a cadeia de caracteres do URL, ela fica disponível para seus sites e aplicativos.

Trabalhe com sua equipe de TI para colocar o link para o eCatalog no local apropriado em sua página da Web. Quando os usuários selecionam o link, o eCatalog Viewer é exibido e os usuários podem navegar pelo seu eCatalog.

Consulte [Vincular um eCatalog a uma página da Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
