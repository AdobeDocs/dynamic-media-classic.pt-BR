---
title: Envio de conjuntos de ofertas para o Adobe Target Standard/Premium
description: Saiba como encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---


# Envio de conjuntos de ofertas para o Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Depois de criar ou editar um conjunto de ofertas, envie-o para o Target Standard/Premium seguindo estas etapas:

1. Na tela Conjunto de ofertas do Test&amp;Target, clique em **[!UICONTROL Push Offers]**.
1. Insira seu código de cliente e credenciais de logon.
1. Clique em **[!UICONTROL Login]**.

Durante a transferência para o Target Standard/Premium, o prefixo S7_ é anexado automaticamente ao início dos nomes das ofertas. Este prefixo é anexado para garantir que você possa encontrar facilmente ofertas do Dynamic Media Classic na lista de ofertas do Test&amp;Target. Por exemplo, a oferta aparece como S7_&lt;name of offer set>_&lt;offer name>.

O Dynamic Media Classic é enviado para as ofertas de widget do Target Standard/Premium. Você pode usar ofertas de Widget para hospedar seu próprio conteúdo de oferta fora do Target Standard/Premium. As ofertas de widget são semelhantes a uma oferta padrão hospedada fora do Target Standard/Premium. Eles permitem que o Target Standard/Premium implante conteúdo de oferta que é armazenado em seu servidor, permitindo um uso mais sofisticado e dinâmico. As ofertas de widget recuperam o conteúdo de um URL, armazenando em cache e disponibilizando esse conteúdo por aproximadamente duas horas. As ofertas de widget oferecem alguns recursos de geração de conteúdo dinâmico que outras ofertas fora do Target Standard/Premium não oferecem. Se a mbox que serve a oferta contém parâmetros de mbox como `mboxProductID` e `mbox.offerId`, os parâmetros de URL `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` são anexados ao URL solicitado. Esses parâmetros podem ser usados por um serviço disponível no URL de oferta do Widget para retornar conteúdo fora do Target Standard/Premium que usa informações do produto ou pedido de suas mboxes. A oferta de Widget também é acessível por meio da API para criar ofertas de maneira programática fora do Target Standard/Premium.
