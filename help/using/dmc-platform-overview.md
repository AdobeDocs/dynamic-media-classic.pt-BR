---
title: Visão geral do programa Adobe Dynamic Media Classic
description: Uma visão geral do programa Adobe Dynamic Media Classic e de todo o processo de fluxo de trabalho.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Visão geral do programa Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Adobe Dynamic Media Classic é um ambiente integrado de gerenciamento, publicação e fornecimento de mídia avançada. A mídia avançada pode ser entregue a todos os canais de marketing e vendas. Esses canais incluem a Web, material impresso, campanhas de email, portais da Web, desktops e dispositivos.

Consulte também o vídeo de treinamento [Visão geral da plataforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Processo de fluxo de trabalho {#workflow-process}

As principais etapas do fluxo de trabalho do Adobe Dynamic Media Classic são:

* **Fazer upload e gerenciar ativos**: faça upload dos ativos de mídia para a Adobe Dynamic Media Classic. Você pode organizar, procurar e procurar ativos no sistema. Também é possível aplicar metadados a ativos.

* **Criar mídia avançada**: crie configurações diferentes de seus ativos, como eCatalogs, Conjuntos de Imagens, Conjuntos de Rotação, Conjuntos de Amostras, Conjuntos de Mídias Mistas, Modelos básicos e Modelos FXG.

* **Publicar e administrar**: publique ativos na rede SaaS da Adobe Dynamic Media Classic. Monitorar o status de ativos quando eles são publicados. Administre os direitos do usuário e mantenha a segurança.

* **Servidor**: forneça mídia da rede SaaS da Adobe Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; a mídia tem desempenho otimizado e é fornecida com cache CDN. A Adobe Dynamic Media Classic fornece um URL para cada ativo. Depois de publicar o ativo, o URL torna-se ativo.

![O processo de fluxo de trabalho do Adobe Dynamic Media Classic](/help/using/assets/gs_workflow.png)

## Imagens principais únicas e chamadas de URL únicas {#single-master-images-and-single-url-calls}

O Adobe Dynamic Media Classic é fundamentalmente diferente de outros sistemas, pois você pode usar o Adobe Dynamic Media Classic para fornecer mídia dinamicamente a partir de ativos principais únicos e chamadas de URL.

As cadeias de caracteres de URL geradas com o Adobe Dynamic Media Classic incluem instruções que informam ao servidor como exibir o ativo quando entregue. Por exemplo, a mesma imagem principal pode ser fornecida em diferentes tamanhos, formatos, pesos, cores e visualizações de zoom. Como parte da criação e publicação de ativos de mídia com o Adobe Dynamic Media Classic, você pode configurar visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam corretamente ao servidor como apresentar seu ativo principal aos aplicativos.

O ![Adobe Dynamic Media Classic pode fornecer a mesma imagem principal a diferentes mídias, em tamanhos e formatos diferentes.](/help/using/assets/gs_dynamic_publishing.png)
*O Adobe Dynamic Media Classic garante que experiências consistentes e de qualidade sejam entregues a qualquer tela, independentemente do tamanho ou da largura de banda.*

## Armazenamento em cache de conteúdo {#content-caching}

As imagens geradas dinamicamente pelo Adobe Dynamic Media Classic são favoráveis ao cache; geralmente, são imagens do JPEG com chamadas de URL exclusivas que as identificam. As imagens são entregues na rede de entrega de conteúdo (CDN), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo mais rapidamente. As imagens são distribuídas de servidores localizados globalmente e, em seguida, para computadores. Ao implementar um mecanismo de armazenamento em cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Servidor de imagens do Dynamic Media habilitado para CDN. Todas as edições do Adobe Dynamic Media Classic incluem armazenamento em cache agrupado de CDN.
