---
title: '" Início rápido: Publicação de modelo "'
seo-title: '" Início rápido: Publicação de modelo "'
description: 'null'
seo-description: Uma introdução e uma Introdução rápida à publicação do modelo para ajudá-lo a começar a usar rapidamente.
uuid: 101 b 6211-2421-4565-8635-944315 a 5 c 512
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/modelo-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Início rápido: Publicação de modelo{#quick-start-template-publishing}

O Adobe Dynamic Media Classic Web-to-Print permite criar conteúdo de impressão com marca profissional, fácil para os clientes, clientes e funcionários personalizarem e personalizarem. Você pode manter o conteúdo corporativo e a identidade da marca durante todo o processo de publicação. Os usuários finais podem personalizar o conteúdo de impressão— mas apenas a parte do conteúdo que você permite personalizar. Cartões, cartões comerciais, pôsteres, cartões de saudação, rótulos, verificações, presentes, roupas, calendários, cartões de recortes e álbuns de fotos personalizados são exemplos de produtos de impressão personalizados que podem ser entregues. As empresas podem manter uma identidade de marca comum em sua assinatura que pode ser personalizada para diferentes regiões, franquias, lojas e escritórios de ramificação.

Comece criando um modelo no Adobe Illustrator. O modelo define cuidadosamente o que é constante e o que é uma variável. os componentes da variável que podem ser personalizados. Por exemplo, após o texto em um arquivo do Illustrator ser instrumentado, os usuários finais poderão digitar seu próprio texto. Da mesma forma, uma cor de plano de fundo, depois que é paramétrica como um componente de variável, pode ser trocada para uma cor de plano de fundo diferente.

O Dynamic Media Classic oferece dois fluxos de trabalho de Publicação de modelo, um para casos de uso básicos e outro para casos de uso avançados. Casos de uso básicos envolvem criar um design no Adobe Illustrator, carregá-lo no Dynamic Media Classic e definir elementos de variáveis com parâmetros no SPS. Casos de uso avançados exigem uma definição mais abrangente da variação. Casos de uso avançados envolvem criar elementos de variável no Adobe Illustrator, carregando o arquivo no Dynamic Media Classic e manipulando diretamente esses elementos em um nível XML com chamadas de URL. Esse cenário é chamado *`*DOM manipulation*`*.

>[!NOTE]
>
>Para obter mais informações sobre fluxos de trabalho da Web do Dynamic Media Classic, criação de modelos, paramrimoração, manipulação de DOM e muito mais, consulte o Guia de fluxo de trabalho da Web para impressão aqui: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Baixe o arquivo Zip em seu disco rígido local e extraia seu conteúdo (o documento Tutorial da Web do Dynamic Media Classic e ativos do tutorial).

**Início rápido**

Este Início rápido descreve o fluxo de trabalho básico para usar arquivos do Illustrator para criar produtos de impressão de alta qualidade e personalizáveis.

**1. Projetar seu arquivo do Illustrator para publicação de modelo**

No Illustrator, crie seu modelo. Caso deseje usar o método de manipulação avançado e de DOM para personalizar seu modelo, defina s 7: Elementids para elementos de variáveis no Illustrator.

Consulte [Criar o modelo inicial no Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) e [manipulação de DOM](dom-manipulation.md#dom_manipulation).

**2. Converta seu modelo no FXG clássico do Media Media Classic e carregue-o no Sistema de publicação do Scene 7**

Os usuários da Adobe Creative Cloud podem usar o Plug-in Adobe Illustrator para imprimir. Esse plug-in converte modelos no FXG clássico do Dynamic Media. Se um modelo contiver fontes, os arquivos de fonte correspondentes deverão ser carregados no Sistema de publicação Scene 7 antes de carregar o arquivo FXG.

Consulte [Carregar arquivos para Publicação](upload-files-template-publishing.md#upload_files_for_template_publishing)de modelo.

**3. Exibir, definir ou refinar parâmetros no Dynamic Media Classic**

Nas telas de Visualização de modelo de publicação e build, você pode definir e refinar elementos de variáveis por parâmetros, visualizar os resultados e testar os resultados. Nessas telas, é possível:

* Criar e modificar parâmetros.
* Especifique os valores padrão para propriedades e atributos de parâmetros.
* Clique em Copiar URL para copiar o URL de visualização para a área de transferência e visualizar o resultado em uma janela do navegador.

Consulte [Parâmetro de um modelo no Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Publicar o modelo FXG**

Depois de concluir a definição e testar parâmetros e atributos, publique o arquivo. Publicar seu modelo FXG a coloca nos servidores de imagem do Dynamic Media e ativa o URL.

Certifique-se de publicar todas as imagens e fontes associadas ao modelo FXG.

Consulte [Publicar modelos FXG](dom-manipulation.md#publish_fxg_templates).

**5. Obter o URL**

Por meio do URL, o modelo está pronto para ser incorporado em seu site para que os usuários finais personalizem o conteúdo da variável.

Consulte [Vincular um modelo FXG a uma página da Web](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
