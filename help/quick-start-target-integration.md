---
title: '"Início rápido: Integração do Adobe Target Standard/Premium"'
description: Uma introdução e o Início rápido para o Adobe Target Standard/Premium para ajudar você a ativar e executar rapidamente com as técnicas de integração do Adobe Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Início rápido: Integração do Adobe Target Standard/Premium{#quick-start-target-integration}

O Adobe Target Standard/Premium coloca o controle diretamente nas mãos dos profissionais de marketing para executar de forma rápida e contínua vários testes A/B e multivariados, medir a eficácia e aumentar a relevância do conteúdo online por meio da segmentação, direcionamento e personalização automatizada.

O Dynamic Media Classic permite criar ofertas e conjuntos de ofertas para campanhas do Adobe Target Standard/Premium. Por exemplo, você pode criar um conjunto de ofertas com três variações do mesmo ativo de mídia avançada. Em seguida, é possível fazer com que o Adobe Target Standard/Premium determine qual ativo oferece melhor aumento de conversão. Você pode criar ofertas e conjuntos de ofertas a partir de um Modelo básico ou de imagens individuais. Depois que o conjunto de ofertas é enviado ou salvo para o Adobe Target Standard/Premium, onde as ofertas são associadas a mboxes e experiências, o Adobe Target Standard/Premium pode executar campanhas. Essas campanhas determinam qual variação de site provavelmente terá melhor desempenho para click-throughs e conversão.

Para uma maior personalização do conteúdo dinâmico do Dynamic Media Classic, use as ofertas HTML do Adobe Target Standard/Premium . Consulte a [documentação do produto Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) para obter mais informações.

>[!NOTE]
>
>Uma conta válida do Adobe Target Standard/Premium é necessária para usar o Adobe Target Standard/Premium com o Dynamic Media Classic.

Este Início rápido foi projetado para ajudar você a funcionar rapidamente com os conjuntos de ofertas HTML do Adobe Target Standard/Premium. Siga as etapas de 1 a 3. Após cada etapa é uma referência cruzada a um cabeçalho de tópico, onde você pode encontrar mais informações.

## 1. Insira seu URL do Adobe Target Standard/Premium na página Configurações gerais do aplicativo

O Dynamic Media Classic precisa que seu URL do Adobe Target Standard/Premium se integre ao Adobe Target Standard/Premium. Copie a parte do URL do Adobe Target Standard/Premium até `.com`, inclusive, e insira-a na página **[!UICONTROL Application General Settings]** do Dynamic Media Classic, no campo de texto **[!UICONTROL Servers]** grupo, **[!UICONTROL Test&Target Server Name]**. Consulte [Integração do Dynamic Media Classic com o Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Criar o conjunto de ofertas

Use um modelo ou imagens parametrizadas para criar um conjunto de ofertas. Você cria conjuntos de ofertas HTML na página Conjunto de Ofertas do Test&amp;Target. Para abrir esta página, selecione seu modelo ou imagens e, na barra Navegação global, clique em **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

Para criar uma oferta com um modelo, clique em **[!UICONTROL Add & Preview]**. Na página Adicionar e visualizar , altere os valores dos parâmetros.

Para criar uma oferta com imagens, arraste as imagens para a página Conjunto de ofertas do Test&amp;Target. Clique em **[!UICONTROL Preview]** e escolha uma Predefinição de imagem para uma imagem ou para todas as imagens no conjunto de ofertas.

Salve o conjunto de ofertas depois de criá-lo.

Consulte [Criação de um conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## 3. Encaminhe a oferta para o Adobe Target Standard/Premium

Na página Conjunto de ofertas do Test&amp;Target, clique em **[!UICONTROL Push Offers]** e insira suas credenciais de logon na caixa de diálogo Logon do Test&amp;Target. Consulte [Envio de conjuntos de ofertas para o Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
