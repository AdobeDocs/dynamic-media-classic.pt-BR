---
title: Visão geral da plataforma Adobe Dynamic Media Classic
description: Uma visão geral da plataforma Dynamic Media Classic e do processo do fluxo de trabalho.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Visão geral da plataforma Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Dynamic Media Classic é um ambiente integrado de gerenciamento de mídia avançada, publicação e serviço. A mídia avançada pode ser entregue a todos os canais de marketing e venda, incluindo a Web, material impresso, campanhas por email, portais da Web, desktops e dispositivos.

## Processo de fluxo de trabalho {#workflow-process}

As principais etapas do fluxo de trabalho do Dynamic Media Classic são:

* **Faça upload e gerencie seus**
ativosFaça upload dos ativos de mídia para o Dynamic Media Classic. Você pode organizar, navegar e procurar ativos no sistema. Também é possível aplicar metadados a ativos.

* **Criar rich**
mediaCrie diferentes configurações de ativos, como eCatalogs, Conjuntos de imagens, Conjuntos de rotação, Conjuntos de amostras, Conjuntos de mídia mista, Modelos básicos e Modelos FXG. Para obter mais informações, consulte Sobre rich media.

* **Publique e**
administre ativos na rede do Saas do Dynamic Media Classic, bem como monitore o status dos ativos quando eles são publicados, administre os direitos do usuário e mantenha a segurança.

* ****
Fornecer mídia da rede SaaS do Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; as mídias são otimizadas para desempenho e fornecidas com o armazenamento em cache CDN. O Dynamic Media Classic fornece um URL para cada ativo. Após publicar o ativo, o URL fica ativo.

![O processo de fluxo de trabalho do Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imagens principais únicas e chamadas de URL único {#single-master-images-and-single-url-calls}

O Dynamic Media Classic é fundamentalmente diferente de outros sistemas, pois você pode usar o Dynamic Media Classic para fornecer mídia dinamicamente de ativos principais únicos e chamadas de URL.

As cadeias de caracteres de URL geradas com o Dynamic Media Classic incluem instruções que informam o servidor sobre como exibir o ativo quando ele é entregue. Por exemplo, a mesma imagem principal pode ser entregue em diferentes tamanhos, formatos, pesos, cores e exibições de zoom. Como parte da criação e publicação de ativos de mídia com o Dynamic Media Classic, você configura visualmente os efeitos. Ao fazer isso, você cria as chamadas de URL que informam o servidor corretamente sobre como apresentar seu ativo principal aos aplicativos.

![O Dynamic Media Classic pode fornecer a mesma imagem principal a diferentes mídias em diferentes tamanhos e formatos.](/help/assets/gs_dynamic_publishing.png)

## Armazenamento de conteúdo em cache {#content-caching}

As imagens geradas dinamicamente pelo Dynamic Media Classic são compatíveis com cache; na maioria dos casos, são imagens JPEG com chamadas de URL exclusivas que as identificam. As imagens são fornecidas na rede de entrega de conteúdo (CDN), um sistema de servidores que são conectados em rede na Internet para fornecer conteúdo com mais rapidez. As imagens são distribuídas de servidores localizados globalmente e, em seguida, de computadores. Ao implementar um mecanismo de armazenamento em cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o Dynamic Media Image Server habilitado para CDN. Todas as edições do Dynamic Media Classic incluem armazenamento em cache CDN empacotado.
