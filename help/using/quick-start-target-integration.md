---
title: 'Início rápido: integração do Adobe Target Standard/Premium'
description: Uma introdução e o Início rápido do Adobe Target Standard/Premium para ajudar você a começar a usar rapidamente as técnicas de integração do Adobe Target Standard/Premium no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T19:56:29.690Z'
TQID: 'https://experienceleague.adobe.com/urNoJw6SrzPpsfpoTtudKndZfJOmWsZKtBZ3Za4aE0I'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 0f0abef2ec6e1d0743eca66e59673547f70ad7b0
workflow-type: tm+mt
source-wordcount: 511
ht-degree: 0%

---

# Início rápido: integração com o Adobe Target Standard/Premium{#quick-start-target-integration}

O Adobe Target Standard/Premium oferece controle administrativo às equipes de marketing. Esse recurso pode ajudá-lo a executar rápida e continuamente vários testes A/B e multivariados e medir sua eficácia. Além disso, ela pode aumentar a relevância do conteúdo online por meio da segmentação, do direcionamento e do Automated Personalization.

O Adobe Dynamic Media Classic permite criar ofertas e Conjuntos de ofertas para campanhas do Adobe Target Standard/Premium. Por exemplo, você pode criar um Conjunto de ofertas com três variações do mesmo ativo de mídia avançada. Em seguida, você pode fazer com que o Adobe Target Standard ou Premium determine qual ativo oferece melhor desempenho de conversão. É possível criar ofertas e Conjuntos de ofertas a partir de um Modelo básico ou de imagens individuais. Depois que o Conjunto de ofertas é enviado ou salvo para o Adobe Target Standard/Premium, onde as ofertas são associadas a mboxes e experiências, o Adobe Target Standard/Premium pode executar campanhas. Essas campanhas determinam qual variação de um site tem melhor desempenho para click-throughs e conversão.

Para maior personalização do conteúdo dinâmico do Adobe Dynamic Media Classic, use as ofertas do Adobe Target Standard/Premium HTML. Consulte a [documentação do produto Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target) para obter mais informações.

>[!NOTE]
>
>É necessária uma conta válida do Adobe Target Standard/Premium para usar o Adobe Target Standard/Premium com o Adobe Dynamic Media Classic.

Este guia foi projetado para ajudar você a começar a usar os Conjuntos de ofertas do Adobe Target Standard/Premium HTML rapidamente. Siga as etapas de 1 a 3. Após cada etapa, há uma referência cruzada a um cabeçalho de tópico onde você pode encontrar mais informações.

## &#x200B;1. Insira seu URL do Adobe Target Standard/Premium na página Configurações gerais do aplicativo

O Adobe Dynamic Media Classic precisa do URL do Adobe Target Standard/Premium para se integrar ao Adobe Target Standard/Premium. Copie a parte da sua URL do Adobe Target Standard/Premium até `.com` (inclusive) e insira-a no campo de texto **[!UICONTROL Test&Target Server Name]**, no grupo **[!UICONTROL Servers]**, na página **[!UICONTROL Application General Settings]** do Adobe Dynamic Media Classic. Consulte [Integrar o Adobe Dynamic Media Classic com o Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## &#x200B;2. Criar o conjunto de ofertas

Use um modelo ou imagens com parâmetros para criar um Conjunto de ofertas. Você pode criar Conjuntos de ofertas do HTML na página Conjunto de ofertas do Test&amp;Target. Para abrir esta página, selecione o modelo ou as imagens e, na barra de Navegação Global, vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

Para criar uma oferta com um modelo, selecione **[!UICONTROL Add & Preview]**. Na página Adicionar e visualizar, altere os valores dos parâmetros.

Para criar uma oferta com imagens, arraste as imagens para a página Conjunto de ofertas Test&amp;Target. Selecione **[!UICONTROL Preview]** e escolha uma Predefinição de imagem para uma imagem ou todas as imagens no Conjunto de ofertas.

Salve o Conjunto de ofertas depois de criá-lo.

Consulte [Criar um conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## &#x200B;3. Encaminhar o conjunto de ofertas para o Adobe Target Standard/Premium

Na página Conjunto de ofertas Test&amp;Target, selecione **[!UICONTROL Push Offers]** e insira suas credenciais de logon na caixa de diálogo Logon Test&amp;Target. Consulte [Enviar conjuntos de ofertas para o Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
