---
title: Encaminhando conjuntos de ofertas para o Adobe Target Standard/Premium
seo-title: Encaminhando conjuntos de ofertas para o Adobe Target Standard/Premium
description: nulo
seo-description: Saiba como encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Encaminhando conjuntos de ofertas para o Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Depois de criar ou editar um conjunto de ofertas, envie-o para o Target Standard/Premium seguindo estas etapas:

1. Na tela Conjunto de Ofertas do Test&amp;Público alvo, clique em **[!UICONTROL Push Offers]**.
1. Insira o código do cliente e as credenciais de logon.
1. Clique em **[!UICONTROL Login]**.

Durante a transferência para o Target Standard/Premium, o prefixo S7_ é anexado automaticamente ao start de nomes de ofertas. Este prefixo é anexado para garantir que você possa encontrar facilmente ofertas do Dynamic Media Classic na lista de oferta do Test&amp;Público alvo. Por exemplo, a oferta aparece como S7_&lt;nome da oferta definida>_&lt;nome da oferta>.

O Dynamic Media Classic é direcionado para ofertas de widget do Target Standard/Premium. Você pode usar ofertas de Widget para hospedar seu próprio conteúdo de oferta fora do Target Standard/Premium. Ofertas de widget são semelhantes a uma oferta padrão hospedada fora do Target Standard/Premium. Eles permitem que o Target Standard/Premium implante conteúdo de oferta armazenado em seu servidor, permitindo uma utilização mais sofisticada e dinâmica. As ofertas de widget recuperam conteúdo de um URL, armazenando em cache e disponibilizando esse conteúdo por aproximadamente duas horas. As ofertas de widget fornecem alguns recursos de geração de conteúdo dinâmico que outras ofertas fora do Target Standard/Premium não oferecem. Se a mbox que serve a oferta contiver parâmetros de mbox como `mboxProductID` e `mbox.offerId`, os parâmetros de URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` serão anexados ao URL solicitado. Esses parâmetros podem ser usados por um serviço disponível no URL de oferta do Widget para retornar conteúdo fora do Target Standard/Premium que usa informações de produto ou pedido de suas mboxes. A oferta Widget também é acessível por meio da API para criar ofertas de forma programática fora do Target Standard/Premium.
