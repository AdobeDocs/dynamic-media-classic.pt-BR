---
title: Visão geral do programa Adobe Dynamic Media Classic
description: Uma visão geral do programa Adobe Dynamic Media Classic e de todo o processo de fluxo de trabalho.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Visão geral do programa Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Adobe Dynamic Media Classic é um ambiente integrado de gerenciamento, publicação e fornecimento de mídia avançada. A mídia avançada pode ser fornecida para todos os canais de marketing e vendas, incluindo a Web, material impresso, campanhas de email, portais da Web, desktops e dispositivos.

Consulte também [Visão geral da plataforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) vídeo de treinamento.

## Processo de fluxo de trabalho {#workflow-process}

As principais etapas do fluxo de trabalho do Adobe Dynamic Media Classic são:

* **Fazer upload e gerenciar ativos** - Faça upload dos ativos de mídia para o Adobe Dynamic Media Classic. Você pode organizar, procurar e procurar ativos no sistema. Também é possível aplicar metadados a ativos.

* **Criar mídia avançada** : crie configurações diferentes de seus ativos, como eCatalogs, Conjuntos de imagens, Conjuntos de rotação, Conjuntos de amostras, Conjuntos de mídia mista, Modelos básicos e Modelos FXG.

* **Publicar e administrar** - Publicar ativos na rede SaaS da Adobe Dynamic Media Classic. Monitorar o status de ativos quando eles são publicados. Administre os direitos do usuário e mantenha a segurança.

* **Atendimento** : forneça mídia da rede SaaS da Adobe Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; as mídias têm desempenho otimizado e são fornecidas com armazenamento em cache de CDN. A Adobe Dynamic Media Classic fornece um URL para cada ativo. Depois de publicar o ativo, o URL torna-se ativo.

![O processo de fluxo de trabalho Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Imagens principais únicas e chamadas de URL únicas {#single-master-images-and-single-url-calls}

O Adobe Dynamic Media Classic é fundamentalmente diferente de outros sistemas, pois você pode usar o Adobe Dynamic Media Classic para fornecer mídia dinamicamente a partir de ativos principais únicos e chamadas de URL.

As cadeias de caracteres de URL geradas com o Adobe Dynamic Media Classic incluem instruções que informam ao servidor como exibir o ativo quando entregue. Por exemplo, a mesma imagem principal pode ser fornecida em diferentes tamanhos, formatos, pesos, cores e visualizações de zoom. Como parte da criação e publicação de ativos de mídia com o Adobe Dynamic Media Classic, você configura visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam corretamente ao servidor como apresentar seu ativo principal aos aplicativos.

![O Adobe Dynamic Media Classic pode fornecer a mesma imagem principal a diferentes mídias em diferentes tamanhos e formatos.](/help/using/assets/gs_dynamic_publishing.png)
*A Adobe Dynamic Media Classic garante que experiências consistentes e de qualidade sejam oferecidas em qualquer tela, independentemente do tamanho ou da largura de banda.*

## Armazenamento em cache de conteúdo {#content-caching}

As imagens geradas dinamicamente pelo Adobe Dynamic Media Classic são favoráveis ao cache; geralmente, são imagens JPEG com chamadas de URL exclusivas que as identificam. As imagens são entregues na rede de entrega de conteúdo (CDN), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo mais rapidamente. As imagens são distribuídas de servidores localizados globalmente e, em seguida, para computadores. Ao implementar um mecanismo de armazenamento em cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Servidor de imagens do Dynamic Media habilitado para CDN. Todas as edições do Adobe Dynamic Media Classic incluem armazenamento em cache agrupado de CDN.
