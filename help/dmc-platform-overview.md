---
title: Visão geral do programa Adobe Dynamic Media Classic
description: Uma visão geral do programa Adobe Dynamic Media Classic e de todo o processo de fluxo de trabalho.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 2616c067215196e8145043ba57fba1e3a5667cdc
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Visão geral do programa Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Adobe Dynamic Media Classic é um ambiente integrado de gerenciamento, publicação e fornecimento de mídia avançada. A mídia avançada pode ser entregue a todos os canais de marketing e venda, incluindo a Web, material impresso, campanhas por email, portais da Web, desktops e dispositivos.

Consulte também vídeo de treinamento [Visão geral da plataforma](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Processo de workflow {#workflow-process}

As principais etapas do fluxo de trabalho do Adobe Dynamic Media Classic são:

* **Faça upload e gerencie seus ativos**  - Faça upload dos ativos de mídia para a Adobe Dynamic Media Classic. Você pode organizar, navegar e procurar ativos no sistema. Também é possível aplicar metadados a ativos.

* **Criar rich media**  - crie diferentes configurações de ativos, como catálogos eletrônicos, conjuntos de imagens, conjuntos de rotação, conjuntos de amostras, conjuntos de mídia mista, modelos básicos e modelos FXG.

* **Publicar e administrar**  - Publique ativos na rede Adobe Dynamic Media Classic SaaS. Monitore o status dos ativos quando eles forem publicados. Administre os direitos do usuário e mantenha a segurança.

* **Servir**  - fornecer mídia da rede SaaS da Adobe Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; as mídias são otimizadas para desempenho e fornecidas com o armazenamento em cache CDN. O Adobe Dynamic Media Classic fornece um URL para cada ativo. Após publicar o ativo, o URL fica ativo.

![O processo de workflow do Adobe Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imagens principais únicas e chamadas de URL único {#single-master-images-and-single-url-calls}

O Adobe Dynamic Media Classic é fundamentalmente diferente de outros sistemas, pois você pode usar o Adobe Dynamic Media Classic para fornecer mídia dinamicamente de ativos principais únicos e chamadas de URL.

As cadeias de caracteres de URL geradas com o Adobe Dynamic Media Classic incluem instruções que informam o servidor sobre como exibir o ativo quando ele é entregue. Por exemplo, a mesma imagem principal pode ser entregue em diferentes tamanhos, formatos, pesos, cores e exibições de zoom. Como parte da criação e publicação de ativos de mídia com o Adobe Dynamic Media Classic, você configura visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam o servidor corretamente sobre como apresentar seu ativo principal aos aplicativos.

![O Adobe Dynamic Media Classic pode fornecer a mesma imagem principal para diferentes mídias em diferentes tamanhos e formatos.](/help/assets/gs_dynamic_publishing.png)
*A Adobe Dynamic Media Classic garante que experiências consistentes e de qualidade sejam entregues a qualquer tela, independentemente do tamanho ou da largura de banda.*

## Armazenamento em cache de conteúdo {#content-caching}

As imagens geradas dinamicamente pelo Adobe Dynamic Media Classic são compatíveis com cache; geralmente, são imagens JPEG com chamadas de URL exclusivas que as identificam. As imagens são fornecidas na rede de entrega de conteúdo (CDN), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo com mais rapidez. As imagens são distribuídas de servidores localizados globalmente e, em seguida, de computadores. Ao implementar um mecanismo de armazenamento em cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Dynamic Media Image Server habilitado para CDN. Todas as edições do Adobe Dynamic Media Classic incluem armazenamento em cache CDN empacotado.
