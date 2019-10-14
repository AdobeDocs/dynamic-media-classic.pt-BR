---
title: '"Definindo variabilidade: Parametrização versus manipulação DOM"'
seo-title: '"Definindo variabilidade: Parametrização versus manipulação DOM"'
description: nulo
seo-description: Saiba como definir a variabilidade com parametrização versus manipulação de DOM.
uuid: dce424f2-07d8-4703-aa3a-40d2eee12f74
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Definindo variabilidade: Parametrização versus manipulação DOM{#defining-variability-parameterization-versus-dom-manipulation}

O Dynamic Media Classic oferece duas técnicas para gerenciar conteúdo variável em um modelo. Com ambas as técnicas, você cria o modelo inicial no Illustrator, converte o modelo para o formato de arquivo FXG do Dynamic Media Classic e o carrega para a SPS. No entanto, as técnicas diferem no grau de controle que você tem sobre elementos variáveis e na habilidade necessária para usá-los:

* **Parametrização no Scene7 Publishing System** Essa técnica exige a definição da variabilidade nas telas de Criação e Visualização da Publicação de Modelos na SPS ou no Plug-in do Adobe Illustrator para Web-to-Print. Qualquer um dos métodos fornece as ferramentas para você criar parâmetros, atribuir valores de parâmetros e testar os resultados.

* **Usando a manipulação** de DOM Essa técnica permite que você assuma o controle do design e do modelo em um nível XML. Os arquivos FXG do Dynamic Media Classic são XML. Com essa abordagem, você pode editar seu modelo de design diretamente por meio de seu DOM XML (modelo de objeto de exibição). No Illustrator, você marca elementos variáveis com s7:elementIDs para manipulá-los posteriormente com comandos de URL.

>[!MORELIKETHIS]
>
>* [Como parametrizar um modelo no Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [Manipulação de DOM](dom-manipulation.md#dom_manipulation)

