---
title: '"Início rápido: Catálogos eletrônicos"'
description: Uma introdução e o início rápido dos catálogos eletrônicos para ajudá-lo a ativar e executar rapidamente com as técnicas do catálogo eletrônico no Adobe Dynamic Media Classic.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1529'
ht-degree: 0%

---

# Início rápido: Catálogos eletrônicos{#quick-start-ecatalogs}

Um eCatalog é uma versão digital da Web de material impresso — catálogo, brochura, panfleto, manual do produto ou circular de publicidade, por exemplo. Um eCatalog é exibido em um eCatalog Viewer em um site. Esse visualizador simula a experiência de ler material impresso.

Veja também os seguintes vídeos de treinamento:

* [Início rápido 1: Catálogos eletrônicos](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Início rápido 2: Catálogos eletrônicos](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Dependendo das configurações escolhidas para seu eCatalog, o visualizador pode permitir que você faça o seguinte:

* Pesquise no catálogo uma palavra-chave ou palavras-chave. Os resultados da pesquisa são exibidos como uma lista de miniaturas em um painel de pesquisa no lado esquerdo do catálogo. Cada miniatura clicável representa uma propagação de catálogo onde o termo de pesquisa destacado foi encontrado.

* Compartilhar o catálogo por meio de redes sociais; baixe o catálogo para visualizar offline; ative Favoritos para marcar itens para os quais deseja retornar rapidamente ou imprima o catálogo.
* Navegar pelo catálogo usando o índice ou a exibição de grade da página; página para frente ou para trás clicando na borda média de uma página.
* Amplie, diminua o zoom e desloque para examinar os itens em uma página.
* Mova o ponteiro sobre uma região da página (chamada de Mapa de imagem) para que você possa ver uma janela pop-up com informações sobre um item.
* Selecione uma região de página para que ela abra uma nova página da Web com mais informações sobre um item.
* Escreva uma nota autoadesiva e anexe-a a uma página eCatalog.
* Toque em ícones do mapa de imagem se desejar iniciar páginas da Web relacionadas ou painéis de informações de contexto.
* Use interações de gesto, incluindo os pincéis para aplicar zoom e deslizar para girar as páginas.
* Pesquisar por palavra-chave por itens.

![O eCatalog como ele aparece para os usuários. A) Página de abertura do eCatalog. B)Catálogo eletrônico transformado na página 2.](/help/assets/ec_cat_viewer_popup.png)

Para criar um eCatalog, você normalmente usa arquivos PDF de alta resolução criados no Adobe® Acrobat® ou em outro programa de impressão, mas também pode criar um eCatalog a partir de arquivos de imagem.

Como parte da criação do seu eCatalog, você pode organizar páginas ou páginas espelhadas na ordem escolhida. Você também pode declarar se deseja páginas únicas, páginas espelhadas duplas ou páginas espelhadas. Você pode criar Mapas de imagem para regiões de página, de modo que os visualizadores possam, por exemplo, selecionar uma área na página e abrir uma nova página em seu site. Você pode gerenciar o texto de sobreposição que aparece usando as configurações do InfoPanel na tela eCatalog. Você também pode configurar o Visualizador de catálogo eletrônico escolhendo entre mais de 100 opções de configuração diferentes. Você pode adaptar os recursos e a aparência de seu visualizador para seu público-alvo específico.

