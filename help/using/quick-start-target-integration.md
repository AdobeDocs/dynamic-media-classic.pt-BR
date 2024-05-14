---
title: "Início rápido: integração do Adobe Target Standard/Premium"
description: Uma introdução e o Início rápido do Adobe Target Standard/Premium para ajudar você a começar a usar rapidamente as técnicas de integração do Adobe Target Standard/Premium no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Início rápido: integração com o Adobe Target Standard/Premium{#quick-start-target-integration}

O Adobe Target Standard/Premium coloca o controle diretamente nas mãos dos profissionais de marketing. Isso pode ajudar a executar de maneira rápida e contínua vários testes A/B e multivariados, além de medir a eficácia. Além disso, ela pode aumentar a relevância do conteúdo online por meio da segmentação, do direcionamento e do Automated Personalization.

O Adobe Dynamic Media Classic permite criar ofertas e Conjuntos de ofertas para campanhas do Adobe Target Standard/Premium. Por exemplo, você pode criar um Conjunto de ofertas com três variações do mesmo ativo de mídia avançada. Em seguida, você pode ter o Adobe Target Standard ou Premium para determinar qual ativo oferece melhor aumento de conversão. É possível criar ofertas e Conjuntos de ofertas a partir de um Modelo básico ou de imagens individuais. Depois que o Conjunto de ofertas é enviado ou salvo para o Adobe Target Standard/Premium, onde as ofertas são associadas a mboxes e experiências, o Adobe Target Standard/Premium pode executar campanhas. Essas campanhas determinam qual variação de um site provavelmente terá melhor desempenho para click-throughs e conversão.

Para maior personalização de conteúdo dinâmico do Adobe Dynamic Media Classic, use as ofertas de HTML do Adobe Target Standard/Premium. Consulte a [Documentação do produto Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target) para obter mais informações.

>[!NOTE]
>
>É necessária uma conta válida do Adobe Target Standard/Premium para usar o Adobe Target Standard/Premium com o Adobe Dynamic Media Classic.

Esse Início rápido foi projetado para colocar suas operações em funcionamento rapidamente com os Conjuntos de ofertas de HTML do Adobe Target Standard/Premium. Siga as etapas de 1 a 3. Após cada etapa, há uma referência cruzada a um cabeçalho de tópico onde você pode encontrar mais informações.

## 1. Insira seu URL do Adobe Target Standard/Premium na página Configurações gerais do aplicativo

O Adobe Dynamic Media Classic precisa do URL do Adobe Target Standard/Premium para se integrar ao Adobe Target Standard/Premium. Copie a parte do seu URL do Adobe Target Standard/Premium até e incluindo `.com`e insira-o na Adobe Dynamic Media Classic **[!UICONTROL Application General Settings]** página, no campo **[!UICONTROL Servers]** grupo, **[!UICONTROL Test&Target Server Name]** campo de texto. Consulte [Integrar o Adobe Dynamic Media Classic com o Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Criar o conjunto de ofertas

Use um modelo ou imagens com parâmetros para criar um Conjunto de ofertas. Você pode criar Conjuntos de ofertas HTML na página Conjunto de ofertas Test&amp;Target. Para abrir esta página, selecione o modelo ou as imagens e, na barra de Navegação global, vá para **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

Para criar uma oferta com um modelo, selecione **[!UICONTROL Add & Preview]**. Na página Adicionar e visualizar, altere os valores dos parâmetros.

Para criar uma oferta com imagens, arraste as imagens para a página Conjunto de ofertas Test&amp;Target. Selecionar **[!UICONTROL Preview]** e escolha uma Predefinição de imagem para uma imagem ou todas as imagens no Conjunto de ofertas.

Salve o Conjunto de ofertas depois de criá-lo.

Consulte [Criar um conjunto de ofertas](creating-offer-set.md#creating_an_offer_set).

## 3. Encaminhar o conjunto de ofertas para o Adobe Target Standard/Premium

Na página Conjunto de ofertas Test&amp;Target, selecione **[!UICONTROL Push Offers]** e digite suas credenciais de logon na caixa de diálogo Logon do Test&amp;Target. Consulte [Encaminhar conjuntos de ofertas para o Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
