---
title: Testar ativos antes de torná-los públicos
description: Saiba como testar ativos no Adobe Dynamic Media Classic antes de torná-los públicos.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Testar ativos antes de torná-los públicos {#testing-assets-before-making-them-public}

O Teste Seguro ajuda você a definir um ambiente de teste seguro e criar uma solução B2B robusta, com base em um conjunto configurável de endereços IP e intervalos. Essa funcionalidade permite que você combine suas implantações do Adobe Dynamic Media Classic com a arquitetura do seu sistema de negócios e de gerenciamento de conteúdo.

Com o Teste Seguro, você pode visualizar a versão de preparo do site com conteúdo não publicado.

Se desejar, crie um ambiente de preparo em vez de tornar os ativos disponíveis publicamente pelos seguintes motivos:

* Visualizar sites antes do lançamento público (site de preparo).
* Adicione ativos que exigem acesso restrito, como eCatalogs que mostrem preços em uma aplicação Web B2B.
* Use os ativos por trás de um firewall como parte do sistema de gerenciamento de informações do produto, do aplicativo de atendimento ao cliente, do site de treinamento e assim por diante.

>[!NOTE]
>
>O Teste Seguro não afeta o acesso ao Adobe Dynamic Media Classic. A segurança do Adobe Dynamic Media Classic permanece consistente e requer as credenciais usuais para acesso ao Adobe Dynamic Media Classic e serviços da Web relacionados.

## Como o teste seguro funciona {#how-secure-testing-works}

A maioria das corporações mantém a Internet por trás de um firewall. O acesso à Internet é possível através de determinadas rotas e geralmente através de uma gama limitada de endereços IP públicos.

Na sua rede corporativa, você pode descobrir seu endereço IP público usando sites como [https://www.whatismyip.com](https://www.whatismyip.com/) ou solicite essas informações à sua organização de TI corporativa.

Com o Teste Seguro, a Adobe Dynamic Media Classic estabelece um Servidor de Imagem dedicado para ambientes de preparo temporário ou aplicativos internos. Qualquer solicitação para este servidor verifica o endereço IP de origem. Se a solicitação recebida não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada. O Administrador da empresa da Adobe Dynamic Media Classic configura a lista aprovada de endereços IP para o ambiente de Teste Seguro da empresa.

Como a localização da solicitação original deve ser confirmada, o tráfego do serviço de Teste Seguro não é roteado por meio de uma rede de distribuição de conteúdo como o tráfego público do Dynamic Media Image Server. As solicitações para o serviço de teste seguro têm uma latência ligeiramente maior em comparação com os servidores públicos de imagem da Dynamic Media.

Os ativos não publicados ficam imediatamente disponíveis nos serviços de Teste Seguro, sem a necessidade de publicar. Dessa forma, é possível executar uma visualização antes que os ativos sejam publicados em seu servidor de imagens aberto ao público.

>[!NOTE]
>
>Os serviços de Teste Seguro usam o Servidor de Catálogo configurado com um contexto de publicação interno. Portanto, se sua empresa estiver configurada para publicar no Teste Seguro, todos os ativos carregados no Adobe Dynamic Media Classic imediatamente se tornarão disponíveis nos serviços de Teste Seguro. Essa funcionalidade é verdadeira independentemente de os ativos serem marcados para publicação no upload.

Os serviços de Teste Seguro atualmente oferecem suporte aos seguintes tipos de ativos e funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imagens.
* Vinhetas (Solicitações do Servidor de Renderização).
* Solicitações do Servidor de Renderização (suportadas, mas devem ser solicitadas explicitamente pelo cliente).
* Conjuntos, incluindo conjuntos de imagens, eCatalog, conjuntos de renderização e conjuntos de mídia.
* Visualizadores de mídia avançada padrão do Adobe Dynamic Media Classic.
* Páginas JSP Adobe Dynamic Media Classic OnDemand.
* Conteúdo estático, como arquivos PDF e vídeos fornecidos progressivamente.
* streaming de vídeo HTTP.
* Transmissão contínua de vídeo.

Os seguintes tipos de ativos e funcionalidades não são suportados no momento:

* Pesquisa de informações ou eCatalog do Adobe Dynamic Media Classic
* Transmissão de vídeo RTMP
* Web-to-print
* Serviços UGC (Conteúdo gerado pelo usuário)

>[!IMPORTANT]
>
>O suporte para ativos de imagem vetorial UGC novos ou existentes no Adobe Dynamic Media Classic terminou em 30 de setembro de 2021.

## Testar o serviço de teste seguro {#testing-the-secure-testing-service}

Teste o serviço de Teste Seguro para garantir que funcione conforme o esperado.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Prepare sua conta

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Entre em contato com o Atendimento ao cliente do Adobe e solicite que ele ative o Teste seguro em sua conta.
1. No Adobe Dynamic Media Classic, na barra Navegação global, acesse **[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**.
1. Na página Publicação do servidor de imagens, no **[!UICONTROL Publish Context]** , selecione **[!UICONTROL Test Image Serving]**.
1. Para o Filtro de endereço do cliente, selecione **[!UICONTROL Add]**.
1. Marque a caixa de seleção para que o endereço seja ativado (ativado) e digite um endereço IP e uma máscara de rede nos respectivos campos de texto.

   >[!NOTE]
   >
   >Se você adicionar um único endereço IP e máscara de rede, esse endereço poderá fazer chamadas de ativos. No entanto, quaisquer outros endereços IP e máscaras de rede adicionados não têm permissão para fazer chamadas de ativos. Dessa forma, considere desabilitar (desabilitar) a caixa de seleção na etapa acima para desabilitar a capacidade de especificar um endereço IP e uma máscara de rede. Isso permite *all* Endereços IP para fazer chamadas de ativos e todos aparecem.

1. Siga um destes procedimentos:
   * Repita as duas etapas anteriores se precisar adicionar mais endereços IP.
   * Prossiga para a próxima etapa.
1. Na parte inferior esquerda da página Publicação do servidor de imagens, selecione **[!UICONTROL Save]**
1. Faça upload das imagens desejadas para sua conta do Adobe Dynamic Media Classic.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. Certifique-se de que algumas imagens estejam marcadas para publicação e outras não estejam marcadas e envie o trabalho de publicação.

   Consulte [Publicar arquivos](publishing-files.md#publishing_files).

1. Determine o nome do seu serviço de Teste Seguro acessando **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Na página Configurações gerais do aplicativo , no grupo Servidores , localize o nome à direita de **[!UICONTROL Test Publish Context Server Name]**.

Entre em contato com o Adobe Care se o nome do servidor estiver ausente ou se os URLs do servidor não funcionarem.

### Preparar variações do site

Você precisa de duas variações de um site que vincula os ativos publicados e não publicados:

* Versão pública - Vincule ativos usando a sintaxe de URL tradicional do Adobe Dynamic Media Classic.
* Versão de armazenamento temporário - Vincule ativos usando a mesma sintaxe, mas com o nome do site Teste seguro .

### Executar os testes

Execute os seguintes testes:

1. Verifique se os ativos estão visíveis na rede corporativa.

   Na rede corporativa identificada pelo intervalo de endereços IP definido anteriormente, a versão de preparo do site exibe todas as imagens, independentemente de serem ou não marcadas para publicação. Dessa forma, é possível testar sem disponibilizar acidentalmente as imagens antes de visualizar a aprovação ou o lançamento do produto.

   Confirme se a versão pública do seu site mostra os ativos publicados como anteriormente tinham experiência com o Adobe Dynamic Media Classic.

1. De fora da rede corporativa, verifique se os ativos não publicados (ou seja, não marcados para publicação) estão protegidos do acesso de terceiros.

   Acesse sua rede de fora (por exemplo, de seu computador pessoal ou por uma conexão 3G) e verifique se a versão pública do site mostra todos os ativos publicados, mas nenhum conteúdo não publicado.

   Confirme se a versão de armazenamento temporário não mostra nenhum ativo porque você está acessando o serviço de Teste Seguro a partir de um endereço IP não aprovado.
