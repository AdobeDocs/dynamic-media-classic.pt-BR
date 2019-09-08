---
title: Visão geral da plataforma do Adobe Dynamic Media Classic
seo-title: Visão geral da plataforma do Adobe Dynamic Media Classic
description: 'null'
seo-description: Uma visão geral do processo de plataforma e fluxo de trabalho do Dynamic Media Classic.
uuid: e 7 d 3 bfb 3-1 cfe -43 ea-b 862-aae 3 b 3928 c 71
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/getting_ started
discoiquuid: 2 b 134 cfa -7 f 46-4 f 5 f -959 e-b 30 aae 610 bb 9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Visão geral da plataforma do Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

O Dynamic Media Classic é um conteúdo integrado, de gerenciamento de mídia avançada, de publicação e de serviço. A mídia avançada pode ser entregue a todos os canais de marketing e venda, incluindo a Web, material de impressão, campanhas por email, portais da Web, desktops e dispositivos.

## Processo de fluxo de trabalho {#workflow-process}

As etapas principais do fluxo de trabalho do Dynamic Media Classic são:

**Carregar e gerenciar seus ativos** Carregue seus ativos de mídia para SPS. Você pode organizar, navegar e pesquisar ativos no sistema. Também é possível aplicar metadados a ativos. Se você instalar o aplicativo de desktop do Adobe Scene 7 Publishing System, poderá carregar arquivos e pastas arrastando-os da área de trabalho para uma pasta de upload.

**Criar mídia avançada** Crie configurações diferentes de seus ativos, como ecatalogs, Conjuntos de imagens, Conjuntos de rotação, Conjuntos de amostras, Conjuntos de mídia mista, Modelos básicos e Modelos FXG. Para obter mais informações, consulte Sobre mídia avançada.

**Publique e administre** Publicar ativos na rede Saas do Dynamic Media Classic, além de monitorar o status dos ativos quando eles forem publicados, administrar os direitos do usuário e manter a segurança.

**Forneça** mídia da rede saas do Dynamic Media Classic para páginas da Web, aplicativos e dispositivos móveis; a mídia é otimizada ao desempenho e é entregue com armazenamento em cache de CDN. O Dynamic Media Classic fornece um URL para cada ativo. Depois de publicar o ativo, o URL fica ativo.

![Processo de fluxo de trabalho do Dynamic Media Classic](/help/assets/gs_workflow.png)

## Imagens mestre simples e chamadas de URL simples {#single-master-images-and-single-url-calls}

O Dynamic Media Classic é fundamentalmente diferente de outros sistemas porque você pode usar o Dynamic Media Classic para fornecer mídia dinamicamente a partir de ativos mestre únicos e chamadas de URL.

As sequências de caracteres de URL geradas com o Dynamic Media Classic incluem instruções que informam ao servidor como exibir o ativo quando ele é entregue. Por exemplo, a mesma imagem mestre pode ser entregue em tamanhos diferentes, formatos, pesos, cores e exibições de zoom. Como parte de criar e publicar ativos de mídia com o Dynamic Media Classic, você configura visualmente os efeitos. Assim, você cria as chamadas de URL que informam corretamente ao servidor como apresentar seu ativo mestre aos aplicativos.

![O Dynamic Media Classic pode fornecer a mesma imagem mestre a diferentes meios de medianiz em tamanhos e formatos diferentes.](/help/assets/gs_dynamic_publishing.png)

## Armazenamento de conteúdo em cache {#content-caching}

As imagens geradas pelo Dynamic Media Classic são, de forma dinâmica, amigáveis; na maioria dos casos, são imagens JPEG com chamadas de URL exclusivas que os identificam. As imagens são fornecidas na rede de entrega de conteúdo (CDN), um sistema de servidores que está conectado na Internet para fornecer conteúdo mais rápido. As imagens são distribuídas de servidores localizados globalmente e, em seguida, para computadores. Ao implementar um mecanismo de cache usando qualquer fornecedor de CDN, basta alterar o nome do servidor para apontar para o servidor de imagem do Dynamic Media habilitado para CDN. Todas as edições do Dynamic Media Classic incluem armazenamento de CDN armazenado em cache.
