---
title: Recortar uma imagem
description: Saiba como recortar uma imagem.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Gerenciamento de ativos
role: Profissional
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---


# Recortar uma imagem{#cropping-an-image}

Você pode recortar imagens no Dynamic Media Classic. O sistema retém informações sobre imagens que foram cortadas para que você possa restaurá-las ao estado original. Também é possível recortar uma imagem e salvar a versão cortada com um novo nome.

Você pode recortar uma imagem para remover o espaço em branco ao seu redor ou recortar uma área da imagem.

>[!NOTE]
>
>Após cortar, você pode clicar no botão Salvar como e salvar uma versão recortada da imagem com um nome diferente. Na janela Salvar como, escolha Salvar como novo Principal para salvar uma segunda cópia da imagem. Escolha Salvar como exibição de adição de Principal para salvar o original e sua versão cortada com um nome diferente. Escolha Substituir original para excluir o arquivo original do qual você cortou a imagem. Em seguida, insira um nome para a imagem e selecione o botão Submit .

## Recorte para remover o espaço em branco ao redor de uma imagem {#crop-to-remove-white-space-around-an-image}

Você pode cortar os pixels transparentes ou de cor sólida da borda de uma imagem.

1. Para recortar uma imagem, clique no botão Editar sobreposição e escolha Recortar ou exiba-o no Painel de navegação na exibição Detalhes e clique no botão Recortar. A tela Editor de corte é aberta.
1. Siga um destes procedimentos:

   * Para aparar pixels de cor, selecione o menu Cortar e escolha Cor. A caixa de diálogo Cortar automaticamente por cor é exibida. Selecione o menu Canto e escolha um canto com a cor de plano de fundo para cortar. Em seguida, insira uma configuração de Tolerância de 0 a 1. A configuração 0 corta pixels somente se eles corresponderem exatamente à cor selecionada no canto da imagem. Os números mais próximos de 1 permitem mais diferenças de cor. Selecione o botão Cortar.
   * Para aparar pixels transparentes, selecione o menu Cortar e escolha Transparente. A caixa de diálogo Cortar automaticamente por transparência é exibida. Insira uma configuração de tolerância de 0 a 1. A configuração 0 recorta pixels de corte somente se eles forem totalmente transparentes. Os números mais próximos de 1 permitem mais transparência. Selecione o botão Cortar.

1. Clique em **Salvar**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de corte e selecione o botão Redefinir .

## Selecione uma área para cortar {#select-an-area-to-crop}

1. Para recortar uma imagem, clique no botão Editar sobreposição e escolha **Recortar**, ou exiba-a no Painel de navegação na exibição Detalhes e clique em **Recortar**.

1. Na janela Editor de corte, coloque a parte da imagem que não deseja cortar na caixa de corte. O que aparece dentro da caixa permanece quando você clica em **Salvar** e corta a imagem.
1. Para ajustar a área de corte, siga um destes procedimentos:

   * Arraste um lado ou canto da caixa. Mantenha pressionada a tecla Shift enquanto arrasta para alterar o tamanho, mas mantém a proporção (a forma) da caixa de corte.
   * Insira medições de pixel nas caixas Tamanho.
   * Arraste para mover a caixa de corte. Mova o ponteiro para dentro do limite da caixa. Ao ver a seta de quatro pontas, arraste a caixa até um novo local na imagem.

1. Clique em **Salvar**.

>[!NOTE]
>
>Para restaurar uma imagem ao seu estado original depois de cortá-la, exiba a imagem na tela Editor de corte e selecione o botão Redefinir .

>[!MORELIKETHIS]
>
>* [Opções de edição de imagem no upload](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Recortar espaço em branco de um arquivo PDF](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Recortar das laterais das páginas PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)

