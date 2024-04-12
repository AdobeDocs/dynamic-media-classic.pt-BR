---
title: Perfis ICC (International Color Consortium)
description: Saiba mais sobre perfis ICC no Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Perfis ICC{#icc-profiles}

Um perfil ICC (International Color Consortium) é um arquivo que descreve como converter corretamente arquivos de imagem de um espaço de cores para outro. Os perfis ICC ajudam você a obter as cores corretas para suas imagens. Por exemplo, para exibir corretamente imagens projetadas para impressão em um monitor de computador, você pode escolher um perfil ICC. Esse perfil converte a imagem em um espaço de cores diferente e garante que as cores sejam exibidas corretamente online.

No Adobe Dynamic Media Classic, você pode escolher um perfil ICC para converter imagens em um espaço de cores diferente ao fazer upload das imagens. Todos os perfis padrão do Photoshop ICC estão disponíveis por padrão no Adobe Dynamic Media Classic. Para ver os nomes dos perfis de cores na tela Upload, selecione o menu Perfil de cores. Em seguida, escolha Personalizar de > Para e escolha um nome de perfil ICC nos menus Convertido de e Convertido para.

Consulte [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).

Além de usar os perfis ICC padrão, você pode fazer upload de outros perfis ICC para o Adobe Dynamic Media Classic e disponibilizá-los para conversão de espaço de cores. Alterne para a Exibição de detalhes no Painel de navegação para investigar a classe de perfil, o tipo de espaço de cores e o tipo de PCS de um perfil ICC.

## Carregar perfis ICC {#uploading-icc-profiles}

Carregue perfis ICC com as mesmas técnicas usadas para carregar arquivos. Você pode armazenar perfis ICC em qualquer pasta da Adobe Dynamic Media Classic.

Consulte [Fazer upload dos arquivos](uploading-files.md#uploading_your_files).

## Examinar um perfil ICC {#examining-an-icc-profile}

Para examinar um perfil ICC, selecione-o no Painel de navegação e exiba-o na Exibição de detalhes. A Exibição de detalhes fornece estas informações sobre perfis ICC:

* **[!UICONTROL Profile Class]** - O ICC (International Color Consortium) define cada classe para abranger um tipo de aplicativo. Por exemplo, perfis de entrada se aplicam a dispositivos como câmeras digitais e scanners, e perfis de saída se aplicam a impressoras.

* **[!UICONTROL Color Space Type]** - Este número é o espaço de cores de &quot;entrada&quot; do perfil, conforme definido pelo ICC. O tipo de espaço de cores define o número de componentes do espaço de cores e a interpretação desses componentes. Por exemplo, RGB é um espaço de cores com três componentes: vermelho, verde e azul. O tipo de espaço de cor não define as características de cor específicas do espaço (por exemplo, as cromaticidades das primárias).

* **[!UICONTROL PCS Type]** - Este tipo de PCS é o espaço de cores de &quot;saída&quot; do perfil—seu espaço de conexão de perfil. Por exemplo, um perfil de cores pode converter RGB para o PCS, que então o converte em CMYK.

Para um perfil de entrada, exibição ou saída útil para marcar cores ou imagens, o PCS tipo é XYZ ou Lab. Interprete esse perfil como o espaço de cor específico correspondente definido na especificação ICC.
