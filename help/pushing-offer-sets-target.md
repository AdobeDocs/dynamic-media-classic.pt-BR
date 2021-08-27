---
title: Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium
description: Saiba como encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium do Adobe Dynamic Media Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Depois de criar ou editar um conjunto de ofertas, envie-o para o Adobe Target Standard/Premium seguindo estas etapas:

1. Na tela Conjunto de ofertas do Test&amp;Target, selecione **[!UICONTROL Push Offers]**.
1. Insira seu código de cliente e credenciais de logon.
1. Selecione **[!UICONTROL Login]**.

Durante a transferência para o Adobe Target Standard/Premium, o prefixo `S7_` é anexado automaticamente ao início dos nomes das ofertas. Este prefixo é anexado para garantir que você possa encontrar facilmente ofertas do Adobe Dynamic Media Classic na lista de ofertas do Test&amp;Target. Por exemplo, a oferta aparece como `S7_<name of offer set>_<offer name>`.

O Adobe Dynamic Media Classic envia as ofertas de widget do Adobe Target Standard/Premium. Você pode usar ofertas de Widget para hospedar seu próprio conteúdo de oferta fora do Adobe Target Standard/Premium. As ofertas de widget são semelhantes a uma oferta padrão hospedada fora do Adobe Target Standard/Premium. Eles permitem que o Adobe Target Standard/Premium implante conteúdo de oferta que é armazenado em seu servidor, permitindo um uso mais sofisticado e dinâmico. As ofertas de widget podem recuperar o conteúdo de um URL, armazenando o conteúdo em cache e disponibilizando-o por aproximadamente duas horas. As ofertas de widget oferecem alguns recursos de geração de conteúdo dinâmico que outras ofertas fora do Adobe Target Standard/Premium não oferecem. Se a mbox que serve a oferta contém parâmetros de mbox como `mboxProductID` e `mbox.offerId`, os parâmetros de URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` são anexados ao URL solicitado. Esses parâmetros podem ser usados por um serviço disponível no URL de oferta do Widget para retornar conteúdo fora do Adobe Target Standard/Premium que usa informações do produto ou pedido de suas mboxes. A oferta de Widget também é acessível por meio da API para criar ofertas programaticamente fora do Adobe Target Standard/Premium.
