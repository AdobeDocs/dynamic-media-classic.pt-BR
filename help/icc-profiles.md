---
title: PERFIS ICC
seo-title: PERFIS ICC
description: nulo
seo-description: Saiba mais sobre perfis ICC.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# PERFIS ICC{#icc-profiles}

Um perfil ICC (International Color Consortium) é um arquivo que descreve como converter corretamente arquivos de imagem de um espaço de cor para outro. Os perfis ICC ajudam você a obter as cores corretas para suas imagens. Por exemplo, para exibir corretamente imagens projetadas para impressão em um monitor de computador, você pode escolher um perfil ICC. Esse perfil converte a imagem em um espaço de cor diferente e garante que as cores sejam exibidas corretamente on-line.

No Dynamic Media Classic, você pode escolher um perfil ICC para converter imagens em um espaço de cor diferente ao fazer upload das imagens. Todos os perfis Photoshop ICC padrão estão disponíveis por padrão no Dynamic Media Classic. Para ver os nomes dos perfis coloridos na tela Carregar, selecione o menu Perfil de cores. Em seguida, escolha Personalizado de > Para e escolha um nome de perfil ICC nos menus Convertido de e Convertido em. Consulte Opções de edição de [imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).

Além de usar os perfis ICC padrão, você pode fazer upload de outros perfis ICC para o Dynamic Media Classic e disponibilizá-los para conversão de espaço de cores. Alterne para visualização de detalhes no Painel de navegação para investigar a classe do perfil, o tipo de espaço de cor e o tipo PCS de um perfil ICC.

## Carregando perfis ICC {#uploading-icc-profiles}

Carregue perfis ICC com as mesmas técnicas usadas para carregar arquivos. Você pode armazenar perfis ICC em qualquer pasta do Dynamic Media Classic. Consulte [Fazer upload dos arquivos](uploading-files.md#uploading_your_files).

## Examinando um perfil ICC {#examining-an-icc-profile}

Para examinar um perfil ICC, selecione-o no Painel de navegação e exiba-o na visualização Detalhe. A visualização Detail fornece estas informações sobre perfis ICC:

**Classe** do perfil O ICC (International Color Consortium) define cada classe para abranger um tipo de aplicativo. Por exemplo, perfis de entrada se aplicam a dispositivos como câmeras digitais e scanners, e perfis de saída se aplicam a impressoras.

**Tipo** de espaço de cor Esse número é o espaço de cor &quot;entrada&quot; do perfil, conforme definido pelo ICC. O tipo de espaço de cores define o número de componentes do espaço de cores e a interpretação desses componentes. Por exemplo, RGB é um espaço de cor com três componentes: vermelho, verde e azul. O tipo de espaço de cor não define as características de cor específicas do espaço (por exemplo, as cromatrizes das primárias).

**Tipo** PCS Este tipo de PCS é o espaço de cor de &quot;saída&quot; do perfil — seu espaço de conexão do perfil. Por exemplo, um perfil colorido pode converter RGB para PCS, que o converte em CMYK.

Para um perfil de entrada, exibição ou saída útil para marcar cores ou imagens, o tipo PCS é XYZ ou Lab. Interprete esse perfil como o espaço de cor específico correspondente definido na especificação ICC.