>[!NOTE]
>
>Se você for um usuário do modo Dynamic Media - Scene7 e quiser usar eCatalogs, edite o valor `pdfbrochure` no CRXDE Lite. Para fazer isso, no Adobe Experience Manager, vá para **[!UICONTROL Tools]** > **[!UICONTROL General]** > **[!UICONTROL CRXDE Lite]**. Na árvore de navegação do painel esquerdo, navegue até `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>No painel inferior direito, na guia **[!UICONTROL Properties]**, selecione a linha `jobParam`. Defina o valor de `pdfbrochure` de `false` para `true`. Como em `pdfbrochure=true`
>
>No canto superior esquerdo da página CRXDE Lite, selecione **[!UICONTROL Save All]**.
>
>Agora é possível criar eCatalogs no Adobe Dynamic Media Classic.

Este eCatalog Quick Start foi projetado para ajudar você a ativar e executar rapidamente com eCatalogs. Siga as etapas de 1 a 7. Após cada etapa é uma referência cruzada a um cabeçalho de tópico, onde você pode encontrar mais informações.

## 1. Faça upload dos arquivos PDF

Os arquivos Adobe PDF geralmente são a origem de um eCatalog. Como devem ser impressos, os arquivos PDF geralmente contêm imagens CMYK. O Adobe Dynamic Media Classic detecta essas imagens e as converte usando um perfil de cor CMYK padrão. No entanto, você deve carregar e usar um perfil de cor personalizado.

Na barra Navegação global, selecione **[!UICONTROL Upload]** para iniciar o upload de arquivos PDF ou imagens para seu eCatalog. Você pode fazer upload de arquivos do desktop ou via FTP; O FTP é recomendado se você estiver carregando muitos arquivos ou arquivos com mais de 100 MB.

Em Opções de PDF, a tela Upload fornece opções para carregar arquivos PDF na resolução correta e o espaço de cores correto. Recomenda-se uma resolução de 150 pixels por polegada. Você pode selecionar a opção Gerar catálogo eletrônico automaticamente para criar um catálogo eletrônico ao carregar um arquivo de PDF.

Consulte [Fazer upload dos arquivos PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Criar um eCatalog

Crie seu eCatalog selecionando PDF ou arquivos de imagem no painel Procurar. Selecione **[!UICONTROL Build]** e escolha **[!UICONTROL eCatalogs]**.

Na página Catálogo eletrônico , na guia **[!UICONTROL Order Pages]** , selecione uma opção de Layout : **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** ou **[!UICONTROL Custom]**. Você pode reorganizar páginas ou páginas espelhadas arrastando-as ou, em um eCatalog grande, escolhendo um nome de página no menu Mover para.

Para adicionar páginas, selecione uma pasta na Biblioteca de ativos e arraste PDF ou arquivos de imagem para a tela Páginas de pedidos. Em vez dos números de página padrão, você pode fornecer nomes de página personalizados ou importar muitos nomes de página.

Selecione **[!UICONTROL Save]**, insira um nome para seu eCatalog, escolha uma pasta do Adobe Dynamic Media Classic para armazená-lo e selecione **[!UICONTROL Save]**. Sempre que alterar a ordem da página ou editar seu eCatalog, salve as alterações clicando em **[!UICONTROL Save]**.

Consulte [Criar um eCatalog](creating-ecatalog.md).

## 3. Criar mapas de imagem

Os mapas de imagem adicionam outro aspecto às páginas de catálogo eletrônico. Um Mapa de imagem é uma região em uma página que fornece mais informações sobre um item. Quando os visualizadores passam o ponteiro sobre um Mapa de imagem, eles veem uma descrição do item. Clicar em um Mapa de imagem ativa uma referência externa que abre uma nova página da Web, onde você pode saber mais sobre um item.

Para criar um Mapa de imagem, abra a tela Catálogo eletrônico . Em seguida, vá para a guia **[!UICONTROL Map Pages]** da tela eCatalog e enquadre o mapa com a ferramenta Mapa de imagem do retângulo ou ferramenta Mapa de imagem do polígono. É possível ajustar a posição e o tamanho dos mapas de imagem arrastando as bordas do mapa com a ferramenta Deslocar.

Depois de enquadrar o Mapa de imagem, insira o endereço de URL para o qual você deseja ir ao selecionar o Mapa de imagem. Você também pode inserir o texto sobreposto que aparece quando você move o ponteiro sobre o Mapa de imagem.

Consulte [Criar mapas de imagem do catálogo eletrônico](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Consulte [Usar mapas de imagem para incorporar mídia avançada em um eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Você pode configurar e gerenciar o texto do mapa de imagem usando as configurações do Painel de informações na tela eCatalog.

Consulte [Gerenciar conteúdo do painel de informações em Catálogos eletrônicos](/help/info-panel-content-ecatalog.md).

## 4. Configurar predefinições do visualizador de catálogo eletrônico

Os usuários finais visualizam seu eCatalog no Visualizador do eCatalog. Se você for um administrador, poderá configurar o eCatalog Viewer. Você pode alterar a cor do contorno e selecionar uma nova &quot;capa&quot; para marcar seu eCatalog. O Adobe Dynamic Media Classic vem com várias Predefinições de visualizador de catálogo eletrônico de &quot;práticas recomendadas&quot;. Você pode escolher uma dessas predefinições para exibir seus eCatalogs. Você também pode criar uma predefinição do visualizador do eCatalog própria se você for um administrador.

Para criar uma Predefinição do Visualizador de Catálogo Eletrônico, na barra Navegação Global, selecione **[!UICONTROL Setup]** e escolha **[!UICONTROL Viewer Presets]**. Selecione **[!UICONTROL Add]**, escolha uma plataforma e selecione **[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]**.

Consulte [Configurar predefinições do visualizador do catálogo eletrônico](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Visualizar eCatalogs no Visualizador de Catálogo Eletrônico

As Predefinições do visualizador de catálogo eletrônico determinam o estilo e o comportamento dos visualizadores de catálogo eletrônico.

Para descobrir como as Predefinições do visualizador de eCatalog exibem seu eCatalog, selecione seu eCatalog no painel Procurar e selecione **[!UICONTROL Preview]**. A tela Visualização é aberta no visualizador padrão.

Observe a orientação, o esquema de cores, a aparência dos controles para alteração de páginas e a aparência das páginas quando elas são giradas.

Consulte [Visualizar eCatalogs no Visualizador de eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publicar eCatalog e PDF associados

Publicar seu eCatalog e o PDF associado o coloca em Servidores de Imagem Dynamic Media para que ele possa ser entregue ao seu site e aplicativo. Como parte do processo de publicação, o Adobe Dynamic Media Classic ativa a string do URL para seu eCatalog. Use este URL para chamar o eCatalog dos Servidores de Imagem da Dynamic Media para seu site ou aplicativo.

Depois de marcar seu eCatalog e o PDF para publicação no Painel de navegação, selecione o botão Publicar na barra de navegação global para iniciar uma publicação. Na tela Publicar , selecione **[!UICONTROL Submit Publish]**.

Consulte [Publicar catálogos eletrônicos e PDF associados](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Vincular um eCatalog a uma página da Web

O Adobe Dynamic Media Classic ativa a string de chamada de URL necessária para exibir seu eCatalog quando você o publica nos Dynamic Media Image Servers. Você pode copiar essa cadeia de caracteres do URL da tela Visualização e do Painel de navegação (na Exibição de detalhes) selecionando URLs no painel. Após copiar a string do URL, ele fica disponível para seus sites e aplicativos.

Trabalhe com sua equipe de TI para colocar o link para o eCatalog no local apropriado em sua página da Web. Quando os usuários selecionam o link, o Visualizador de catálogo eletrônico é exibido e os usuários podem navegar pelo seu eCatalog.

Consulte [Vincular um eCatalog a uma página da Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
