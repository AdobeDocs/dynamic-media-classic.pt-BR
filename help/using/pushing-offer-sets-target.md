---
title: Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium
description: Saiba como enviar conjuntos de ofertas do Adobe Dynamic Media Classic para o Adobe Target Standard/Premium.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Após criar ou editar um conjunto de ofertas, envie-o para o Adobe Target Standard/Premium seguindo estas etapas:

1. Na tela Conjunto de ofertas Test&amp;Target, selecione **[!UICONTROL Push Offers]**.
1. Insira o código do cliente e as credenciais de logon.
1. Selecionar **[!UICONTROL Login]**.

Durante a transferência para o Adobe Target Standard/Premium, o `S7_` é anexado automaticamente ao início dos nomes de oferta. Esse prefixo é anexado para garantir que você possa encontrar facilmente ofertas do Adobe Dynamic Media Classic na lista de ofertas Test&amp;Target. Por exemplo, a oferta aparece como `S7_<name of offer set>_<offer name>`.

O Adobe Dynamic Media Classic envia para as ofertas de widget do Adobe Target Standard/Premium. Você pode usar ofertas de widgets para hospedar seu próprio conteúdo oferecido fora do Adobe Target Standard/Premium. As ofertas de widgets são semelhantes a uma oferta padrão hospedada fora do Adobe Target Standard/Premium. Eles permitem que o Adobe Target Standard/Premium implante conteúdo de oferta armazenado no servidor, permitindo um uso mais sofisticado e dinâmico. As ofertas de widgets podem recuperar conteúdo de um URL, armazenando em cache e disponibilizando esse conteúdo por aproximadamente duas horas. As ofertas de widgets fornecem alguns recursos de geração de conteúdo dinâmico que outras ofertas fora do Adobe Target Standard/Premium não oferecem. Se a mbox que veicula a oferta contiver parâmetros de mbox como `mboxProductID` e `mbox.offerId`, o `productId=[PRODUCT_ID]`e `offerID=[OFFERID]` Os parâmetros de URL são anexados ao URL solicitado. Esses parâmetros podem ser usados por um serviço disponível no URL de oferta do Widget para retornar conteúdo fora do Adobe Target Standard/Premium que usa informações de produto ou pedido de suas mboxes. A oferta do Widget também é acessível por meio da API para criar ofertas de forma programática fora do Adobe Target Standard/Premium.
