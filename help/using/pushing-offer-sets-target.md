---
title: Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium
description: Saiba como enviar conjuntos de ofertas do Adobe Dynamic Media Classic para o Adobe Target Standard/Premium.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 8a9d304ced3a218ae6393961a278f5ab9581c229
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 0%

---

# Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Após criar ou editar um conjunto de ofertas, envie-o para o Adobe Target Standard/Premium seguindo estas etapas:

1. Na tela Conjunto de Ofertas Test &amp; Target, selecione **[!UICONTROL Push Offers]**.
1. Insira o código do cliente e as credenciais de logon.
1. Selecione **[!UICONTROL Login]**.

Durante a transferência para o Adobe Target Standard/Premium, o prefixo `S7_` é adicionado automaticamente ao início dos nomes das ofertas. Esse prefixo é adicionado para garantir que você possa encontrar facilmente ofertas do Adobe Dynamic Media Classic na lista de ofertas do Test &amp; Target. Por exemplo, a oferta aparece como `S7_<name of offer set>_<offer name>`.

O Adobe Dynamic Media Classic envia as ofertas do widget para o Adobe Target Standard/Premium. Você pode usar ofertas do Widget para hospedar o conteúdo oferecido no Adobe Target Standard/Premium. As ofertas de widgets são comparáveis a uma oferta padrão hospedada pelo Adobe Target Standard/Premium. Eles permitem que o Adobe Target Standard/Premium implante conteúdo de oferta armazenado no servidor, permitindo um uso mais sofisticado e dinâmico. As ofertas de widgets recuperam o conteúdo de um URL, armazenando em cache e disponibilizando esse conteúdo por duas horas. As ofertas de widgets fornecem alguns recursos de geração de conteúdo dinâmico que outras ofertas fora do Adobe Target Standard/Premium não oferecem. Se a mbox que atende a oferta contiver parâmetros de mbox, como `mboxProductID` e `mbox.offerId`, os parâmetros de URL `productId=[PRODUCT_ID]` e `offerID=[OFFERID]` serão anexados à URL solicitada. Um serviço disponível no URL de oferta do Widget usa esses parâmetros para retornar conteúdo fora do Adobe Target Standard/Premium que usa informações de produto ou pedido de suas mboxes. A oferta do Widget também é acessível por meio da API, para que você possa criar ofertas de forma programática fora do Adobe Target Standard/Premium.
