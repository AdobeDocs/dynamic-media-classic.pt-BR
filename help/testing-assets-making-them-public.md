---
title: Teste de ativos antes de torná-los públicos
seo-title: Teste de ativos antes de torná-los públicos
description: 'null'
seo-description: Saiba como testar ativos antes de torná-los públicos.
uuid: 5 e 8 f 3 bec -6 cf 1-408 e -8 ea 1-aebde 0012 a 70
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/upload_ and_ publish_ assets
discoiquuid: 52 fadf 99-7 d 11-46 f 7-8483-a 9 f 87 ffc 2 f 67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Teste de ativos antes de torná-los públicos {#testing-assets-before-making-them-public}

O Teste seguro ajuda você a definir um ambiente de teste seguro e construir uma solução B 2 B robusta, com base em um conjunto configurável de endereços IP e intervalos. Essa funcionalidade permite que você corresponda às implantações do Dynamic Media Classic com a arquitetura de seu gerenciamento de conteúdo e plataforma de comércio.

Com o teste seguro, você pode visualizar a versão de armazenamento temporário do site com conteúdo não publicado.

Você pode preferir criar um ambiente de preparo, em vez de disponibilizar os ativos publicamente pelos seguintes motivos:

* Visualize sites antes da inicialização pública (site de preparo temporário).
* Forneça ativos que exigem acesso restrito, como o ecatalogs que mostra os preços em um aplicativo da Web B 2 B.
* Use ativos atrás de um firewall como parte do sistema de gerenciamento de informações do produto, aplicativo de atendimento ao cliente, site de treinamento e assim por diante.

>[!NOTE]
>
>O Teste seguro não afeta o acesso ao Sistema de publicação Scene 7. A segurança do SPS permanece consistente e exige as credenciais comuns para acesso ao SPS e serviços da Web relacionados.

## Como funciona o teste seguro {#how-secure-testing-works}

A maioria das empresas executa a Internet por trás de um firewall. O acesso à Internet é possível por meio de certas rotas e geralmente por um intervalo limitado de endereços IP públicos.

Na rede corporativa, você pode descobrir seu endereço IP público usando sites como https://whatismyip.com ou solicitar essas informações de sua organização corporativa de TI.

Com o teste seguro, o Dynamic Media Classic estabelece um Servidor de imagens dedicado para ambientes de armazenamento temporário ou aplicativos internos. Qualquer solicitação a esse servidor verifica o endereço IP de origem. Se a solicitação de entrada não estiver na lista aprovada de endereços IP, uma resposta de falha será retornada. O Administrador da empresa do Dynamic Media clássica configura a lista aprovada de endereços IP para o ambiente de teste seguro da sua empresa.

Como a localização da solicitação original deve ser confirmada, o tráfego do serviço de Teste seguro não é direcionado por uma rede de distribuição de conteúdo, como tráfego público do servidor de imagem dinâmica. As solicitações para o serviço de teste seguro podem ter uma latência um pouco maior em comparação aos servidores de imagem do Dynamic Media.

Os ativos não publicados ficam imediatamente disponíveis nos serviços de Teste seguro, sem precisar publicar. Isso permite que você execute uma visualização antes dos ativos serem publicados em seu servidor de imagem de rosto público.

***observação**: Os serviços de teste seguro utilizam o Servidor de catálogo configurado com um contexto de publicação interno. Portanto, se sua empresa estiver configurada para publicar em Teste seguro, esteja ciente de que todos os ativos carregados no Scene 7 Publishing System imediatamente ficam disponíveis em serviços de teste seguro. Essa funcionalidade é verdadeira, independentemente dos ativos serem marcados ou não para publicação no upload.*

Os serviços de teste seguro suportam atualmente os seguintes tipos de ativos e funcionalidades:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Imagens.
* Vinhetas (solicitações de servidor de renderização).
* Solicitações de servidor de renderização (suportadas, mas devem ser solicitadas explicitamente pelo cliente).
* Define, incluindo conjuntos de imagens, ecatalog, conjuntos de renderização e conjuntos de mídia.
* Visualizadores de mídia avançada do Dynamic Media Classic.
* Páginas JSP do Dynamic Media Classic ondemand.
* Conteúdo estático, como arquivos PDF e vídeos progressivamente transmitidos.
* Streaming de vídeo HTTP.
* Streaming progressivo de vídeo.

Atualmente, os seguintes tipos de ativos e funcionalidades não são suportados:

* Streaming de vídeo RTMP
* Serviços UGC
* Web-to-Print
* Pesquisa do Dynamic Media Classic ou pesquisa do ecatalog

## Teste do serviço de teste seguro {#testing-the-secure-testing-service}

Você deve testar o serviço de Teste seguro para certificar-se de que ele funciona conforme esperado.

**Prepare sua conta**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Entre em contato com o Suporte técnico e solicite que Teste seguro seja ativado em sua conta.
1. No Scene 7 Publishing System, clique **em Configuração** &gt; Configuração **de publicação** &gt; **Servidor de imagens**.
1. Na página Publicação do servidor de imagens, na lista suspensa Publicação de contexto, selecione **Teste de imagem de teste**.
1. Para o Filtro de endereço do cliente, clique **em Adicionar**.
1. Marque a caixa de seleção para ativar (ativar) o endereço e digite um endereço IP e uma máscara de rede nos respectivos campos de texto.
1. Repita as duas etapas anteriores para adicionar mais endereços IP. Caso contrário, prossiga para a próxima etapa.
1. Na página inferior esquerda da página Publicação do servidor de imagens, clique **em Salvar**
1. Faça upload das imagens desejadas para a sua conta do Scene 7 Publishing System.

   Consulte [Carregamento de arquivos](uploading-files.md#uploading_files).

1. Verifique se algumas imagens estão marcadas para publicação e outras não marcadas e envie o trabalho de publicação.

   Consulte [Publicação](publishing-files.md#publishing_files).

1. Determine o nome do serviço de Teste seguro clicando **em Configuração** &gt; Configuração **do aplicativo** &gt; **Configurações gerais**.
1. Na página Configurações gerais do aplicativo, no grupo Servidores, localize o nome à direita do **Nome do servidor de contexto de publicação**.

Entre em contato com o Suporte técnico se o nome do servidor estiver ausente ou urls para o servidor não funcionar.

**Preparar variações do site**

Você precisa de duas variações de um site que vincula os ativos publicados e não publicados:

* Versão pública: Vincular ativos usando a sintaxe clássica do URL clássica do Dynamic Media
* Versão de armazenamento temporário: Vincular ativos usando a mesma sintaxe, mas com o nome do site de Teste seguro

**Executar os testes**

Realize os seguintes testes:

1. Verifique se os ativos estão visíveis em sua rede corporativa.

   Na rede corporativa identificada pelo intervalo de endereço IP definido anteriormente, a versão de armazenamento temporário do site deve exibir todas as imagens, seja marcadas para publicação ou não. Isso permite que você teste sem tornar as imagens acidentalmente disponíveis antes da aprovação da visualização ou inicialização do produto.

   Confirme se a versão pública do site mostra ativos publicados como anteriormente com o Dynamic Media Classic.

1. De fora da rede corporativa, verifique se ativos não publicados (ou seja, não marcados para publicação) estão protegidos de acesso de terceiros.

   Acesse sua rede de fora (por exemplo, de seu computador pessoal ou de uma conexão 3 G) e verifique se a versão pública do site mostra todos os ativos publicados, mas nenhum do conteúdo não publicado.

   Confirme se a versão de armazenamento temporário não mostra nenhum ativo porque você está acessando o serviço de Teste seguro a partir de um endereço IP não aprovado.

