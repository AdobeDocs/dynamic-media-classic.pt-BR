---
title: Testar ativos antes de torná-los públicos
description: Saiba como testar ativos no Adobe Dynamic Media Classic antes de torná-los públicos.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 0%

---

# Testar ativos antes de torná-los públicos {#testing-assets-before-making-them-public}

O Teste seguro ajuda você a definir um ambiente de teste seguro e criar uma solução B2B robusta, com base em um conjunto configurável de endereços IP e intervalos. Essa funcionalidade permite combinar as implantações do Adobe Dynamic Media Classic com a arquitetura do sistema de gerenciamento de conteúdo e de negócios.

Com o Teste seguro, é possível visualizar a versão de preparo do site com conteúdo não publicado.

Se desejar, crie um ambiente de preparo em vez de disponibilizar os ativos publicamente pelos seguintes motivos:

* Visualizar sites antes do lançamento público (site de preparo).
* Atenda a ativos que exigem acesso restrito, como eCatalogs que mostram preços em um aplicativo Web B2B.
* Use ativos protegidos por um firewall como parte de um sistema de gerenciamento de informações de produtos, aplicativo de atendimento ao cliente, local de treinamento etc.

>[!NOTE]
>
>O teste seguro não afeta o acesso ao Adobe Dynamic Media Classic. A segurança do Adobe Dynamic Media Classic permanece consistente e requer as credenciais normais para acessar o Adobe Dynamic Media Classic e os serviços da Web relacionados.

## Como funciona o teste seguro {#how-secure-testing-works}

A maioria das corporações usa a Internet com um firewall. O acesso à Internet é possível por meio de determinadas rotas e, normalmente, por meio de um intervalo limitado de endereços IP públicos.

