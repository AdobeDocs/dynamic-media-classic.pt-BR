---
title: Perfis ICC (International Color Consortium)
description: Saiba mais sobre perfis ICC no Adobe Dynamic Media Classic.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Perfis ICC{#icc-profiles}

Um perfil ICC (International Color Consortium) é um arquivo que descreve como converter corretamente arquivos de imagem de um espaço de cores para outro. Os perfis ICC ajudam você a obter as cores corretas para suas imagens. Por exemplo, para exibir corretamente imagens projetadas para impressão em um monitor de computador, você pode escolher um perfil ICC. Esse perfil converte a imagem em um espaço de cores diferente e garante que as cores sejam exibidas corretamente online.

No Adobe Dynamic Media Classic, você pode escolher um perfil ICC para converter imagens em um espaço de cores diferente ao fazer upload das imagens. Todos os perfis padrão do Photoshop ICC estão disponíveis por padrão no Adobe Dynamic Media Classic. Para ver os nomes dos perfis de cores na tela Upload, selecione o menu Perfil de cores . Em seguida, escolha Personalizado de > Para e escolha um nome de perfil ICC nos menus Convertido de e Convertido em .

Consulte [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload).

Além de usar os perfis ICC padrão, você pode fazer upload de outros perfis ICC para o Adobe Dynamic Media Classic e disponibilizá-los para a conversão do espaço de cores. Alterne para Exibição de detalhes no Painel de navegação para investigar a classe de perfil, o tipo de espaço de cores e o tipo PCS de um perfil ICC.

## Fazer upload de perfis ICC {#uploading-icc-profiles}

Faça upload de perfis ICC com as mesmas técnicas usadas para fazer upload de arquivos. Você pode armazenar perfis ICC em qualquer pasta Adobe Dynamic Media Classic.

Consulte [Carregar os arquivos](uploading-files.md#uploading_your_files).

## Examinar um perfil ICC {#examining-an-icc-profile}

Para examinar um perfil ICC, selecione-o no Painel de navegação e exiba-o na Exibição de detalhes. A Exibição detalhada fornece estas informações sobre perfis ICC:

* **[!UICONTROL Profile Class]** - O ICC (International Color Consortium) define cada classe para abranger um tipo de aplicativo. Por exemplo, os perfis de entrada se aplicam a dispositivos como câmeras digitais e scanners, e os perfis de saída se aplicam a impressoras.

* **[!UICONTROL Color Space Type]** - Esse número é o espaço de cores &quot;de entrada&quot; do perfil, conforme definido pelo ICC. O tipo de espaço de cores define o número de componentes do espaço de cores e a interpretação desses componentes. Por exemplo, RGB é um espaço de cores com três componentes: vermelho, verde e azul. O tipo de espaço de cores não define as características de cor específicas do espaço (por exemplo, as cromatrizes das primárias).

* **[!UICONTROL PCS Type]** - Esse tipo de PCS é o espaço de cores de &quot;saída&quot; do perfil, o espaço de conexão do perfil. Por exemplo, um perfil de cor pode converter RGB para PCS, o que o converte em CMYK.

Para um perfil de entrada, exibição ou saída útil para marcação de cores ou imagens, o tipo PCS é XYZ ou Lab. Interprete esse perfil como o espaço de cores específico correspondente definido na especificação ICC.
