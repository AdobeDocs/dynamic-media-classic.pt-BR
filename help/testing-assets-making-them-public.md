---
title: Testar ativos antes de torná-los públicos
description: Saiba como testar ativos antes de torná-los públicos.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Business Practitioner
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1100'
ht-degree: 0%

---

# Testar ativos antes de torná-los públicos {#testing-assets-before-making-them-public}

O Teste Seguro ajuda você a definir um ambiente de teste seguro e criar uma solução B2B robusta, com base em um conjunto configurável de endereços IP e intervalos. Essa funcionalidade permite que você corresponda suas implantações do Dynamic Media Classic à arquitetura da sua plataforma de comércio e gerenciamento de conteúdo.

Com o Teste Seguro, você pode visualizar a versão de preparo do site com conteúdo não publicado.

Você pode preferir criar um ambiente de preparo em vez de tornar os ativos disponíveis publicamente pelos seguintes motivos:

* Visualizar sites antes do lançamento público (site de preparo).
* Adicione ativos que exigem acesso restrito, como eCatalogs que mostrem preços em uma aplicação Web B2B.
* Use os ativos por trás de um firewall como parte do sistema de gerenciamento de informações do produto, do aplicativo de atendimento ao cliente, do site de treinamento e assim por diante.

>[!NOTE]
>
>O Teste Seguro não afeta o acesso ao Dynamic Media Classic. A segurança do Dynamic Media Classic permanece consistente e requer as credenciais usuais para acessar o Dynamic Media Classic e serviços da Web relacionados.

## Como o teste seguro funciona {#how-secure-testing-works}

A maioria das corporações mantém a Internet por trás de um firewall. O acesso à Internet é possível através de determinadas rotas e geralmente através de uma gama limitada de endereços IP públicos.

Em sua rede corporativa, você pode descobrir seu endereço IP público usando sites como https://whatismyip.com ou solicitar essas informações de sua organização corporativa de TI.

Com o Teste Seguro, o Dynamic Media Classic estabelece um Servidor de Imagem dedicado para ambientes de preparo temporário ou aplicativos internos. Qualquer solicitação para este servidor verifica o endereço IP de origem. Se a solicitação recebida não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada. O Administrador da empresa do Dynamic Media Classic configura a lista aprovada de endereços IP para o ambiente de Teste Seguro da empresa.

Como a localização da solicitação original deve ser confirmada, o tráfego do serviço de Teste Seguro não é roteado por meio de uma rede de distribuição de conteúdo como o tráfego público do Dynamic Media Image Server. As solicitações para o serviço de teste seguro podem ter uma latência ligeiramente maior em comparação com os servidores de imagem Dynamic Media públicos.

Os ativos não publicados ficam imediatamente disponíveis nos serviços de Teste Seguro, sem a necessidade de publicar. Isso permite que você execute uma pré-visualização antes que os ativos sejam publicados em seu servidor de imagens voltado para o público.

>[!NOTE]
>
>Os serviços de Teste Seguro usam o Servidor de Catálogo que está configurado com um contexto de publicação interno. Portanto, se sua empresa estiver configurada para publicar no Teste Seguro, esteja ciente de que todos os ativos carregados no Dynamic Media Classic imediatamente se tornam disponíveis nos serviços de Teste Seguro. Essa funcionalidade é verdadeira independentemente de os ativos serem ou não marcados para publicação no upload.

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
* Visualizadores de mídia avançada padrão do Dynamic Media Classic.
* Páginas JSP OnDemand do Dynamic Media Classic.
* Conteúdo estático, como arquivos PDF e vídeos fornecidos progressivamente.
* streaming de vídeo HTTP.
* Transmissão contínua de vídeo.

Os seguintes tipos de ativos e funcionalidades não são suportados no momento:

* Transmissão de vídeo RTMP
* Serviços UGC
* Web-to-print
* Pesquisa de informações ou catálogo eletrônico do Dynamic Media Classic

## Testando o serviço de Teste Seguro {#testing-the-secure-testing-service}

