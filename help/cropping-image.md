---
title: Recortar uma imagem
seo-title: Recortar uma imagem
description: 'null'
seo-description: Saiba como recortar uma imagem.
uuid: 84 f 199 de-cbfc -4 d 06-877 f -6 e 9148 e 82 e 15
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 99 dfa 476-4 f 11-4569-a 27 e-a 76 ed 77ed 7674
translation-type: tm+mt
source-git-commit: b8d245bfc8375966af314ed95e81a519c5ee6c24

---


# Recortar uma imagem{#cropping-an-image}

Você pode recortar imagens no Sistema de publicação Scene 7. O sistema retém informações sobre imagens cortadas para que você possa restaurá-las para o estado original. Também é possível recortar uma imagem e salvar a versão cortada com um novo nome.

É possível recortar uma imagem para remover o espaço em branco ao redor dele ou recortar uma área da imagem.

>[!NOTE]
>
>Depois de cortar, clique no botão Salvar como e salve uma versão cortada da imagem com um nome diferente. Na janela Salvar como, escolha Salvar como novo mestre para salvar uma segunda cópia da imagem. Escolha Salvar como exibição de adição do Master para salvar a versão original e recortada com um nome diferente. Escolha Substituir original para excluir o arquivo original do qual você recortou a imagem. Em seguida, insira um nome para a imagem e selecione o botão Enviar.

## Cortar para remover o espaço em branco em torno de uma imagem {#crop-to-remove-white-space-around-an-image}

É possível cortar os pixels transparentes ou de cor sólida da borda de uma imagem.

1. Para recortar uma imagem, clique no botão Editar sobreposições e escolha Cortar, ou exiba-o no Painel Procurar na exibição Detalhe e clique no botão Cortar. A tela Editor de corte é aberta.
1. Execute um dos procedimentos a seguir:

   * Para aparar pixels coloridos, selecione o menu Aparar e escolha Cor. A caixa de diálogo Cortar automaticamente por cor é exibida. Selecione o menu Canto e escolha um canto com a cor de plano de fundo para cortar. Em seguida, insira uma configuração de Tolerância de 0 a 1. A configuração 0 recorta os pixels apenas se eles corresponderem exatamente à cor selecionada no canto da imagem. Números mais próximos a 1 permitem mais diferença de cor. Selecione o botão Cortar.
   * Para aparar pixels transparentes, selecione o menu Aparar e escolha Transparente. É exibida a caixa de diálogo Cortar automaticamente por transparência. Insira uma configuração de tolerância de 0 a 1. A configuração 0 recorta recortar pixels somente se eles forem totalmente transparentes. Os números mais próximos a 1 permitem mais transparência. Selecione o botão Cortar.

1. Clique **em Salvar**.

>[!NOTE]
>
>Para restaurar uma imagem para seu estado original após recortá-la, exiba a imagem na tela Editor de recorte e selecione o botão Redefinir.

## Selecione uma área para cortar {#select-an-area-to-crop}

1. Para recortar uma imagem, clique no botão Editar sobreposições e escolha **Cortar**, ou exiba-o no Painel Procurar na exibição Detalhe e clique **em Cortar**.

1. Na janela Editor de recorte, coloque a parte da imagem que você não deseja cortar na caixa de corte. O que aparece dentro da caixa permanece quando você clica **em Salvar** e recorta a imagem.
1. Para ajustar a área de corte, execute um dos seguintes procedimentos:

   * Arraste um lado ou canto da caixa. Mantenha a tecla Shift pressionada enquanto arrasta para alterar o tamanho, mas mantenha a proporção (a forma) da caixa de corte.
   * Insira medições de pixel nas caixas Tamanho.
   * Arraste para mover a caixa de corte. Mova o ponteiro para dentro do limite da caixa. Ao visualizar a seta de quatro pontas, arraste a caixa até um novo local na imagem.

1. Clique **em Salvar**.

>[!NOTE]
>
>Para restaurar uma imagem para seu estado original após recortá-la, exiba a imagem na tela Editor de recorte e selecione o botão Redefinir.

>[!MORELIKETHIS]
>
>* [Opções de edição de imagens no upload](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recortar o espaço em branco de um arquivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recortar dos lados das páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

