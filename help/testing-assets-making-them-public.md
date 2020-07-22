---
title: Teste de ativos antes de torná-los públicos
seo-title: Teste de ativos antes de torná-los públicos
description: nulo
seo-description: Saiba como testar ativos antes de torná-los públicos.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---


# Teste de ativos antes de torná-los públicos {#testing-assets-before-making-them-public}

O teste seguro ajuda a definir um ambiente de teste seguro e a criar uma solução B2B robusta, com base em um conjunto configurável de endereços IP e intervalos. Essa funcionalidade permite que você corresponda as implantações do Dynamic Media Classic à arquitetura da sua plataforma de gestão de conteúdo e comércio.

Com o Secure Testing, você pode pré-visualização a versão de preparo do site com conteúdo não publicado.

Você pode preferir criar um ambiente de preparo em vez de tornar os ativos disponíveis ao público pelos seguintes motivos:

* Pré-visualização de sites antes do lançamento público (site de preparo).
* Servir ativos que exigem acesso restrito, como eCatalogs que mostram preços em um aplicativo Web B2B.
* Use ativos por trás de um firewall como parte do sistema de gerenciamento de informações sobre produtos, do aplicativo de atendimento ao cliente, do site de treinamento e assim por diante.

>[!NOTE]
>
>O teste seguro não afeta o acesso ao Dynamic Media Classic. A segurança do Dynamic Media Classic permanece consistente e requer as credenciais comuns para acesso ao Dynamic Media Classic e aos serviços da Web relacionados.

## Como o teste seguro funciona {#how-secure-testing-works}

A maioria das corporações administra a Internet por trás de um firewall. O acesso à Internet é possível por meio de determinadas rotas e, normalmente, por meio de uma faixa limitada de endereços IP públicos.

Na sua rede corporativa, você pode descobrir seu endereço IP público usando sites como https://whatismyip.com ou solicitar essas informações à sua organização de TI corporativa.

Com o teste seguro, o Dynamic Media Classic estabelece um servidor de imagem dedicado para ambientes de preparo ou aplicativos internos. Qualquer solicitação para este servidor verifica o endereço IP da origem. Se a solicitação recebida não estiver dentro da lista aprovada de endereços IP, uma resposta de falha será retornada. O administrador da Empresa Dynamic Media Classic configura a lista aprovada de endereços IP para o ambiente de teste seguro da empresa.

Como o local da solicitação original deve ser confirmado, o tráfego do serviço de Teste seguro não é roteado por meio de uma rede de distribuição de conteúdo, como o tráfego público do Dynamic Media Image Server. As solicitações ao serviço de teste seguro podem ter uma latência ligeiramente maior em comparação aos servidores de imagem Dynamic Media públicos.

Os ativos não publicados estão imediatamente disponíveis nos serviços de teste seguro, sem a necessidade de publicação. Isso permite que você execute uma pré-visualização antes que os ativos sejam publicados em seu servidor de imagens voltado para o público.

***observação **: Os serviços de Testes seguros aproveitam o servidor de catálogo configurado com um contexto de publicação interno. Portanto, se sua empresa estiver configurada para publicar em Testes seguros, esteja ciente de que todos os ativos carregados no Dynamic Media Classic imediatamente se tornam disponíveis nos serviços de Testes seguros. Essa funcionalidade é verdadeira independentemente de os ativos estarem ou não marcados para publicação no upload.*

Atualmente, os serviços de Testes seguros oferecem suporte aos seguintes tipos de ativos e funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imagens.
* Vinhetas (solicitações do Servidor de renderização).
* Solicitações do Servidor de renderização (suportadas, mas devem ser solicitadas explicitamente pelo cliente).
* Conjuntos, incluindo conjuntos de imagens, eCatalog, conjuntos de renderização e conjuntos de mídia.
* Visualizadores de mídia avançada padrão Dynamic Media Classic.
* Páginas JSP Dynamic Media Classic OnDemand.
* Conteúdo estático, como arquivos PDF e vídeos progressivamente servidos.
* Streaming de vídeo HTTP.
* Streaming progressivo de vídeo.

Os seguintes tipos de ativos e funcionalidades não são suportados atualmente:

* Streaming de vídeo RTMP
* Serviços UGC
* Web-to-print
* Pesquisa do Dynamic Media Classic Info ou eCatalog

## Teste do serviço de teste seguro {#testing-the-secure-testing-service}

Você deve testar o serviço de teste seguro para garantir que ele funcione como esperado.

**Preparar sua conta**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Entre em contato com o suporte técnico e solicite que o Secure Testing seja ativado em sua conta.
1. No Dynamic Media Classic, clique em **Configuração** > **Instalação** de publicação > Servidor **de** imagem.
1. Na página de Publicação do Servidor de Imagens, na lista suspensa Contexto de Publicação, selecione **Testar Servidor** de Imagens.
1. Para o Filtro de endereço do cliente, clique em **Adicionar**.
1. Marque a caixa de seleção para ativar (ativar) o endereço e digite um endereço IP e uma máscara de rede nos respectivos campos de texto.
1. Repita as duas etapas anteriores para adicionar mais endereços IP. Caso contrário, continue para a próxima etapa.
1. Na parte inferior esquerda da página Publicação do servidor de imagens, clique em **Salvar**
1. Carregue as imagens desejadas para sua conta do Dynamic Media Classic.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. Verifique se algumas imagens estão marcadas para publicação, outras não estão marcadas e envie o trabalho de publicação.

   Consulte [Publicação](publishing-files.md#publishing_files).

1. Determine o nome do serviço de Teste seguro clicando em **Configuração** > Configuração **** do aplicativo > Configurações **** gerais.
1. Na página Configurações gerais do aplicativo, no grupo Servidores, localize o nome à direita de **Testar o nome** do servidor de contexto de publicação.

Entre em contato com o suporte técnico se o nome do servidor estiver ausente ou se os URLs do servidor não funcionarem.

**Preparar variações do site**

Você precisa de duas variações de um site que vinculam os ativos publicados e não publicados:

* Versão pública: Vincule ativos usando sua sintaxe de URL tradicional do Dynamic Media Classic
* Versão de armazenamento temporário: Vincule ativos usando a mesma sintaxe, mas com o nome do site Teste seguro

**Executar os testes**

Execute os seguintes testes:

1. Verifique se os ativos estão visíveis na sua rede corporativa.

   Na rede corporativa identificada pelo intervalo de endereços IP definido anteriormente, a versão de preparo do site deve exibir todas as imagens, sejam elas marcadas para publicação ou não. Isso permite testar sem disponibilizar acidentalmente imagens antes da aprovação da pré-visualização ou da inicialização do produto.

   Confirme se a versão pública do seu site mostra ativos publicados como anteriormente eram experientes com o Dynamic Media Classic.

1. De fora da sua rede corporativa, verifique se os ativos não publicados (ou seja, não marcados para publicação) estão protegidos do acesso de terceiros.

   Acesse sua rede de fora (como, de seu computador doméstico ou de uma conexão 3G) e verifique se a versão pública do site mostra todos os ativos publicados, mas nenhum conteúdo não publicado.

   Confirme se a versão de armazenamento temporário não mostra nenhum ativo porque você está acessando o serviço de teste seguro de um endereço IP não aprovado.