Na rede corporativa, você pode descobrir seu endereço IP público usando sites como o [https://www.whatismyip.com](https://www.whatismyip.com/) ou solicitar essas informações à organização de TI corporativa.

Com o teste seguro, a Adobe Dynamic Media Classic estabelece um servidor de imagens dedicado para ambientes de preparo ou aplicativos internos. Qualquer solicitação a esse servidor verifica o endereço IP de origem. Se a solicitação recebida não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada. O Administrador da empresa do Adobe Dynamic Media Classic configura a lista aprovada de endereços IP para o ambiente de teste seguro da empresa.

Como o local da solicitação original deve ser confirmado, o tráfego do serviço de Teste seguro não é roteado por uma rede de distribuição de conteúdo, como o tráfego público do Dynamic Media Image Server. As solicitações para o serviço de Teste seguro têm uma latência um pouco maior em comparação aos servidores de imagem públicos Dynamic Media.

Os ativos não publicados estão imediatamente disponíveis nos serviços de teste seguro, sem a necessidade de publicar. Dessa forma, é possível executar uma pré-visualização antes que os ativos sejam publicados no Servidor de imagens voltado para o público.

>[!NOTE]
>
>Os serviços de teste seguro usam o Servidor de catálogo configurado com um contexto de publicação interno. Portanto, se sua empresa estiver configurada para publicar no Teste seguro, todos os ativos carregados no Adobe Dynamic Media Classic estarão imediatamente disponíveis nos serviços de Teste seguro. Essa funcionalidade é verdadeira independentemente de os ativos estarem marcados para publicação durante o upload.

Atualmente, os serviços de teste seguro são compatíveis com os seguintes tipos de ativos e funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imagens.
* Vinhetas (solicitações do Servidor de Renderização).
* Renderizar solicitações do servidor (compatível, mas o cliente deve solicitá-las explicitamente).
* Conjuntos, incluindo conjuntos de imagens, eCatalog, conjuntos de renderização e conjuntos de mídia.
* Visualizadores padrão de mídia avançada Adobe Dynamic Media Classic.
* Páginas JSP do Adobe Dynamic Media Classic OnDemand.
* Conteúdo estático, como arquivos PDF e vídeos progressivamente exibidos.
* Transmissão de vídeo HTTP.
* Transmissão de vídeo progressiva.

Os seguintes tipos de ativos e funcionalidades não são compatíveis no momento:

* Pesquisa no Adobe Dynamic Media Classic Info ou eCatalog
* Transmissão contínua de vídeo RTMP
* Web para impressão
* Serviços UGC (User-Generated Content, conteúdo gerado pelo usuário)

>[!IMPORTANT]
>
>O suporte a ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

## Testar o serviço de teste seguro {#testing-the-secure-testing-service}

Teste o serviço de teste seguro para garantir que ele funcione conforme esperado.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Preparar sua conta

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Entre em contato com o Atendimento ao cliente da Adobe e solicite que ele ative o Teste seguro em sua conta.
1. No Adobe Dynamic Media Classic, na barra Navegação Global, vá para **[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**.
1. Na página Publish do Servidor de imagens, na lista suspensa **[!UICONTROL `Publish Context`]**, selecione **[!UICONTROL Test Image Serving]**.
1. Para o Filtro de Endereço de Cliente, selecione **[!UICONTROL Add]**.
1. Marque a caixa de seleção para que o endereço seja ativado e digite um endereço IP e uma máscara de rede nos respectivos campos de texto.

   >[!NOTE]
   >
   >Se você adicionar um único endereço IP e máscara de rede, esse endereço poderá fazer chamadas de ativos. No entanto, qualquer outro endereço IP e máscara de rede adicionados não têm permissão para fazer chamadas de ativos. Dessa forma, considere desativar (desativar) a caixa de seleção na etapa acima para desativar a capacidade de especificar um endereço IP e uma máscara de rede. Com isso, *todos* os endereços IP efetivamente podem fazer chamadas de ativos, e todos eles são exibidos.

1. Siga um destes procedimentos:
   * Repita as duas etapas anteriores se precisar adicionar mais endereços IP.
   * Continue com a próxima etapa.
1. Na parte inferior esquerda da página do Publish do Servidor de imagens, selecione **[!UICONTROL Save]**
1. Carregue as imagens desejadas na sua conta do Adobe Dynamic Media Classic.

   Consulte [Carregar arquivos](uploading-files.md#uploading_files).

1. Verifique se algumas imagens estão marcadas para publicação e outras estão desmarcadas e envie o trabalho de publicação.

   Consulte [arquivos Publish](publishing-files.md#publishing_files).

1. Determine o nome do seu serviço de Teste Seguro indo até **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Na página Configurações Gerais do Aplicativo, no grupo Servidores, encontre o nome à direita de **[!UICONTROL Test Publish Context Server Name]**.

Entre em contato com o Adobe Care se o nome do servidor estiver ausente ou se os URLs do servidor não funcionarem.

### Preparar variações de site

Você precisa de duas variações de um site que vincula os ativos publicados e não publicados:

* Versão pública: vincule ativos usando a sintaxe tradicional do URL do Adobe Dynamic Media Classic.
* Versão de preparo: vincule ativos usando a mesma sintaxe, mas com o nome do site de teste seguro.

### Executar os testes

Execute os seguintes testes:

1. Verifique se os ativos estão visíveis na rede corporativa.

   Dentro da rede corporativa identificada pelo intervalo de endereços IP definido anteriormente, a versão de preparo do site exibe todas as imagens, marcadas para publicação ou não. Dessa forma, você pode testar sem disponibilizar acidentalmente as imagens antes da aprovação de visualização ou do lançamento do produto.

   Confirme se a versão pública do site mostra os ativos publicados conforme anteriormente visto no Adobe Dynamic Media Classic.

1. De fora da rede corporativa, verifique se os ativos não publicados (ou seja, desmarcados para publicação) estão protegidos do acesso de terceiros.

   Acesse sua rede de fora (como a partir de seu computador doméstico ou por uma conexão 3G) e verifique se a versão pública do site mostra todos os ativos publicados, mas nenhum do conteúdo não publicado.

   Confirme se a versão de preparo não mostra nenhum ativo porque você está acessando o serviço de Teste seguro de um endereço IP não aprovado.
