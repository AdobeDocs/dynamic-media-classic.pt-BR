---
title: Mover conjuntos de ofertas para o Adobe Target Classic
seo-title: Mover conjuntos de ofertas para o Adobe Target Classic
description: 'null'
seo-description: Saiba como mover conjuntos de ofertas para o Adobe Target Classic.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/target_ classic_ integration
discoiquuid: 39 a 05654-4 f 66-4 f 1 e-ight5-ebe 6 d 174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Mover conjuntos de ofertas para o Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Depois de criar ou editar um conjunto de ofertas, envie-o para o Target Classic seguindo estas etapas:

1. Na tela Conjunto de ofertas do Target Classic, clique no botão Ofertas de push.
1. Insira suas credenciais de login.
1. Clique no botão Logon.

Durante a transferência para o Target Classic, o prefixo S 7_ é anexado automaticamente ao início de nomes de ofertas. Esse prefixo é anexado para garantir que você possa encontrar facilmente ofertas do Dynamic Media Classic na lista de ofertas do Target Classic. Por exemplo, a oferta aparece como S 7_ &lt; nome do conjunto de ofertas &gt;_ &lt; nome da oferta &gt;.

Os SPS são empurrados para ofertas de widget do Target Classic. Você pode usar ofertas de Widget para hospedar seu próprio conteúdo da oferta fora do Target Classic. Ofertas de widget são semelhantes a uma oferta padrão hospedada fora do Target Classic. Eles permitem que o Target Classic implemente conteúdo da oferta armazenado em seu servidor, permitindo um uso mais sofisticado e dinâmico. As ofertas de widget recuperam conteúdo de um URL, armazenando o conteúdo em cache e disponibilizando esse conteúdo por aproximadamente duas horas. As ofertas de widget oferecem alguns recursos de geração de conteúdo dinâmico que outras ofertas, fora do Target Classic, não oferecem. Se a mbox que serve a oferta contiver parâmetros de mbox, como `mboxProductID` e `mbox.offerId`, os parâmetros `productId=[PRODUCT_ID]`e, os parâmetros `offerID=[OFFERID]` de URL serão anexados ao URL solicitado. Esses parâmetros podem ser usados por um serviço disponível no URL de oferta do Widget para retornar conteúdo fora do Target Classic que usa informações de produto ou pedido de suas mboxes. A oferta de Widget também pode ser acessada por meio da API para criar ofertas de forma programática fora do Target Classic.