Você deve testar o serviço de Teste Seguro para garantir que ele funcione conforme o esperado.

Observação: Se você não mencionar nenhum IP em Configurar > Configuração de publicação > Servidor de imagem > Serviço de imagem de teste
se você adicionar um IP, somente esse IP poderá chamar os ativos e nenhum outro IP poderá fazer as chamadas. Desde que não haja um IP mencionado nessa seção, todos os IPs têm permissão para fazer as chamadas para os ativos e eles serão exibidos.

**Prepare sua conta**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Entre em contato com o Suporte Técnico e solicite que o Teste Seguro seja ativado em sua conta.
1. No Dynamic Media Classic, clique em **Configurar** > **Publicar configuração** > **Servidor de imagem**.
1. Na página Publicação do servidor de imagens, na lista suspensa Publicar contexto , selecione **Servir imagem de teste**.
1. Para o Filtro de endereço do cliente, clique em **Adicionar**.
1. Marque a caixa de seleção para ativar (ativar) o endereço e digite um endereço IP e uma máscara de rede nos respectivos campos de texto.

   >[!NOTE]
   >
   >Se você adicionar um único endereço IP e máscara de rede, esse endereço poderá fazer chamadas de ativos. No entanto, quaisquer outros endereços IP e máscaras de rede adicionados não têm permissão para fazer chamadas de ativos. Dessa forma, talvez você queira desabilitar (desabilitar) a caixa de seleção na etapa acima para desabilitar a capacidade de especificar um endereço IP e uma máscara de rede. Isso permite que *todos* endereços IP façam chamadas de ativos e todos serão exibidos.

1. Siga um destes procedimentos:
   * Repita as duas etapas anteriores para adicionar mais endereços IP.
   * Prossiga para a próxima etapa.
1. Na parte inferior esquerda da página Publicação do servidor de imagens, clique em **Salvar**
1. Faça upload das imagens desejadas para sua conta do Dynamic Media Classic.

   Consulte [Upload de arquivos](uploading-files.md#uploading_files).

1. Certifique-se de que algumas imagens estejam marcadas para publicação e outras não estejam marcadas e envie o trabalho de publicação.

   Consulte [Publicação](publishing-files.md#publishing_files).

1. Determine o nome do seu serviço de Teste Seguro clicando em **Configurar** > **Configuração do Aplicativo** > **Configurações Gerais**.
1. Na página Configurações gerais do aplicativo , no grupo Servidores , localize o nome à direita de **Testar nome do servidor de contexto de publicação**.

Entre em contato com o Adobe Care se o nome do servidor estiver ausente ou se os URLs do servidor não funcionarem.

**Preparar variações do site**

Você precisa de duas variações de um site que vincula os ativos publicados e não publicados:

* Versão pública - Vincule ativos usando a sintaxe de URL tradicional do Dynamic Media Classic.
* Versão de armazenamento temporário - Vincule ativos usando a mesma sintaxe, mas com o nome do site Teste seguro .

**Executar os testes**

Execute os seguintes testes:

1. Verifique se os ativos estão visíveis na rede corporativa.

   A partir da rede corporativa identificada pelo intervalo de endereços IP definido anteriormente, a versão de preparo do site deve exibir todas as imagens, independentemente de estar marcada para publicação ou não. Isso permite testar sem disponibilizar acidentalmente as imagens antes de visualizar a aprovação ou o lançamento do produto.

   Confirme se a versão pública do seu site mostra os ativos publicados como anteriormente tinham experiência com o Dynamic Media Classic.

1. De fora da rede corporativa, verifique se os ativos não publicados (ou seja, não marcados para publicação) estão protegidos do acesso de terceiros.

   Acesse sua rede de fora (por exemplo, de seu computador pessoal ou por uma conexão 3G) e verifique se a versão pública do site mostra todos os ativos publicados, mas nenhum conteúdo não publicado.

   Confirme se a versão de armazenamento temporário não mostra nenhum ativo porque você está acessando o serviço de Teste Seguro a partir de um endereço IP não aprovado.
