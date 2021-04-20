---
title: '"Início rápido: Integração do Target Standard/Premium"'
description: Uma introdução e o Início rápido para o Adobe Target Standard/Premium para ajudar você a ativar e executar rapidamente com as técnicas de integração do Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Início rápido: Integração do Adobe Target Standard/Premium{#quick-start-target-integration}

O Adobe Target Standard/Premium coloca o controle diretamente nas mãos dos profissionais de marketing para executar de forma rápida e contínua vários testes A/B e multivariados, medir a eficácia e aumentar a relevância do conteúdo online por meio da segmentação, direcionamento e personalização automatizada.

O Dynamic Media Classic permite criar ofertas e conjuntos de ofertas para campanhas do Target Standard/Premium. Por exemplo, você pode criar um conjunto de ofertas com três variações do mesmo ativo de mídia avançada. Em seguida, você pode fazer com que o Target Standard/Premium determine qual ativo fornece melhor aumento de conversão. Você pode criar ofertas e conjuntos de ofertas a partir de um Modelo básico ou de imagens individuais. Depois que o conjunto de ofertas é enviado ou salvo para o Adobe Target Standard/Premium, onde as ofertas estão associadas a mboxes e experiências, o Target Standard/Premium pode executar campanhas para determinar qual variação de site deve ter o melhor desempenho para click-throughs e conversão.

Para uma maior personalização do conteúdo dinâmico do Dynamic Media Classic, use as ofertas HTML do Target Standard/Premium . Consulte a documentação do produto Target Standard/Premium para obter mais informações.

>[!NOTE]
>
>Uma conta válida do Adobe Target Standard/Premium é necessária para usar o Target Standard/Premium com o Dynamic Media Classic.

**Início rápido**

Este Início rápido foi projetado para ajudar você a funcionar rapidamente com os conjuntos de ofertas HTML do Target Standard/Premium. Siga as etapas de 1 a 3. Após cada etapa é uma referência cruzada a um cabeçalho de tópico, onde você pode encontrar mais informações.

**1. Insira seu URL do Adobe Target Standard/Premium na tela Configurações gerais do aplicativo .**

O Dynamic Media Classic precisa do URL do Target Standard/Premium para se integrar ao Target Standard/Premium. Copie a parte do URL do Target Standard/Premium até *.com*, inclusive, e insira-a na tela Configurações gerais do aplicativo Dynamic Media Classic . Consulte [Integração do Dynamic Media Classic com o Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Criar o conjunto de ofertas**

Use um modelo ou imagens parametrizadas para criar um conjunto de ofertas. Você cria conjuntos de ofertas HTML na tela Conjunto de Ofertas do Test&amp;Target. Para abrir esta tela, selecione seu modelo ou imagens e clique em **Criar** > **Conjunto de Ofertas do Test&amp;Target**.

Para criar uma oferta com um modelo, clique em **Adicionar e visualizar**. Na tela Adicionar e visualizar , altere os valores dos parâmetros.

Para criar uma oferta com imagens, arraste as imagens para a tela Conjunto de ofertas do Test&amp;Target. Clique em **Preview** para escolher uma Predefinição de imagem para uma imagem ou para todas as imagens no conjunto de ofertas.

Salve o conjunto de ofertas depois de criá-lo.

Consulte [Criação de um conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

**3. Encaminhe a oferta para o Adobe Target Standard/Premium**

Na tela Conjunto de ofertas do Test&amp;Target, clique em **Ofertas de push** e insira suas credenciais de logon na caixa de diálogo Logon do Test&amp;Target. Consulte [Envio de conjuntos de ofertas para Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
