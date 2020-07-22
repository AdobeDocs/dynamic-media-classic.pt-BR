---
title: Exportar ativos do Dynamic Media Classic
seo-title: Exportar ativos do Dynamic Media Classic
description: nulo
seo-description: Saiba como exportar ativos do Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Exportar ativos do Dynamic Media Classic{#exporting-assets-from-dmc}

É possível salvar ativos que você editou no Dynamic Media Classic em uma unidade de rede local. Os ativos exportados são fornecidos em um arquivo ZIP para download ou envio por email.

O arquivo Zip compactado tem um tamanho máximo de 1 GB para o trabalho de exportação. Além disso, esteja ciente de que você tem permissão para um máximo de 500 ativos totais por trabalho de exportação.

O Dynamic Media Classic mantém um registro de trabalhos de exportação na tela Tarefas.

**Para exportar ativos do Dynamic Media Classic**

1. Selecione os ativos que deseja exportar e clique em **Arquivo** > **Exportar**.
1. Na janela Exportar ativos selecionados, clique em Opções **de** imagem e especifique qualquer uma das seguintes opções (os administradores determinam quais opções estão disponíveis para seus usuários):

   * **Predefinições** Opcionalmente, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma predefinição de imagem, as outras opções de formatação não estarão disponíveis, já que o ativo adota os formatos definidos pela predefinição de imagem.

   * **Conversão** Converte o arquivo de ativo ou a imagem original.

   * **Tamanho** Você pode selecionar um tamanho padrão. Ou você pode clicar em Outro na lista suspensa Tamanho, escolher a unidade de medida desejada e especificar a largura e a altura.

      Consulte também [Especificação de opções de exportação disponíveis para usuários](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)do Portal de mídia.

   * **Formato** Escolha um formato de imagem.

   * **Cor** Escolha RGB, CMYK ou Cinza.

   * **Resolução** Escolha 72, 150 ou 300 ppi.

   * **Nome** da tarefaVocê pode atribuir um nome de tarefa à exportação.

   * **Enviar email para** opcionalmente, insira um endereço de email para enviar os ativos por email. A mensagem de email lista no URL para onde o recipient pode ir para baixar os ativos.

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

Além disso, os modelos não podem ser exportados como um &quot;arquivo original&quot;.

Você pode usar a conversão para exportar os seguintes tipos de ativos:

* Imagens
* Modelos
* Imagens ajustadas
* PDF (gerará páginas convertidas)
* Postscript

O comportamento a seguir resulta quando uma grande seleção de vários tipos de ativos é alimentada no exportador:

* Todos os tipos de ativos que não podem ser exportados são removidos da lista antes do envio do trabalho
* Se uma conversão for solicitada, todos os tipos que podem ser convertidos serão e todos os outros serão exportados como originais

