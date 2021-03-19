---
title: Exportar ativos do Dynamic Media Classic
description: Saiba como exportar ativos do Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Profissional
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Exportar ativos do Dynamic Media Classic{#exporting-assets-from-dmc}

Você pode salvar ativos editados no Dynamic Media Classic em uma unidade de rede local. Os ativos exportados são agrupados em um arquivo ZIP para download ou envio por email.

O arquivo Zip compactado tem um tamanho máximo de arquivo de 1 GB para o trabalho de exportação. Além disso, esteja ciente de que é permitido um máximo de 500 ativos totais por trabalho de exportação.

O Dynamic Media Classic mantém um registro de trabalhos de exportação na tela Trabalhos .

**Para exportar ativos do Dynamic Media Classic**

1. Selecione os ativos que deseja exportar e clique em **Arquivo** > **Exportar**.
1. Na janela Exportar ativos selecionados , clique em **Opções de imagem** e especifique qualquer uma das seguintes opções (os administradores determinam quais opções estão disponíveis para os usuários):

   * ****
PredefiniçõesOpcionalmente, escolha uma Predefinição de imagem para formatar o ativo ao exportá-lo. Se você escolher uma Predefinição de imagem, as outras opções de formatação não estarão disponíveis, pois o ativo adota os formatos definidos pela Predefinição de imagem.

   * ****
ConversãoConverte o arquivo de ativo ou a imagem original.

   * ****
TamanhoVocê pode selecionar um tamanho padrão. Ou, você pode clicar em Outro na lista suspensa Tamanho, escolher a unidade de medida desejada e especificar a largura e a altura.

      Consulte também [Especificar opções de exportação disponíveis para usuários do Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * ****
FormatoEscolha um formato de imagem.

   * ****
CorEscolha RGB, CMYK ou Cinza.

   * ****
SoluçãoEscolha 72, 150 ou 300 ppi.

   * **Nome**
do trabalhoVocê pode atribuir um nome de trabalho à exportação.

   * **Enviar Email**
Para Opcionalmente, insira um endereço de email para enviar os ativos por email. A mensagem de email lista o URL para onde o recipient pode baixar os ativos.

1. Clique em **Exportar**.

Há suporte para três ações básicas de exportação:

* Arquivo original (exportar o arquivo original do ativo)
* Converter usando predefinição (use uma predefinição de imagem para formatar o ativo)
* Converter sem predefinição (use a caixa de diálogo exportar para especificar modificadores de imagem)

Os seguintes tipos de ativos não podem ser exportados. Todos os outros devem gerar uma exportação.

* Conjuntos de imagens
* Conjuntos de renderização
* Conjuntos de rotação
* Conjuntos de mídia
* Conjuntos de taxa de bits múltipla
* Catálogos eletrônicos

Além disso, os modelos não podem ser exportados como um &quot;arquivo original&quot;.

Você pode usar a conversão para exportar os seguintes tipos de ativos:

* Imagens
* Modelos
* Imagens ajustadas
* PDF (gerará páginas convertidas)
* Postscript

O comportamento a seguir resulta quando uma grande seleção de vários tipos de ativos é inserida no exportador:

* Todos os tipos de ativos que não podem ser exportados são removidos da lista antes do envio do trabalho
* Se uma conversão for solicitada, todos os tipos que podem ser convertidos serão e todos os outros serão exportados como originais

