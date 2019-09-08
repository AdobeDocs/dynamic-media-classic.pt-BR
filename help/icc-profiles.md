---
title: perfis ICC
seo-title: perfis ICC
description: 'null'
seo-description: Saiba mais sobre perfis ICC.
uuid: 708 ff 2 ad -9 a 47-4 e 3 e-b 643-5 b 19648 f 726 b
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/support_ files
discoiquuid: 44 f 1 b 4 c 4-6 d 7 f -4 e 0 f -84 ce -11 d 26745 e 0 f 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# perfis ICC{#icc-profiles}

Um perfil ICC (International Color Consortium) é um arquivo que descreve como converter corretamente arquivos de imagem de um espaço de cores para outro. Os perfis ICC ajudam você a obter as cores corretas das suas imagens. Por exemplo, para exibir corretamente imagens projetadas para impressão em um monitor de computador, você pode escolher um perfil ICC. Esse perfil converte a imagem em um espaço de cores diferente e garante que as cores sejam exibidas corretamente online.

No Sistema de publicação Scene 7, é possível escolher um perfil ICC para converter imagens em um espaço de cores diferente ao carregar as imagens. Todos os perfis padrão do Photoshop ICC estão disponíveis por padrão no SPS. Para ver os nomes dos perfis de cores na tela Carregar, selecione o menu Perfil de cor. Em seguida, escolha Personalizado de &gt; Para e escolha um nome de perfil ICC nos menus Convertido de e Convertido em. Consulte [Opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload).

Além de usar os perfis ICC padrão, você pode carregar outros perfis ICC para o SPS e disponibilizá-los para conversão de espaço de cores. Alterne para a exibição Detalhe no Painel Procurar para investigar a classe do perfil, o tipo de espaço de cores e o tipo de PCS de um perfil ICC.

## Carregamento de perfis ICC {#uploading-icc-profiles}

Faça upload de perfis ICC com as mesmas técnicas usadas para carregar arquivos. É possível armazenar perfis ICC em qualquer pasta SPS. Consulte [Carregar seus arquivos](uploading-files.md#uploading_your_files).

## Examinar um perfil ICC {#examining-an-icc-profile}

Para examinar um perfil ICC, selecione-o no Painel Procurar e exiba-o na exibição Detalhe. A exibição de detalhes fornece essas informações sobre perfis ICC:

**Classe Profile** O ICC (International Color Consortium) define cada classe para abranger um tipo de aplicativo. Por exemplo, os perfis de Entrada se aplicam a dispositivos como câmeras e scanners digitais, e os perfis de Saída se aplicam a impressoras.

**Tipo de espaço de cor** Esse número é o espaço de cores "input" do perfil, conforme definido pelo ICC. O tipo de espaço de cores define o número de componentes do espaço de cores e a interpretação desses componentes. Por exemplo, RGB é um espaço de cores com três componentes: vermelho, verde e azul. O tipo de espaço de cores não define as características de cores específicas do espaço (por exemplo, as cromaticicas das primárias).

**Tipo PCS** Este tipo PCS é o espaço de cores "saída" do perfil - seu espaço de conexão de perfil. Por exemplo, um perfil de cor pode converter RGB para o PCS, o que o converte em CMYK.

Para um perfil de entrada, exibição ou saída útil para marcar cores ou imagens, o tipo PCS é XYZ ou Lab. Interprete esse perfil como o espaço de cor específico correspondente definido na especificação ICC.
