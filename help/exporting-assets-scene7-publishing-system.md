---
title: Exportar ativos do Scene7 Publishing System
seo-title: Exportar ativos do Scene7 Publishing System
description: nulo
seo-description: Saiba como exportar ativos do Scene7 Publishing System.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Exportar ativos do Scene7 Publishing System{#exporting-assets-from-scene-publishing-system}

É possível salvar ativos que você editou no Scene7 Publishing System em uma unidade de rede local. Os ativos exportados são fornecidos em um arquivo ZIP para download ou envio por email.

O arquivo Zip compactado tem um tamanho máximo de 1 GB para o trabalho de exportação. Além disso, esteja ciente de que você tem permissão para um máximo de 500 ativos totais por trabalho de exportação.

O Dynamic Media Classic mantém um registro de trabalhos de exportação na tela Tarefas.

**Para exportar ativos do Scene7 Publishing System**

1. Selecione os ativos que deseja exportar e clique em **Arquivo** &gt; **Exportar**.
1. Na janela Exportar ativos selecionados, clique em Opções **de** imagem e especifique qualquer uma das seguintes opções (os administradores determinam quais opções estão disponíveis para seus usuários):

   * **Predefinições** Opcionalmente, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma predefinição de imagem, as outras opções de formatação não estarão disponíveis, já que o ativo adota os formatos definidos pela predefinição de imagem.

   * **Conversão** Converte o arquivo de ativo ou a imagem original.

   * **Tamanho** Você pode selecionar um tamanho padrão. Ou você pode clicar em Outro na lista suspensa Tamanho, escolher a unidade de medida desejada e especificar a largura e a altura.

      Consulte também [Especificação de opções de exportação disponíveis para usuários](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)do Portal de mídia.

   * **Formato** Escolha um formato de imagem.

   * **Cor** Escolha RGB, CMYK ou Cinza.

   * **Resolução** Escolha 72, 150 ou 300 ppi.

   * **Nome** da tarefaVocê pode atribuir um nome de tarefa à exportação.

   * **Enviar email para** opcionalmente, insira um endereço de email para enviar os ativos por email. A mensagem de email lista o URL para o qual o destinatário pode fazer download dos ativos.

1. Clique em **Exportar**.

Há suporte para três ações básicas de exportação:

* Arquivo original (exportar o arquivo original para o ativo)
* Converter usando predefinição (use uma predefinição de imagem para formatar o ativo)
* Converter sem predefinição (use a caixa de diálogo de exportação para especificar modificadores de imagem)

Os seguintes tipos de ativos não podem ser exportados. Todos os outros devem gerar uma exportação.

* Conjuntos de imagens
* Conjuntos de renderização
* Conjuntos de rotação
* Conjuntos de mídia
* Conjuntos de várias taxas de bits
* eCatalogs

Além disso, os modelos não podem ser exportados como um "arquivo original".

Você pode usar a conversão para exportar os seguintes tipos de ativos:

* Imagens
* Modelos
* Imagens ajustadas
* PDF (gerará páginas convertidas)
* Postscript

O comportamento a seguir resulta quando uma grande seleção de vários tipos de ativos é alimentada no exportador:

* Todos os tipos de ativos que não podem ser exportados são removidos da lista antes do envio da tarefa
* Se uma conversão for solicitada, todos os tipos que podem ser convertidos serão e todos os outros serão exportados como originais

