---
title: Exportar ativos do sistema de publicação Scene 7
seo-title: Exportar ativos do sistema de publicação Scene 7
description: 'null'
seo-description: Saiba como exportar ativos do Scene 7 Publishing System.
uuid: d 42 b 7 a 73-80 c 0-4 a 9 a-a 04 e -7 ef 53 e 6 fcf 22
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/managing_ assets
discoiquuid: eb 850 ec 7-a 669-41 ea-b 2 b 0-4 c 9178 e 34 f 95
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Exportar ativos do sistema de publicação Scene 7{#exporting-assets-from-scene-publishing-system}

Você pode salvar ativos editados no Scene 7 Publishing System em uma unidade de rede local. Os ativos exportados são agrupados em um arquivo ZIP para download ou envio por e-mail.

O arquivo Zip compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação. Além disso, esteja ciente de que você recebe um máximo de 500 ativos por trabalho de exportação.

O Dynamic Media Classic mantém um registro de trabalhos de exportação na tela Tarefas.

**Para exportar ativos do sistema de publicação Scene 7**

1. Selecione os ativos que deseja exportar e clique **em Arquivo** &gt; **Exportar**.
1. Na janela Exportar ativos selecionados, clique **em Opções de imagem** e especifique qualquer uma das opções a seguir (os administradores determinam quais opções estão disponíveis para seus usuários):

   **Predefinições** Opcionalmente, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma Predefinição de imagem, as outras opções de formatação não estarão disponíveis, já que o ativo adota os formatos definidos pela Predefinição de imagem.

   **Conversão** Converta o arquivo de ativo ou a imagem original.

   **Tamanho É** possível selecionar um tamanho padrão. Ou, você pode clicar em Outros na lista suspensa Tamanho, escolher a unidade de medida desejada e especificar a largura e a altura.

   Consulte [também Especificação das opções de exportação disponíveis para usuários](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)do Media Portal.

   **Formato** Escolha um formato de imagem.

   **Cor** Escolha RGB, CMYK ou Cinza.

   **Resolução** Escolha 72, 150 ou 300 ppi.

   **Nome do serviço** Você pode atribuir um nome de serviço à exportação.

   **Enviar e-mail para** selecionar como opção, insira um endereço de email para enviar os ativos por e-mail. A mensagem de email lista o URL no qual o destinatário pode fazer o download dos ativos.

1. Clique **em Exportar**.

Há suporte para três ações básicas de exportação:

* Arquivo original (exportar o arquivo original para o ativo)
* Converter usando predefinido (use uma predefinição de imagem para formatar o ativo)
* Converter sem predefinido (use a caixa de diálogo Exportar para especificar modificadores de imagem)

Os seguintes tipos de ativos não podem ser exportados. Todos os outros devem gerar uma exportação.

* Conjuntos de imagens
* Conjuntos de renderização
* Conjuntos de rotação
* Conjuntos de mídia
* Conjuntos de multi-bitrate
* Ecatalogs

Além disso, os modelos não podem ser exportados como um «arquivo original». »

Você pode usar a conversão para exportar os seguintes tipos de ativos:

* Imagens
* Modelos
* Imagens ajustadas
* PDF (vai gerar páginas convertidas)
* Postscript

Os seguintes resultados de comportamento quando uma grande seleção de vários tipos de ativos é alimentada no exportador:

* Todos os tipos de ativos que não podem ser exportados são removidos da lista antes da criação do serviço
* Se uma conversão for solicitada, todos os tipos que podem ser convertidos são, e todos os outros são exportados como originais.

